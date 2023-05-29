# Comparing `tmp/scisdk-0.0.3.tar.gz` & `tmp/scisdk-0.0.4.tar.gz`

## Comparing `scisdk-0.0.3.tar` & `scisdk-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scisdk-0.0.3/src/scisdk/__init__.py
--rw-r--r--   0        0        0    24966 2020-02-02 00:00:00.000000 scisdk-0.0.3/src/scisdk/scisdk.py
--rw-r--r--   0        0        0    15054 2020-02-02 00:00:00.000000 scisdk-0.0.3/src/scisdk/scisdk_defines.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 scisdk-0.0.3/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 scisdk-0.0.3/LICENSE
--rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 scisdk-0.0.3/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 scisdk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 scisdk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scisdk-0.0.4/src/scisdk/__init__.py
+-rw-r--r--   0        0        0    25458 2020-02-02 00:00:00.000000 scisdk-0.0.4/src/scisdk/scisdk.py
+-rw-r--r--   0        0        0    14671 2020-02-02 00:00:00.000000 scisdk-0.0.4/src/scisdk/scisdk_defines.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 scisdk-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 scisdk-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 scisdk-0.0.4/README.md
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 scisdk-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 scisdk-0.0.4/PKG-INFO
```

### Comparing `scisdk-0.0.3/src/scisdk/scisdk.py` & `scisdk-0.0.4/src/scisdk/scisdk.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,468 +1,486 @@
-import ctypes
-import os
-from scisdk.scisdk_defines import *
-
-
-class SciSDK:
-    scisdk_dll = None
-    lib_ptr = None
-    libname = None
-
-    def __init__(self) -> None:
-        #os.path.dirname(__file__) + "\\
-        libname = ""
-
-        if os.name == 'nt':
-            self.libname = "SciSDK_DLL.dll"
-        else:
-            self.libname = "libscisdk.so"
-
-        try:
-            self.scisdk_dll = ctypes.CDLL(self.libname)
-        except OSError as e:
-            if e.errno == os.errno.ENOENT:
-                print("Error: " + self.libname + " not found")
-            elif e.errno == os.errno.EINVAL:
-                print("Error: " + self.libname + " has the wrong architecture for the current process")
-            elif e.errno == os.errno.ELIBBAD:
-                print("Error:" + self.libname + " has missing dependencies")
-            else:
-                print("Error: unable to load libscisdk.so: " + str(e))
-            
-
-
-
-        init_lib_api = self.scisdk_dll.SCISDK_InitLib
-        init_lib_api.restype = ctypes.c_void_p
-        self.lib_ptr = init_lib_api()
-        
-        
-    def AddNewDevice(self, device_path: str, device_model: str, json_file_path: str, name: str) -> int:
-        add_new_device_api = self.scisdk_dll.SCISDK_AddNewDevice
-        add_new_device_api.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_void_p]
-        add_new_device_api.restype = ctypes.c_int
-        # convert strings to bytes array
-        b_device_path = device_path.encode('utf-8')
-        b_device_model = device_model.encode('utf-8')
-        b_json_file_path = json_file_path.encode('utf-8')
-        b_name = name.encode('utf-8')
-        # call C lib function
-        err = add_new_device_api(b_device_path, b_device_model, b_json_file_path, b_name, self.lib_ptr)
-        return err
-        
-    def DetachDevice(self, name: str) -> int:
-        detach_device_api = self.scisdk_dll.SCISDK_DetachDevice
-        detach_device_api.argtypes = [ctypes.c_char_p, ctypes.c_void_p]
-        detach_device_api.restype = ctypes.c_int
-        # convert string to bytes array
-        b_name = name.encode('utf-8')
-        # call C lib function
-        err = detach_device_api(b_name, self.lib_ptr)
-        return err
-
-    def GetComponentList(self, board_name: str, node_type: str, return_json: bool):
-        get_components_list_api = self.scisdk_dll.SCISDK_GetComponentList
-        get_components_list_api.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p), ctypes.c_bool, ctypes.c_void_p]
-        get_components_list_api.restype = ctypes.c_int
-        # convert string to bytes array
-        board_name_b = board_name.encode('utf-8')
-        node_type_b = node_type.encode('utf-8')
-        ret_string_char_ptr = ctypes.c_char_p()
-        # call C lib function
-        err = get_components_list_api(ctypes.c_char_p(board_name_b), ctypes.c_char_p(node_type_b), ctypes.byref(ret_string_char_ptr), ctypes.c_bool(return_json), self.lib_ptr)
-        return err, ret_string_char_ptr.value.decode('utf-8')
-
-    def s_error(self, value: int) -> int:
-        s_error_api = self.scisdk_dll.SCISDK_s_error
-        s_error_api.argtypes = [ctypes.c_int, ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
-        s_error_api.restype = ctypes.c_int
-        # convert string to bytes array
-        ret_string_char_ptr = ctypes.c_char_p()
-        err = s_error_api(ctypes.c_int(value), ctypes.byref(ret_string_char_ptr),self.lib_ptr)
-        return err, ret_string_char_ptr.value.decode('utf-8')
-
-    def SetParameterInteger(self, path: str, val: int) -> int:
-        set_parameter_api = self.scisdk_dll.SCISDK_SetParameterInteger
-        set_parameter_api.argtypes = [ctypes.c_char_p, ctypes.c_int, ctypes.c_void_p]
-        set_parameter_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        # call C lib function
-        err = set_parameter_api(ctypes.c_char_p(path_b), val, self.lib_ptr)
-        return err
-
-    def GetParameterInteger(self, path: str):
-        get_parameter_api = self.scisdk_dll.SCISDK_GetParameterInteger
-        get_parameter_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_int), ctypes.c_void_p]
-        get_parameter_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        ret_int = ctypes.c_int()
-        # call C lib function
-        err = get_parameter_api(ctypes.c_char_p(path_b), ctypes.byref(ret_int), self.lib_ptr)
-        return err, ret_int.value
-
-    def SetParameterString(self, path: str, value: str):
-        set_parameter_api = self.scisdk_dll.SCISDK_SetParameterString
-        set_parameter_api.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.c_void_p]
-        set_parameter_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        value_b = value.encode('utf-8')
-        # call C lib function
-        err = set_parameter_api(ctypes.c_char_p(path_b), ctypes.c_char_p(value_b), self.lib_ptr)
-        return err
-
-    def GetParameterString(self, path: str):
-        get_parameter_api = self.scisdk_dll.SCISDK_GetParameterString
-        get_parameter_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
-        get_parameter_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        value_b = ctypes.c_char_p()
-        # call C lib function
-        err = get_parameter_api(ctypes.c_char_p(path_b), ctypes.byref(value_b), self.lib_ptr)
-        return err, value_b.value.decode('utf-8')
-
-    def SetParameterDouble(self, path: str, value: float):
-        set_parameter_api = self.scisdk_dll.SCISDK_SetParameterDouble
-        set_parameter_api.argtypes = [ctypes.c_char_p, ctypes.c_double, ctypes.c_void_p]
-        set_parameter_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        # call C lib function
-        err = set_parameter_api(ctypes.c_char_p(path_b), ctypes.c_double(value), self.lib_ptr)
-        return err
-
-    def GetParameterDouble(self, path:str):
-        get_parameter_api = self.scisdk_dll.SCISDK_SetParameterDouble
-        get_parameter_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_double), ctypes.c_void_p]
-        get_parameter_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        value = ctypes.c_double()
-        # call C lib function
-        err = get_parameter_api(ctypes.c_char_p(path_b), ctypes.POINTER(value), self.lib_ptr)
-        return err, value.value
-
-    def AllocateBuffer(self, path: str, size = None):
-        buffer_pointer = None
-        buffer_type = 0
-        res, type = self.GetParameterString(path+".buffer_type")
-        if(res == 0):
-            if type == "SCISDK_OSCILLOSCOPE_DECODED_BUFFER":
-                buffer_pointer = ctypes.POINTER(OscilloscopeDecodedBuffer)
-                buffer_type = 1
-            elif type == "SCISDK_OSCILLOSCOPE_RAW_BUFFER":
-                buffer_pointer = ctypes.POINTER(OscilloscopeRawBuffer)
-            elif type == "SCISDK_OSCILLOSCOPE_DUAL_DECODED_BUFFER":
-                buffer_pointer = ctypes.POINTER(OscilloscopeDualDecodedBuffer)
-                buffer_type = 1
-            elif type == "SCISDK_OSCILLOSCOPE_DUAL_RAW_BUFFER":
-                buffer_pointer = ctypes.POINTER(OscilloscopeDualRawBuffer)
-            elif type == "SCISDK_DIGITIZER_DECODED_BUFFER":
-                buffer_pointer = ctypes.POINTER(DigitizerDecodedBuffer)
-                buffer_type = 1
-            elif type == "SCISDK_LIST_RAW_BUFFER":
-                buffer_pointer = ctypes.POINTER(ListRawBuffer)
-            elif type == "SCISDK_CP_DECODED_BUFFER":
-                buffer_pointer = ctypes.POINTER(CustomPacketDecodedBuffer)
-                buffer_type = 1
-            elif type == "SCISDK_CP_RAW_BUFFER":
-                buffer_pointer = ctypes.POINTER(CustomPacketRawBuffer)
-            elif type == "SCISDK_RM_RAW_BUFFER":
-                buffer_pointer = ctypes.POINTER(RatemeterRawBuffer)
-            elif type == "SCISDK_SPECTRUM_DECODED_BUFFER":
-                buffer_pointer = ctypes.POINTER(SpectrumDecodedBuffer)
-                buffer_type = 1
-            elif type == "SCISDK_FFT_DECODED_BUFFER":
-                buffer_pointer = ctypes.POINTER(FFTDecodedBuffer)
-                buffer_type = 1
-            elif type == "SCISDK_FFT_RAW_BUFFER":
-                buffer_pointer = ctypes.POINTER(FFTRawBuffer)
-            elif type == "SCISDK_FRAME_DECODED_BUFFER":
-                buffer_pointer = ctypes.POINTER(FramePacketDecodedBuffer)
-                buffer_type = 1
-            elif type == "SCISDK_FRAME_RAW_BUFFER":
-                buffer_pointer = ctypes.POINTER(FramePacketRawBuffer)
-            elif type == "SCISDK_CITIROC_DECODED_BUFFER":
-                buffer_pointer = ctypes.POINTER(CitirocDecodedBuffer)
-                buffer_type = 1
-            elif type == "SCISDK_CITIROC_RAW_BUFFER":
-                buffer_pointer = ctypes.POINTER(CitirocRawBuffer)
-            elif type == "SCISDK_PETIROC_DECODED_BUFFER":
-                buffer_pointer = ctypes.POINTER(PetirocDecodedBuffer)
-                buffer_type = 1
-            elif type == "SCISDK_PETIROC_RAW_BUFFER":
-                buffer_pointer = ctypes.POINTER(PetirocRawBuffer)      
-            elif type == "SCISDK_FE_SCOPE_EVENT":
-                buffer_pointer = ctypes.POINTER(FEScopePacket)
-            elif type == "SCISDK_FE_OPENDPP_EVENT":
-                buffer_pointer = ctypes.POINTER(FEOpenDppPacket)      
-            else:
-                raise Exception("Isn't a valid buffer type") 
-
-            if size == None:
-                allocate_buffer_api = self.scisdk_dll.SCISDK_AllocateBuffer
-                allocate_buffer_api.argtypes = [ctypes.c_char_p, ctypes.c_int, ctypes.POINTER(buffer_pointer), ctypes.c_void_p]    
-                allocate_buffer_api.restype = ctypes.c_int
-                # convert string to bytes array
-                path_b = path.encode('utf-8')
-                # call C lib function
-                buf_tmp = buffer_pointer()
-                err = allocate_buffer_api(ctypes.c_char_p(path_b), ctypes.c_int(buffer_type), ctypes.byref(buf_tmp), self.lib_ptr)
-                if err == 0:
-                    buffer = buf_tmp.contents
-                    return err, buffer   
-                else:
-                    return err, None
-            else:
-                allocate_buffer_api = self.scisdk_dll.SCISDK_AllocateBufferSize
-                allocate_buffer_api.argtypes = [ctypes.c_char_p, ctypes.c_int, ctypes.POINTER(buffer_pointer), ctypes.c_void_p, ctypes.c_int]    
-                allocate_buffer_api.restype = ctypes.c_int
-                # convert string to bytes array
-                path_b = path.encode('utf-8')
-                # call C lib function
-                buf_tmp = buffer_pointer()
-                err = allocate_buffer_api(ctypes.c_char_p(path_b), ctypes.c_int(buffer_type), ctypes.byref(buf_tmp), self.lib_ptr, size)
-                if err == 0:
-                    buffer = buf_tmp.contents
-                    return err, buffer
-                else:
-                    return err, None
-
-
-    # read data
-    def ReadData(self, path: str, buffer):
-        read_data_api = self.scisdk_dll.SCISDK_ReadData
-        if type(buffer) == OscilloscopeDecodedBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(OscilloscopeDecodedBuffer), ctypes.c_void_p]    
-        elif type(buffer) == OscilloscopeRawBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(OscilloscopeRawBuffer), ctypes.c_void_p]    
-        elif type(buffer) == OscilloscopeDualDecodedBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(OscilloscopeDualDecodedBuffer), ctypes.c_void_p]    
-        elif type(buffer) == OscilloscopeDualRawBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(OscilloscopeDualRawBuffer), ctypes.c_void_p]    
-        elif type(buffer) == DigitizerDecodedBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(DigitizerDecodedBuffer), ctypes.c_void_p]    
-        elif type(buffer) == ListRawBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ListRawBuffer), ctypes.c_void_p]    
-        elif type(buffer) == CustomPacketDecodedBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(CustomPacketDecodedBuffer), ctypes.c_void_p]    
-        elif type(buffer) == CustomPacketRawBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(CustomPacketRawBuffer), ctypes.c_void_p]    
-        elif type(buffer) == RatemeterRawBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(RatemeterRawBuffer), ctypes.c_void_p]    
-        elif type(buffer) == SpectrumDecodedBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(SpectrumDecodedBuffer), ctypes.c_void_p]    
-        elif type(buffer) == FFTDecodedBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(FFTDecodedBuffer), ctypes.c_void_p]    
-        elif type(buffer) == FFTRawBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(FFTRawBuffer), ctypes.c_void_p]  
-        elif type(buffer) == FramePacketDecodedBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(FramePacketDecodedBuffer), ctypes.c_void_p]   
-        elif type(buffer) == FramePacketRawBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(FramePacketRawBuffer), ctypes.c_void_p]      
-        elif type(buffer) == CitirocDecodedBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(CitirocDecodedBuffer), ctypes.c_void_p]    
-        elif type(buffer) == CitirocRawBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(CitirocRawBuffer), ctypes.c_void_p]    
-        elif type(buffer) == PetirocDecodedBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(PetirocDecodedBuffer), ctypes.c_void_p]    
-        elif type(buffer) == PetirocRawBuffer:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(PetirocRawBuffer), ctypes.c_void_p]    
-        elif type(buffer) == FEScopePacket:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(FEScopePacket), ctypes.c_void_p]    
-        elif type(buffer) == FEOpenDppPacket:
-            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(FEOpenDppPacket), ctypes.c_void_p]    
-        else:
-            raise Exception(type(buffer).__name__ + " isn't a valid buffer type") 
-
-        read_data_api = self.scisdk_dll.SCISDK_ReadData
-        read_data_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        err = read_data_api(ctypes.c_char_p(path_b), ctypes.byref(buffer), self.lib_ptr)
-        return err, buffer
-
-    def FreeBuffer(self, path: str, buffer):
-        free_buffer_api = self.scisdk_dll.SCISDK_FreeBuffer
-        buffer_pointer = None
-        buffer_type = 0
-        if type(buffer) == OscilloscopeDecodedBuffer:
-            buffer_pointer = ctypes.POINTER(OscilloscopeDecodedBuffer)
-            buffer_type = 1
-        elif type(buffer) == OscilloscopeRawBuffer:
-            buffer_pointer = ctypes.POINTER(OscilloscopeRawBuffer)
-        elif type(buffer) == OscilloscopeDualDecodedBuffer:
-            buffer_pointer = ctypes.POINTER(OscilloscopeDualDecodedBuffer)
-            buffer_type = 1
-        elif type(buffer) == OscilloscopeDualRawBuffer:
-            buffer_pointer = ctypes.POINTER(OscilloscopeDualRawBuffer)
-        elif type(buffer) == DigitizerDecodedBuffer:
-            buffer_pointer = ctypes.POINTER(DigitizerDecodedBuffer)
-            buffer_type = 1
-        elif type(buffer) == ListRawBuffer:
-            buffer_pointer = ctypes.POINTER(ListRawBuffer)
-        elif type(buffer) == CustomPacketDecodedBuffer:
-            buffer_pointer = ctypes.POINTER(CustomPacketDecodedBuffer)
-            buffer_type = 1
-        elif type(buffer) == CustomPacketRawBuffer:
-            buffer_pointer = ctypes.POINTER(CustomPacketRawBuffer)
-        elif type(buffer) == RatemeterRawBuffer:
-            buffer_pointer = ctypes.POINTER(RatemeterRawBuffer)
-        elif type(buffer) == SpectrumDecodedBuffer:
-            buffer_pointer = ctypes.POINTER(SpectrumDecodedBuffer)
-            buffer_type = 1
-        elif type(buffer) == FFTDecodedBuffer:
-            buffer_pointer = ctypes.POINTER(FFTDecodedBuffer)
-            buffer_type = 1
-        elif type(buffer) == FFTRawBuffer:
-            buffer_pointer = ctypes.POINTER(FFTRawBuffer)
-        elif type(buffer) == FramePacketDecodedBuffer:
-            buffer_pointer = ctypes.POINTER(FramePacketDecodedBuffer)
-            buffer_type = 1
-        elif type(buffer) == FramePacketRawBuffer:
-            buffer_pointer = ctypes.POINTER(FramePacketRawBuffer)
-        elif type(buffer) == CitirocDecodedBuffer:
-            buffer_pointer = ctypes.POINTER(CitirocDecodedBuffer)
-            buffer_type = 1
-        elif type(buffer) == CitirocRawBuffer:
-            buffer_pointer = ctypes.POINTER(CitirocRawBuffer)
-        elif type(buffer) == PetirocDecodedBuffer:
-            buffer_pointer = ctypes.POINTER(PetirocDecodedBuffer)
-            buffer_type = 1
-        elif type(buffer) == PetirocRawBuffer:
-            buffer_pointer = ctypes.POINTER(PetirocRawBuffer)
-        elif type(buffer) == FEScopePacket:
-            buffer_pointer = ctypes.POINTER(FEScopePacket)
-        elif type(buffer) == FEOpenDppPacket:
-            buffer_pointer = ctypes.POINTER(FEOpenDppPacket)
-        else:
-            raise Exception(type(buffer).__name__ + " isn't a valid buffer type") 
-
-        free_buffer_api.argtypes = [ctypes.c_char_p, ctypes.c_int, ctypes.POINTER(buffer_pointer), ctypes.c_void_p]    
-        free_buffer_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        # call C lib function
-        buf_tmp = buffer_pointer(buffer)
-        err = free_buffer_api(ctypes.c_char_p(path_b), ctypes.c_int(buffer_type), ctypes.byref(buf_tmp), self.lib_ptr)
-        return err
-
-    def ExecuteCommand(self, path: str, value: str):
-        execute_command_api = self.scisdk_dll.SCISDK_ExecuteCommand
-        execute_command_api.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.c_void_p]    
-        execute_command_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        value_b = value.encode('utf-8')
-        # call C lib function
-        err = execute_command_api(ctypes.c_char_p(path_b), ctypes.c_char_p(value_b), self.lib_ptr)
-        return err
-
-    def DecodeData(self, path: str, buffer_in: OscilloscopeRawBuffer):
-        decode_data_api = self.scisdk_dll.SCISDK_DecodeData
-        decode_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(OscilloscopeRawBuffer), ctypes.POINTER(OscilloscopeDecodedBuffer), ctypes.c_void_p]
-        decode_data_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        # call C lib function
-        buffer_out = OscilloscopeDecodedBuffer()
-        err = decode_data_api(ctypes.c_char_p(path_b), ctypes.byref(buffer_in), ctypes.byref(buffer_out), self.lib_ptr)
-        return err, buffer_out
-
-    def SetRegister(self, path: str, value: int):
-        set_register_api = self.scisdk_dll.SCISDK_SetRegister
-        set_register_api.argtypes = [ctypes.c_char_p, ctypes.c_int, ctypes.c_void_p]
-        set_register_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        # call C lib function
-        err = set_register_api(ctypes.c_char_p(path_b), value, self.lib_ptr)
-        return err
-
-    def GetRegister(self, path: str):
-        get_register_api = self.scisdk_dll.SCISDK_GetRegister
-        get_register_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_int), ctypes.c_void_p]
-        get_register_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        ret_int = ctypes.c_int()
-        # call C lib function
-        err = get_register_api(ctypes.c_char_p(path_b), ctypes.byref(ret_int), self.lib_ptr)
-        return err, ret_int.value
-
-    def GetAllParameters(self, path: str):
-        get_all_parameters_api = self.scisdk_dll.SCISDK_GetAllParameters
-        get_all_parameters_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
-        get_all_parameters_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        ret_char_p = ctypes.c_char_p()
-        # call C lib function
-        err = get_all_parameters_api(ctypes.c_char_p(path_b), ctypes.byref(ret_char_p), self.lib_ptr)
-        return err, ret_char_p.value.decode('utf-8')
-
-    def GetParameterDescription(self, path: str):
-        get_parameter_description_api = self.scisdk_dll.SCISDK_GetParameterDescription
-        get_parameter_description_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
-        get_parameter_description_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        ret_char_p = ctypes.c_char_p()
-        # call C lib function
-        err = get_parameter_description_api(ctypes.c_char_p(path_b), ctypes.byref(ret_char_p), self.lib_ptr)
-        return err, ret_char_p.value.decode('utf-8')
-
-    def GetParameterListOfValues(self, path: str):
-        get_parameter_list_of_values_api = self.scisdk_dll.SCISDK_GetParameterListOfValues
-        get_parameter_list_of_values_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
-        get_parameter_list_of_values_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        ret_char_p = ctypes.c_char_p()
-        # call C lib function
-        err = get_parameter_list_of_values_api(ctypes.c_char_p(path_b), ctypes.byref(ret_char_p), self.lib_ptr)
-        return err, ret_char_p.value.decode('utf-8')
-
-    def GetParameterMinimumValue(self, path: str):
-        get_parameters_min_value_api = self.scisdk_dll.SCISDK_GetParameterMinimumValue
-        get_parameters_min_value_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_double), ctypes.c_void_p]
-        get_parameters_min_value_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        ret_double_p = ctypes.c_double()
-        # call C lib function
-        err = get_parameters_min_value_api(ctypes.c_char_p(path_b), ctypes.byref(ret_double_p), self.lib_ptr)
-        return err, ret_double_p.value
-
-    def GetParameterMaximumValue(self, path: str):
-        get_parameters_max_value_api = self.scisdk_dll.SCISDK_GetParameterMaximumValue
-        get_parameters_max_value_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_double), ctypes.c_void_p]
-        get_parameters_max_value_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        ret_double_p = ctypes.c_double()
-        # call C lib function
-        err = get_parameters_max_value_api(ctypes.c_char_p(path_b), ctypes.byref(ret_double_p), self.lib_ptr)
-        return err, ret_double_p.value
-
-    def GetParametersProperties(self, path: str):
-        get_parameters_properties_api = self.scisdk_dll.SCISDK_GetParametersProperties
-        get_parameters_properties_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
-        get_parameters_properties_api.restype = ctypes.c_int
-        # convert string to bytes array
-        path_b = path.encode('utf-8')
-        ret_char_p = ctypes.c_char_p()
-        # call C lib function
-        err = get_parameters_properties_api(ctypes.c_char_p(path_b), ctypes.byref(ret_char_p), self.lib_ptr)
-        return err, ret_char_p.value.decode('utf-8')
-
-    def FreeLib(self):
-        free_lib_api = self.scisdk_dll.SCISDK_FreeLib
-        free_lib_api.argtypes = [ctypes.c_void_p]
-        free_lib_api.restype = ctypes.c_int
-        # call C lib function
-        err = free_lib_api(self.lib_ptr)
-        return err
+import ctypes
+import os
+from scisdk.scisdk_defines import *
+
+
+class SciSDK:
+    scisdk_dll = None
+    lib_ptr = None
+    libname = None
+
+    def __init__(self) -> None:
+        #os.path.dirname(__file__) + "\\
+        libname = ""
+
+        if os.name == 'nt':
+            self.libname = "SciSDK_DLL.dll"
+        else:
+            self.libname = "libscisdk.so"
+
+        try:
+            self.scisdk_dll = ctypes.CDLL(self.libname)
+        except OSError as e:
+            if e.errno == os.errno.ENOENT:
+                print("Error: " + self.libname + " not found")
+            elif e.errno == os.errno.EINVAL:
+                print("Error: " + self.libname + " has the wrong architecture for the current process")
+            elif e.errno == os.errno.ELIBBAD:
+                print("Error:" + self.libname + " has missing dependencies")
+            else:
+                print("Error: unable to load libscisdk.so: " + str(e))
+            
+
+
+
+        init_lib_api = self.scisdk_dll.SCISDK_InitLib
+        init_lib_api.restype = ctypes.c_void_p
+        self.lib_ptr = init_lib_api()
+        
+        
+    def AddNewDevice(self, device_path: str, device_model: str, json_file_path: str, name: str) -> int:
+        add_new_device_api = self.scisdk_dll.SCISDK_AddNewDevice
+        add_new_device_api.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_void_p]
+        add_new_device_api.restype = ctypes.c_int
+        # convert strings to bytes array
+        b_device_path = device_path.encode('utf-8')
+        b_device_model = device_model.encode('utf-8')
+        b_json_file_path = json_file_path.encode('utf-8')
+        b_name = name.encode('utf-8')
+        # call C lib function
+        err = add_new_device_api(b_device_path, b_device_model, b_json_file_path, b_name, self.lib_ptr)
+        return err
+        
+    def DetachDevice(self, name: str) -> int:
+        detach_device_api = self.scisdk_dll.SCISDK_DetachDevice
+        detach_device_api.argtypes = [ctypes.c_char_p, ctypes.c_void_p]
+        detach_device_api.restype = ctypes.c_int
+        # convert string to bytes array
+        b_name = name.encode('utf-8')
+        # call C lib function
+        err = detach_device_api(b_name, self.lib_ptr)
+        return err
+
+    def GetComponentList(self, board_name: str, node_type: str, return_json: bool):
+        get_components_list_api = self.scisdk_dll.SCISDK_GetComponentList
+        get_components_list_api.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p), ctypes.c_bool, ctypes.c_void_p]
+        get_components_list_api.restype = ctypes.c_int
+        # convert string to bytes array
+        board_name_b = board_name.encode('utf-8')
+        node_type_b = node_type.encode('utf-8')
+        ret_string_char_ptr = ctypes.c_char_p()
+        # call C lib function
+        err = get_components_list_api(ctypes.c_char_p(board_name_b), ctypes.c_char_p(node_type_b), ctypes.byref(ret_string_char_ptr), ctypes.c_bool(return_json), self.lib_ptr)
+        return err, ret_string_char_ptr.value.decode('utf-8')
+
+    def s_error(self, value: int) -> int:
+        s_error_api = self.scisdk_dll.SCISDK_s_error
+        s_error_api.argtypes = [ctypes.c_int, ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
+        s_error_api.restype = ctypes.c_int
+        # convert string to bytes array
+        ret_string_char_ptr = ctypes.c_char_p()
+        err = s_error_api(ctypes.c_int(value), ctypes.byref(ret_string_char_ptr),self.lib_ptr)
+        return err, ret_string_char_ptr.value.decode('utf-8')
+
+    def SetParameterInteger(self, path: str, val: int) -> int:
+        set_parameter_api = self.scisdk_dll.SCISDK_SetParameterInteger
+        set_parameter_api.argtypes = [ctypes.c_char_p, ctypes.c_int, ctypes.c_void_p]
+        set_parameter_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        # call C lib function
+        err = set_parameter_api(ctypes.c_char_p(path_b), val, self.lib_ptr)
+        return err
+
+    def GetParameterInteger(self, path: str):
+        get_parameter_api = self.scisdk_dll.SCISDK_GetParameterInteger
+        get_parameter_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_int), ctypes.c_void_p]
+        get_parameter_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        ret_int = ctypes.c_int()
+        # call C lib function
+        err = get_parameter_api(ctypes.c_char_p(path_b), ctypes.byref(ret_int), self.lib_ptr)
+        return err, ret_int.value
+
+    def SetParameterString(self, path: str, value: str):
+        set_parameter_api = self.scisdk_dll.SCISDK_SetParameterString
+        set_parameter_api.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.c_void_p]
+        set_parameter_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        value_b = value.encode('utf-8')
+        # call C lib function
+        err = set_parameter_api(ctypes.c_char_p(path_b), ctypes.c_char_p(value_b), self.lib_ptr)
+        return err
+
+    def GetParameterString(self, path: str):
+        get_parameter_api = self.scisdk_dll.SCISDK_GetParameterString
+        get_parameter_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
+        get_parameter_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        value_b = ctypes.c_char_p()
+        # call C lib function
+        err = get_parameter_api(ctypes.c_char_p(path_b), ctypes.byref(value_b), self.lib_ptr)
+        return err, value_b.value.decode('utf-8')
+
+    def SetParameterDouble(self, path: str, value: float):
+        set_parameter_api = self.scisdk_dll.SCISDK_SetParameterDouble
+        set_parameter_api.argtypes = [ctypes.c_char_p, ctypes.c_double, ctypes.c_void_p]
+        set_parameter_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        # call C lib function
+        err = set_parameter_api(ctypes.c_char_p(path_b), ctypes.c_double(value), self.lib_ptr)
+        return err
+
+    def GetParameterDouble(self, path:str):
+        get_parameter_api = self.scisdk_dll.SCISDK_SetParameterDouble
+        get_parameter_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_double), ctypes.c_void_p]
+        get_parameter_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        value = ctypes.c_double()
+        # call C lib function
+        err = get_parameter_api(ctypes.c_char_p(path_b), ctypes.POINTER(value), self.lib_ptr)
+        return err, value.value
+
+    def AllocateBuffer(self, path: str, size = None):
+        buffer_pointer = None
+        buffer_type = 0
+        res, type = self.GetParameterString(path+".buffer_type")
+        if(res == 0):
+            if type == "SCISDK_OSCILLOSCOPE_DECODED_BUFFER":
+                buffer_pointer = ctypes.POINTER(OscilloscopeDecodedBuffer)
+                buffer_type = 1
+            elif type == "SCISDK_OSCILLOSCOPE_RAW_BUFFER":
+                buffer_pointer = ctypes.POINTER(OscilloscopeRawBuffer)
+            elif type == "SCISDK_OSCILLOSCOPE_DUAL_DECODED_BUFFER":
+                buffer_pointer = ctypes.POINTER(OscilloscopeDualDecodedBuffer)
+                buffer_type = 1
+            elif type == "SCISDK_OSCILLOSCOPE_DUAL_RAW_BUFFER":
+                buffer_pointer = ctypes.POINTER(OscilloscopeDualRawBuffer)
+            elif type == "SCISDK_DIGITIZER_DECODED_BUFFER":
+                buffer_pointer = ctypes.POINTER(DigitizerDecodedBuffer)
+                buffer_type = 1
+            elif type == "SCISDK_LIST_RAW_BUFFER":
+                buffer_pointer = ctypes.POINTER(ListRawBuffer)
+            elif type == "SCISDK_CP_DECODED_BUFFER":
+                buffer_pointer = ctypes.POINTER(CustomPacketDecodedBuffer)
+                buffer_type = 1
+            elif type == "SCISDK_CP_RAW_BUFFER":
+                buffer_pointer = ctypes.POINTER(CustomPacketRawBuffer)
+            elif type == "SCISDK_RM_RAW_BUFFER":
+                buffer_pointer = ctypes.POINTER(RatemeterRawBuffer)
+            elif type == "SCISDK_SPECTRUM_DECODED_BUFFER":
+                buffer_pointer = ctypes.POINTER(SpectrumDecodedBuffer)
+                buffer_type = 1
+            elif type == "SCISDK_FFT_DECODED_BUFFER":
+                buffer_pointer = ctypes.POINTER(FFTDecodedBuffer)
+                buffer_type = 1
+            elif type == "SCISDK_FFT_RAW_BUFFER":
+                buffer_pointer = ctypes.POINTER(FFTRawBuffer)
+            elif type == "SCISDK_FRAME_DECODED_BUFFER":
+                buffer_pointer = ctypes.POINTER(FramePacketDecodedBuffer)
+                buffer_type = 1
+            elif type == "SCISDK_FRAME_RAW_BUFFER":
+                buffer_pointer = ctypes.POINTER(FramePacketRawBuffer)
+            elif type == "SCISDK_CITIROC_DECODED_BUFFER":
+                buffer_pointer = ctypes.POINTER(CitirocDecodedBuffer)
+                buffer_type = 1
+            elif type == "SCISDK_CITIROC_RAW_BUFFER":
+                buffer_pointer = ctypes.POINTER(CitirocRawBuffer)
+            elif type == "SCISDK_PETIROC_DECODED_BUFFER":
+                buffer_pointer = ctypes.POINTER(PetirocDecodedBuffer)
+                buffer_type = 1
+            elif type == "SCISDK_PETIROC_RAW_BUFFER":
+                buffer_pointer = ctypes.POINTER(PetirocRawBuffer)      
+            elif type == "SCISDK_FE_SCOPE_EVENT":
+                buffer_pointer = ctypes.POINTER(FEScopePacket)
+            elif type == "SCISDK_FE_OPENDPP_EVENT":
+                buffer_pointer = ctypes.POINTER(FEOpenDppPacket)      
+            else:
+                raise Exception("Isn't a valid buffer type") 
+
+            if size == None:
+                allocate_buffer_api = self.scisdk_dll.SCISDK_AllocateBuffer
+                allocate_buffer_api.argtypes = [ctypes.c_char_p, ctypes.c_int, ctypes.POINTER(buffer_pointer), ctypes.c_void_p]    
+                allocate_buffer_api.restype = ctypes.c_int
+                # convert string to bytes array
+                path_b = path.encode('utf-8')
+                # call C lib function
+                buf_tmp = buffer_pointer()
+                err = allocate_buffer_api(ctypes.c_char_p(path_b), ctypes.c_int(buffer_type), ctypes.byref(buf_tmp), self.lib_ptr)
+                if err == 0:
+                    buffer = buf_tmp.contents
+                    return err, buffer   
+                else:
+                    return err, None
+            else:
+                allocate_buffer_api = self.scisdk_dll.SCISDK_AllocateBufferSize
+                allocate_buffer_api.argtypes = [ctypes.c_char_p, ctypes.c_int, ctypes.POINTER(buffer_pointer), ctypes.c_void_p, ctypes.c_int]    
+                allocate_buffer_api.restype = ctypes.c_int
+                # convert string to bytes array
+                path_b = path.encode('utf-8')
+                # call C lib function
+                buf_tmp = buffer_pointer()
+                err = allocate_buffer_api(ctypes.c_char_p(path_b), ctypes.c_int(buffer_type), ctypes.byref(buf_tmp), self.lib_ptr, size)
+                if err == 0:
+                    buffer = buf_tmp.contents
+                    return err, buffer
+                else:
+                    return err, None
+
+
+    # read data
+    def ReadData(self, path: str, buffer):
+        read_data_api = self.scisdk_dll.SCISDK_ReadData
+        if type(buffer) == OscilloscopeDecodedBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(OscilloscopeDecodedBuffer), ctypes.c_void_p]    
+        elif type(buffer) == OscilloscopeRawBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(OscilloscopeRawBuffer), ctypes.c_void_p]    
+        elif type(buffer) == OscilloscopeDualDecodedBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(OscilloscopeDualDecodedBuffer), ctypes.c_void_p]    
+        elif type(buffer) == OscilloscopeDualRawBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(OscilloscopeDualRawBuffer), ctypes.c_void_p]    
+        elif type(buffer) == DigitizerDecodedBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(DigitizerDecodedBuffer), ctypes.c_void_p]    
+        elif type(buffer) == ListRawBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ListRawBuffer), ctypes.c_void_p]    
+        elif type(buffer) == CustomPacketDecodedBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(CustomPacketDecodedBuffer), ctypes.c_void_p]    
+        elif type(buffer) == CustomPacketRawBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(CustomPacketRawBuffer), ctypes.c_void_p]    
+        elif type(buffer) == RatemeterRawBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(RatemeterRawBuffer), ctypes.c_void_p]    
+        elif type(buffer) == SpectrumDecodedBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(SpectrumDecodedBuffer), ctypes.c_void_p]    
+        elif type(buffer) == FFTDecodedBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(FFTDecodedBuffer), ctypes.c_void_p]    
+        elif type(buffer) == FFTRawBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(FFTRawBuffer), ctypes.c_void_p]  
+        elif type(buffer) == FramePacketDecodedBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(FramePacketDecodedBuffer), ctypes.c_void_p]   
+        elif type(buffer) == FramePacketRawBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(FramePacketRawBuffer), ctypes.c_void_p]      
+        elif type(buffer) == CitirocDecodedBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(CitirocDecodedBuffer), ctypes.c_void_p]    
+        elif type(buffer) == CitirocRawBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(CitirocRawBuffer), ctypes.c_void_p]    
+        elif type(buffer) == PetirocDecodedBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(PetirocDecodedBuffer), ctypes.c_void_p]    
+        elif type(buffer) == PetirocRawBuffer:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(PetirocRawBuffer), ctypes.c_void_p]    
+        elif type(buffer) == FEScopePacket:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(FEScopePacket), ctypes.c_void_p]    
+        elif type(buffer) == FEOpenDppPacket:
+            read_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(FEOpenDppPacket), ctypes.c_void_p]    
+        else:
+            raise Exception(type(buffer).__name__ + " isn't a valid buffer type") 
+
+        read_data_api = self.scisdk_dll.SCISDK_ReadData
+        read_data_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        err = read_data_api(ctypes.c_char_p(path_b), ctypes.byref(buffer), self.lib_ptr)
+        return err, buffer
+
+    def FreeBuffer(self, path: str, buffer):
+        free_buffer_api = self.scisdk_dll.SCISDK_FreeBuffer
+        buffer_pointer = None
+        buffer_type = 0
+        if type(buffer) == OscilloscopeDecodedBuffer:
+            buffer_pointer = ctypes.POINTER(OscilloscopeDecodedBuffer)
+            buffer_type = 1
+        elif type(buffer) == OscilloscopeRawBuffer:
+            buffer_pointer = ctypes.POINTER(OscilloscopeRawBuffer)
+        elif type(buffer) == OscilloscopeDualDecodedBuffer:
+            buffer_pointer = ctypes.POINTER(OscilloscopeDualDecodedBuffer)
+            buffer_type = 1
+        elif type(buffer) == OscilloscopeDualRawBuffer:
+            buffer_pointer = ctypes.POINTER(OscilloscopeDualRawBuffer)
+        elif type(buffer) == DigitizerDecodedBuffer:
+            buffer_pointer = ctypes.POINTER(DigitizerDecodedBuffer)
+            buffer_type = 1
+        elif type(buffer) == ListRawBuffer:
+            buffer_pointer = ctypes.POINTER(ListRawBuffer)
+        elif type(buffer) == CustomPacketDecodedBuffer:
+            buffer_pointer = ctypes.POINTER(CustomPacketDecodedBuffer)
+            buffer_type = 1
+        elif type(buffer) == CustomPacketRawBuffer:
+            buffer_pointer = ctypes.POINTER(CustomPacketRawBuffer)
+        elif type(buffer) == RatemeterRawBuffer:
+            buffer_pointer = ctypes.POINTER(RatemeterRawBuffer)
+        elif type(buffer) == SpectrumDecodedBuffer:
+            buffer_pointer = ctypes.POINTER(SpectrumDecodedBuffer)
+            buffer_type = 1
+        elif type(buffer) == FFTDecodedBuffer:
+            buffer_pointer = ctypes.POINTER(FFTDecodedBuffer)
+            buffer_type = 1
+        elif type(buffer) == FFTRawBuffer:
+            buffer_pointer = ctypes.POINTER(FFTRawBuffer)
+        elif type(buffer) == FramePacketDecodedBuffer:
+            buffer_pointer = ctypes.POINTER(FramePacketDecodedBuffer)
+            buffer_type = 1
+        elif type(buffer) == FramePacketRawBuffer:
+            buffer_pointer = ctypes.POINTER(FramePacketRawBuffer)
+        elif type(buffer) == CitirocDecodedBuffer:
+            buffer_pointer = ctypes.POINTER(CitirocDecodedBuffer)
+            buffer_type = 1
+        elif type(buffer) == CitirocRawBuffer:
+            buffer_pointer = ctypes.POINTER(CitirocRawBuffer)
+        elif type(buffer) == PetirocDecodedBuffer:
+            buffer_pointer = ctypes.POINTER(PetirocDecodedBuffer)
+            buffer_type = 1
+        elif type(buffer) == PetirocRawBuffer:
+            buffer_pointer = ctypes.POINTER(PetirocRawBuffer)
+        elif type(buffer) == FEScopePacket:
+            buffer_pointer = ctypes.POINTER(FEScopePacket)
+        elif type(buffer) == FEOpenDppPacket:
+            buffer_pointer = ctypes.POINTER(FEOpenDppPacket)
+        else:
+            raise Exception(type(buffer).__name__ + " isn't a valid buffer type") 
+
+        free_buffer_api.argtypes = [ctypes.c_char_p, ctypes.c_int, ctypes.POINTER(buffer_pointer), ctypes.c_void_p]    
+        free_buffer_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        # call C lib function
+        buf_tmp = buffer_pointer(buffer)
+        err = free_buffer_api(ctypes.c_char_p(path_b), ctypes.c_int(buffer_type), ctypes.byref(buf_tmp), self.lib_ptr)
+        return err
+
+    def ExecuteCommand(self, path: str, value: str):
+        execute_command_api = self.scisdk_dll.SCISDK_ExecuteCommand
+        execute_command_api.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.c_void_p]    
+        execute_command_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        value_b = value.encode('utf-8')
+        # call C lib function
+        err = execute_command_api(ctypes.c_char_p(path_b), ctypes.c_char_p(value_b), self.lib_ptr)
+        return err
+
+    def DecodeData(self, path: str, buffer_in: OscilloscopeRawBuffer):
+        decode_data_api = self.scisdk_dll.SCISDK_DecodeData
+        decode_data_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(OscilloscopeRawBuffer), ctypes.POINTER(OscilloscopeDecodedBuffer), ctypes.c_void_p]
+        decode_data_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        # call C lib function
+        buffer_out = OscilloscopeDecodedBuffer()
+        err = decode_data_api(ctypes.c_char_p(path_b), ctypes.byref(buffer_in), ctypes.byref(buffer_out), self.lib_ptr)
+        return err, buffer_out
+
+    def SetRegister(self, path: str, value: int):
+        set_register_api = self.scisdk_dll.SCISDK_SetRegister
+        set_register_api.argtypes = [ctypes.c_char_p, ctypes.c_int, ctypes.c_void_p]
+        set_register_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        # call C lib function
+        err = set_register_api(ctypes.c_char_p(path_b), value, self.lib_ptr)
+        return err
+
+    def GetRegister(self, path: str):
+        get_register_api = self.scisdk_dll.SCISDK_GetRegister
+        get_register_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_int), ctypes.c_void_p]
+        get_register_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        ret_int = ctypes.c_int()
+        # call C lib function
+        err = get_register_api(ctypes.c_char_p(path_b), ctypes.byref(ret_int), self.lib_ptr)
+        return err, ret_int.value
+
+    def GetAllParameters(self, path: str):
+        get_all_parameters_api = self.scisdk_dll.SCISDK_GetAllParameters
+        get_all_parameters_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
+        get_all_parameters_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        ret_char_p = ctypes.c_char_p()
+        # call C lib function
+        err = get_all_parameters_api(ctypes.c_char_p(path_b), ctypes.byref(ret_char_p), self.lib_ptr)
+        return err, ret_char_p.value.decode('utf-8')
+
+    def GetParameterDescription(self, path: str):
+        get_parameter_description_api = self.scisdk_dll.SCISDK_GetParameterDescription
+        get_parameter_description_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
+        get_parameter_description_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        ret_char_p = ctypes.c_char_p()
+        # call C lib function
+        err = get_parameter_description_api(ctypes.c_char_p(path_b), ctypes.byref(ret_char_p), self.lib_ptr)
+        return err, ret_char_p.value.decode('utf-8')
+
+    def GetParameterListOfValues(self, path: str):
+        get_parameter_list_of_values_api = self.scisdk_dll.SCISDK_GetParameterListOfValues
+        get_parameter_list_of_values_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
+        get_parameter_list_of_values_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        ret_char_p = ctypes.c_char_p()
+        # call C lib function
+        err = get_parameter_list_of_values_api(ctypes.c_char_p(path_b), ctypes.byref(ret_char_p), self.lib_ptr)
+        return err, ret_char_p.value.decode('utf-8')
+
+    def GetParameterMinimumValue(self, path: str):
+        get_parameters_min_value_api = self.scisdk_dll.SCISDK_GetParameterMinimumValue
+        get_parameters_min_value_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_double), ctypes.c_void_p]
+        get_parameters_min_value_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        ret_double_p = ctypes.c_double()
+        # call C lib function
+        err = get_parameters_min_value_api(ctypes.c_char_p(path_b), ctypes.byref(ret_double_p), self.lib_ptr)
+        return err, ret_double_p.value
+
+    def GetParameterMaximumValue(self, path: str):
+        get_parameters_max_value_api = self.scisdk_dll.SCISDK_GetParameterMaximumValue
+        get_parameters_max_value_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_double), ctypes.c_void_p]
+        get_parameters_max_value_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        ret_double_p = ctypes.c_double()
+        # call C lib function
+        err = get_parameters_max_value_api(ctypes.c_char_p(path_b), ctypes.byref(ret_double_p), self.lib_ptr)
+        return err, ret_double_p.value
+
+    def GetParametersProperties(self, path: str):
+        get_parameters_properties_api = self.scisdk_dll.SCISDK_GetParametersProperties
+        get_parameters_properties_api.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
+        get_parameters_properties_api.restype = ctypes.c_int
+        # convert string to bytes array
+        path_b = path.encode('utf-8')
+        ret_char_p = ctypes.c_char_p()
+        # call C lib function
+        err = get_parameters_properties_api(ctypes.c_char_p(path_b), ctypes.byref(ret_char_p), self.lib_ptr)
+        return err, ret_char_p.value.decode('utf-8')
+
+    def FreeLib(self):
+        free_lib_api = self.scisdk_dll.SCISDK_FreeLib
+        free_lib_api.argtypes = [ctypes.c_void_p]
+        free_lib_api.restype = ctypes.c_int
+        # call C lib function
+        err = free_lib_api(self.lib_ptr)
+        return err
+    
+    def GetAttachedDevicesList(self):
+        get_attached_devices_list_api = self.scisdk_dll.SCISDK_GetAttachedDevicesList
+        get_attached_devices_list_api.argtypes = [ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
+        get_attached_devices_list_api.restype = ctypes.c_int
+        # call C lib function
+        ret_char_p = ctypes.c_char_p()
+        err = get_attached_devices_list_api(ctypes.byref(ret_char_p), self.lib_ptr)
+        return err, ret_char_p.value.decode('utf-8')
+    
+    def GetLibraryVersion(self):
+        get_library_version_api = self.scisdk_dll.SCISDK_GetLibraryVersion
+        get_library_version_api.argtypes = [ctypes.POINTER(ctypes.c_char_p), ctypes.c_void_p]
+        get_library_version_api.restype = ctypes.c_int
+        # call C lib function
+        ret_char_p = ctypes.c_char_p()
+        err = get_library_version_api(ctypes.byref(ret_char_p), self.lib_ptr)
+        return err, ret_char_p.value.decode('utf-8')
```

### Comparing `scisdk-0.0.3/src/scisdk/scisdk_defines.py` & `scisdk-0.0.4/src/scisdk/scisdk_defines.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,383 +1,383 @@
-import ctypes
-
-# defines
-# Oscilloscope decoded buffer
-class OscilloscopeDecodedBufferInfo(ctypes.Structure):
-    _fields_ = [('samples_analog', ctypes.c_uint32),
-            ('samples_digital', ctypes.c_uint32),
-            ('tracks_analog_per_channel',  ctypes.c_uint32),
-            ('tracks_digital_per_channel', ctypes.c_uint32),
-            ('channels', ctypes.c_uint32)]
-
-class OscilloscopeDecodedBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-            ('analog', ctypes.POINTER(ctypes.c_int32)),
-            ('digital',  ctypes.POINTER(ctypes.c_int8)),
-            ('trigger_position', ctypes.c_uint32),
-            ('timecode', ctypes.c_uint64),
-            ('info', OscilloscopeDecodedBufferInfo)]
-
-# Oscilloscope raw buffer
-class OscilloscopeRawBufferInfo(ctypes.Structure):
-    _fields = [('buffer_size', ctypes.c_uint32),
-            ('samples_analog', ctypes.c_uint32),
-            ('samples_digital', ctypes.c_uint32),
-            ('tracks_analog_per_channel',  ctypes.c_uint32),
-            ('tracks_digital_per_channel', ctypes.c_uint32),
-            ('channels', ctypes.c_uint32)]
-
-class OscilloscopeRawBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-            ('data', ctypes.POINTER(ctypes.c_uint32)),
-            ('zero_position', ctypes.c_uint32),
-            ('trigger_position', ctypes.c_uint32),
-            ('timecode', ctypes.c_uint64),
-            ('info', OscilloscopeRawBufferInfo)]
-
-# Oscilloscope dual decoded buffer
-class OscilloscopeDualDecodedBufferInfo(ctypes.Structure):
-    _fields_ = [('samples_analog', ctypes.c_uint32),
-            ('samples_digital', ctypes.c_uint32),
-            ('tracks_analog_per_channel',  ctypes.c_uint32),
-            ('tracks_digital_per_channel', ctypes.c_uint32),
-            ('channels', ctypes.c_uint32)]
-
-class OscilloscopeDualDecodedBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-            ('analog', ctypes.POINTER(ctypes.c_int32)),
-            ('digital',  ctypes.POINTER(ctypes.c_int8)),
-            ('trigger_position', ctypes.c_uint32),
-            ('timecode', ctypes.c_uint64),
-            ('info', OscilloscopeDecodedBufferInfo)]
-
-# Oscilloscope dual raw buffer
-class OscilloscopeDualRawBufferInfo(ctypes.Structure):
-    _fields = [('buffer_size', ctypes.c_uint32),
-            ('samples_analog', ctypes.c_uint32),
-            ('samples_digital', ctypes.c_uint32),
-            ('tracks_analog_per_channel',  ctypes.c_uint32),
-            ('tracks_digital_per_channel', ctypes.c_uint32),
-            ('channels', ctypes.c_uint32)]
-
-class OscilloscopeDualRawBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-            ('data', ctypes.POINTER(ctypes.c_uint32)),
-            ('zero_position', ctypes.c_uint32),
-            ('trigger_position', ctypes.c_uint32),
-            ('timecode', ctypes.c_uint64),
-            ('info', OscilloscopeRawBufferInfo)]
-
-# Digitizer decoded buffer
-class DigitizerDecodedBufferInfo(ctypes.Structure):
-    _fields_ = [('samples', ctypes.c_uint32),
-                ('valid_samples', ctypes.c_uint32),
-                ('channels', ctypes.c_uint32)]
-
-class DigitizerDecodedBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('analog', ctypes.POINTER(ctypes.c_int32)),
-                ('hits', ctypes.c_uint64),
-                ('timecode', ctypes.c_uint64),
-                ('counter', ctypes.c_uint32),
-                ('user', ctypes.c_uint32),
-                ('info', DigitizerDecodedBufferInfo)]
-
-# List raw buffer
-class ListRawBufferInfo(ctypes.Structure):
-    _fields_ = [('buffer_size', ctypes.c_uint32),
-                ('samples', ctypes.c_uint32),
-                ('valid_samples', ctypes.c_uint32),
-                ('channels', ctypes.c_uint32)]
-
-class ListRawBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('data', ctypes.POINTER(ctypes.c_char)),
-                ('info', ListRawBufferInfo)]
-
-# Custom packet packet
-class CustomPacketPacket(ctypes.Structure):
-    _fields_ = [('row', ctypes.POINTER(ctypes.c_uint32)),
-                ('n', ctypes.c_uint32)]
-
-# Custom packet decoded buffer
-class CustomPacketDecodedBufferInfo(ctypes.Structure):
-    _fields_ = [('buffer_size', ctypes.c_uint32),
-                ('packet_size', ctypes.c_uint32),
-                ('valid_data', ctypes.c_uint32)]
-
-class CustomPacketDecodedBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('data', ctypes.POINTER(CustomPacketPacket)),
-                ('info', CustomPacketDecodedBufferInfo)]
-
-# Custom packet raw buffer
-class CustomPacketRawBufferInfo(ctypes.Structure):
-    _fields_ = [('buffer_size', ctypes.c_uint32),
-                ('valid_data', ctypes.c_uint32)]
-
-class CustomPacketRawBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('data', ctypes.POINTER(ctypes.c_uint32)),
-                ('info', CustomPacketRawBufferInfo)]
-
-# Ratemeter raw buffer
-class RatemeterRawBufferInfo(ctypes.Structure):
-    _fields_ = [('buffer_size', ctypes.c_uint32),
-                ('valid_data', ctypes.c_uint32),
-                ('nchannels', ctypes.c_uint32)]
-
-class RatemeterRawBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('data', ctypes.POINTER(ctypes.c_double)),
-                ('info', RatemeterRawBufferInfo)]
-
-# Spectrum decoded buffer
-class SpectrumDecodedBufferInfo(ctypes.Structure):
-    _fields_ = [('buffer_size', ctypes.c_uint32),
-                ('total_bins', ctypes.c_uint32),
-                ('valid_bins', ctypes.c_uint32)]
-
-class SpectrumDecodedBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('data', ctypes.POINTER(ctypes.c_uint32)),
-                ('timecode', ctypes.c_uint64),
-                ('inttime', ctypes.c_uint32),
-                ('info', SpectrumDecodedBufferInfo),]
-
-# FFT decoded buffer
-class FFTDecodedBufferInfo(ctypes.Structure):
-    _fields_ = [('samples', ctypes.c_uint32),
-                ('channels', ctypes.c_uint32)]
-
-class FFTDecodedBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('double', ctypes.POINTER(ctypes.c_double)),
-                ('ph', ctypes.POINTER(ctypes.c_double)),
-                ('timecode', ctypes.c_uint64),
-                ('info', FFTDecodedBufferInfo)]
-
-# FFT raw buffer
-class FFTRawBufferInfo(ctypes.Structure):
-    _fields_ = [('buffer_size', ctypes.c_uint32),
-                ('samples', ctypes.c_uint32),
-                ('channels', ctypes.c_uint32)]
-
-class FFTRawBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('data', ctypes.POINTER(ctypes.c_uint32)),
-                ('timecode', ctypes.c_uint64),
-                ('info', FFTRawBufferInfo)]
-
-
-# Frame packet decoded info
-class CustomPacketDecodedBufferInfo(ctypes.Structure):
-    _fields_ = [('timestamp', ctypes.c_uint64),
-                ('trigger_count', ctypes.c_uint64),
-                ('event_count', ctypes.c_uint64),
-                ('hits', ctypes.c_uint64)]
-
-# Frame packet packet
-class FramePacket(ctypes.Structure):
-    _fields_ = [('pixel', ctypes.POINTER(ctypes.c_uint32)),
-                ('n', ctypes.c_uint32),
-                ('info', CustomPacketDecodedBufferInfo)
-                ]
-
-# Custom packet decoded buffer
-class FramePacketDecodedBufferInfo(ctypes.Structure):
-    _fields_ = [('buffer_size', ctypes.c_uint32),
-                ('valid_data', ctypes.c_uint32)]
-
-class FramePacketDecodedBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('data', ctypes.POINTER(FramePacket)),
-                ('info', FramePacketDecodedBufferInfo)]
-
-# Custom packet raw buffer
-class FramePacketRawBufferInfo(ctypes.Structure):
-    _fields_ = [('buffer_size', ctypes.c_uint32),
-                ('packet_size', ctypes.c_uint32),
-                ('valid_data', ctypes.c_uint32)]
-
-class FramePacketRawBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('data', ctypes.POINTER(ctypes.c_uint32)),
-                ('info', FramePacketRawBufferInfo)]
-
-
-# Citiroc Pixel
-class CitirocPixel(ctypes.Structure):
-    _fields_ = [('hg', ctypes.c_uint16),
-                ('lg', ctypes.c_uint16),
-                ('hit', ctypes.c_uint8)
-                ]
-
-# Citiroc packet info
-class CitirocPacketInfo(ctypes.Structure):
-    _fields_ = [('asic', ctypes.c_uint8),
-                ('timestamp_from_t0', ctypes.c_uint64),
-                ('timestamp_from_run', ctypes.c_uint64),
-                ('event_id', ctypes.c_uint32),
-                ('trigger_count', ctypes.c_uint32),
-                ('validation_counter', ctypes.c_uint32),
-                ('flags', ctypes.c_uint32)
-                ]
-# Citiroc packet
-class CitirocPacket(ctypes.Structure):
-    _fields_ = [('pixel', ctypes.POINTER(CitirocPixel)),
-                ('n', ctypes.c_uint32),
-                ('info', CitirocPacketInfo)
-                ]
-
-# Citiroc decoded buffer info
-class CitirocDecodedBufferInfo(ctypes.Structure):
-    _fields_ = [('buffer_size', ctypes.c_uint32),
-                ('valid_data', ctypes.c_uint32)]
-
-# Citiroc decoded buffer
-class CitirocDecodedBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('data', ctypes.POINTER(CitirocPacket)),
-                ('info', CitirocDecodedBufferInfo)]
-
-# Citiroc raw buffer info
-class CitirocRawBufferInfo(ctypes.Structure):
-    _fields_ = [('buffer_size', ctypes.c_uint32),
-                ('packet_size', ctypes.c_uint32),
-                ('valid_data', ctypes.c_uint32)]
-
-# Citiroc raw buffer
-class CitirocRawBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('data', ctypes.POINTER(ctypes.c_uint32)),
-                ('info', CitirocRawBufferInfo)]
-
-# Petiroc Pixel
-class PetirocPixel(ctypes.Structure):   
-    _fields_ = [('charge', ctypes.c_uint16),
-                ('fine', ctypes.c_uint16),
-                ('coarse', ctypes.c_uint16),
-                ('hit', ctypes.c_uint8)
-                ]
-
-# Petiroc packet info
-class PetirocPacketInfo(ctypes.Structure):
-    _fields_ = [('asic', ctypes.c_uint8),
-                ('timestamp_from_t0', ctypes.c_uint64),
-                ('timestamp_from_run', ctypes.c_uint64),
-                ('event_id', ctypes.c_uint32),
-                ('trigger_count', ctypes.c_uint32),
-                ('validation_counter', ctypes.c_uint32),
-                ('flags', ctypes.c_uint32)
-                ]
-
-# Petiroc packet
-class PetirocPacket(ctypes.Structure):
-    _fields_ = [('pixel', ctypes.POINTER(PetirocPixel)),
-                ('n', ctypes.c_uint32),
-                ('info', PetirocPacketInfo)
-                ]
-
-# Petiroc decoded buffer info
-class PetirocDecodedBufferInfo(ctypes.Structure):
-    _fields_ = [('buffer_size', ctypes.c_uint32),
-                ('valid_data', ctypes.c_uint32)]
-
-# Petiroc decoded buffer
-class PetirocDecodedBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('data', ctypes.POINTER(PetirocPacket)),
-                ('info', PetirocDecodedBufferInfo)]
-
-# Petiroc raw buffer info
-class PetirocRawBufferInfo(ctypes.Structure):
-    _fields_ = [('buffer_size', ctypes.c_uint32),
-                ('packet_size', ctypes.c_uint32),
-                ('valid_data', ctypes.c_uint32)]
-
-# Petiroc raw buffer
-class PetirocRawBuffer(ctypes.Structure):
-    _fields_ = [('magic', ctypes.c_uint32),
-                ('data', ctypes.POINTER(ctypes.c_uint32)),
-                ('info', PetirocRawBufferInfo)]
-
-# FE-Scope packet
-class FEScopePacket(ctypes.Structure):
-    _fields_ = [('timestamp', ctypes.c_uint64),
-                ('trigger_id', ctypes.c_uint32),
-                ('event_size', ctypes.c_uint32),
-                ('waveform', ctypes.POINTER(ctypes.POINTER(ctypes.c_uint16))),
-                ('n_samples', ctypes.POINTER(ctypes.c_uint32)),
-                ('n_channels', ctypes.c_uint32)]
-
-
-# FE_OpenDpp packet
-class FEOpenDppPacket(ctypes.Structure):
-    _fields_ = [('channel', ctypes.c_uint8),
-                ('timestamp', ctypes.c_uint64),
-                ('timestamp_ns', ctypes.c_uint64),
-                ('fine_timestamp', ctypes.c_uint16),
-                ('energy', ctypes.c_uint16),
-                ('flags_b', ctypes.c_uint16),
-                ('flags_a', ctypes.c_uint8),
-                ('psd', ctypes.c_uint16),
-                ('user_info', ctypes.POINTER(ctypes.c_uint64)),
-                ('user_info_size', ctypes.c_uint32),
-                ('truncated', ctypes.c_bool),
-                ('waveform', ctypes.POINTER(ctypes.c_uint16)),
-                ('waveform_size', ctypes.c_uint32),
-                ('board_fail', ctypes.c_bool),
-                ('special_event', ctypes.c_bool),
-                ('event_size', ctypes.c_uint32),
-                ('flush', ctypes.c_bool),
-                ('aggregate_counter', ctypes.c_uint32),
-                ]
-
-
-
-class NIErrors:
-    NI_OK = 0x00000000
-    NI_ERROR_GENERIC = 0x00000001
-    NI_ERROR_INTERFACE = 0x00000002
-    NI_ERROR_FPGA = 0x00000003
-    NI_ERROR_TRANSFER_MAX_LENGTH = 0x00000004
-    NI_ERROR_NOTCONNECTED = 0x00000005
-    NI_NO_DATA_AVAILABLE = 0x00000006
-    NI_TOO_MANY_DEVICES_CONNECTED = 0x00000007
-    NI_INVALID_HANDLE = 0x00000008
-    NI_INVALID_KEY = 0x00000009
-    NI_INVALID_PARAMETER = 0x0000000A
-    NI_PARAMETER_OUT_OF_RANGE = 0x0000000B
-    NI_INCOMPLETE_READ = 0x0000000C
-    NI_INVALID_COMMAND = 0x0000000D
-    NI_PARAMETER_CAN_NOT_BE_CANGHED_IN_RUN = 0x0000000E
-    NI_PARAMETER_CAN_NOT_BE_SET_WITH_THIS_CONFIG = 0x0000000F
-    NI_PARAMETER_CAN_NOT_BE_SET = 0x00000010
-    NI_PARAMETER_MIN_MAX_NOT_SET = 0x00000011
-    NI_UNABLE_TO_LOAD_EXTERNAL_LIBRARY = 0x00000012
-    NI_INVALID_PARAMETER_PATH = 0x00000013
-    NI_INVALID_PARAMETER_ROOT = 0x00000014
-    NI_NOT_SUPPORTED = 0x00000015
-    NI_INVALID_ACQ_MODE = 0x00000016
-    NI_INVALID_METHOD = 0x00000017
-    NI_ALREADY_CONNECTED = 0x00000100
-    NI_ALLOC_FAILED = 0x00000200
-    NI_MEMORY_NOT_ALLOCATED = 0x00000201
-    NI_INVALID_BUFFER_TYPE = 0x00000202
-    NI_INVALID_BUFFER_SIZE = 0x00000203
-    NI_INCOMPATIBLE_BUFFER = 0x00000204
-    NI_INVALID_BUFFER = 0x00000205
-    NI_NOT_ARMED = 0x00000206
-    NI_TIMEOUT = 0x00000300
-    NI_INVALID_CFG_JSON = 0x10000000
-    NI_CFG_JSON_NOT_FOUND = 0x10000001
-    NI_DEVICE_NAME_ALREADY_EXISTS = 0x10000002
-    NI_INVALID_PATH = 0x10001000
-    NI_NOT_FOUND = 0x10001FFE
-    NI_INVALID_TYPE = 0x10001FFF
-    NI_ALREADY_RUNNING = 0x10003000
-    NI_NOT_RUNNING = 0x10003001
-    NI_FEELIB_INTERNAL_ERROR = 0x20000000
-
-    NI_SPECIFIC_ERROR = 0xFFFFFFFD
-    NI_LIBRARY_ERROR = 0xFFFFFFFE
+import ctypes
+
+# defines
+# Oscilloscope decoded buffer
+class OscilloscopeDecodedBufferInfo(ctypes.Structure):
+    _fields_ = [('samples_analog', ctypes.c_uint32),
+            ('samples_digital', ctypes.c_uint32),
+            ('tracks_analog_per_channel',  ctypes.c_uint32),
+            ('tracks_digital_per_channel', ctypes.c_uint32),
+            ('channels', ctypes.c_uint32)]
+
+class OscilloscopeDecodedBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+            ('analog', ctypes.POINTER(ctypes.c_int32)),
+            ('digital',  ctypes.POINTER(ctypes.c_int8)),
+            ('trigger_position', ctypes.c_uint32),
+            ('timecode', ctypes.c_uint64),
+            ('info', OscilloscopeDecodedBufferInfo)]
+
+# Oscilloscope raw buffer
+class OscilloscopeRawBufferInfo(ctypes.Structure):
+    _fields = [('buffer_size', ctypes.c_uint32),
+            ('samples_analog', ctypes.c_uint32),
+            ('samples_digital', ctypes.c_uint32),
+            ('tracks_analog_per_channel',  ctypes.c_uint32),
+            ('tracks_digital_per_channel', ctypes.c_uint32),
+            ('channels', ctypes.c_uint32)]
+
+class OscilloscopeRawBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+            ('data', ctypes.POINTER(ctypes.c_uint32)),
+            ('zero_position', ctypes.c_uint32),
+            ('trigger_position', ctypes.c_uint32),
+            ('timecode', ctypes.c_uint64),
+            ('info', OscilloscopeRawBufferInfo)]
+
+# Oscilloscope dual decoded buffer
+class OscilloscopeDualDecodedBufferInfo(ctypes.Structure):
+    _fields_ = [('samples_analog', ctypes.c_uint32),
+            ('samples_digital', ctypes.c_uint32),
+            ('tracks_analog_per_channel',  ctypes.c_uint32),
+            ('tracks_digital_per_channel', ctypes.c_uint32),
+            ('channels', ctypes.c_uint32)]
+
+class OscilloscopeDualDecodedBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+            ('analog', ctypes.POINTER(ctypes.c_int32)),
+            ('digital',  ctypes.POINTER(ctypes.c_int8)),
+            ('trigger_position', ctypes.c_uint32),
+            ('timecode', ctypes.c_uint64),
+            ('info', OscilloscopeDecodedBufferInfo)]
+
+# Oscilloscope dual raw buffer
+class OscilloscopeDualRawBufferInfo(ctypes.Structure):
+    _fields = [('buffer_size', ctypes.c_uint32),
+            ('samples_analog', ctypes.c_uint32),
+            ('samples_digital', ctypes.c_uint32),
+            ('tracks_analog_per_channel',  ctypes.c_uint32),
+            ('tracks_digital_per_channel', ctypes.c_uint32),
+            ('channels', ctypes.c_uint32)]
+
+class OscilloscopeDualRawBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+            ('data', ctypes.POINTER(ctypes.c_uint32)),
+            ('zero_position', ctypes.c_uint32),
+            ('trigger_position', ctypes.c_uint32),
+            ('timecode', ctypes.c_uint64),
+            ('info', OscilloscopeRawBufferInfo)]
+
+# Digitizer decoded buffer
+class DigitizerDecodedBufferInfo(ctypes.Structure):
+    _fields_ = [('samples', ctypes.c_uint32),
+                ('valid_samples', ctypes.c_uint32),
+                ('channels', ctypes.c_uint32)]
+
+class DigitizerDecodedBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('analog', ctypes.POINTER(ctypes.c_int32)),
+                ('hits', ctypes.c_uint64),
+                ('timecode', ctypes.c_uint64),
+                ('counter', ctypes.c_uint32),
+                ('user', ctypes.c_uint32),
+                ('info', DigitizerDecodedBufferInfo)]
+
+# List raw buffer
+class ListRawBufferInfo(ctypes.Structure):
+    _fields_ = [('buffer_size', ctypes.c_uint32),
+                ('samples', ctypes.c_uint32),
+                ('valid_samples', ctypes.c_uint32),
+                ('channels', ctypes.c_uint32)]
+
+class ListRawBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('data', ctypes.POINTER(ctypes.c_char)),
+                ('info', ListRawBufferInfo)]
+
+# Custom packet packet
+class CustomPacketPacket(ctypes.Structure):
+    _fields_ = [('row', ctypes.POINTER(ctypes.c_uint32)),
+                ('n', ctypes.c_uint32)]
+
+# Custom packet decoded buffer
+class CustomPacketDecodedBufferInfo(ctypes.Structure):
+    _fields_ = [('buffer_size', ctypes.c_uint32),
+                ('packet_size', ctypes.c_uint32),
+                ('valid_data', ctypes.c_uint32)]
+
+class CustomPacketDecodedBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('data', ctypes.POINTER(CustomPacketPacket)),
+                ('info', CustomPacketDecodedBufferInfo)]
+
+# Custom packet raw buffer
+class CustomPacketRawBufferInfo(ctypes.Structure):
+    _fields_ = [('buffer_size', ctypes.c_uint32),
+                ('valid_data', ctypes.c_uint32)]
+
+class CustomPacketRawBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('data', ctypes.POINTER(ctypes.c_uint32)),
+                ('info', CustomPacketRawBufferInfo)]
+
+# Ratemeter raw buffer
+class RatemeterRawBufferInfo(ctypes.Structure):
+    _fields_ = [('buffer_size', ctypes.c_uint32),
+                ('valid_data', ctypes.c_uint32),
+                ('nchannels', ctypes.c_uint32)]
+
+class RatemeterRawBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('data', ctypes.POINTER(ctypes.c_double)),
+                ('info', RatemeterRawBufferInfo)]
+
+# Spectrum decoded buffer
+class SpectrumDecodedBufferInfo(ctypes.Structure):
+    _fields_ = [('buffer_size', ctypes.c_uint32),
+                ('total_bins', ctypes.c_uint32),
+                ('valid_bins', ctypes.c_uint32)]
+
+class SpectrumDecodedBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('data', ctypes.POINTER(ctypes.c_uint32)),
+                ('timecode', ctypes.c_uint64),
+                ('inttime', ctypes.c_uint32),
+                ('info', SpectrumDecodedBufferInfo),]
+
+# FFT decoded buffer
+class FFTDecodedBufferInfo(ctypes.Structure):
+    _fields_ = [('samples', ctypes.c_uint32),
+                ('channels', ctypes.c_uint32)]
+
+class FFTDecodedBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('double', ctypes.POINTER(ctypes.c_double)),
+                ('ph', ctypes.POINTER(ctypes.c_double)),
+                ('timecode', ctypes.c_uint64),
+                ('info', FFTDecodedBufferInfo)]
+
+# FFT raw buffer
+class FFTRawBufferInfo(ctypes.Structure):
+    _fields_ = [('buffer_size', ctypes.c_uint32),
+                ('samples', ctypes.c_uint32),
+                ('channels', ctypes.c_uint32)]
+
+class FFTRawBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('data', ctypes.POINTER(ctypes.c_uint32)),
+                ('timecode', ctypes.c_uint64),
+                ('info', FFTRawBufferInfo)]
+
+
+# Frame packet decoded info
+class CustomPacketDecodedBufferInfo(ctypes.Structure):
+    _fields_ = [('timestamp', ctypes.c_uint64),
+                ('trigger_count', ctypes.c_uint64),
+                ('event_count', ctypes.c_uint64),
+                ('hits', ctypes.c_uint64)]
+
+# Frame packet packet
+class FramePacket(ctypes.Structure):
+    _fields_ = [('pixel', ctypes.POINTER(ctypes.c_uint32)),
+                ('n', ctypes.c_uint32),
+                ('info', CustomPacketDecodedBufferInfo)
+                ]
+
+# Custom packet decoded buffer
+class FramePacketDecodedBufferInfo(ctypes.Structure):
+    _fields_ = [('buffer_size', ctypes.c_uint32),
+                ('valid_data', ctypes.c_uint32)]
+
+class FramePacketDecodedBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('data', ctypes.POINTER(FramePacket)),
+                ('info', FramePacketDecodedBufferInfo)]
+
+# Custom packet raw buffer
+class FramePacketRawBufferInfo(ctypes.Structure):
+    _fields_ = [('buffer_size', ctypes.c_uint32),
+                ('packet_size', ctypes.c_uint32),
+                ('valid_data', ctypes.c_uint32)]
+
+class FramePacketRawBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('data', ctypes.POINTER(ctypes.c_uint32)),
+                ('info', FramePacketRawBufferInfo)]
+
+
+# Citiroc Pixel
+class CitirocPixel(ctypes.Structure):
+    _fields_ = [('hg', ctypes.c_uint16),
+                ('lg', ctypes.c_uint16),
+                ('hit', ctypes.c_uint8)
+                ]
+
+# Citiroc packet info
+class CitirocPacketInfo(ctypes.Structure):
+    _fields_ = [('asic', ctypes.c_uint8),
+                ('timestamp_from_t0', ctypes.c_uint64),
+                ('timestamp_from_run', ctypes.c_uint64),
+                ('event_id', ctypes.c_uint32),
+                ('trigger_count', ctypes.c_uint32),
+                ('validation_counter', ctypes.c_uint32),
+                ('flags', ctypes.c_uint32)
+                ]
+# Citiroc packet
+class CitirocPacket(ctypes.Structure):
+    _fields_ = [('pixel', ctypes.POINTER(CitirocPixel)),
+                ('n', ctypes.c_uint32),
+                ('info', CitirocPacketInfo)
+                ]
+
+# Citiroc decoded buffer info
+class CitirocDecodedBufferInfo(ctypes.Structure):
+    _fields_ = [('buffer_size', ctypes.c_uint32),
+                ('valid_data', ctypes.c_uint32)]
+
+# Citiroc decoded buffer
+class CitirocDecodedBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('data', ctypes.POINTER(CitirocPacket)),
+                ('info', CitirocDecodedBufferInfo)]
+
+# Citiroc raw buffer info
+class CitirocRawBufferInfo(ctypes.Structure):
+    _fields_ = [('buffer_size', ctypes.c_uint32),
+                ('packet_size', ctypes.c_uint32),
+                ('valid_data', ctypes.c_uint32)]
+
+# Citiroc raw buffer
+class CitirocRawBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('data', ctypes.POINTER(ctypes.c_uint32)),
+                ('info', CitirocRawBufferInfo)]
+
+# Petiroc Pixel
+class PetirocPixel(ctypes.Structure):   
+    _fields_ = [('charge', ctypes.c_uint16),
+                ('fine', ctypes.c_uint16),
+                ('coarse', ctypes.c_uint16),
+                ('hit', ctypes.c_uint8)
+                ]
+
+# Petiroc packet info
+class PetirocPacketInfo(ctypes.Structure):
+    _fields_ = [('asic', ctypes.c_uint8),
+                ('timestamp_from_t0', ctypes.c_uint64),
+                ('timestamp_from_run', ctypes.c_uint64),
+                ('event_id', ctypes.c_uint32),
+                ('trigger_count', ctypes.c_uint32),
+                ('validation_counter', ctypes.c_uint32),
+                ('flags', ctypes.c_uint32)
+                ]
+
+# Petiroc packet
+class PetirocPacket(ctypes.Structure):
+    _fields_ = [('pixel', ctypes.POINTER(PetirocPixel)),
+                ('n', ctypes.c_uint32),
+                ('info', PetirocPacketInfo)
+                ]
+
+# Petiroc decoded buffer info
+class PetirocDecodedBufferInfo(ctypes.Structure):
+    _fields_ = [('buffer_size', ctypes.c_uint32),
+                ('valid_data', ctypes.c_uint32)]
+
+# Petiroc decoded buffer
+class PetirocDecodedBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('data', ctypes.POINTER(PetirocPacket)),
+                ('info', PetirocDecodedBufferInfo)]
+
+# Petiroc raw buffer info
+class PetirocRawBufferInfo(ctypes.Structure):
+    _fields_ = [('buffer_size', ctypes.c_uint32),
+                ('packet_size', ctypes.c_uint32),
+                ('valid_data', ctypes.c_uint32)]
+
+# Petiroc raw buffer
+class PetirocRawBuffer(ctypes.Structure):
+    _fields_ = [('magic', ctypes.c_uint32),
+                ('data', ctypes.POINTER(ctypes.c_uint32)),
+                ('info', PetirocRawBufferInfo)]
+
+# FE-Scope packet
+class FEScopePacket(ctypes.Structure):
+    _fields_ = [('timestamp', ctypes.c_uint64),
+                ('trigger_id', ctypes.c_uint32),
+                ('event_size', ctypes.c_uint32),
+                ('waveform', ctypes.POINTER(ctypes.POINTER(ctypes.c_uint16))),
+                ('n_samples', ctypes.POINTER(ctypes.c_uint32)),
+                ('n_channels', ctypes.c_uint32)]
+
+
+# FE_OpenDpp packet
+class FEOpenDppPacket(ctypes.Structure):
+    _fields_ = [('channel', ctypes.c_uint8),
+                ('timestamp', ctypes.c_uint64),
+                ('timestamp_ns', ctypes.c_uint64),
+                ('fine_timestamp', ctypes.c_uint16),
+                ('energy', ctypes.c_uint16),
+                ('flags_b', ctypes.c_uint16),
+                ('flags_a', ctypes.c_uint8),
+                ('psd', ctypes.c_uint16),
+                ('user_info', ctypes.POINTER(ctypes.c_uint64)),
+                ('user_info_size', ctypes.c_uint32),
+                ('truncated', ctypes.c_bool),
+                ('waveform', ctypes.POINTER(ctypes.c_uint16)),
+                ('waveform_size', ctypes.c_uint32),
+                ('board_fail', ctypes.c_bool),
+                ('special_event', ctypes.c_bool),
+                ('event_size', ctypes.c_uint32),
+                ('flush', ctypes.c_bool),
+                ('aggregate_counter', ctypes.c_uint32),
+                ]
+
+
+
+class NIErrors:
+    NI_OK = 0x00000000
+    NI_ERROR_GENERIC = 0x00000001
+    NI_ERROR_INTERFACE = 0x00000002
+    NI_ERROR_FPGA = 0x00000003
+    NI_ERROR_TRANSFER_MAX_LENGTH = 0x00000004
+    NI_ERROR_NOTCONNECTED = 0x00000005
+    NI_NO_DATA_AVAILABLE = 0x00000006
+    NI_TOO_MANY_DEVICES_CONNECTED = 0x00000007
+    NI_INVALID_HANDLE = 0x00000008
+    NI_INVALID_KEY = 0x00000009
+    NI_INVALID_PARAMETER = 0x0000000A
+    NI_PARAMETER_OUT_OF_RANGE = 0x0000000B
+    NI_INCOMPLETE_READ = 0x0000000C
+    NI_INVALID_COMMAND = 0x0000000D
+    NI_PARAMETER_CAN_NOT_BE_CANGHED_IN_RUN = 0x0000000E
+    NI_PARAMETER_CAN_NOT_BE_SET_WITH_THIS_CONFIG = 0x0000000F
+    NI_PARAMETER_CAN_NOT_BE_SET = 0x00000010
+    NI_PARAMETER_MIN_MAX_NOT_SET = 0x00000011
+    NI_UNABLE_TO_LOAD_EXTERNAL_LIBRARY = 0x00000012
+    NI_INVALID_PARAMETER_PATH = 0x00000013
+    NI_INVALID_PARAMETER_ROOT = 0x00000014
+    NI_NOT_SUPPORTED = 0x00000015
+    NI_INVALID_ACQ_MODE = 0x00000016
+    NI_INVALID_METHOD = 0x00000017
+    NI_ALREADY_CONNECTED = 0x00000100
+    NI_ALLOC_FAILED = 0x00000200
+    NI_MEMORY_NOT_ALLOCATED = 0x00000201
+    NI_INVALID_BUFFER_TYPE = 0x00000202
+    NI_INVALID_BUFFER_SIZE = 0x00000203
+    NI_INCOMPATIBLE_BUFFER = 0x00000204
+    NI_INVALID_BUFFER = 0x00000205
+    NI_NOT_ARMED = 0x00000206
+    NI_TIMEOUT = 0x00000300
+    NI_INVALID_CFG_JSON = 0x10000000
+    NI_CFG_JSON_NOT_FOUND = 0x10000001
+    NI_DEVICE_NAME_ALREADY_EXISTS = 0x10000002
+    NI_INVALID_PATH = 0x10001000
+    NI_NOT_FOUND = 0x10001FFE
+    NI_INVALID_TYPE = 0x10001FFF
+    NI_ALREADY_RUNNING = 0x10003000
+    NI_NOT_RUNNING = 0x10003001
+    NI_FEELIB_INTERNAL_ERROR = 0x20000000
+
+    NI_SPECIFIC_ERROR = 0xFFFFFFFD
+    NI_LIBRARY_ERROR = 0xFFFFFFFE
```

### Comparing `scisdk-0.0.3/LICENSE` & `scisdk-0.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2022 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2022 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `scisdk-0.0.3/README.md` & `scisdk-0.0.4/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-#SciSDK: SciCompiler Python SDK wrapper
-
-This package will install a wrapper for the SciCompiler SDK, the software layer to develop Python application to readout and configure firmware generated by SciCompiler
-
-## Introduction
-The SciSDK is a cross-platform library to write custom control and readout software for SciCompiler generated user firmware.
-
-SciCompiler is a Nuclear Instruments (http://www.nuclearinstruments.eu) tool to generate FPGA firmware con NI/Caen OpenHardware FPGA (https://www.caen.it/families/open-fpga-digitizers/)
-
-The SciCompiler convert a block diagram description of the user firmware is a hardware compatible bitstream managing also the readout of the data from the hardware. This library is intended to be used to write the control and readout software for the user firmware and works only with firmware generated by SciCompiler.
-
-
-## Installation
-
-### Pre-requisites (Binary files installation)
-
-**This library requires that the SciSDK and all hardware related libraries are installed in the system.**
-
-The SciSDK can be installed precompiled or compiled from source.
-Detailed instructions on haw install the SciSDK are explained at this link: SciSDK installation(https://nuclearinstruments.github.io/SCISDK/)
-The last version of the compiled SciSDK libraries setup are available here: SciSDK setup (https://github.com/NuclearInstruments/SCISDK/releases)
-
-It is also possible to install avoid to install the SciSDK libraries system wide copying all DLL or so in the python script exectuable folder. It that case double check to execute the python.exe command from the folder where the script and all the libraries are located otherwise the script will be unable to locate the required libraries and an exception is rised.
-While the setup will install in the system folder the SciSDK dll and all the libraries for the supported boards, if manual setup is used, the user must ensure thal all dll are copied in the python script executable folder. 
-For example if the user intent to connecto to the DT1260 on windows system ( Python x64 ) the following libraries are required: SciSDK_DLL.dll SCIDK_Lib.dll ftd2xx64.dll
-For example if the user intent to connecto to the R5560 on windows system ( Python x64 ) the following libraries are required: SciSDK_DLL.dll R5560_SDKLib.dll libzmq-v140-mt-4_3_4.dll libsodium.dll
-Please double check the version of python (32 or 64 bit) and use dll/so accordingly.
-
-### Python wrapper installation
-In order to install the SciSDK python wrapper, just run the following command:
-
-```bash
-pip install scisdk
-```
-
-## Usage
-
-### Import the library
-
-Import the library in your python script:
-
-```python
-from scisdk.scisdk import SciSDK
-from scisdk.scisdk_defines import *
-```
-
-### Create the SciSDK object
-
-Create the SciSDK object and pass the connection string and the path to the JSON file:
-
-```python   
-
-# initialize scisdk library
-sdk = SciSDK()
-
-# add new device
-
-# USB board (DT1260)                usb:10500
-# ETHERNET (X556X) board            192.168.90.2:8888
-# FELIB based board (CAEN X274x):   10.105.250.18
-res = sdk.AddNewDevice("usb:10500","dt1260", "./DT1260RegisterFile.json","board0")
-if res != 0:
-    print ("Script exit due to connetion error")
-    exit()
-
-```
-
-### Readout the data
-Please refere to the official documentation (https://nuclearinstruments.github.io/SCISDK/)
-
-Example of readout of the data from the oscilloscope:
-
-```python
-res = sdk.SetParameterString("board0:/MMCComponents/Oscilloscope_0.data_processing","decode")
-res = sdk.SetParameterInteger("board0:/MMCComponents/Oscilloscope_0.trigger_level", 1000)
-res = sdk.SetParameterString("board0:/MMCComponents/Oscilloscope_0.trigger_mode","self")
-res = sdk.SetParameterInteger("board0:/MMCComponents/Oscilloscope_0.trigger_channel", 0)
-res = sdk.SetParameterInteger("board0:/MMCComponents/Oscilloscope_0.pretrigger", 150)
-res = sdk.SetParameterString("board0:/MMCComponents/Oscilloscope_0.acq_mode", "blocking")
-res = sdk.SetParameterInteger("board0:/MMCComponents/Oscilloscope_0.timeout", 3000)
-
-res, buf = sdk.AllocateBuffer("board0:/MMCComponents/Oscilloscope_0")
-
-res, buffer = sdk.ReadData("board0:/MMCComponents/Oscilloscope_0", buffer)# read data from board
-
-```
-
-
-
+#SciSDK: SciCompiler Python SDK wrapper
+
+This package will install a wrapper for the SciCompiler SDK, the software layer to develop Python application to readout and configure firmware generated by SciCompiler
+
+## Introduction
+The SciSDK is a cross-platform library to write custom control and readout software for SciCompiler generated user firmware.
+
+SciCompiler is a Nuclear Instruments (http://www.nuclearinstruments.eu) tool to generate FPGA firmware con NI/Caen OpenHardware FPGA (https://www.caen.it/families/open-fpga-digitizers/)
+
+The SciCompiler convert a block diagram description of the user firmware is a hardware compatible bitstream managing also the readout of the data from the hardware. This library is intended to be used to write the control and readout software for the user firmware and works only with firmware generated by SciCompiler.
+
+
+## Installation
+
+### Pre-requisites (Binary files installation)
+
+**This library requires that the SciSDK and all hardware related libraries are installed in the system.**
+
+The SciSDK can be installed precompiled or compiled from source.
+Detailed instructions on haw install the SciSDK are explained at this link: SciSDK installation(https://nuclearinstruments.github.io/SCISDK/)
+The last version of the compiled SciSDK libraries setup are available here: SciSDK setup (https://github.com/NuclearInstruments/SCISDK/releases)
+
+It is also possible to install avoid to install the SciSDK libraries system wide copying all DLL or so in the python script exectuable folder. It that case double check to execute the python.exe command from the folder where the script and all the libraries are located otherwise the script will be unable to locate the required libraries and an exception is rised.
+While the setup will install in the system folder the SciSDK dll and all the libraries for the supported boards, if manual setup is used, the user must ensure thal all dll are copied in the python script executable folder. 
+For example if the user intent to connecto to the DT1260 on windows system ( Python x64 ) the following libraries are required: SciSDK_DLL.dll SCIDK_Lib.dll ftd2xx64.dll
+For example if the user intent to connecto to the R5560 on windows system ( Python x64 ) the following libraries are required: SciSDK_DLL.dll R5560_SDKLib.dll libzmq-v140-mt-4_3_4.dll libsodium.dll
+Please double check the version of python (32 or 64 bit) and use dll/so accordingly.
+
+### Python wrapper installation
+In order to install the SciSDK python wrapper, just run the following command:
+
+```bash
+pip install scisdk
+```
+
+## Usage
+
+### Import the library
+
+Import the library in your python script:
+
+```python
+from scisdk.scisdk import SciSDK
+from scisdk.scisdk_defines import *
+```
+
+### Create the SciSDK object
+
+Create the SciSDK object and pass the connection string and the path to the JSON file:
+
+```python   
+
+# initialize scisdk library
+sdk = SciSDK()
+
+# add new device
+
+# USB board (DT1260)                usb:10500
+# ETHERNET (X556X) board            192.168.90.2:8888
+# FELIB based board (CAEN X274x):   10.105.250.18
+res = sdk.AddNewDevice("usb:10500","dt1260", "./DT1260RegisterFile.json","board0")
+if res != 0:
+    print ("Script exit due to connetion error")
+    exit()
+
+```
+
+### Readout the data
+Please refere to the official documentation (https://nuclearinstruments.github.io/SCISDK/)
+
+Example of readout of the data from the oscilloscope:
+
+```python
+res = sdk.SetParameterString("board0:/MMCComponents/Oscilloscope_0.data_processing","decode")
+res = sdk.SetParameterInteger("board0:/MMCComponents/Oscilloscope_0.trigger_level", 1000)
+res = sdk.SetParameterString("board0:/MMCComponents/Oscilloscope_0.trigger_mode","self")
+res = sdk.SetParameterInteger("board0:/MMCComponents/Oscilloscope_0.trigger_channel", 0)
+res = sdk.SetParameterInteger("board0:/MMCComponents/Oscilloscope_0.pretrigger", 150)
+res = sdk.SetParameterString("board0:/MMCComponents/Oscilloscope_0.acq_mode", "blocking")
+res = sdk.SetParameterInteger("board0:/MMCComponents/Oscilloscope_0.timeout", 3000)
+
+res, buf = sdk.AllocateBuffer("board0:/MMCComponents/Oscilloscope_0")
+
+res, buffer = sdk.ReadData("board0:/MMCComponents/Oscilloscope_0", buffer)# read data from board
+
+```
+
+
+
```

### Comparing `scisdk-0.0.3/pyproject.toml` & `scisdk-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "scisdk"
-version = "0.0.3"
-authors = [
-  { name="Andrea Abba", email="abba@nuclearinstruments.eu" },
-]
-description = "SDK for SciCompiler generated firmware"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-keywords = ["SciCompiler", "firmware", "fpga", "Nuclear Instruments", "CAEN"]
-dependencies = [
-]
-[project.urls]
-"Homepage" = "https://github.com/NuclearInstruments/SCISDK"
-"Bug Tracker" = "https://github.com/NuclearInstruments/SCISDK/issues"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "scisdk"
+version = "0.0.4"
+authors = [
+  { name="Andrea Abba", email="abba@nuclearinstruments.eu" },
+]
+description = "SDK for SciCompiler generated firmware"
+readme = "README.md"
+requires-python = ">=3.5"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+keywords = ["SciCompiler", "firmware", "fpga", "Nuclear Instruments", "CAEN"]
+dependencies = [
+]
+[project.urls]
+"Homepage" = "https://github.com/NuclearInstruments/SCISDK"
+"Bug Tracker" = "https://github.com/NuclearInstruments/SCISDK/issues"
```

### Comparing `scisdk-0.0.3/PKG-INFO` & `scisdk-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: scisdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: SDK for SciCompiler generated firmware
 Project-URL: Homepage, https://github.com/NuclearInstruments/SCISDK
 Project-URL: Bug Tracker, https://github.com/NuclearInstruments/SCISDK/issues
 Author-email: Andrea Abba <abba@nuclearinstruments.eu>
 License-File: LICENSE
 Keywords: CAEN,Nuclear Instruments,SciCompiler,firmware,fpga
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 #SciSDK: SciCompiler Python SDK wrapper
 
 This package will install a wrapper for the SciCompiler SDK, the software layer to develop Python application to readout and configure firmware generated by SciCompiler
 
 ## Introduction
```


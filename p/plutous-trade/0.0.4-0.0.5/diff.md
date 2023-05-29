# Comparing `tmp/plutous_trade-0.0.4.tar.gz` & `tmp/plutous_trade-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutous_trade-0.0.4.tar", max compression
+gzip compressed data, was "plutous_trade-0.0.5.tar", max compression
```

## Comparing `plutous_trade-0.0.4.tar` & `plutous_trade-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1064 2023-05-16 06:32:04.597270 plutous_trade-0.0.4/LICENSE
--rw-r--r--   0        0        0       40 2023-05-16 06:32:04.597270 plutous_trade-0.0.4/README.md
--rw-r--r--   0        0        0       65 2023-05-16 06:36:17.270223 plutous_trade-0.0.4/plutous/__init__.py
--rw-r--r--   0        0        0       83 2023-05-28 12:54:48.055674 plutous_trade-0.0.4/plutous/trade/__init__.py
--rw-r--r--   0        0        0     3380 2023-05-23 04:04:54.046424 plutous_trade-0.0.4/plutous/trade/alembic.ini
--rw-r--r--   0        0        0        0 2023-05-16 06:44:14.005733 plutous_trade-0.0.4/plutous/trade/app/__init__.py
--rw-r--r--   0        0        0     1396 2023-05-23 08:28:17.690022 plutous_trade-0.0.4/plutous/trade/app/main.py
--rw-r--r--   0        0        0      616 2023-05-28 12:53:16.136715 plutous_trade-0.0.4/plutous/trade/app/models.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:41.262810 plutous_trade-0.0.4/plutous/trade/cli/__init__.py
--rw-r--r--   0        0        0      565 2023-05-21 14:49:47.617177 plutous_trade-0.0.4/plutous/trade/cli/database.py
--rw-r--r--   0        0        0      253 2023-05-16 09:53:06.465010 plutous_trade-0.0.4/plutous/trade/cli/main.py
--rw-r--r--   0        0        0      221 2023-05-22 15:46:21.868004 plutous_trade-0.0.4/plutous/trade/enums/__init__.py
--rw-r--r--   0        0        0       78 2023-05-21 16:59:31.441696 plutous_trade-0.0.4/plutous/trade/enums/action.py
--rw-r--r--   0        0        0      575 2023-05-16 18:35:53.699585 plutous_trade-0.0.4/plutous/trade/enums/asset_type.py
--rw-r--r--   0        0        0       90 2023-05-22 03:47:08.998276 plutous_trade-0.0.4/plutous/trade/enums/bot_type.py
--rw-r--r--   0        0        0       87 2023-05-16 18:50:39.068724 plutous_trade-0.0.4/plutous/trade/enums/position_side.py
--rw-r--r--   0        0        0      111 2023-05-21 18:52:25.169077 plutous_trade-0.0.4/plutous/trade/enums/strategy_direction.py
--rw-r--r--   0        0        0      244 2023-05-21 15:33:24.216798 plutous_trade-0.0.4/plutous/trade/enums/strategy_type.py
--rw-r--r--   0        0        0       38 2023-05-16 07:55:03.225919 plutous_trade-0.0.4/plutous/trade/migrations/README
--rw-r--r--   0        0        0     2252 2023-05-27 03:28:54.379452 plutous_trade-0.0.4/plutous/trade/migrations/env.py
--rw-r--r--   0        0        0      510 2023-05-16 07:55:03.225919 plutous_trade-0.0.4/plutous/trade/migrations/script.py.mako
--rw-r--r--   0        0        0     7944 2023-05-28 12:54:19.153486 plutous_trade-0.0.4/plutous/trade/migrations/versions/2023-05-23_03-57_3e037c0f4152_init.py
--rw-r--r--   0        0        0      159 2023-05-22 03:55:30.430494 plutous_trade-0.0.4/plutous/trade/models/__init__.py
--rw-r--r--   0        0        0     1089 2023-05-22 15:48:07.454158 plutous_trade-0.0.4/plutous/trade/models/api_key.py
--rw-r--r--   0        0        0      401 2023-05-22 13:39:10.362131 plutous_trade-0.0.4/plutous/trade/models/base.py
--rw-r--r--   0        0        0     1007 2023-05-28 12:51:29.676654 plutous_trade-0.0.4/plutous/trade/models/bot.py
--rw-r--r--   0        0        0      941 2023-05-22 19:13:23.674596 plutous_trade-0.0.4/plutous/trade/models/position.py
--rw-r--r--   0        0        0      647 2023-05-22 13:38:30.726320 plutous_trade-0.0.4/plutous/trade/models/strategy.py
--rw-r--r--   0        0        0      968 2023-05-22 18:41:14.933111 plutous_trade-0.0.4/plutous/trade/models/trade.py
--rw-r--r--   0        0        0      560 2023-05-28 12:54:52.496010 plutous_trade-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 plutous_trade-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-16 06:32:04.597270 plutous_trade-0.0.5/LICENSE
+-rw-r--r--   0        0        0       40 2023-05-16 06:32:04.597270 plutous_trade-0.0.5/README.md
+-rw-r--r--   0        0        0       65 2023-05-16 06:36:17.270223 plutous_trade-0.0.5/plutous/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-29 14:57:21.638827 plutous_trade-0.0.5/plutous/trade/__init__.py
+-rw-r--r--   0        0        0     3380 2023-05-23 04:04:54.046424 plutous_trade-0.0.5/plutous/trade/alembic.ini
+-rw-r--r--   0        0        0        0 2023-05-16 06:44:14.005733 plutous_trade-0.0.5/plutous/trade/app/__init__.py
+-rw-r--r--   0        0        0     1396 2023-05-23 08:28:17.690022 plutous_trade-0.0.5/plutous/trade/app/main.py
+-rw-r--r--   0        0        0      616 2023-05-28 12:53:16.136715 plutous_trade-0.0.5/plutous/trade/app/models.py
+-rw-r--r--   0        0        0        0 2023-05-16 09:19:41.262810 plutous_trade-0.0.5/plutous/trade/cli/__init__.py
+-rw-r--r--   0        0        0      565 2023-05-21 14:49:47.617177 plutous_trade-0.0.5/plutous/trade/cli/database.py
+-rw-r--r--   0        0        0      253 2023-05-16 09:53:06.465010 plutous_trade-0.0.5/plutous/trade/cli/main.py
+-rw-r--r--   0        0        0      221 2023-05-22 15:46:21.868004 plutous_trade-0.0.5/plutous/trade/enums/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-21 16:59:31.441696 plutous_trade-0.0.5/plutous/trade/enums/action.py
+-rw-r--r--   0        0        0      575 2023-05-16 18:35:53.699585 plutous_trade-0.0.5/plutous/trade/enums/asset_type.py
+-rw-r--r--   0        0        0       90 2023-05-22 03:47:08.998276 plutous_trade-0.0.5/plutous/trade/enums/bot_type.py
+-rw-r--r--   0        0        0       87 2023-05-16 18:50:39.068724 plutous_trade-0.0.5/plutous/trade/enums/position_side.py
+-rw-r--r--   0        0        0      111 2023-05-21 18:52:25.169077 plutous_trade-0.0.5/plutous/trade/enums/strategy_direction.py
+-rw-r--r--   0        0        0      244 2023-05-21 15:33:24.216798 plutous_trade-0.0.5/plutous/trade/enums/strategy_type.py
+-rw-r--r--   0        0        0       38 2023-05-16 07:55:03.225919 plutous_trade-0.0.5/plutous/trade/migrations/README
+-rw-r--r--   0        0        0     2252 2023-05-27 03:28:54.379452 plutous_trade-0.0.5/plutous/trade/migrations/env.py
+-rw-r--r--   0        0        0      510 2023-05-16 07:55:03.225919 plutous_trade-0.0.5/plutous/trade/migrations/script.py.mako
+-rw-r--r--   0        0        0     8055 2023-05-29 13:28:42.703899 plutous_trade-0.0.5/plutous/trade/migrations/versions/2023-05-23_03-57_3e037c0f4152_init.py
+-rw-r--r--   0        0        0      159 2023-05-22 03:55:30.430494 plutous_trade-0.0.5/plutous/trade/models/__init__.py
+-rw-r--r--   0        0        0     1089 2023-05-22 15:48:07.454158 plutous_trade-0.0.5/plutous/trade/models/api_key.py
+-rw-r--r--   0        0        0      401 2023-05-22 13:39:10.362131 plutous_trade-0.0.5/plutous/trade/models/base.py
+-rw-r--r--   0        0        0     1007 2023-05-28 12:51:29.676654 plutous_trade-0.0.5/plutous/trade/models/bot.py
+-rw-r--r--   0        0        0      998 2023-05-29 13:29:59.635867 plutous_trade-0.0.5/plutous/trade/models/position.py
+-rw-r--r--   0        0        0      647 2023-05-22 13:38:30.726320 plutous_trade-0.0.5/plutous/trade/models/strategy.py
+-rw-r--r--   0        0        0      968 2023-05-22 18:41:14.933111 plutous_trade-0.0.5/plutous/trade/models/trade.py
+-rw-r--r--   0        0        0      560 2023-05-29 14:57:27.115394 plutous_trade-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 plutous_trade-0.0.5/PKG-INFO
```

### Comparing `plutous_trade-0.0.4/LICENSE` & `plutous_trade-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.4/plutous/trade/alembic.ini` & `plutous_trade-0.0.5/plutous/trade/alembic.ini`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.4/plutous/trade/app/main.py` & `plutous_trade-0.0.5/plutous/trade/app/main.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.4/plutous/trade/app/models.py` & `plutous_trade-0.0.5/plutous/trade/app/models.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.4/plutous/trade/cli/database.py` & `plutous_trade-0.0.5/plutous/trade/cli/database.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.4/plutous/trade/enums/asset_type.py` & `plutous_trade-0.0.5/plutous/trade/enums/asset_type.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.4/plutous/trade/migrations/env.py` & `plutous_trade-0.0.5/plutous/trade/migrations/env.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.4/plutous/trade/migrations/versions/2023-05-23_03-57_3e037c0f4152_init.py` & `plutous_trade-0.0.5/plutous/trade/migrations/versions/2023-05-23_03-57_3e037c0f4152_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,17 @@
     op.create_index('ix_bot_created_at', 'bot', ['created_at'], unique=False, schema='trade')
     op.create_index('ix_bot_updated_at', 'bot', ['updated_at'], unique=False, schema='trade')
     op.create_table('position',
     sa.Column('asset_type', sa.Enum('CASH', 'STOCK', 'CRYPTO', 'ETF', 'FUND', 'PROPERTY', 'COMMODITY', 'NFT', 'STOCK_FUTURES', 'STOCK_OPTION', 'COMMODITY_FUTURES', 'COMMODITY_OPTION', 'CRYPTO_FUTURES', 'CRYPTO_INVERSE_FUTURES', 'CRYPTO_OPTION', 'CRYPTO_PERP', 'CRYPTO_INVERSE_PERP', name='assettype', schema='trade'), nullable=False),
     sa.Column('exchange', exchange_enum, nullable=False),
     sa.Column('symbol', sa.String(), nullable=False),
     sa.Column('side', sa.Enum('LONG', 'SHORT', name='positionside', schema='trade'), nullable=False),
+    sa.Column('price', sa.Float(), nullable=False),
     sa.Column('quantity', sa.Float(), nullable=False),
+    sa.Column('realized_pnl', sa.Float(), nullable=False),
     sa.Column('opened_at', sa.DateTime(), nullable=False),
     sa.Column('closed_at', sa.DateTime(), nullable=True),
     sa.Column('bot_id', sa.Integer(), nullable=False),
     sa.Column('id', sa.Integer(), nullable=False),
     sa.Column('created_at', sa.TIMESTAMP(), nullable=False),
     sa.Column('updated_at', sa.TIMESTAMP(), nullable=False),
     sa.ForeignKeyConstraint(['bot_id'], ['trade.bot.id'], ),
```

### Comparing `plutous_trade-0.0.4/plutous/trade/models/api_key.py` & `plutous_trade-0.0.5/plutous/trade/models/api_key.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.4/plutous/trade/models/bot.py` & `plutous_trade-0.0.5/plutous/trade/models/bot.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.4/plutous/trade/models/position.py` & `plutous_trade-0.0.5/plutous/trade/models/position.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 
 class Position(Base):
     asset_type: Mapped[AssetType] = mapped_column(Enum(AssetType))
     exchange: Mapped[Exchange] = mapped_column(Enum(Exchange, schema="public"))
     symbol: Mapped[str]
     side: Mapped[PositionSide] = mapped_column(Enum(PositionSide))
+    price: Mapped[float]
     quantity: Mapped[float]
+    realized_pnl: Mapped[float]
     opened_at: Mapped[datetime]
     closed_at: Mapped[Optional[datetime]]
     bot_id: Mapped[int] = mapped_column(ForeignKey(Bot.id))
 
     bot: Mapped[Bot] = relationship(Bot, back_populates="positions")
     trades: Mapped[list["Trade"]] = relationship("Trade", back_populates="position")
```

### Comparing `plutous_trade-0.0.4/plutous/trade/models/strategy.py` & `plutous_trade-0.0.5/plutous/trade/models/strategy.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.4/plutous/trade/models/trade.py` & `plutous_trade-0.0.5/plutous/trade/models/trade.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.4/pyproject.toml` & `plutous_trade-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plutous-trade"
-version = "0.0.4"
+version = "0.0.5"
 description = "Plutous Trading Library"
 packages = [{include = "plutous"}]
 authors = ["Cheun Hong <cheunhong@plutous.io>"]
 readme = "README.md"
 license="MIT"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `plutous_trade-0.0.4/PKG-INFO` & `plutous_trade-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutous-trade
-Version: 0.0.4
+Version: 0.0.5
 Summary: Plutous Trading Library
 License: MIT
 Author: Cheun Hong
 Author-email: cheunhong@plutous.io
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/fhir.resources-7.0.0.tar.gz` & `tmp/fhir.resources-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhir.resources-7.0.0.tar", last modified: Sat Apr  8 12:10:43 2023, max compression
+gzip compressed data, was "fhir.resources-7.0.1.tar", last modified: Mon May 29 12:03:25 2023, max compression
```

## Comparing `fhir.resources-7.0.0.tar` & `fhir.resources-7.0.1.tar`

### file list

```diff
@@ -1,730 +1,729 @@
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:43.139525 fhir.resources-7.0.0/
--rw-r--r--   0 nazrul     (501) staff       (20)      255 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/AUTHORS.rst
--rw-r--r--   0 nazrul     (501) staff       (20)     4595 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/CONTRIBUTING.rst
--rw-r--r--   0 nazrul     (501) staff       (20)     9980 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/HISTORY.rst
--rw-r--r--   0 nazrul     (501) staff       (20)     1509 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/LICENSE
--rw-r--r--   0 nazrul     (501) staff       (20)      500 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/MANIFEST.in
--rw-r--r--   0 nazrul     (501) staff       (20)    41868 2023-04-08 12:10:43.139609 fhir.resources-7.0.0/PKG-INFO
--rw-r--r--   0 nazrul     (501) staff       (20)    30110 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/README.rst
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:43.046213 fhir.resources-7.0.0/fhir/
--rw-r--r--   0 nazrul     (501) staff       (20)       55 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/__init__.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:43.076246 fhir.resources-7.0.0/fhir/resources/
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:43.091934 fhir.resources-7.0.0/fhir/resources/DSTU2/
--rw-r--r--   0 nazrul     (501) staff       (20)      822 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/__init__.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2984 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/account.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2588 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/address.py
--rw-r--r--   0 nazrul     (501) staff       (20)      499 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/age.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6378 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/allergyintolerance.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3447 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/annotation.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4785 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/appointment.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2595 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/appointmentresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2078 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/attachment.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9925 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/auditevent.py
--rw-r--r--   0 nazrul     (501) staff       (20)      774 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/backboneelement.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1772 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/basic.py
--rw-r--r--   0 nazrul     (501) staff       (20)      868 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/binary.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1938 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/bodysite.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7233 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/bundle.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15002 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/careplan.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19956 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/claim.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19205 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/claimresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10208 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/clinicalimpression.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1106 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/codeableconcept.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1909 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/coding.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6809 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/communication.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9538 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/communicationrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8480 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/composition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10908 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/conceptmap.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11352 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/condition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22229 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/conformance.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1607 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/contactpoint.py
--rw-r--r--   0 nazrul     (501) staff       (20)    34499 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/contract.py
--rw-r--r--   0 nazrul     (501) staff       (20)      522 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/count.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4500 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/coverage.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5648 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/dataelement.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5595 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/detectedissue.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4230 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/device.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4586 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/devicecomponent.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7358 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/devicemetric.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8132 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/deviceuserequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6220 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/deviceusestatement.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9542 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/diagnosticorder.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8620 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/diagnosticreport.py
--rw-r--r--   0 nazrul     (501) staff       (20)      444 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/distance.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9258 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/documentmanifest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    13328 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/documentreference.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1473 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/domainresource.py
--rw-r--r--   0 nazrul     (501) staff       (20)      436 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/duration.py
--rw-r--r--   0 nazrul     (501) staff       (20)      890 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/element.py
--rw-r--r--   0 nazrul     (501) staff       (20)   139889 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/elementdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2672 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/eligibilityrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3445 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/eligibilityresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11725 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/encounter.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3460 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/enrollmentrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3368 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/enrollmentresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7537 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/episodeofcare.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3582 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/explanationofbenefit.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10926 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/extension.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15803 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/familymemberhistory.py
--rw-r--r--   0 nazrul     (501) staff       (20)    13921 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/fhirabstractmodel.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1697 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/fhirprimitiveextension.py
--rw-r--r--   0 nazrul     (501) staff       (20)      669 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/fhirresourcemodel.py
--rw-r--r--   0 nazrul     (501) staff       (20)    59249 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/fhirtypes.py
--rw-r--r--   0 nazrul     (501) staff       (20)    83454 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/fhirtypesvalidators.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2513 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/flag.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9753 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/goal.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7205 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/group.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10717 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/healthcareservice.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1980 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/humanname.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1760 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/identifier.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6981 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/imagingobjectselection.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10901 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/imagingstudy.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9005 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/immunization.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6417 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/immunizationrecommendation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18060 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/implementationguide.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5721 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/list.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4441 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/location.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3237 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/media.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5173 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/medication.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11331 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/medicationadministration.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18235 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/medicationdispense.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20165 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/medicationorder.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14759 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/medicationstatement.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9139 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/messageheader.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1666 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/meta.py
--rw-r--r--   0 nazrul     (501) staff       (20)      568 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/money.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8065 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/namingsystem.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1017 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/narrative.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17472 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/nutritionorder.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19452 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/observation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14583 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/operationdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2030 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/operationoutcome.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7224 2023-04-08 12:10:41.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/order.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3028 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/orderresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3673 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/organization.py
--rw-r--r--   0 nazrul     (501) staff       (20)    13360 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/parameters.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11800 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/patient.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3568 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/paymentnotice.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7979 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/paymentreconciliation.py
--rw-r--r--   0 nazrul     (501) staff       (20)      848 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/period.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3653 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/person.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6475 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/practitioner.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10327 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/procedure.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7572 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/procedurerequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5440 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/processrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5011 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/processresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9407 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/provenance.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1568 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/quantity.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9683 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/questionnaire.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15921 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/questionnaireresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)      770 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/range.py
--rw-r--r--   0 nazrul     (501) staff       (20)      861 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/ratio.py
--rw-r--r--   0 nazrul     (501) staff       (20)      782 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/reference.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6367 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/referralrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2882 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/relatedperson.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1210 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/resource.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9509 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/riskassessment.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1965 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/sampleddata.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2515 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/schedule.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6052 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/searchparameter.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4116 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/signature.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2546 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/slot.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14047 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/specimen.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4698 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/subscription.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4216 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/substance.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3960 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/supplydelivery.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7073 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/supplyrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    33410 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/testscript.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6571 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/timing.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20175 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/valueset.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9975 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/DSTU2/visionprescription.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:43.117155 fhir.resources-7.0.0/fhir/resources/R4B/
--rw-r--r--   0 nazrul     (501) staff       (20)      830 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/__init__.py
--rw-r--r--   0 nazrul     (501) staff       (20)    13539 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/account.py
--rw-r--r--   0 nazrul     (501) staff       (20)    50060 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/activitydefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6744 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/address.py
--rw-r--r--   0 nazrul     (501) staff       (20)    25728 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/administrableproductdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19227 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/adverseevent.py
--rw-r--r--   0 nazrul     (501) staff       (20)      854 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/age.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20908 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/allergyintolerance.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7797 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/annotation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23914 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/appointment.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8807 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/appointmentresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4966 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/attachment.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32696 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/auditevent.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2313 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/backboneelement.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3540 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/basic.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6329 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/binary.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22890 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/biologicallyderivedproduct.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4520 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/bodystructure.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32409 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/bundle.py
--rw-r--r--   0 nazrul     (501) staff       (20)    99187 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/capabilitystatement.py
--rw-r--r--   0 nazrul     (501) staff       (20)    40250 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/careplan.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10040 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/careteam.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14810 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/catalogentry.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23255 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/chargeitem.py
--rw-r--r--   0 nazrul     (501) staff       (20)    30345 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/chargeitemdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    95627 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/citation.py
--rw-r--r--   0 nazrul     (501) staff       (20)   104245 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/claim.py
--rw-r--r--   0 nazrul     (501) staff       (20)    78305 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/claimresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21601 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/clinicalimpression.py
--rw-r--r--   0 nazrul     (501) staff       (20)    33030 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/clinicalusedefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1898 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/codeableconcept.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1811 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/codeablereference.py
--rw-r--r--   0 nazrul     (501) staff       (20)    54546 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/codesystem.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3954 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/coding.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21634 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/communication.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23292 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/communicationrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18666 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/compartmentdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    34249 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/composition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    45816 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/conceptmap.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20942 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/condition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    33320 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/consent.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1707 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/contactdetail.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3830 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/contactpoint.py
--rw-r--r--   0 nazrul     (501) staff       (20)   111474 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/contract.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5346 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/contributor.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1049 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/count.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23490 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/coverage.py
--rw-r--r--   0 nazrul     (501) staff       (20)    31385 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/coverageeligibilityrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32405 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/coverageeligibilityresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    28362 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/datarequirement.py
--rw-r--r--   0 nazrul     (501) staff       (20)    16945 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/detectedissue.py
--rw-r--r--   0 nazrul     (501) staff       (20)    31767 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/device.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32799 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/devicedefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    13593 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/devicemetric.py
--rw-r--r--   0 nazrul     (501) staff       (20)    26992 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/devicerequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    13738 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/deviceusestatement.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19547 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/diagnosticreport.py
--rw-r--r--   0 nazrul     (501) staff       (20)      862 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/distance.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12517 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/documentmanifest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23502 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/documentreference.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4499 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/domainresource.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14027 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/dosage.py
--rw-r--r--   0 nazrul     (501) staff       (20)      820 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/duration.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2070 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/element.py
--rw-r--r--   0 nazrul     (501) staff       (20)   285014 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/elementdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    33499 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/encounter.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10437 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/endpoint.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4346 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/enrollmentrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5153 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/enrollmentresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17317 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/episodeofcare.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22850 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/eventdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    42202 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/evidence.py
--rw-r--r--   0 nazrul     (501) staff       (20)    37151 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/evidencereport.py
--rw-r--r--   0 nazrul     (501) staff       (20)    34996 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/evidencevariable.py
--rw-r--r--   0 nazrul     (501) staff       (20)    54510 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/examplescenario.py
--rw-r--r--   0 nazrul     (501) staff       (20)   153338 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/explanationofbenefit.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7002 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/expression.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32859 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/extension.py
--rw-r--r--   0 nazrul     (501) staff       (20)    28665 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/familymemberhistory.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1972 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/fhirprimitiveextension.py
--rw-r--r--   0 nazrul     (501) staff       (20)      689 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/fhirresourcemodel.py
--rw-r--r--   0 nazrul     (501) staff       (20)   116670 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/fhirtypes.py
--rw-r--r--   0 nazrul     (501) staff       (20)   180878 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/fhirtypesvalidators.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8228 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/flag.py
--rw-r--r--   0 nazrul     (501) staff       (20)    26278 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/goal.py
--rw-r--r--   0 nazrul     (501) staff       (20)    28845 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/graphdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21190 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/group.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17006 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/guidanceresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22540 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/healthcareservice.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5058 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/humanname.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3886 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/identifier.py
--rw-r--r--   0 nazrul     (501) staff       (20)    31624 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/imagingstudy.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32808 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/immunization.py
--rw-r--r--   0 nazrul     (501) staff       (20)    13962 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/immunizationevaluation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21004 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/immunizationrecommendation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    73115 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/implementationguide.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27815 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/ingredient.py
--rw-r--r--   0 nazrul     (501) staff       (20)    25493 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/insuranceplan.py
--rw-r--r--   0 nazrul     (501) staff       (20)    25269 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/invoice.py
--rw-r--r--   0 nazrul     (501) staff       (20)    24627 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/library.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7601 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/linkage.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12397 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/list.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18304 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/location.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12896 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/manufactureditemdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4263 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/marketingstatus.py
--rw-r--r--   0 nazrul     (501) staff       (20)    44394 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/measure.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23949 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/measurereport.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17584 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/media.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11656 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/medication.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27500 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/medicationadministration.py
--rw-r--r--   0 nazrul     (501) staff       (20)    28466 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/medicationdispense.py
--rw-r--r--   0 nazrul     (501) staff       (20)    53647 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/medicationknowledge.py
--rw-r--r--   0 nazrul     (501) staff       (20)    38964 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/medicationrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19295 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/medicationstatement.py
--rw-r--r--   0 nazrul     (501) staff       (20)    41125 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/medicinalproductdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32489 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/messagedefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    26908 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/messageheader.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4891 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/meta.py
--rw-r--r--   0 nazrul     (501) staff       (20)    55714 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/molecularsequence.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1594 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/money.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18173 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/namingsystem.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5186 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/narrative.py
--rw-r--r--   0 nazrul     (501) staff       (20)    36907 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/nutritionorder.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21176 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/nutritionproduct.py
--rw-r--r--   0 nazrul     (501) staff       (20)    45787 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/observation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    16617 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/observationdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    42395 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/operationdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9397 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/operationoutcome.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7329 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/organization.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6666 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/organizationaffiliation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    31017 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/packagedproductdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7856 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/parameterdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    34815 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/parameters.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22486 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/patient.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9483 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/paymentnotice.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17904 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/paymentreconciliation.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2031 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/period.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6889 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/person.py
--rw-r--r--   0 nazrul     (501) staff       (20)    83343 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/plandefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4739 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/population.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8273 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/practitioner.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15738 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/practitionerrole.py
--rw-r--r--   0 nazrul     (501) staff       (20)    28668 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/procedure.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6997 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/prodcharacteristic.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3196 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/productshelflife.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19730 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/provenance.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3855 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/quantity.py
--rw-r--r--   0 nazrul     (501) staff       (20)    61641 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/questionnaire.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27489 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/questionnaireresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1386 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/range.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1463 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/ratio.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1754 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/ratiorange.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4459 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/reference.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15372 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/regulatedauthorization.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8056 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/relatedartifact.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8102 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/relatedperson.py
--rw-r--r--   0 nazrul     (501) staff       (20)    43137 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/requestgroup.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27479 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/researchdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    44428 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/researchelementdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23368 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/researchstudy.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8449 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/researchsubject.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2913 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/resource.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21329 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/riskassessment.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8009 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/sampleddata.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5117 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/schedule.py
--rw-r--r--   0 nazrul     (501) staff       (20)    26904 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/searchparameter.py
--rw-r--r--   0 nazrul     (501) staff       (20)    29332 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/servicerequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8366 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/signature.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9200 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/slot.py
--rw-r--r--   0 nazrul     (501) staff       (20)    25765 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/specimen.py
--rw-r--r--   0 nazrul     (501) staff       (20)    24076 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/specimendefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    34768 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/structuredefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    93850 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/structuremap.py
--rw-r--r--   0 nazrul     (501) staff       (20)    13989 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/subscription.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14583 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/subscriptionstatus.py
--rw-r--r--   0 nazrul     (501) staff       (20)    49885 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/subscriptiontopic.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10384 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/substance.py
--rw-r--r--   0 nazrul     (501) staff       (20)    54084 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/substancedefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    13996 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/supplydelivery.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17377 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/supplyrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    81842 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/task.py
--rw-r--r--   0 nazrul     (501) staff       (20)    54613 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/terminologycapabilities.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32457 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/testreport.py
--rw-r--r--   0 nazrul     (501) staff       (20)    95713 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/testscript.py
--rw-r--r--   0 nazrul     (501) staff       (20)    16486 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/timing.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10684 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/triggerdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6155 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/usagecontext.py
--rw-r--r--   0 nazrul     (501) staff       (20)    62016 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/valueset.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20833 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/verificationresult.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22470 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/R4B/visionprescription.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:43.138502 fhir.resources-7.0.0/fhir/resources/STU3/
--rw-r--r--   0 nazrul     (501) staff       (20)      830 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/__init__.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10847 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/account.py
--rw-r--r--   0 nazrul     (501) staff       (20)    35926 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/activitydefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6554 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/address.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14178 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/adverseevent.py
--rw-r--r--   0 nazrul     (501) staff       (20)      849 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/age.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22884 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/allergyintolerance.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7827 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/annotation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21666 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/appointment.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8991 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/appointmentresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4992 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/attachment.py
--rw-r--r--   0 nazrul     (501) staff       (20)    29854 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/auditevent.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2026 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/backboneelement.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3428 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/basic.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5477 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/binary.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4003 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/bodysite.py
--rw-r--r--   0 nazrul     (501) staff       (20)    30660 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/bundle.py
--rw-r--r--   0 nazrul     (501) staff       (20)   103071 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/capabilitystatement.py
--rw-r--r--   0 nazrul     (501) staff       (20)    35389 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/careplan.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9577 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/careteam.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20344 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/chargeitem.py
--rw-r--r--   0 nazrul     (501) staff       (20)    99818 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/claim.py
--rw-r--r--   0 nazrul     (501) staff       (20)    51155 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/claimresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23343 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/clinicalimpression.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1893 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/codeableconcept.py
--rw-r--r--   0 nazrul     (501) staff       (20)    51796 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/codesystem.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3949 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/coding.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18981 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/communication.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23368 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/communicationrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18397 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/compartmentdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    31988 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/composition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    41254 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/conceptmap.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21630 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/condition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    40275 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/consent.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1702 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/contactdetail.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3785 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/contactpoint.py
--rw-r--r--   0 nazrul     (501) staff       (20)    54217 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/contract.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5341 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/contributor.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1044 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/count.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17564 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/coverage.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19605 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/dataelement.py
--rw-r--r--   0 nazrul     (501) staff       (20)    26647 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/datarequirement.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12273 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/detectedissue.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15323 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/device.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9378 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/devicecomponent.py
--rw-r--r--   0 nazrul     (501) staff       (20)    13809 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/devicemetric.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17558 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/devicerequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11964 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/deviceusestatement.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20202 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/diagnosticreport.py
--rw-r--r--   0 nazrul     (501) staff       (20)      857 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/distance.py
--rw-r--r--   0 nazrul     (501) staff       (20)    16414 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/documentmanifest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    25213 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/documentreference.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4281 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/domainresource.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10303 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/dosage.py
--rw-r--r--   0 nazrul     (501) staff       (20)      815 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/duration.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2094 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/element.py
--rw-r--r--   0 nazrul     (501) staff       (20)   208084 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/elementdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10713 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/eligibilityrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20164 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/eligibilityresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    31315 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/encounter.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10413 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/endpoint.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4828 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/enrollmentrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5303 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/enrollmentresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17295 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/episodeofcare.py
--rw-r--r--   0 nazrul     (501) staff       (20)    34906 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/expansionprofile.py
--rw-r--r--   0 nazrul     (501) staff       (20)   124920 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/explanationofbenefit.py
--rw-r--r--   0 nazrul     (501) staff       (20)    25086 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/extension.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27883 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/familymemberhistory.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1972 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/fhirprimitiveextension.py
--rw-r--r--   0 nazrul     (501) staff       (20)      689 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/fhirresourcemodel.py
--rw-r--r--   0 nazrul     (501) staff       (20)    85336 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/fhirtypes.py
--rw-r--r--   0 nazrul     (501) staff       (20)   123530 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/fhirtypesvalidators.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8025 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/flag.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21580 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/goal.py
--rw-r--r--   0 nazrul     (501) staff       (20)    29359 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/graphdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19652 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/group.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15973 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/guidanceresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20902 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/healthcareservice.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4894 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/humanname.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3824 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/identifier.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20233 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/imagingmanifest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    29744 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/imagingstudy.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22782 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/immunization.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17627 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/immunizationrecommendation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    46599 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/implementationguide.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19407 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/library.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7441 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/linkage.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12451 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/list.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14346 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/location.py
--rw-r--r--   0 nazrul     (501) staff       (20)    39914 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/measure.py
--rw-r--r--   0 nazrul     (501) staff       (20)    24765 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/measurereport.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15160 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/media.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17734 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/medication.py
--rw-r--r--   0 nazrul     (501) staff       (20)    28079 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/medicationadministration.py
--rw-r--r--   0 nazrul     (501) staff       (20)    25458 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/medicationdispense.py
--rw-r--r--   0 nazrul     (501) staff       (20)    31914 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/medicationrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20069 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/medicationstatement.py
--rw-r--r--   0 nazrul     (501) staff       (20)    25231 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/messagedefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    26304 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/messageheader.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3873 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/meta.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11752 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/metadataresource.py
--rw-r--r--   0 nazrul     (501) staff       (20)      844 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/money.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18550 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/namingsystem.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5017 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/narrative.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32915 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/nutritionorder.py
--rw-r--r--   0 nazrul     (501) staff       (20)    41604 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/observation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    36395 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/operationdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9342 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/operationoutcome.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7314 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/organization.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7712 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/parameterdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27659 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/parameters.py
--rw-r--r--   0 nazrul     (501) staff       (20)    24319 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/patient.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5749 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/paymentnotice.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11845 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/paymentreconciliation.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1988 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/period.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6893 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/person.py
--rw-r--r--   0 nazrul     (501) staff       (20)    69678 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/plandefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7577 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/practitioner.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15509 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/practitionerrole.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23971 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/procedure.py
--rw-r--r--   0 nazrul     (501) staff       (20)    24213 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/procedurerequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12589 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/processrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8375 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/processresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23918 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/provenance.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3850 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/quantity.py
--rw-r--r--   0 nazrul     (501) staff       (20)    58838 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/questionnaire.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27697 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/questionnaireresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1381 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/range.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1458 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/ratio.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3351 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/reference.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21663 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/referralrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7369 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/relatedartifact.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5763 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/relatedperson.py
--rw-r--r--   0 nazrul     (501) staff       (20)    43966 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/requestgroup.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18893 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/researchstudy.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8413 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/researchsubject.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2775 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/resource.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21572 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/riskassessment.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8105 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/sampleddata.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5066 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/schedule.py
--rw-r--r--   0 nazrul     (501) staff       (20)    24995 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/searchparameter.py
--rw-r--r--   0 nazrul     (501) staff       (20)    45204 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/sequence.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18949 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/servicedefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11455 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/signature.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9182 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/slot.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23593 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/specimen.py
--rw-r--r--   0 nazrul     (501) staff       (20)    30110 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/structuredefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    85476 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/structuremap.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14313 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/subscription.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10379 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/substance.py
--rw-r--r--   0 nazrul     (501) staff       (20)    13970 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/supplydelivery.py
--rw-r--r--   0 nazrul     (501) staff       (20)    16352 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/supplyrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    70667 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/task.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32460 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/testreport.py
--rw-r--r--   0 nazrul     (501) staff       (20)   123792 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/testscript.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15534 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/timing.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9856 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/triggerdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5184 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/usagecontext.py
--rw-r--r--   0 nazrul     (501) staff       (20)    59750 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/valueset.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15071 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/STU3/visionprescription.py
--rw-r--r--   0 nazrul     (501) staff       (20)      852 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/__init__.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27683 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/account.py
--rw-r--r--   0 nazrul     (501) staff       (20)    52909 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/activitydefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21070 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/actordefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6867 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/address.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27846 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/administrableproductdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    47835 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/adverseevent.py
--rw-r--r--   0 nazrul     (501) staff       (20)      853 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/age.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22319 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/allergyintolerance.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7831 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/annotation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    48734 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/appointment.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11503 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/appointmentresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18581 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/artifactassessment.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7507 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/attachment.py
--rw-r--r--   0 nazrul     (501) staff       (20)    38324 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/auditevent.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5564 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/availability.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2311 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/backboneelement.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2298 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/backbonetype.py
--rw-r--r--   0 nazrul     (501) staff       (20)      861 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/base.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3589 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/basic.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6321 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/binary.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19339 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/biologicallyderivedproduct.py
--rw-r--r--   0 nazrul     (501) staff       (20)    13571 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/biologicallyderivedproductdispense.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11717 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/bodystructure.py
--rw-r--r--   0 nazrul     (501) staff       (20)    33439 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/bundle.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17569 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/canonicalresource.py
--rw-r--r--   0 nazrul     (501) staff       (20)   105958 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/capabilitystatement.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21195 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/careplan.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11459 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/careteam.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22191 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/chargeitem.py
--rw-r--r--   0 nazrul     (501) staff       (20)    28752 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/chargeitemdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    91486 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/citation.py
--rw-r--r--   0 nazrul     (501) staff       (20)   120177 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/claim.py
--rw-r--r--   0 nazrul     (501) staff       (20)   100008 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/claimresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18870 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/clinicalimpression.py
--rw-r--r--   0 nazrul     (501) staff       (20)    35458 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/clinicalusedefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1900 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/codeableconcept.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1813 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/codeablereference.py
--rw-r--r--   0 nazrul     (501) staff       (20)    63830 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/codesystem.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3956 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/coding.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21082 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/communication.py
--rw-r--r--   0 nazrul     (501) staff       (20)    24388 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/communicationrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23839 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/compartmentdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    25721 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/composition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    86135 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/conceptmap.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21674 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/condition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    37143 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/conditiondefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    34892 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/consent.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1709 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/contactdetail.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3832 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/contactpoint.py
--rw-r--r--   0 nazrul     (501) staff       (20)   109905 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/contract.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5348 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/contributor.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:43.138716 fhir.resources-7.0.0/fhir/resources/core/
--rw-r--r--   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/core/__init__.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17826 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/core/fhirabstractmodel.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:43.138948 fhir.resources-7.0.0/fhir/resources/core/patch/
--rw-r--r--   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/core/patch/__init__.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3094 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/core/patch/patch_r4b_test.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:43.139411 fhir.resources-7.0.0/fhir/resources/core/utils/
--rw-r--r--   0 nazrul     (501) staff       (20)     4186 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/core/utils/__init__.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1917 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/core/utils/common.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32378 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/core/utils/xml.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2162 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/core/utils/yaml.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1048 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/count.py
--rw-r--r--   0 nazrul     (501) staff       (20)    25653 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/coverage.py
--rw-r--r--   0 nazrul     (501) staff       (20)    35872 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/coverageeligibilityrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    37667 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/coverageeligibilityresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    35714 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/datarequirement.py
--rw-r--r--   0 nazrul     (501) staff       (20)      857 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/datatype.py
--rw-r--r--   0 nazrul     (501) staff       (20)    18884 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/detectedissue.py
--rw-r--r--   0 nazrul     (501) staff       (20)    46834 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/device.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6242 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/deviceassociation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    72710 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/devicedefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    16368 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/devicedispense.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12191 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/devicemetric.py
--rw-r--r--   0 nazrul     (501) staff       (20)    28352 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/devicerequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17094 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/deviceusage.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23798 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/diagnosticreport.py
--rw-r--r--   0 nazrul     (501) staff       (20)      861 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/distance.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27464 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/documentreference.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4642 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/domainresource.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12029 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/dosage.py
--rw-r--r--   0 nazrul     (501) staff       (20)      819 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/duration.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2000 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/element.py
--rw-r--r--   0 nazrul     (501) staff       (20)   336603 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/elementdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    31177 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/encounter.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12931 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/encounterhistory.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12770 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/endpoint.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4345 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/enrollmentrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5152 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/enrollmentresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19364 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/episodeofcare.py
--rw-r--r--   0 nazrul     (501) staff       (20)    25187 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/eventdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    47098 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/evidence.py
--rw-r--r--   0 nazrul     (501) staff       (20)    36926 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/evidencereport.py
--rw-r--r--   0 nazrul     (501) staff       (20)    59043 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/evidencevariable.py
--rw-r--r--   0 nazrul     (501) staff       (20)    67834 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/examplescenario.py
--rw-r--r--   0 nazrul     (501) staff       (20)   184073 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/explanationofbenefit.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3899 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/expression.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3292 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/extendedcontactdetail.py
--rw-r--r--   0 nazrul     (501) staff       (20)    34655 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/extension.py
--rw-r--r--   0 nazrul     (501) staff       (20)    40454 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/familymemberhistory.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2055 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/fhirprimitiveextension.py
--rw-r--r--   0 nazrul     (501) staff       (20)      689 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/fhirresourcemodel.py
--rw-r--r--   0 nazrul     (501) staff       (20)   140270 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/fhirtypes.py
--rw-r--r--   0 nazrul     (501) staff       (20)   224498 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/fhirtypesvalidators.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8332 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/flag.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2806 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/formularyitem.py
--rw-r--r--   0 nazrul     (501) staff       (20)    28537 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/genomicstudy.py
--rw-r--r--   0 nazrul     (501) staff       (20)    26478 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/goal.py
--rw-r--r--   0 nazrul     (501) staff       (20)    38493 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/graphdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23025 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/group.py
--rw-r--r--   0 nazrul     (501) staff       (20)    16969 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/guidanceresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14157 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/healthcareservice.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5250 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/humanname.py
--rw-r--r--   0 nazrul     (501) staff       (20)     3898 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/identifier.py
--rw-r--r--   0 nazrul     (501) staff       (20)    33736 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/imagingselection.py
--rw-r--r--   0 nazrul     (501) staff       (20)    31562 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/imagingstudy.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32588 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/immunization.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10530 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/immunizationevaluation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17370 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/immunizationrecommendation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    74780 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/implementationguide.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32777 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/ingredient.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23681 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/insuranceplan.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1250 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/integer64.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32280 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/inventoryitem.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12950 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/inventoryreport.py
--rw-r--r--   0 nazrul     (501) staff       (20)    23752 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/invoice.py
--rw-r--r--   0 nazrul     (501) staff       (20)    26988 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/library.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7600 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/linkage.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12723 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/list.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15870 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/location.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21416 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/manufactureditemdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4253 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/marketingstatus.py
--rw-r--r--   0 nazrul     (501) staff       (20)    63709 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/measure.py
--rw-r--r--   0 nazrul     (501) staff       (20)    52921 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/measurereport.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14129 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/medication.py
--rw-r--r--   0 nazrul     (501) staff       (20)    29781 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/medicationadministration.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27280 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/medicationdispense.py
--rw-r--r--   0 nazrul     (501) staff       (20)    69462 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/medicationknowledge.py
--rw-r--r--   0 nazrul     (501) staff       (20)    38124 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/medicationrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20705 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/medicationstatement.py
--rw-r--r--   0 nazrul     (501) staff       (20)    43321 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/medicinalproductdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    34663 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/messagedefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    26076 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/messageheader.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4893 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/meta.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5706 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/metadataresource.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21225 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/molecularsequence.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5565 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/monetarycomponent.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1596 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/money.py
--rw-r--r--   0 nazrul     (501) staff       (20)    32328 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/namingsystem.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5188 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/narrative.py
--rw-r--r--   0 nazrul     (501) staff       (20)    26852 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/nutritionintake.py
--rw-r--r--   0 nazrul     (501) staff       (20)    49638 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/nutritionorder.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22222 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/nutritionproduct.py
--rw-r--r--   0 nazrul     (501) staff       (20)    56718 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/observation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    41090 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/observationdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    49489 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/operationdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9417 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/operationoutcome.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9036 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/organization.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6801 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/organizationaffiliation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27823 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/packagedproductdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7858 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/parameterdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    37058 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/parameters.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22462 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/patient.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9407 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/paymentnotice.py
--rw-r--r--   0 nazrul     (501) staff       (20)    29923 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/paymentreconciliation.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2033 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/period.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20362 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/permission.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12650 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/person.py
--rw-r--r--   0 nazrul     (501) staff       (20)   104212 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/plandefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14188 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/practitioner.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8537 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/practitionerrole.py
--rw-r--r--   0 nazrul     (501) staff       (20)      899 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/primitivetype.py
--rw-r--r--   0 nazrul     (501) staff       (20)    34220 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/procedure.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5794 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/productshelflife.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19418 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/provenance.py
--rw-r--r--   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/py.typed
--rw-r--r--   0 nazrul     (501) staff       (20)     3868 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/quantity.py
--rw-r--r--   0 nazrul     (501) staff       (20)    69392 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/questionnaire.py
--rw-r--r--   0 nazrul     (501) staff       (20)    27950 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/questionnaireresponse.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1388 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/range.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1465 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/ratio.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1756 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/ratiorange.py
--rw-r--r--   0 nazrul     (501) staff       (20)     4534 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/reference.py
--rw-r--r--   0 nazrul     (501) staff       (20)    15970 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/regulatedauthorization.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10954 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/relatedartifact.py
--rw-r--r--   0 nazrul     (501) staff       (20)     8217 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/relatedperson.py
--rw-r--r--   0 nazrul     (501) staff       (20)    65672 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/requestorchestration.py
--rw-r--r--   0 nazrul     (501) staff       (20)    29907 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/requirements.py
--rw-r--r--   0 nazrul     (501) staff       (20)    41014 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/researchstudy.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12039 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/researchsubject.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2873 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/resource.py
--rw-r--r--   0 nazrul     (501) staff       (20)    21107 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/riskassessment.py
--rw-r--r--   0 nazrul     (501) staff       (20)    10115 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/sampleddata.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5775 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/schedule.py
--rw-r--r--   0 nazrul     (501) staff       (20)    33129 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/searchparameter.py
--rw-r--r--   0 nazrul     (501) staff       (20)    42296 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/servicerequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)     5498 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/signature.py
--rw-r--r--   0 nazrul     (501) staff       (20)     9334 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/slot.py
--rw-r--r--   0 nazrul     (501) staff       (20)    29691 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/specimen.py
--rw-r--r--   0 nazrul     (501) staff       (20)    45103 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/specimendefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    39442 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/structuredefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    65978 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/structuremap.py
--rw-r--r--   0 nazrul     (501) staff       (20)    26517 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/subscription.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14669 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/subscriptionstatus.py
--rw-r--r--   0 nazrul     (501) staff       (20)    55698 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/subscriptiontopic.py
--rw-r--r--   0 nazrul     (501) staff       (20)    12373 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/substance.py
--rw-r--r--   0 nazrul     (501) staff       (20)    58680 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/substancedefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14006 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/substancenucleicacid.py
--rw-r--r--   0 nazrul     (501) staff       (20)    16879 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/substancepolymer.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11131 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/substanceprotein.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11213 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/substancereferenceinformation.py
--rw-r--r--   0 nazrul     (501) staff       (20)    25015 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/substancesourcematerial.py
--rw-r--r--   0 nazrul     (501) staff       (20)    14242 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/supplydelivery.py
--rw-r--r--   0 nazrul     (501) staff       (20)    17413 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/supplyrequest.py
--rw-r--r--   0 nazrul     (501) staff       (20)    89564 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/task.py
--rw-r--r--   0 nazrul     (501) staff       (20)    62982 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/terminologycapabilities.py
--rw-r--r--   0 nazrul     (501) staff       (20)    38948 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/testplan.py
--rw-r--r--   0 nazrul     (501) staff       (20)    37374 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/testreport.py
--rw-r--r--   0 nazrul     (501) staff       (20)   114767 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/testscript.py
--rw-r--r--   0 nazrul     (501) staff       (20)    16986 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/timing.py
--rw-r--r--   0 nazrul     (501) staff       (20)    88330 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/transport.py
--rw-r--r--   0 nazrul     (501) staff       (20)    11790 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/triggerdefinition.py
--rw-r--r--   0 nazrul     (501) staff       (20)     6157 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/usagecontext.py
--rw-r--r--   0 nazrul     (501) staff       (20)   101600 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/valueset.py
--rw-r--r--   0 nazrul     (501) staff       (20)    20952 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/verificationresult.py
--rw-r--r--   0 nazrul     (501) staff       (20)     7771 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/virtualservicedetail.py
--rw-r--r--   0 nazrul     (501) staff       (20)    22469 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir/resources/visionprescription.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-04-08 12:10:43.047029 fhir.resources-7.0.0/fhir.resources.egg-info/
--rw-r--r--   0 nazrul     (501) staff       (20)    41868 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir.resources.egg-info/PKG-INFO
--rw-r--r--   0 nazrul     (501) staff       (20)    25076 2023-04-08 12:10:43.000000 fhir.resources-7.0.0/fhir.resources.egg-info/SOURCES.txt
--rw-r--r--   0 nazrul     (501) staff       (20)        1 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir.resources.egg-info/dependency_links.txt
--rw-r--r--   0 nazrul     (501) staff       (20)        5 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir.resources.egg-info/namespace_packages.txt
--rw-r--r--   0 nazrul     (501) staff       (20)        1 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir.resources.egg-info/not-zip-safe
--rw-r--r--   0 nazrul     (501) staff       (20)      798 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir.resources.egg-info/requires.txt
--rw-r--r--   0 nazrul     (501) staff       (20)        5 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/fhir.resources.egg-info/top_level.txt
--rw-r--r--   0 nazrul     (501) staff       (20)      142 2023-04-08 12:10:43.139835 fhir.resources-7.0.0/setup.cfg
--rw-r--r--   0 nazrul     (501) staff       (20)     4523 2023-04-08 12:10:42.000000 fhir.resources-7.0.0/setup.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.996608 fhir.resources-7.0.1/
+-rw-r--r--   0 nazrul     (501) staff       (20)      255 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/AUTHORS.rst
+-rw-r--r--   0 nazrul     (501) staff       (20)     4595 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 nazrul     (501) staff       (20)    10247 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/HISTORY.rst
+-rw-r--r--   0 nazrul     (501) staff       (20)     1509 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/LICENSE
+-rw-r--r--   0 nazrul     (501) staff       (20)      500 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/MANIFEST.in
+-rw-r--r--   0 nazrul     (501) staff       (20)    42135 2023-05-29 12:03:25.996740 fhir.resources-7.0.1/PKG-INFO
+-rw-r--r--   0 nazrul     (501) staff       (20)    30110 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/README.rst
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.899844 fhir.resources-7.0.1/fhir/
+-rw-r--r--   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/__init__.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.931541 fhir.resources-7.0.1/fhir/resources/
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.947304 fhir.resources-7.0.1/fhir/resources/DSTU2/
+-rw-r--r--   0 nazrul     (501) staff       (20)      822 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/__init__.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2984 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/account.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2588 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/address.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      499 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/age.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6378 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/allergyintolerance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3447 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/annotation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4785 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/appointment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2595 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/appointmentresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2078 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/attachment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9925 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/auditevent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      774 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/backboneelement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1772 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/basic.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      868 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/binary.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1938 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/bodysite.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7233 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/bundle.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15002 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/careplan.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19956 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/claim.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19205 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/claimresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10208 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/clinicalimpression.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1106 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/codeableconcept.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1909 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/coding.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6809 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/communication.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9538 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/communicationrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8480 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/composition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10908 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/conceptmap.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11352 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/condition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22229 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/conformance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1607 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/contactpoint.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    34499 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/contract.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      522 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/count.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4500 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/coverage.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5648 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/dataelement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5595 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/detectedissue.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4230 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/device.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4586 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/devicecomponent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7358 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/devicemetric.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8132 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/deviceuserequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6220 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/deviceusestatement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9542 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/diagnosticorder.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8620 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/diagnosticreport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      444 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/distance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9258 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/documentmanifest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    13328 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/documentreference.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1473 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/domainresource.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      436 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/duration.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      890 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/element.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   139889 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/elementdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2672 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/eligibilityrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3445 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/eligibilityresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11725 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/encounter.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3460 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/enrollmentrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3368 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/enrollmentresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7537 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/episodeofcare.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3582 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/explanationofbenefit.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10926 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/extension.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15803 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/familymemberhistory.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    13921 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/fhirabstractmodel.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1697 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/fhirprimitiveextension.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      669 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/fhirresourcemodel.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    59249 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/fhirtypes.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    83454 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/fhirtypesvalidators.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2513 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/flag.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9753 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/goal.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7205 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/group.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10717 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/healthcareservice.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1980 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/humanname.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1760 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/identifier.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6981 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/imagingobjectselection.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10901 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/imagingstudy.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9005 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/immunization.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6417 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/immunizationrecommendation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18060 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/implementationguide.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5721 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/list.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4441 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/location.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3237 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/media.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5173 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/medication.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11331 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/medicationadministration.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18235 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/medicationdispense.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20165 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/medicationorder.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14759 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/medicationstatement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9139 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/messageheader.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1666 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/meta.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      568 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/money.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8065 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/namingsystem.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1017 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/narrative.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17472 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/nutritionorder.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19452 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/observation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14583 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/operationdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2030 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/operationoutcome.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7224 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/order.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3028 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/orderresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3673 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/organization.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    13360 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/parameters.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11800 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/patient.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3568 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/paymentnotice.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7979 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/paymentreconciliation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      848 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/period.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3653 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/person.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6475 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/practitioner.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10327 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/procedure.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7572 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/procedurerequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5440 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/processrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5011 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/processresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9407 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/provenance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1568 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/quantity.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9683 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/questionnaire.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15921 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/questionnaireresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      770 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/range.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      861 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/ratio.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      782 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/reference.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6367 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/referralrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2882 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/relatedperson.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1210 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/resource.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9509 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/riskassessment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1965 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/sampleddata.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2515 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/schedule.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6052 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/searchparameter.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4116 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/signature.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2546 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/slot.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14047 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/specimen.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4698 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/subscription.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4216 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/substance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3960 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/supplydelivery.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7073 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/supplyrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    33410 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/testscript.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6571 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/timing.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20175 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/valueset.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9975 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/DSTU2/visionprescription.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.973678 fhir.resources-7.0.1/fhir/resources/R4B/
+-rw-r--r--   0 nazrul     (501) staff       (20)      830 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/__init__.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    13539 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/account.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    50060 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/activitydefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6744 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/address.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    25728 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/administrableproductdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19227 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/adverseevent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      854 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/age.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20908 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/allergyintolerance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7797 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/annotation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23914 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/appointment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8807 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/appointmentresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4966 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/attachment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32696 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/auditevent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2313 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/backboneelement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3540 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/basic.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6329 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/binary.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22890 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/biologicallyderivedproduct.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4520 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/bodystructure.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32409 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/bundle.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    99187 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/capabilitystatement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    40250 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/careplan.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10040 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/careteam.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14810 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/catalogentry.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23255 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/chargeitem.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    30345 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/chargeitemdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    95627 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/citation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   104245 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/claim.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    78305 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/claimresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21601 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/clinicalimpression.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    33030 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/clinicalusedefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1898 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/codeableconcept.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1811 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/codeablereference.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    54546 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/codesystem.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3954 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/coding.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21634 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/communication.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23292 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/communicationrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18666 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/compartmentdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    34249 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/composition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    45816 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/conceptmap.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20942 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/condition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    33320 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/consent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1707 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/contactdetail.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3830 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/contactpoint.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   111474 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/contract.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5346 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/contributor.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1049 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/count.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23490 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/coverage.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    31385 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/coverageeligibilityrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32405 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/coverageeligibilityresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    28362 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/datarequirement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    16945 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/detectedissue.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    31767 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/device.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32799 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/devicedefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    13593 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/devicemetric.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    26992 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/devicerequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    13738 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/deviceusestatement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19547 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/diagnosticreport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      862 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/distance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12517 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/documentmanifest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23502 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/documentreference.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4499 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/domainresource.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14027 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/dosage.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      820 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/duration.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2070 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/element.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   285014 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/elementdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    33499 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/encounter.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10437 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/endpoint.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4346 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/enrollmentrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5153 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/enrollmentresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17317 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/episodeofcare.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22850 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/eventdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    42202 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/evidence.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    37151 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/evidencereport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    34996 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/evidencevariable.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    54510 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/examplescenario.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   153338 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/explanationofbenefit.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7002 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/expression.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32859 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/extension.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    28665 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/familymemberhistory.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1972 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/fhirprimitiveextension.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      689 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/fhirresourcemodel.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   116838 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/fhirtypes.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   180878 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/fhirtypesvalidators.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8228 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/flag.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    26278 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/goal.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    28845 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/graphdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21190 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/group.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17006 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/guidanceresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22540 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/healthcareservice.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5058 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/humanname.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3886 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/identifier.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    31624 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/imagingstudy.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32808 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/immunization.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    13962 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/immunizationevaluation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21004 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/immunizationrecommendation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    73115 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/implementationguide.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27815 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/ingredient.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    25493 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/insuranceplan.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    25269 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/invoice.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    24627 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/library.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7601 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/linkage.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12397 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/list.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18304 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/location.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12896 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/manufactureditemdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4263 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/marketingstatus.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    44394 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/measure.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23949 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/measurereport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17584 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/media.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11656 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/medication.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27500 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/medicationadministration.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    28466 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/medicationdispense.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    53647 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/medicationknowledge.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    38964 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/medicationrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19295 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/medicationstatement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    41125 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/medicinalproductdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32489 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/messagedefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    26908 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/messageheader.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4891 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/meta.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    55714 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/molecularsequence.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1594 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/money.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18173 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/namingsystem.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5186 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/narrative.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    36907 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/nutritionorder.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21176 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/nutritionproduct.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    45787 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/observation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    16617 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/observationdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    42395 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/operationdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9397 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/operationoutcome.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7329 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/organization.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6666 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/organizationaffiliation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    31017 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/packagedproductdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7856 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/parameterdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    34815 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/parameters.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22486 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/patient.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9483 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/paymentnotice.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17904 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/paymentreconciliation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2031 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/period.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6889 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/person.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    83343 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/plandefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4739 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/population.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8273 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/practitioner.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15738 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/practitionerrole.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    28668 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/procedure.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6997 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/prodcharacteristic.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3196 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/productshelflife.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19730 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/provenance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3855 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/quantity.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    61641 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/questionnaire.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27489 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/questionnaireresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1386 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/range.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1463 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/ratio.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1754 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/ratiorange.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4459 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/reference.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15372 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/regulatedauthorization.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8056 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/relatedartifact.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8102 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/relatedperson.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    43137 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/requestgroup.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27479 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/researchdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    44428 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/researchelementdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23368 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/researchstudy.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8449 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/researchsubject.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2913 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/resource.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21329 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/riskassessment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8009 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/sampleddata.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5117 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/schedule.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    26904 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/searchparameter.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    29332 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/servicerequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8366 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/signature.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9200 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/slot.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    25765 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/specimen.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    24076 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/specimendefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    34768 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/structuredefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    93850 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/structuremap.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    13989 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/subscription.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14583 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/subscriptionstatus.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    49885 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/subscriptiontopic.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10384 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/substance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    54084 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/substancedefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    13996 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/supplydelivery.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17377 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/supplyrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    81842 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/task.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    54613 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/terminologycapabilities.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32457 2023-05-29 12:03:24.000000 fhir.resources-7.0.1/fhir/resources/R4B/testreport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    95713 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/R4B/testscript.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    16486 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/R4B/timing.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10684 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/R4B/triggerdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6155 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/R4B/usagecontext.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    62016 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/R4B/valueset.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20833 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/R4B/verificationresult.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22470 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/R4B/visionprescription.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.995356 fhir.resources-7.0.1/fhir/resources/STU3/
+-rw-r--r--   0 nazrul     (501) staff       (20)      830 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/__init__.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10847 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/account.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    35926 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/activitydefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6554 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/address.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14178 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/adverseevent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      849 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/age.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22884 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/allergyintolerance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7827 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/annotation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21666 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/appointment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8991 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/appointmentresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4992 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/attachment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    29854 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/auditevent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2026 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/backboneelement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3428 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/basic.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5477 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/binary.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4003 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/bodysite.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    30660 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/bundle.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   103071 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/capabilitystatement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    35389 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/careplan.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9577 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/careteam.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20344 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/chargeitem.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    99818 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/claim.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    51155 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/claimresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23343 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/clinicalimpression.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1893 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/codeableconcept.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    51796 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/codesystem.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3949 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/coding.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18981 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/communication.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23368 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/communicationrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18397 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/compartmentdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    31988 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/composition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    41254 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/conceptmap.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21630 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/condition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    40275 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/consent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1702 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/contactdetail.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3785 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/contactpoint.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    54217 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/contract.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5341 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/contributor.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1044 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/count.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17564 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/coverage.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19605 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/dataelement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    26647 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/datarequirement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12273 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/detectedissue.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15323 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/device.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9378 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/devicecomponent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    13809 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/devicemetric.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17558 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/devicerequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11964 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/deviceusestatement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20202 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/diagnosticreport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      857 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/distance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    16414 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/documentmanifest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    25213 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/documentreference.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4281 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/domainresource.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10303 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/dosage.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      815 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/duration.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2094 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/element.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   208084 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/elementdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10713 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/eligibilityrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20164 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/eligibilityresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    31315 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/encounter.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10413 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/endpoint.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4828 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/enrollmentrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5303 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/enrollmentresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17295 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/episodeofcare.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    34906 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/expansionprofile.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   124920 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/explanationofbenefit.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    25086 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/extension.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27883 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/familymemberhistory.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1972 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/fhirprimitiveextension.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      689 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/fhirresourcemodel.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    85504 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/fhirtypes.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   123530 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/fhirtypesvalidators.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8025 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/flag.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21580 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/goal.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    29359 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/graphdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19652 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/group.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15973 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/guidanceresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20902 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/healthcareservice.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4894 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/humanname.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3824 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/identifier.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20233 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/imagingmanifest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    29744 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/imagingstudy.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22782 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/immunization.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17627 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/immunizationrecommendation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    46599 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/implementationguide.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19407 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/library.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7441 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/linkage.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12451 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/list.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14346 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/location.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    39914 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/measure.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    24765 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/measurereport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15160 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/media.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17734 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/medication.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    28079 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/medicationadministration.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    25458 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/medicationdispense.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    31914 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/medicationrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20069 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/medicationstatement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    25231 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/messagedefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    26304 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/messageheader.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3873 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/meta.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11752 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/metadataresource.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      844 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/money.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18550 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/namingsystem.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5017 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/narrative.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32915 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/nutritionorder.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    41604 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/observation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    36395 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/operationdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9342 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/operationoutcome.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7314 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/organization.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7712 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/parameterdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27659 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/parameters.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    24319 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/patient.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5749 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/paymentnotice.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11845 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/paymentreconciliation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1988 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/period.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6893 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/person.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    69678 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/plandefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7577 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/practitioner.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15509 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/practitionerrole.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23971 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/procedure.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    24213 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/procedurerequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12589 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/processrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8375 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/processresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23918 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/provenance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3850 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/quantity.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    58838 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/questionnaire.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27697 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/questionnaireresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1381 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/range.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1458 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/ratio.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3351 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/reference.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21663 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/referralrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7369 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/relatedartifact.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5763 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/relatedperson.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    43966 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/requestgroup.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18893 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/researchstudy.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8413 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/researchsubject.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2775 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/resource.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21572 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/riskassessment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8105 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/sampleddata.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5066 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/schedule.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    24995 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/searchparameter.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    45204 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/sequence.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18949 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/servicedefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11455 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/signature.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9182 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/slot.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23593 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/specimen.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    30110 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/structuredefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    85476 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/structuremap.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14313 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/subscription.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10379 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/substance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    13970 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/supplydelivery.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    16352 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/supplyrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    70667 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/task.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32460 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/testreport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   123792 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/testscript.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15534 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/timing.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9856 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/triggerdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5184 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/usagecontext.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    59750 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/valueset.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15071 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/STU3/visionprescription.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      852 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/__init__.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27683 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/account.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    52909 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/activitydefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21070 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/actordefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6867 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/address.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27846 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/administrableproductdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    47835 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/adverseevent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      853 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/age.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22319 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/allergyintolerance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7831 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/annotation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    48734 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/appointment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11503 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/appointmentresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18581 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/artifactassessment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7507 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/attachment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    38324 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/auditevent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5564 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/availability.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2311 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/backboneelement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2298 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/backbonetype.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      861 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/base.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3589 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/basic.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6321 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/binary.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19339 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/biologicallyderivedproduct.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    13571 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/biologicallyderivedproductdispense.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11717 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/bodystructure.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    33439 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/bundle.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17569 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/canonicalresource.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   105958 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/capabilitystatement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21195 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/careplan.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11459 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/careteam.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22191 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/chargeitem.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    28752 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/chargeitemdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    91486 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/citation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   120177 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/claim.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   100008 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/claimresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18870 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/clinicalimpression.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    35458 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/clinicalusedefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1900 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/codeableconcept.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1813 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/codeablereference.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    63830 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/codesystem.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3956 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/coding.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21082 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/communication.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    24388 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/communicationrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23839 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/compartmentdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    25721 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/composition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    86135 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/conceptmap.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21674 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/condition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    37143 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/conditiondefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    34892 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/consent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1709 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/contactdetail.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3832 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/contactpoint.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   109905 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/contract.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5348 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/contributor.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.995607 fhir.resources-7.0.1/fhir/resources/core/
+-rw-r--r--   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/core/__init__.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17826 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/core/fhirabstractmodel.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.995871 fhir.resources-7.0.1/fhir/resources/core/patch/
+-rw-r--r--   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/core/patch/__init__.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3094 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/core/patch/patch_r4b_test.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.996454 fhir.resources-7.0.1/fhir/resources/core/utils/
+-rw-r--r--   0 nazrul     (501) staff       (20)     4186 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/core/utils/__init__.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1917 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/core/utils/common.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32378 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/core/utils/xml.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2162 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/core/utils/yaml.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1048 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/count.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    25653 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/coverage.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    35872 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/coverageeligibilityrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    37667 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/coverageeligibilityresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    35714 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/datarequirement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      857 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/datatype.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    18884 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/detectedissue.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    46834 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/device.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6242 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/deviceassociation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    72710 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/devicedefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    16368 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/devicedispense.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12191 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/devicemetric.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    28352 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/devicerequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17094 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/deviceusage.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23798 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/diagnosticreport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      861 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/distance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27464 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/documentreference.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4642 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/domainresource.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12029 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/dosage.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      819 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/duration.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2000 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/element.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   336603 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/elementdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    31177 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/encounter.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12931 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/encounterhistory.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12770 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/endpoint.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4345 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/enrollmentrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5152 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/enrollmentresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19364 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/episodeofcare.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    25187 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/eventdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    47098 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/evidence.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    36926 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/evidencereport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    59043 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/evidencevariable.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    67834 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/examplescenario.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   184073 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/explanationofbenefit.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3899 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/expression.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3292 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/extendedcontactdetail.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    34655 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/extension.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    40454 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/familymemberhistory.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2055 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/fhirprimitiveextension.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      689 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/fhirresourcemodel.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   140438 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/fhirtypes.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   224498 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/fhirtypesvalidators.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8332 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/flag.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2806 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/formularyitem.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    28537 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/genomicstudy.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    26478 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/goal.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    38493 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/graphdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23025 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/group.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    16969 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/guidanceresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14157 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/healthcareservice.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5250 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/humanname.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     3898 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/identifier.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    33736 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/imagingselection.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    31562 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/imagingstudy.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32588 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/immunization.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10530 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/immunizationevaluation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17370 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/immunizationrecommendation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    74780 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/implementationguide.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32777 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/ingredient.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23681 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/insuranceplan.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1250 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/integer64.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32280 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/inventoryitem.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12950 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/inventoryreport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23752 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/invoice.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    26988 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/library.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7600 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/linkage.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12723 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/list.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15870 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/location.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21416 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/manufactureditemdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4253 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/marketingstatus.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    63709 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/measure.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    52921 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/measurereport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14129 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/medication.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    29781 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/medicationadministration.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27280 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/medicationdispense.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    69462 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/medicationknowledge.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    38124 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/medicationrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20705 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/medicationstatement.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    43321 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/medicinalproductdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    34663 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/messagedefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    26076 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/messageheader.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4893 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/meta.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5706 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/metadataresource.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21225 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/molecularsequence.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5565 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/monetarycomponent.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1596 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/money.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    32328 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/namingsystem.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5188 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/narrative.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    26852 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/nutritionintake.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    49638 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/nutritionorder.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22222 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/nutritionproduct.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    56718 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/observation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    41090 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/observationdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    49489 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/operationdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9417 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/operationoutcome.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9036 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/organization.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6801 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/organizationaffiliation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27823 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/packagedproductdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7858 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/parameterdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    37058 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/parameters.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22462 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/patient.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9407 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/paymentnotice.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    29923 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/paymentreconciliation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2033 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/period.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20362 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/permission.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12650 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/person.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   104212 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/plandefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14188 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/practitioner.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8537 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/practitionerrole.py
+-rw-r--r--   0 nazrul     (501) staff       (20)      899 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/primitivetype.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    34220 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/procedure.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5794 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/productshelflife.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    19418 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/provenance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/py.typed
+-rw-r--r--   0 nazrul     (501) staff       (20)     3868 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/quantity.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    69392 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/questionnaire.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    27950 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/questionnaireresponse.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1388 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/range.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1465 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/ratio.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1756 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/ratiorange.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     4534 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/reference.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    15970 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/regulatedauthorization.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10954 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/relatedartifact.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     8217 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/relatedperson.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    65672 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/requestorchestration.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    29907 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/requirements.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    41014 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/researchstudy.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12039 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/researchsubject.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2873 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/resource.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    21107 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/riskassessment.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    10115 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/sampleddata.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5775 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/schedule.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    33129 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/searchparameter.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    42296 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/servicerequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     5498 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/signature.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     9334 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/slot.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    29691 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/specimen.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    45103 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/specimendefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    39442 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/structuredefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    65978 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/structuremap.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    26517 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/subscription.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14669 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/subscriptionstatus.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    55698 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/subscriptiontopic.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    12373 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/substance.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    58680 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/substancedefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14006 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/substancenucleicacid.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    16879 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/substancepolymer.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11131 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/substanceprotein.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11213 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/substancereferenceinformation.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    25015 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/substancesourcematerial.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    14242 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/supplydelivery.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    17413 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/supplyrequest.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    89564 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/task.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    62982 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/terminologycapabilities.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    38948 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/testplan.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    37374 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/testreport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   114767 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/testscript.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    16986 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/timing.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    88330 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/transport.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    11790 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/triggerdefinition.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     6157 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/usagecontext.py
+-rw-r--r--   0 nazrul     (501) staff       (20)   101600 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/valueset.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    20952 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/verificationresult.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     7771 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/virtualservicedetail.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    22469 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir/resources/visionprescription.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-05-29 12:03:25.900644 fhir.resources-7.0.1/fhir.resources.egg-info/
+-rw-r--r--   0 nazrul     (501) staff       (20)    42135 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir.resources.egg-info/PKG-INFO
+-rw-r--r--   0 nazrul     (501) staff       (20)    25029 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir.resources.egg-info/SOURCES.txt
+-rw-r--r--   0 nazrul     (501) staff       (20)        1 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir.resources.egg-info/dependency_links.txt
+-rw-r--r--   0 nazrul     (501) staff       (20)        1 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir.resources.egg-info/not-zip-safe
+-rw-r--r--   0 nazrul     (501) staff       (20)      798 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir.resources.egg-info/requires.txt
+-rw-r--r--   0 nazrul     (501) staff       (20)        5 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/fhir.resources.egg-info/top_level.txt
+-rw-r--r--   0 nazrul     (501) staff       (20)      142 2023-05-29 12:03:25.997024 fhir.resources-7.0.1/setup.cfg
+-rw-r--r--   0 nazrul     (501) staff       (20)     4490 2023-05-29 12:03:25.000000 fhir.resources-7.0.1/setup.py
```

### Comparing `fhir.resources-7.0.0/CONTRIBUTING.rst` & `fhir.resources-7.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/HISTORY.rst` & `fhir.resources-7.0.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =======
 History
 =======
 
+7.0.1 (2023-05-29)
+------------------
+
+Fixes
+
+- Issue #128 `pkg_resources.declare_namespace deprecation <https://github.com/nazrulworld/fhir.resources/issues/128>`_
+
+- Issue #129 `urn not supported in Url <https://github.com/nazrulworld/fhir.resources/issues/129>`_
+
 7.0.0 (2023-04-08)
 ------------------
 
 New Feature
 
 - Support for `FHIR version R5 <https://www.hl7.org/fhir/R5/resourcelist.html>`_ has been added under root package.
```

### Comparing `fhir.resources-7.0.0/LICENSE` & `fhir.resources-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/PKG-INFO` & `fhir.resources-7.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhir.resources
-Version: 7.0.0
+Version: 7.0.1
 Summary: FHIR Resources as Model Class
 Home-page: https://github.com/nazrulworld/fhir.resources
 Author: Md Nazrul Islam
 Author-email: email2nazrul@gmail.com
 License: BSD license
 Project-URL: CI: Travis, https://travis-ci.org/github/nazrulworld/fhir.resources
 Project-URL: Coverage: codecov, https://codecov.io/gh/nazrulworld/fhir.resources
@@ -841,14 +841,23 @@
     :format: html
 
 
 =======
 History
 =======
 
+7.0.1 (2023-05-29)
+------------------
+
+Fixes
+
+- Issue #128 `pkg_resources.declare_namespace deprecation <https://github.com/nazrulworld/fhir.resources/issues/128>`_
+
+- Issue #129 `urn not supported in Url <https://github.com/nazrulworld/fhir.resources/issues/129>`_
+
 7.0.0 (2023-04-08)
 ------------------
 
 New Feature
 
 - Support for `FHIR version R5 <https://www.hl7.org/fhir/R5/resourcelist.html>`_ has been added under root package.
```

### Comparing `fhir.resources-7.0.0/README.rst` & `fhir.resources-7.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/__init__.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/__init__.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/account.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/account.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/address.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/address.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/allergyintolerance.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/allergyintolerance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/annotation.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/annotation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/appointment.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/appointment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/appointmentresponse.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/appointmentresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/attachment.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/attachment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/auditevent.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/auditevent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/backboneelement.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/backboneelement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/basic.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/basic.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/binary.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/binary.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/bodysite.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/bodysite.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/bundle.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/bundle.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/careplan.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/careplan.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/claim.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/claim.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/claimresponse.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/claimresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/clinicalimpression.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/clinicalimpression.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/codeableconcept.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/codeableconcept.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/coding.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/coding.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/communication.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/communication.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/communicationrequest.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/communicationrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/composition.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/composition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/conceptmap.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/conceptmap.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/condition.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/condition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/conformance.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/conformance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/contactpoint.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/contract.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/contract.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/count.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/count.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/coverage.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/coverage.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/dataelement.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/dataelement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/detectedissue.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/detectedissue.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/device.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/device.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/devicecomponent.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/devicecomponent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/devicemetric.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/devicemetric.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/deviceuserequest.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/deviceuserequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/deviceusestatement.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/deviceusestatement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/diagnosticorder.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/diagnosticorder.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/diagnosticreport.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/diagnosticreport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/documentmanifest.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/documentmanifest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/documentreference.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/documentreference.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/domainresource.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/domainresource.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/element.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/element.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/elementdefinition.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/elementdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/eligibilityrequest.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/eligibilityrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/eligibilityresponse.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/eligibilityresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/encounter.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/encounter.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/enrollmentrequest.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/enrollmentrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/enrollmentresponse.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/enrollmentresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/episodeofcare.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/episodeofcare.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/explanationofbenefit.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/explanationofbenefit.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/extension.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/extension.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/familymemberhistory.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/familymemberhistory.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/fhirabstractmodel.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/fhirabstractmodel.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/fhirprimitiveextension.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/fhirprimitiveextension.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/fhirresourcemodel.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/fhirresourcemodel.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/fhirtypes.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/fhirtypes.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/fhirtypesvalidators.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/fhirtypesvalidators.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/flag.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/flag.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/goal.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/goal.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/group.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/group.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/healthcareservice.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/healthcareservice.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/humanname.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/humanname.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/identifier.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/identifier.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/imagingobjectselection.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/imagingobjectselection.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/imagingstudy.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/imagingstudy.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/immunization.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/immunization.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/immunizationrecommendation.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/immunizationrecommendation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/implementationguide.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/implementationguide.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/list.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/list.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/location.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/location.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/media.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/media.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/medication.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/medication.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/medicationadministration.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/medicationadministration.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/medicationdispense.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/medicationdispense.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/medicationorder.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/medicationorder.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/medicationstatement.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/medicationstatement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/messageheader.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/messageheader.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/meta.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/meta.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/money.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/money.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/namingsystem.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/namingsystem.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/narrative.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/narrative.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/nutritionorder.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/nutritionorder.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/observation.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/observation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/operationdefinition.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/operationdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/operationoutcome.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/operationoutcome.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/order.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/order.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/orderresponse.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/orderresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/organization.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/organization.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/parameters.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/parameters.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/patient.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/patient.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/paymentnotice.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/paymentnotice.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/paymentreconciliation.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/paymentreconciliation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/period.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/period.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/person.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/person.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/practitioner.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/practitioner.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/procedure.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/procedure.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/procedurerequest.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/procedurerequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/processrequest.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/processrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/processresponse.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/processresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/provenance.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/provenance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/quantity.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/quantity.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/questionnaire.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/questionnaire.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/questionnaireresponse.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/questionnaireresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/range.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/range.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/ratio.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/ratio.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/reference.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/reference.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/referralrequest.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/referralrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/relatedperson.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/relatedperson.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/resource.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/resource.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/riskassessment.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/riskassessment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/sampleddata.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/sampleddata.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/schedule.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/schedule.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/searchparameter.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/searchparameter.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/signature.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/signature.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/slot.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/slot.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/specimen.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/specimen.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/subscription.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/subscription.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/substance.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/substance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/supplydelivery.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/supplydelivery.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/supplyrequest.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/supplyrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/testscript.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/testscript.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/timing.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/timing.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/valueset.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/valueset.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/DSTU2/visionprescription.py` & `fhir.resources-7.0.1/fhir/resources/DSTU2/visionprescription.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/__init__.py` & `fhir.resources-7.0.1/fhir/resources/R4B/__init__.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/account.py` & `fhir.resources-7.0.1/fhir/resources/R4B/account.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/activitydefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/activitydefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/address.py` & `fhir.resources-7.0.1/fhir/resources/R4B/address.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/administrableproductdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/administrableproductdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/adverseevent.py` & `fhir.resources-7.0.1/fhir/resources/R4B/adverseevent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/age.py` & `fhir.resources-7.0.1/fhir/resources/R4B/age.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/allergyintolerance.py` & `fhir.resources-7.0.1/fhir/resources/R4B/allergyintolerance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/annotation.py` & `fhir.resources-7.0.1/fhir/resources/R4B/annotation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/appointment.py` & `fhir.resources-7.0.1/fhir/resources/R4B/appointment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/appointmentresponse.py` & `fhir.resources-7.0.1/fhir/resources/R4B/appointmentresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/attachment.py` & `fhir.resources-7.0.1/fhir/resources/R4B/attachment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/auditevent.py` & `fhir.resources-7.0.1/fhir/resources/R4B/auditevent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/backboneelement.py` & `fhir.resources-7.0.1/fhir/resources/R4B/backboneelement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/basic.py` & `fhir.resources-7.0.1/fhir/resources/R4B/basic.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/binary.py` & `fhir.resources-7.0.1/fhir/resources/R4B/binary.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/biologicallyderivedproduct.py` & `fhir.resources-7.0.1/fhir/resources/R4B/biologicallyderivedproduct.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/bodystructure.py` & `fhir.resources-7.0.1/fhir/resources/R4B/bodystructure.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/bundle.py` & `fhir.resources-7.0.1/fhir/resources/R4B/bundle.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/capabilitystatement.py` & `fhir.resources-7.0.1/fhir/resources/R4B/capabilitystatement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/careplan.py` & `fhir.resources-7.0.1/fhir/resources/R4B/careplan.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/careteam.py` & `fhir.resources-7.0.1/fhir/resources/R4B/careteam.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/catalogentry.py` & `fhir.resources-7.0.1/fhir/resources/R4B/catalogentry.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/chargeitem.py` & `fhir.resources-7.0.1/fhir/resources/R4B/chargeitem.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/chargeitemdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/chargeitemdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/citation.py` & `fhir.resources-7.0.1/fhir/resources/R4B/citation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/claim.py` & `fhir.resources-7.0.1/fhir/resources/R4B/claim.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/claimresponse.py` & `fhir.resources-7.0.1/fhir/resources/R4B/claimresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/clinicalimpression.py` & `fhir.resources-7.0.1/fhir/resources/R4B/clinicalimpression.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/clinicalusedefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/clinicalusedefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/codeableconcept.py` & `fhir.resources-7.0.1/fhir/resources/R4B/codeableconcept.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/codeablereference.py` & `fhir.resources-7.0.1/fhir/resources/R4B/codeablereference.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/codesystem.py` & `fhir.resources-7.0.1/fhir/resources/R4B/codesystem.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/coding.py` & `fhir.resources-7.0.1/fhir/resources/R4B/coding.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/communication.py` & `fhir.resources-7.0.1/fhir/resources/R4B/communication.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/communicationrequest.py` & `fhir.resources-7.0.1/fhir/resources/R4B/communicationrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/compartmentdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/compartmentdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/composition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/composition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/conceptmap.py` & `fhir.resources-7.0.1/fhir/resources/R4B/conceptmap.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/condition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/condition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/consent.py` & `fhir.resources-7.0.1/fhir/resources/R4B/consent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/contactdetail.py` & `fhir.resources-7.0.1/fhir/resources/R4B/contactdetail.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/contactpoint.py` & `fhir.resources-7.0.1/fhir/resources/R4B/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/contract.py` & `fhir.resources-7.0.1/fhir/resources/R4B/contract.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/contributor.py` & `fhir.resources-7.0.1/fhir/resources/R4B/contributor.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/count.py` & `fhir.resources-7.0.1/fhir/resources/R4B/count.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/coverage.py` & `fhir.resources-7.0.1/fhir/resources/R4B/coverage.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/coverageeligibilityrequest.py` & `fhir.resources-7.0.1/fhir/resources/R4B/coverageeligibilityrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/coverageeligibilityresponse.py` & `fhir.resources-7.0.1/fhir/resources/R4B/coverageeligibilityresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/datarequirement.py` & `fhir.resources-7.0.1/fhir/resources/R4B/datarequirement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/detectedissue.py` & `fhir.resources-7.0.1/fhir/resources/R4B/detectedissue.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/device.py` & `fhir.resources-7.0.1/fhir/resources/R4B/device.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/devicedefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/devicedefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/devicemetric.py` & `fhir.resources-7.0.1/fhir/resources/R4B/devicemetric.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/devicerequest.py` & `fhir.resources-7.0.1/fhir/resources/R4B/devicerequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/deviceusestatement.py` & `fhir.resources-7.0.1/fhir/resources/R4B/deviceusestatement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/diagnosticreport.py` & `fhir.resources-7.0.1/fhir/resources/R4B/diagnosticreport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/distance.py` & `fhir.resources-7.0.1/fhir/resources/R4B/distance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/documentmanifest.py` & `fhir.resources-7.0.1/fhir/resources/R4B/documentmanifest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/documentreference.py` & `fhir.resources-7.0.1/fhir/resources/R4B/documentreference.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/domainresource.py` & `fhir.resources-7.0.1/fhir/resources/R4B/domainresource.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/dosage.py` & `fhir.resources-7.0.1/fhir/resources/R4B/dosage.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/duration.py` & `fhir.resources-7.0.1/fhir/resources/R4B/duration.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/element.py` & `fhir.resources-7.0.1/fhir/resources/R4B/element.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/elementdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/elementdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/encounter.py` & `fhir.resources-7.0.1/fhir/resources/R4B/encounter.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/endpoint.py` & `fhir.resources-7.0.1/fhir/resources/R4B/endpoint.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/enrollmentrequest.py` & `fhir.resources-7.0.1/fhir/resources/R4B/enrollmentrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/enrollmentresponse.py` & `fhir.resources-7.0.1/fhir/resources/R4B/enrollmentresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/episodeofcare.py` & `fhir.resources-7.0.1/fhir/resources/R4B/episodeofcare.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/eventdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/eventdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/evidence.py` & `fhir.resources-7.0.1/fhir/resources/R4B/evidence.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/evidencereport.py` & `fhir.resources-7.0.1/fhir/resources/R4B/evidencereport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/evidencevariable.py` & `fhir.resources-7.0.1/fhir/resources/R4B/evidencevariable.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/examplescenario.py` & `fhir.resources-7.0.1/fhir/resources/R4B/examplescenario.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/explanationofbenefit.py` & `fhir.resources-7.0.1/fhir/resources/R4B/explanationofbenefit.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/expression.py` & `fhir.resources-7.0.1/fhir/resources/R4B/expression.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/extension.py` & `fhir.resources-7.0.1/fhir/resources/R4B/extension.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/familymemberhistory.py` & `fhir.resources-7.0.1/fhir/resources/R4B/familymemberhistory.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/fhirprimitiveextension.py` & `fhir.resources-7.0.1/fhir/resources/R4B/fhirprimitiveextension.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/fhirresourcemodel.py` & `fhir.resources-7.0.1/fhir/resources/R4B/fhirresourcemodel.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/fhirtypes.py` & `fhir.resources-7.0.1/fhir/resources/R4B/fhirtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,30 +387,35 @@
             name, email = validate_email(email)
             if realname:
                 email = formataddr((name, email))
             return schema + email
         elif value.startswith("mllp:") or value.startswith("llp:"):
             # xxx: find validation
             return value
+        elif value.startswith("urn:"):
+            # xxx: without validation?
+            return value
         elif value in FHIR_PRIMITIVES:
             # Extensions may contain a valueUrl for a primitive FHIR type
             return value
 
         try:
             return AnyUrl.validate(value, field, config)
         except Exception:
             # we are allowing relative path
             if not value.startswith("/"):
                 matched = cls.path_regex.match("/" + value)
             else:
                 matched = cls.path_regex.match(value)
             if matched is not None:
-                # @ToDo: required resource type validation?
-                # fx: resource type = matched.groupdict().get("resourceType")
-                return value
+                if re.match(
+                    r"^[A-Za-z0-9\-.#]+$", matched.groupdict().get("resourceType", "")
+                ):
+                    # @ToDo: required resource type validation?
+                    return value
             raise
 
     @classmethod
     def to_string(cls, value):
         """ """
         if isinstance(value, bytes):
             value = value.decode()
```

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/fhirtypesvalidators.py` & `fhir.resources-7.0.1/fhir/resources/R4B/fhirtypesvalidators.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/flag.py` & `fhir.resources-7.0.1/fhir/resources/R4B/flag.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/goal.py` & `fhir.resources-7.0.1/fhir/resources/R4B/goal.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/graphdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/graphdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/group.py` & `fhir.resources-7.0.1/fhir/resources/R4B/group.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/guidanceresponse.py` & `fhir.resources-7.0.1/fhir/resources/R4B/guidanceresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/healthcareservice.py` & `fhir.resources-7.0.1/fhir/resources/R4B/healthcareservice.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/humanname.py` & `fhir.resources-7.0.1/fhir/resources/R4B/humanname.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/identifier.py` & `fhir.resources-7.0.1/fhir/resources/R4B/identifier.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/imagingstudy.py` & `fhir.resources-7.0.1/fhir/resources/R4B/imagingstudy.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/immunization.py` & `fhir.resources-7.0.1/fhir/resources/R4B/immunization.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/immunizationevaluation.py` & `fhir.resources-7.0.1/fhir/resources/R4B/immunizationevaluation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/immunizationrecommendation.py` & `fhir.resources-7.0.1/fhir/resources/R4B/immunizationrecommendation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/implementationguide.py` & `fhir.resources-7.0.1/fhir/resources/R4B/implementationguide.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/ingredient.py` & `fhir.resources-7.0.1/fhir/resources/R4B/ingredient.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/insuranceplan.py` & `fhir.resources-7.0.1/fhir/resources/R4B/insuranceplan.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/invoice.py` & `fhir.resources-7.0.1/fhir/resources/R4B/invoice.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/library.py` & `fhir.resources-7.0.1/fhir/resources/R4B/library.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/linkage.py` & `fhir.resources-7.0.1/fhir/resources/R4B/linkage.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/list.py` & `fhir.resources-7.0.1/fhir/resources/R4B/list.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/location.py` & `fhir.resources-7.0.1/fhir/resources/R4B/location.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/manufactureditemdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/manufactureditemdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/marketingstatus.py` & `fhir.resources-7.0.1/fhir/resources/R4B/marketingstatus.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/measure.py` & `fhir.resources-7.0.1/fhir/resources/R4B/measure.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/measurereport.py` & `fhir.resources-7.0.1/fhir/resources/R4B/measurereport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/media.py` & `fhir.resources-7.0.1/fhir/resources/R4B/media.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/medication.py` & `fhir.resources-7.0.1/fhir/resources/R4B/medication.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/medicationadministration.py` & `fhir.resources-7.0.1/fhir/resources/R4B/medicationadministration.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/medicationdispense.py` & `fhir.resources-7.0.1/fhir/resources/R4B/medicationdispense.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/medicationknowledge.py` & `fhir.resources-7.0.1/fhir/resources/R4B/medicationknowledge.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/medicationrequest.py` & `fhir.resources-7.0.1/fhir/resources/R4B/medicationrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/medicationstatement.py` & `fhir.resources-7.0.1/fhir/resources/R4B/medicationstatement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/medicinalproductdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/medicinalproductdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/messagedefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/messagedefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/messageheader.py` & `fhir.resources-7.0.1/fhir/resources/R4B/messageheader.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/meta.py` & `fhir.resources-7.0.1/fhir/resources/R4B/meta.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/molecularsequence.py` & `fhir.resources-7.0.1/fhir/resources/R4B/molecularsequence.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/money.py` & `fhir.resources-7.0.1/fhir/resources/R4B/money.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/namingsystem.py` & `fhir.resources-7.0.1/fhir/resources/R4B/namingsystem.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/narrative.py` & `fhir.resources-7.0.1/fhir/resources/R4B/narrative.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/nutritionorder.py` & `fhir.resources-7.0.1/fhir/resources/R4B/nutritionorder.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/nutritionproduct.py` & `fhir.resources-7.0.1/fhir/resources/R4B/nutritionproduct.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/observation.py` & `fhir.resources-7.0.1/fhir/resources/R4B/observation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/observationdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/observationdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/operationdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/operationdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/operationoutcome.py` & `fhir.resources-7.0.1/fhir/resources/R4B/operationoutcome.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/organization.py` & `fhir.resources-7.0.1/fhir/resources/R4B/organization.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/organizationaffiliation.py` & `fhir.resources-7.0.1/fhir/resources/R4B/organizationaffiliation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/packagedproductdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/packagedproductdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/parameterdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/parameterdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/parameters.py` & `fhir.resources-7.0.1/fhir/resources/R4B/parameters.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/patient.py` & `fhir.resources-7.0.1/fhir/resources/R4B/patient.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/paymentnotice.py` & `fhir.resources-7.0.1/fhir/resources/R4B/paymentnotice.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/paymentreconciliation.py` & `fhir.resources-7.0.1/fhir/resources/R4B/paymentreconciliation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/period.py` & `fhir.resources-7.0.1/fhir/resources/R4B/period.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/person.py` & `fhir.resources-7.0.1/fhir/resources/R4B/person.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/plandefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/plandefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/population.py` & `fhir.resources-7.0.1/fhir/resources/R4B/population.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/practitioner.py` & `fhir.resources-7.0.1/fhir/resources/R4B/practitioner.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/practitionerrole.py` & `fhir.resources-7.0.1/fhir/resources/R4B/practitionerrole.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/procedure.py` & `fhir.resources-7.0.1/fhir/resources/R4B/procedure.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/prodcharacteristic.py` & `fhir.resources-7.0.1/fhir/resources/R4B/prodcharacteristic.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/productshelflife.py` & `fhir.resources-7.0.1/fhir/resources/R4B/productshelflife.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/provenance.py` & `fhir.resources-7.0.1/fhir/resources/R4B/provenance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/quantity.py` & `fhir.resources-7.0.1/fhir/resources/R4B/quantity.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/questionnaire.py` & `fhir.resources-7.0.1/fhir/resources/R4B/questionnaire.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/questionnaireresponse.py` & `fhir.resources-7.0.1/fhir/resources/R4B/questionnaireresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/range.py` & `fhir.resources-7.0.1/fhir/resources/R4B/range.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/ratio.py` & `fhir.resources-7.0.1/fhir/resources/R4B/ratio.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/ratiorange.py` & `fhir.resources-7.0.1/fhir/resources/R4B/ratiorange.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/reference.py` & `fhir.resources-7.0.1/fhir/resources/R4B/reference.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/regulatedauthorization.py` & `fhir.resources-7.0.1/fhir/resources/R4B/regulatedauthorization.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/relatedartifact.py` & `fhir.resources-7.0.1/fhir/resources/R4B/relatedartifact.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/relatedperson.py` & `fhir.resources-7.0.1/fhir/resources/R4B/relatedperson.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/requestgroup.py` & `fhir.resources-7.0.1/fhir/resources/R4B/requestgroup.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/researchdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/researchdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/researchelementdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/researchelementdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/researchstudy.py` & `fhir.resources-7.0.1/fhir/resources/R4B/researchstudy.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/researchsubject.py` & `fhir.resources-7.0.1/fhir/resources/R4B/researchsubject.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/resource.py` & `fhir.resources-7.0.1/fhir/resources/R4B/resource.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/riskassessment.py` & `fhir.resources-7.0.1/fhir/resources/R4B/riskassessment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/sampleddata.py` & `fhir.resources-7.0.1/fhir/resources/R4B/sampleddata.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/schedule.py` & `fhir.resources-7.0.1/fhir/resources/R4B/schedule.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/searchparameter.py` & `fhir.resources-7.0.1/fhir/resources/R4B/searchparameter.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/servicerequest.py` & `fhir.resources-7.0.1/fhir/resources/R4B/servicerequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/signature.py` & `fhir.resources-7.0.1/fhir/resources/R4B/signature.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/slot.py` & `fhir.resources-7.0.1/fhir/resources/R4B/slot.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/specimen.py` & `fhir.resources-7.0.1/fhir/resources/R4B/specimen.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/specimendefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/specimendefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/structuredefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/structuredefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/structuremap.py` & `fhir.resources-7.0.1/fhir/resources/R4B/structuremap.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/subscription.py` & `fhir.resources-7.0.1/fhir/resources/R4B/subscription.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/subscriptionstatus.py` & `fhir.resources-7.0.1/fhir/resources/R4B/subscriptionstatus.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/subscriptiontopic.py` & `fhir.resources-7.0.1/fhir/resources/R4B/subscriptiontopic.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/substance.py` & `fhir.resources-7.0.1/fhir/resources/R4B/substance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/substancedefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/substancedefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/supplydelivery.py` & `fhir.resources-7.0.1/fhir/resources/R4B/supplydelivery.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/supplyrequest.py` & `fhir.resources-7.0.1/fhir/resources/R4B/supplyrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/task.py` & `fhir.resources-7.0.1/fhir/resources/R4B/task.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/terminologycapabilities.py` & `fhir.resources-7.0.1/fhir/resources/R4B/terminologycapabilities.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/testreport.py` & `fhir.resources-7.0.1/fhir/resources/R4B/testreport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/testscript.py` & `fhir.resources-7.0.1/fhir/resources/R4B/testscript.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/timing.py` & `fhir.resources-7.0.1/fhir/resources/R4B/timing.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/triggerdefinition.py` & `fhir.resources-7.0.1/fhir/resources/R4B/triggerdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/usagecontext.py` & `fhir.resources-7.0.1/fhir/resources/R4B/usagecontext.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/valueset.py` & `fhir.resources-7.0.1/fhir/resources/R4B/valueset.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/verificationresult.py` & `fhir.resources-7.0.1/fhir/resources/R4B/verificationresult.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/R4B/visionprescription.py` & `fhir.resources-7.0.1/fhir/resources/R4B/visionprescription.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/__init__.py` & `fhir.resources-7.0.1/fhir/resources/STU3/__init__.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/account.py` & `fhir.resources-7.0.1/fhir/resources/STU3/account.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/activitydefinition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/activitydefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/address.py` & `fhir.resources-7.0.1/fhir/resources/STU3/address.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/adverseevent.py` & `fhir.resources-7.0.1/fhir/resources/STU3/adverseevent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/age.py` & `fhir.resources-7.0.1/fhir/resources/STU3/age.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/allergyintolerance.py` & `fhir.resources-7.0.1/fhir/resources/STU3/allergyintolerance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/annotation.py` & `fhir.resources-7.0.1/fhir/resources/STU3/annotation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/appointment.py` & `fhir.resources-7.0.1/fhir/resources/STU3/appointment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/appointmentresponse.py` & `fhir.resources-7.0.1/fhir/resources/STU3/appointmentresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/attachment.py` & `fhir.resources-7.0.1/fhir/resources/STU3/attachment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/auditevent.py` & `fhir.resources-7.0.1/fhir/resources/STU3/auditevent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/backboneelement.py` & `fhir.resources-7.0.1/fhir/resources/STU3/backboneelement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/basic.py` & `fhir.resources-7.0.1/fhir/resources/STU3/basic.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/binary.py` & `fhir.resources-7.0.1/fhir/resources/STU3/binary.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/bodysite.py` & `fhir.resources-7.0.1/fhir/resources/STU3/bodysite.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/bundle.py` & `fhir.resources-7.0.1/fhir/resources/STU3/bundle.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/capabilitystatement.py` & `fhir.resources-7.0.1/fhir/resources/STU3/capabilitystatement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/careplan.py` & `fhir.resources-7.0.1/fhir/resources/STU3/careplan.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/careteam.py` & `fhir.resources-7.0.1/fhir/resources/STU3/careteam.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/chargeitem.py` & `fhir.resources-7.0.1/fhir/resources/STU3/chargeitem.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/claim.py` & `fhir.resources-7.0.1/fhir/resources/STU3/claim.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/claimresponse.py` & `fhir.resources-7.0.1/fhir/resources/STU3/claimresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/clinicalimpression.py` & `fhir.resources-7.0.1/fhir/resources/STU3/clinicalimpression.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/codeableconcept.py` & `fhir.resources-7.0.1/fhir/resources/STU3/codeableconcept.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/codesystem.py` & `fhir.resources-7.0.1/fhir/resources/STU3/codesystem.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/coding.py` & `fhir.resources-7.0.1/fhir/resources/STU3/coding.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/communication.py` & `fhir.resources-7.0.1/fhir/resources/STU3/communication.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/communicationrequest.py` & `fhir.resources-7.0.1/fhir/resources/STU3/communicationrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/compartmentdefinition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/compartmentdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/composition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/composition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/conceptmap.py` & `fhir.resources-7.0.1/fhir/resources/STU3/conceptmap.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/condition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/condition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/consent.py` & `fhir.resources-7.0.1/fhir/resources/STU3/consent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/contactdetail.py` & `fhir.resources-7.0.1/fhir/resources/STU3/contactdetail.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/contactpoint.py` & `fhir.resources-7.0.1/fhir/resources/STU3/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/contract.py` & `fhir.resources-7.0.1/fhir/resources/STU3/contract.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/contributor.py` & `fhir.resources-7.0.1/fhir/resources/STU3/contributor.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/count.py` & `fhir.resources-7.0.1/fhir/resources/STU3/count.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/coverage.py` & `fhir.resources-7.0.1/fhir/resources/STU3/coverage.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/dataelement.py` & `fhir.resources-7.0.1/fhir/resources/STU3/dataelement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/datarequirement.py` & `fhir.resources-7.0.1/fhir/resources/STU3/datarequirement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/detectedissue.py` & `fhir.resources-7.0.1/fhir/resources/STU3/detectedissue.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/device.py` & `fhir.resources-7.0.1/fhir/resources/STU3/device.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/devicecomponent.py` & `fhir.resources-7.0.1/fhir/resources/STU3/devicecomponent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/devicemetric.py` & `fhir.resources-7.0.1/fhir/resources/STU3/devicemetric.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/devicerequest.py` & `fhir.resources-7.0.1/fhir/resources/STU3/devicerequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/deviceusestatement.py` & `fhir.resources-7.0.1/fhir/resources/STU3/deviceusestatement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/diagnosticreport.py` & `fhir.resources-7.0.1/fhir/resources/STU3/diagnosticreport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/distance.py` & `fhir.resources-7.0.1/fhir/resources/STU3/distance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/documentmanifest.py` & `fhir.resources-7.0.1/fhir/resources/STU3/documentmanifest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/documentreference.py` & `fhir.resources-7.0.1/fhir/resources/STU3/documentreference.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/domainresource.py` & `fhir.resources-7.0.1/fhir/resources/STU3/domainresource.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/dosage.py` & `fhir.resources-7.0.1/fhir/resources/STU3/dosage.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/duration.py` & `fhir.resources-7.0.1/fhir/resources/STU3/duration.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/element.py` & `fhir.resources-7.0.1/fhir/resources/STU3/element.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/elementdefinition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/elementdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/eligibilityrequest.py` & `fhir.resources-7.0.1/fhir/resources/STU3/eligibilityrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/eligibilityresponse.py` & `fhir.resources-7.0.1/fhir/resources/STU3/eligibilityresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/encounter.py` & `fhir.resources-7.0.1/fhir/resources/STU3/encounter.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/endpoint.py` & `fhir.resources-7.0.1/fhir/resources/STU3/endpoint.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/enrollmentrequest.py` & `fhir.resources-7.0.1/fhir/resources/STU3/enrollmentrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/enrollmentresponse.py` & `fhir.resources-7.0.1/fhir/resources/STU3/enrollmentresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/episodeofcare.py` & `fhir.resources-7.0.1/fhir/resources/STU3/episodeofcare.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/expansionprofile.py` & `fhir.resources-7.0.1/fhir/resources/STU3/expansionprofile.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/explanationofbenefit.py` & `fhir.resources-7.0.1/fhir/resources/STU3/explanationofbenefit.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/extension.py` & `fhir.resources-7.0.1/fhir/resources/STU3/extension.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/familymemberhistory.py` & `fhir.resources-7.0.1/fhir/resources/STU3/familymemberhistory.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/fhirprimitiveextension.py` & `fhir.resources-7.0.1/fhir/resources/STU3/fhirprimitiveextension.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/fhirresourcemodel.py` & `fhir.resources-7.0.1/fhir/resources/STU3/fhirresourcemodel.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/fhirtypes.py` & `fhir.resources-7.0.1/fhir/resources/STU3/fhirtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,29 +386,34 @@
             name, email = validate_email(email)
             if realname:
                 email = formataddr((name, email))
             return schema + email
         elif value.startswith("mllp:") or value.startswith("llp:"):
             # xxx: find validation
             return value
+        elif value.startswith("urn:"):
+            # xxx: without validation?
+            return value
         elif value in FHIR_PRIMITIVES:
             # Extensions may contain a valueUrl for a primitive FHIR type
             return value
         try:
             return AnyUrl.validate(value, field, config)
         except Exception:
             # we are allowing relative path
             if not value.startswith("/"):
                 matched = cls.path_regex.match("/" + value)
             else:
                 matched = cls.path_regex.match(value)
             if matched is not None:
-                # @ToDo: required resource type validation?
-                # fx: resource type = matched.groupdict().get("resourceType")
-                return value
+                if re.match(
+                    r"^[A-Za-z0-9\-.#]+$", matched.groupdict().get("resourceType", "")
+                ):
+                    # @ToDo: required resource type validation?
+                    return value
             raise
 
     @classmethod
     def to_string(cls, value):
         """ """
         if isinstance(value, bytes):
             value = value.decode()
```

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/fhirtypesvalidators.py` & `fhir.resources-7.0.1/fhir/resources/STU3/fhirtypesvalidators.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/flag.py` & `fhir.resources-7.0.1/fhir/resources/STU3/flag.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/goal.py` & `fhir.resources-7.0.1/fhir/resources/STU3/goal.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/graphdefinition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/graphdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/group.py` & `fhir.resources-7.0.1/fhir/resources/STU3/group.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/guidanceresponse.py` & `fhir.resources-7.0.1/fhir/resources/STU3/guidanceresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/healthcareservice.py` & `fhir.resources-7.0.1/fhir/resources/STU3/healthcareservice.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/humanname.py` & `fhir.resources-7.0.1/fhir/resources/STU3/humanname.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/identifier.py` & `fhir.resources-7.0.1/fhir/resources/STU3/identifier.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/imagingmanifest.py` & `fhir.resources-7.0.1/fhir/resources/STU3/imagingmanifest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/imagingstudy.py` & `fhir.resources-7.0.1/fhir/resources/STU3/imagingstudy.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/immunization.py` & `fhir.resources-7.0.1/fhir/resources/STU3/immunization.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/immunizationrecommendation.py` & `fhir.resources-7.0.1/fhir/resources/STU3/immunizationrecommendation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/implementationguide.py` & `fhir.resources-7.0.1/fhir/resources/STU3/implementationguide.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/library.py` & `fhir.resources-7.0.1/fhir/resources/STU3/library.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/linkage.py` & `fhir.resources-7.0.1/fhir/resources/STU3/linkage.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/list.py` & `fhir.resources-7.0.1/fhir/resources/STU3/list.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/location.py` & `fhir.resources-7.0.1/fhir/resources/STU3/location.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/measure.py` & `fhir.resources-7.0.1/fhir/resources/STU3/measure.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/measurereport.py` & `fhir.resources-7.0.1/fhir/resources/STU3/measurereport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/media.py` & `fhir.resources-7.0.1/fhir/resources/STU3/media.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/medication.py` & `fhir.resources-7.0.1/fhir/resources/STU3/medication.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/medicationadministration.py` & `fhir.resources-7.0.1/fhir/resources/STU3/medicationadministration.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/medicationdispense.py` & `fhir.resources-7.0.1/fhir/resources/STU3/medicationdispense.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/medicationrequest.py` & `fhir.resources-7.0.1/fhir/resources/STU3/medicationrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/medicationstatement.py` & `fhir.resources-7.0.1/fhir/resources/STU3/medicationstatement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/messagedefinition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/messagedefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/messageheader.py` & `fhir.resources-7.0.1/fhir/resources/STU3/messageheader.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/meta.py` & `fhir.resources-7.0.1/fhir/resources/STU3/meta.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/metadataresource.py` & `fhir.resources-7.0.1/fhir/resources/STU3/metadataresource.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/money.py` & `fhir.resources-7.0.1/fhir/resources/STU3/money.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/namingsystem.py` & `fhir.resources-7.0.1/fhir/resources/STU3/namingsystem.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/narrative.py` & `fhir.resources-7.0.1/fhir/resources/STU3/narrative.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/nutritionorder.py` & `fhir.resources-7.0.1/fhir/resources/STU3/nutritionorder.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/observation.py` & `fhir.resources-7.0.1/fhir/resources/STU3/observation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/operationdefinition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/operationdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/operationoutcome.py` & `fhir.resources-7.0.1/fhir/resources/STU3/operationoutcome.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/organization.py` & `fhir.resources-7.0.1/fhir/resources/STU3/organization.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/parameterdefinition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/parameterdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/parameters.py` & `fhir.resources-7.0.1/fhir/resources/STU3/parameters.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/patient.py` & `fhir.resources-7.0.1/fhir/resources/STU3/patient.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/paymentnotice.py` & `fhir.resources-7.0.1/fhir/resources/STU3/paymentnotice.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/paymentreconciliation.py` & `fhir.resources-7.0.1/fhir/resources/STU3/paymentreconciliation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/period.py` & `fhir.resources-7.0.1/fhir/resources/STU3/period.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/person.py` & `fhir.resources-7.0.1/fhir/resources/STU3/person.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/plandefinition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/plandefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/practitioner.py` & `fhir.resources-7.0.1/fhir/resources/STU3/practitioner.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/practitionerrole.py` & `fhir.resources-7.0.1/fhir/resources/STU3/practitionerrole.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/procedure.py` & `fhir.resources-7.0.1/fhir/resources/STU3/procedure.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/procedurerequest.py` & `fhir.resources-7.0.1/fhir/resources/STU3/procedurerequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/processrequest.py` & `fhir.resources-7.0.1/fhir/resources/STU3/processrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/processresponse.py` & `fhir.resources-7.0.1/fhir/resources/STU3/processresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/provenance.py` & `fhir.resources-7.0.1/fhir/resources/STU3/provenance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/quantity.py` & `fhir.resources-7.0.1/fhir/resources/STU3/quantity.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/questionnaire.py` & `fhir.resources-7.0.1/fhir/resources/STU3/questionnaire.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/questionnaireresponse.py` & `fhir.resources-7.0.1/fhir/resources/STU3/questionnaireresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/range.py` & `fhir.resources-7.0.1/fhir/resources/STU3/range.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/ratio.py` & `fhir.resources-7.0.1/fhir/resources/STU3/ratio.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/reference.py` & `fhir.resources-7.0.1/fhir/resources/STU3/reference.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/referralrequest.py` & `fhir.resources-7.0.1/fhir/resources/STU3/referralrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/relatedartifact.py` & `fhir.resources-7.0.1/fhir/resources/STU3/relatedartifact.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/relatedperson.py` & `fhir.resources-7.0.1/fhir/resources/STU3/relatedperson.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/requestgroup.py` & `fhir.resources-7.0.1/fhir/resources/STU3/requestgroup.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/researchstudy.py` & `fhir.resources-7.0.1/fhir/resources/STU3/researchstudy.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/researchsubject.py` & `fhir.resources-7.0.1/fhir/resources/STU3/researchsubject.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/resource.py` & `fhir.resources-7.0.1/fhir/resources/STU3/resource.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/riskassessment.py` & `fhir.resources-7.0.1/fhir/resources/STU3/riskassessment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/sampleddata.py` & `fhir.resources-7.0.1/fhir/resources/STU3/sampleddata.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/schedule.py` & `fhir.resources-7.0.1/fhir/resources/STU3/schedule.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/searchparameter.py` & `fhir.resources-7.0.1/fhir/resources/STU3/searchparameter.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/sequence.py` & `fhir.resources-7.0.1/fhir/resources/STU3/sequence.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/servicedefinition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/servicedefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/signature.py` & `fhir.resources-7.0.1/fhir/resources/STU3/signature.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/slot.py` & `fhir.resources-7.0.1/fhir/resources/STU3/slot.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/specimen.py` & `fhir.resources-7.0.1/fhir/resources/STU3/specimen.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/structuredefinition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/structuredefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/structuremap.py` & `fhir.resources-7.0.1/fhir/resources/STU3/structuremap.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/subscription.py` & `fhir.resources-7.0.1/fhir/resources/STU3/subscription.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/substance.py` & `fhir.resources-7.0.1/fhir/resources/STU3/substance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/supplydelivery.py` & `fhir.resources-7.0.1/fhir/resources/STU3/supplydelivery.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/supplyrequest.py` & `fhir.resources-7.0.1/fhir/resources/STU3/supplyrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/task.py` & `fhir.resources-7.0.1/fhir/resources/STU3/task.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/testreport.py` & `fhir.resources-7.0.1/fhir/resources/STU3/testreport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/testscript.py` & `fhir.resources-7.0.1/fhir/resources/STU3/testscript.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/timing.py` & `fhir.resources-7.0.1/fhir/resources/STU3/timing.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/triggerdefinition.py` & `fhir.resources-7.0.1/fhir/resources/STU3/triggerdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/usagecontext.py` & `fhir.resources-7.0.1/fhir/resources/STU3/usagecontext.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/valueset.py` & `fhir.resources-7.0.1/fhir/resources/STU3/valueset.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/STU3/visionprescription.py` & `fhir.resources-7.0.1/fhir/resources/STU3/visionprescription.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/__init__.py` & `fhir.resources-7.0.1/fhir/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/account.py` & `fhir.resources-7.0.1/fhir/resources/account.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/activitydefinition.py` & `fhir.resources-7.0.1/fhir/resources/activitydefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/actordefinition.py` & `fhir.resources-7.0.1/fhir/resources/actordefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/address.py` & `fhir.resources-7.0.1/fhir/resources/address.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/administrableproductdefinition.py` & `fhir.resources-7.0.1/fhir/resources/administrableproductdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/adverseevent.py` & `fhir.resources-7.0.1/fhir/resources/adverseevent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/age.py` & `fhir.resources-7.0.1/fhir/resources/age.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/allergyintolerance.py` & `fhir.resources-7.0.1/fhir/resources/allergyintolerance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/annotation.py` & `fhir.resources-7.0.1/fhir/resources/annotation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/appointment.py` & `fhir.resources-7.0.1/fhir/resources/appointment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/appointmentresponse.py` & `fhir.resources-7.0.1/fhir/resources/appointmentresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/artifactassessment.py` & `fhir.resources-7.0.1/fhir/resources/artifactassessment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/attachment.py` & `fhir.resources-7.0.1/fhir/resources/attachment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/auditevent.py` & `fhir.resources-7.0.1/fhir/resources/auditevent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/availability.py` & `fhir.resources-7.0.1/fhir/resources/availability.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/backboneelement.py` & `fhir.resources-7.0.1/fhir/resources/backboneelement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/backbonetype.py` & `fhir.resources-7.0.1/fhir/resources/backbonetype.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/base.py` & `fhir.resources-7.0.1/fhir/resources/base.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/basic.py` & `fhir.resources-7.0.1/fhir/resources/basic.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/binary.py` & `fhir.resources-7.0.1/fhir/resources/binary.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/biologicallyderivedproduct.py` & `fhir.resources-7.0.1/fhir/resources/biologicallyderivedproduct.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/biologicallyderivedproductdispense.py` & `fhir.resources-7.0.1/fhir/resources/biologicallyderivedproductdispense.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/bodystructure.py` & `fhir.resources-7.0.1/fhir/resources/bodystructure.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/bundle.py` & `fhir.resources-7.0.1/fhir/resources/bundle.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/canonicalresource.py` & `fhir.resources-7.0.1/fhir/resources/canonicalresource.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/capabilitystatement.py` & `fhir.resources-7.0.1/fhir/resources/capabilitystatement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/careplan.py` & `fhir.resources-7.0.1/fhir/resources/careplan.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/careteam.py` & `fhir.resources-7.0.1/fhir/resources/careteam.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/chargeitem.py` & `fhir.resources-7.0.1/fhir/resources/chargeitem.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/chargeitemdefinition.py` & `fhir.resources-7.0.1/fhir/resources/chargeitemdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/citation.py` & `fhir.resources-7.0.1/fhir/resources/citation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/claim.py` & `fhir.resources-7.0.1/fhir/resources/claim.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/claimresponse.py` & `fhir.resources-7.0.1/fhir/resources/claimresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/clinicalimpression.py` & `fhir.resources-7.0.1/fhir/resources/clinicalimpression.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/clinicalusedefinition.py` & `fhir.resources-7.0.1/fhir/resources/clinicalusedefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/codeableconcept.py` & `fhir.resources-7.0.1/fhir/resources/codeableconcept.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/codeablereference.py` & `fhir.resources-7.0.1/fhir/resources/codeablereference.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/codesystem.py` & `fhir.resources-7.0.1/fhir/resources/codesystem.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/coding.py` & `fhir.resources-7.0.1/fhir/resources/coding.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/communication.py` & `fhir.resources-7.0.1/fhir/resources/communication.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/communicationrequest.py` & `fhir.resources-7.0.1/fhir/resources/communicationrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/compartmentdefinition.py` & `fhir.resources-7.0.1/fhir/resources/compartmentdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/composition.py` & `fhir.resources-7.0.1/fhir/resources/composition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/conceptmap.py` & `fhir.resources-7.0.1/fhir/resources/conceptmap.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/condition.py` & `fhir.resources-7.0.1/fhir/resources/condition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/conditiondefinition.py` & `fhir.resources-7.0.1/fhir/resources/conditiondefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/consent.py` & `fhir.resources-7.0.1/fhir/resources/consent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/contactdetail.py` & `fhir.resources-7.0.1/fhir/resources/contactdetail.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/contactpoint.py` & `fhir.resources-7.0.1/fhir/resources/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/contract.py` & `fhir.resources-7.0.1/fhir/resources/contract.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/contributor.py` & `fhir.resources-7.0.1/fhir/resources/contributor.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/core/fhirabstractmodel.py` & `fhir.resources-7.0.1/fhir/resources/core/fhirabstractmodel.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/core/patch/patch_r4b_test.py` & `fhir.resources-7.0.1/fhir/resources/core/patch/patch_r4b_test.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/core/utils/__init__.py` & `fhir.resources-7.0.1/fhir/resources/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/core/utils/common.py` & `fhir.resources-7.0.1/fhir/resources/core/utils/common.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/core/utils/xml.py` & `fhir.resources-7.0.1/fhir/resources/core/utils/xml.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/core/utils/yaml.py` & `fhir.resources-7.0.1/fhir/resources/core/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/count.py` & `fhir.resources-7.0.1/fhir/resources/count.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/coverage.py` & `fhir.resources-7.0.1/fhir/resources/coverage.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/coverageeligibilityrequest.py` & `fhir.resources-7.0.1/fhir/resources/coverageeligibilityrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/coverageeligibilityresponse.py` & `fhir.resources-7.0.1/fhir/resources/coverageeligibilityresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/datarequirement.py` & `fhir.resources-7.0.1/fhir/resources/datarequirement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/datatype.py` & `fhir.resources-7.0.1/fhir/resources/datatype.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/detectedissue.py` & `fhir.resources-7.0.1/fhir/resources/detectedissue.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/device.py` & `fhir.resources-7.0.1/fhir/resources/device.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/deviceassociation.py` & `fhir.resources-7.0.1/fhir/resources/deviceassociation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/devicedefinition.py` & `fhir.resources-7.0.1/fhir/resources/devicedefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/devicedispense.py` & `fhir.resources-7.0.1/fhir/resources/devicedispense.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/devicemetric.py` & `fhir.resources-7.0.1/fhir/resources/devicemetric.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/devicerequest.py` & `fhir.resources-7.0.1/fhir/resources/devicerequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/deviceusage.py` & `fhir.resources-7.0.1/fhir/resources/deviceusage.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/diagnosticreport.py` & `fhir.resources-7.0.1/fhir/resources/diagnosticreport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/distance.py` & `fhir.resources-7.0.1/fhir/resources/distance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/documentreference.py` & `fhir.resources-7.0.1/fhir/resources/documentreference.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/domainresource.py` & `fhir.resources-7.0.1/fhir/resources/domainresource.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/dosage.py` & `fhir.resources-7.0.1/fhir/resources/dosage.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/duration.py` & `fhir.resources-7.0.1/fhir/resources/duration.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/element.py` & `fhir.resources-7.0.1/fhir/resources/element.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/elementdefinition.py` & `fhir.resources-7.0.1/fhir/resources/elementdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/encounter.py` & `fhir.resources-7.0.1/fhir/resources/encounter.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/encounterhistory.py` & `fhir.resources-7.0.1/fhir/resources/encounterhistory.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/endpoint.py` & `fhir.resources-7.0.1/fhir/resources/endpoint.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/enrollmentrequest.py` & `fhir.resources-7.0.1/fhir/resources/enrollmentrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/enrollmentresponse.py` & `fhir.resources-7.0.1/fhir/resources/enrollmentresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/episodeofcare.py` & `fhir.resources-7.0.1/fhir/resources/episodeofcare.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/eventdefinition.py` & `fhir.resources-7.0.1/fhir/resources/eventdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/evidence.py` & `fhir.resources-7.0.1/fhir/resources/evidence.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/evidencereport.py` & `fhir.resources-7.0.1/fhir/resources/evidencereport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/evidencevariable.py` & `fhir.resources-7.0.1/fhir/resources/evidencevariable.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/examplescenario.py` & `fhir.resources-7.0.1/fhir/resources/examplescenario.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/explanationofbenefit.py` & `fhir.resources-7.0.1/fhir/resources/explanationofbenefit.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/expression.py` & `fhir.resources-7.0.1/fhir/resources/expression.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/extendedcontactdetail.py` & `fhir.resources-7.0.1/fhir/resources/extendedcontactdetail.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/extension.py` & `fhir.resources-7.0.1/fhir/resources/extension.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/familymemberhistory.py` & `fhir.resources-7.0.1/fhir/resources/familymemberhistory.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/fhirprimitiveextension.py` & `fhir.resources-7.0.1/fhir/resources/fhirprimitiveextension.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/fhirresourcemodel.py` & `fhir.resources-7.0.1/fhir/resources/fhirresourcemodel.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/fhirtypes.py` & `fhir.resources-7.0.1/fhir/resources/fhirtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,30 +395,35 @@
             name, email = validate_email(email)
             if realname:
                 email = formataddr((name, email))
             return schema + email
         elif value.startswith("mllp:") or value.startswith("llp:"):
             # xxx: find validation
             return value
+        elif value.startswith("urn:"):
+            # xxx: without validation?
+            return value
         elif value in FHIR_PRIMITIVES:
             # Extensions may contain a valueUrl for a primitive FHIR type
             return value
 
         try:
             return AnyUrl.validate(value, field, config)
         except Exception:
             # we are allowing relative path
             if not value.startswith("/"):
                 matched = cls.path_regex.match("/" + value)
             else:
                 matched = cls.path_regex.match(value)
             if matched is not None:
-                # @ToDo: required resource type validation?
-                # fx: resource type = matched.groupdict().get("resourceType")
-                return value
+                if re.match(
+                    r"^[A-Za-z0-9\-.#]+$", matched.groupdict().get("resourceType", "")
+                ):
+                    # @ToDo: required resource type validation?
+                    return value
             raise
 
     @classmethod
     def to_string(cls, value):
         """ """
         if isinstance(value, bytes):
             value = value.decode()
```

### Comparing `fhir.resources-7.0.0/fhir/resources/fhirtypesvalidators.py` & `fhir.resources-7.0.1/fhir/resources/fhirtypesvalidators.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/flag.py` & `fhir.resources-7.0.1/fhir/resources/flag.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/formularyitem.py` & `fhir.resources-7.0.1/fhir/resources/formularyitem.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/genomicstudy.py` & `fhir.resources-7.0.1/fhir/resources/genomicstudy.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/goal.py` & `fhir.resources-7.0.1/fhir/resources/goal.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/graphdefinition.py` & `fhir.resources-7.0.1/fhir/resources/graphdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/group.py` & `fhir.resources-7.0.1/fhir/resources/group.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/guidanceresponse.py` & `fhir.resources-7.0.1/fhir/resources/guidanceresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/healthcareservice.py` & `fhir.resources-7.0.1/fhir/resources/healthcareservice.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/humanname.py` & `fhir.resources-7.0.1/fhir/resources/humanname.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/identifier.py` & `fhir.resources-7.0.1/fhir/resources/identifier.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/imagingselection.py` & `fhir.resources-7.0.1/fhir/resources/imagingselection.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/imagingstudy.py` & `fhir.resources-7.0.1/fhir/resources/imagingstudy.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/immunization.py` & `fhir.resources-7.0.1/fhir/resources/immunization.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/immunizationevaluation.py` & `fhir.resources-7.0.1/fhir/resources/immunizationevaluation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/immunizationrecommendation.py` & `fhir.resources-7.0.1/fhir/resources/immunizationrecommendation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/implementationguide.py` & `fhir.resources-7.0.1/fhir/resources/implementationguide.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/ingredient.py` & `fhir.resources-7.0.1/fhir/resources/ingredient.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/insuranceplan.py` & `fhir.resources-7.0.1/fhir/resources/insuranceplan.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/integer64.py` & `fhir.resources-7.0.1/fhir/resources/integer64.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/inventoryitem.py` & `fhir.resources-7.0.1/fhir/resources/inventoryitem.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/inventoryreport.py` & `fhir.resources-7.0.1/fhir/resources/inventoryreport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/invoice.py` & `fhir.resources-7.0.1/fhir/resources/invoice.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/library.py` & `fhir.resources-7.0.1/fhir/resources/library.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/linkage.py` & `fhir.resources-7.0.1/fhir/resources/linkage.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/list.py` & `fhir.resources-7.0.1/fhir/resources/list.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/location.py` & `fhir.resources-7.0.1/fhir/resources/location.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/manufactureditemdefinition.py` & `fhir.resources-7.0.1/fhir/resources/manufactureditemdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/marketingstatus.py` & `fhir.resources-7.0.1/fhir/resources/marketingstatus.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/measure.py` & `fhir.resources-7.0.1/fhir/resources/measure.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/measurereport.py` & `fhir.resources-7.0.1/fhir/resources/measurereport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/medication.py` & `fhir.resources-7.0.1/fhir/resources/medication.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/medicationadministration.py` & `fhir.resources-7.0.1/fhir/resources/medicationadministration.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/medicationdispense.py` & `fhir.resources-7.0.1/fhir/resources/medicationdispense.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/medicationknowledge.py` & `fhir.resources-7.0.1/fhir/resources/medicationknowledge.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/medicationrequest.py` & `fhir.resources-7.0.1/fhir/resources/medicationrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/medicationstatement.py` & `fhir.resources-7.0.1/fhir/resources/medicationstatement.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/medicinalproductdefinition.py` & `fhir.resources-7.0.1/fhir/resources/medicinalproductdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/messagedefinition.py` & `fhir.resources-7.0.1/fhir/resources/messagedefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/messageheader.py` & `fhir.resources-7.0.1/fhir/resources/messageheader.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/meta.py` & `fhir.resources-7.0.1/fhir/resources/meta.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/metadataresource.py` & `fhir.resources-7.0.1/fhir/resources/metadataresource.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/molecularsequence.py` & `fhir.resources-7.0.1/fhir/resources/molecularsequence.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/monetarycomponent.py` & `fhir.resources-7.0.1/fhir/resources/monetarycomponent.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/money.py` & `fhir.resources-7.0.1/fhir/resources/money.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/namingsystem.py` & `fhir.resources-7.0.1/fhir/resources/namingsystem.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/narrative.py` & `fhir.resources-7.0.1/fhir/resources/narrative.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/nutritionintake.py` & `fhir.resources-7.0.1/fhir/resources/nutritionintake.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/nutritionorder.py` & `fhir.resources-7.0.1/fhir/resources/nutritionorder.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/nutritionproduct.py` & `fhir.resources-7.0.1/fhir/resources/nutritionproduct.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/observation.py` & `fhir.resources-7.0.1/fhir/resources/observation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/observationdefinition.py` & `fhir.resources-7.0.1/fhir/resources/observationdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/operationdefinition.py` & `fhir.resources-7.0.1/fhir/resources/operationdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/operationoutcome.py` & `fhir.resources-7.0.1/fhir/resources/operationoutcome.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/organization.py` & `fhir.resources-7.0.1/fhir/resources/organization.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/organizationaffiliation.py` & `fhir.resources-7.0.1/fhir/resources/organizationaffiliation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/packagedproductdefinition.py` & `fhir.resources-7.0.1/fhir/resources/packagedproductdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/parameterdefinition.py` & `fhir.resources-7.0.1/fhir/resources/parameterdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/parameters.py` & `fhir.resources-7.0.1/fhir/resources/parameters.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/patient.py` & `fhir.resources-7.0.1/fhir/resources/patient.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/paymentnotice.py` & `fhir.resources-7.0.1/fhir/resources/paymentnotice.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/paymentreconciliation.py` & `fhir.resources-7.0.1/fhir/resources/paymentreconciliation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/period.py` & `fhir.resources-7.0.1/fhir/resources/period.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/permission.py` & `fhir.resources-7.0.1/fhir/resources/permission.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/person.py` & `fhir.resources-7.0.1/fhir/resources/person.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/plandefinition.py` & `fhir.resources-7.0.1/fhir/resources/plandefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/practitioner.py` & `fhir.resources-7.0.1/fhir/resources/practitioner.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/practitionerrole.py` & `fhir.resources-7.0.1/fhir/resources/practitionerrole.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/primitivetype.py` & `fhir.resources-7.0.1/fhir/resources/primitivetype.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/procedure.py` & `fhir.resources-7.0.1/fhir/resources/procedure.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/productshelflife.py` & `fhir.resources-7.0.1/fhir/resources/productshelflife.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/provenance.py` & `fhir.resources-7.0.1/fhir/resources/provenance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/quantity.py` & `fhir.resources-7.0.1/fhir/resources/quantity.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/questionnaire.py` & `fhir.resources-7.0.1/fhir/resources/questionnaire.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/questionnaireresponse.py` & `fhir.resources-7.0.1/fhir/resources/questionnaireresponse.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/range.py` & `fhir.resources-7.0.1/fhir/resources/range.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/ratio.py` & `fhir.resources-7.0.1/fhir/resources/ratio.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/ratiorange.py` & `fhir.resources-7.0.1/fhir/resources/ratiorange.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/reference.py` & `fhir.resources-7.0.1/fhir/resources/reference.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/regulatedauthorization.py` & `fhir.resources-7.0.1/fhir/resources/regulatedauthorization.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/relatedartifact.py` & `fhir.resources-7.0.1/fhir/resources/relatedartifact.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/relatedperson.py` & `fhir.resources-7.0.1/fhir/resources/relatedperson.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/requestorchestration.py` & `fhir.resources-7.0.1/fhir/resources/requestorchestration.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/requirements.py` & `fhir.resources-7.0.1/fhir/resources/requirements.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/researchstudy.py` & `fhir.resources-7.0.1/fhir/resources/researchstudy.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/researchsubject.py` & `fhir.resources-7.0.1/fhir/resources/researchsubject.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/resource.py` & `fhir.resources-7.0.1/fhir/resources/resource.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/riskassessment.py` & `fhir.resources-7.0.1/fhir/resources/riskassessment.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/sampleddata.py` & `fhir.resources-7.0.1/fhir/resources/sampleddata.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/schedule.py` & `fhir.resources-7.0.1/fhir/resources/schedule.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/searchparameter.py` & `fhir.resources-7.0.1/fhir/resources/searchparameter.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/servicerequest.py` & `fhir.resources-7.0.1/fhir/resources/servicerequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/signature.py` & `fhir.resources-7.0.1/fhir/resources/signature.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/slot.py` & `fhir.resources-7.0.1/fhir/resources/slot.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/specimen.py` & `fhir.resources-7.0.1/fhir/resources/specimen.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/specimendefinition.py` & `fhir.resources-7.0.1/fhir/resources/specimendefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/structuredefinition.py` & `fhir.resources-7.0.1/fhir/resources/structuredefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/structuremap.py` & `fhir.resources-7.0.1/fhir/resources/structuremap.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/subscription.py` & `fhir.resources-7.0.1/fhir/resources/subscription.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/subscriptionstatus.py` & `fhir.resources-7.0.1/fhir/resources/subscriptionstatus.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/subscriptiontopic.py` & `fhir.resources-7.0.1/fhir/resources/subscriptiontopic.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/substance.py` & `fhir.resources-7.0.1/fhir/resources/substance.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/substancedefinition.py` & `fhir.resources-7.0.1/fhir/resources/substancedefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/substancenucleicacid.py` & `fhir.resources-7.0.1/fhir/resources/substancenucleicacid.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/substancepolymer.py` & `fhir.resources-7.0.1/fhir/resources/substancepolymer.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/substanceprotein.py` & `fhir.resources-7.0.1/fhir/resources/substanceprotein.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/substancereferenceinformation.py` & `fhir.resources-7.0.1/fhir/resources/substancereferenceinformation.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/substancesourcematerial.py` & `fhir.resources-7.0.1/fhir/resources/substancesourcematerial.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/supplydelivery.py` & `fhir.resources-7.0.1/fhir/resources/supplydelivery.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/supplyrequest.py` & `fhir.resources-7.0.1/fhir/resources/supplyrequest.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/task.py` & `fhir.resources-7.0.1/fhir/resources/task.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/terminologycapabilities.py` & `fhir.resources-7.0.1/fhir/resources/terminologycapabilities.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/testplan.py` & `fhir.resources-7.0.1/fhir/resources/testplan.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/testreport.py` & `fhir.resources-7.0.1/fhir/resources/testreport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/testscript.py` & `fhir.resources-7.0.1/fhir/resources/testscript.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/timing.py` & `fhir.resources-7.0.1/fhir/resources/timing.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/transport.py` & `fhir.resources-7.0.1/fhir/resources/transport.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/triggerdefinition.py` & `fhir.resources-7.0.1/fhir/resources/triggerdefinition.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/usagecontext.py` & `fhir.resources-7.0.1/fhir/resources/usagecontext.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/valueset.py` & `fhir.resources-7.0.1/fhir/resources/valueset.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/verificationresult.py` & `fhir.resources-7.0.1/fhir/resources/verificationresult.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/virtualservicedetail.py` & `fhir.resources-7.0.1/fhir/resources/virtualservicedetail.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir/resources/visionprescription.py` & `fhir.resources-7.0.1/fhir/resources/visionprescription.py`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/fhir.resources.egg-info/PKG-INFO` & `fhir.resources-7.0.1/fhir.resources.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhir.resources
-Version: 7.0.0
+Version: 7.0.1
 Summary: FHIR Resources as Model Class
 Home-page: https://github.com/nazrulworld/fhir.resources
 Author: Md Nazrul Islam
 Author-email: email2nazrul@gmail.com
 License: BSD license
 Project-URL: CI: Travis, https://travis-ci.org/github/nazrulworld/fhir.resources
 Project-URL: Coverage: codecov, https://codecov.io/gh/nazrulworld/fhir.resources
@@ -841,14 +841,23 @@
     :format: html
 
 
 =======
 History
 =======
 
+7.0.1 (2023-05-29)
+------------------
+
+Fixes
+
+- Issue #128 `pkg_resources.declare_namespace deprecation <https://github.com/nazrulworld/fhir.resources/issues/128>`_
+
+- Issue #129 `urn not supported in Url <https://github.com/nazrulworld/fhir.resources/issues/129>`_
+
 7.0.0 (2023-04-08)
 ------------------
 
 New Feature
 
 - Support for `FHIR version R5 <https://www.hl7.org/fhir/R5/resourcelist.html>`_ has been added under root package.
```

### Comparing `fhir.resources-7.0.0/fhir.resources.egg-info/SOURCES.txt` & `fhir.resources-7.0.1/fhir.resources.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 README.rst
 setup.cfg
 setup.py
 fhir/__init__.py
 fhir.resources.egg-info/PKG-INFO
 fhir.resources.egg-info/SOURCES.txt
 fhir.resources.egg-info/dependency_links.txt
-fhir.resources.egg-info/namespace_packages.txt
 fhir.resources.egg-info/not-zip-safe
 fhir.resources.egg-info/requires.txt
 fhir.resources.egg-info/top_level.txt
 fhir/resources/__init__.py
 fhir/resources/account.py
 fhir/resources/activitydefinition.py
 fhir/resources/actordefinition.py
```

### Comparing `fhir.resources-7.0.0/fhir.resources.egg-info/requires.txt` & `fhir.resources-7.0.1/fhir.resources.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fhir.resources-7.0.0/setup.py` & `fhir.resources-7.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
     description="FHIR Resources as Model Class",
     install_requires=requirements,
     license="BSD license",
     long_description=readme + "\n\n" + history,
     include_package_data=True,
     keywords="fhir, resources, python, hl7, health IT, healthcare",
     name="fhir.resources",
-    namespace_packages=["fhir"],
     packages=find_namespace_packages(
         include=["fhir*"],
         exclude=[
             "ez_setup",
             "tests",
             "fhir-parser*",
             "fhir.resources.tests",
@@ -115,15 +114,15 @@
             + yaml_requirements
             + xml_requirements
         ),
         "dev": (test_requirements + development_requirements),
         "all": (orjson_requirements + yaml_requirements + xml_requirements),
     },
     url="https://github.com/nazrulworld/fhir.resources",
-    version="7.0.0",
+    version="7.0.1",
     zip_safe=False,
     python_requires=">=3.6",
     project_urls={
         "CI: Travis": "https://travis-ci.org/github/nazrulworld/fhir.resources",
         "Coverage: codecov": "https://codecov.io/gh/nazrulworld/fhir.resources",
         "GitHub: issues": "https://github.com/nazrulworld/fhir.resources/issues",
         "GitHub: repo": "https://github.com/nazrulworld/fhir.resources",
```


# Comparing `tmp/fdk_rdf_parser-2.2.8.tar.gz` & `tmp/fdk_rdf_parser-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdk_rdf_parser-2.2.8.tar", max compression
+gzip compressed data, was "fdk_rdf_parser-2.2.9.tar", max compression
```

## Comparing `fdk_rdf_parser-2.2.8.tar` & `fdk_rdf_parser-2.2.9.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0     1207 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/pyproject.toml
--rw-r--r--   0        0        0      172 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/__init__.py
--rw-r--r--   0        0        0     1646 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/__init__.py
--rw-r--r--   0        0        0      270 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/address.py
--rw-r--r--   0        0        0      342 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/agent.py
--rw-r--r--   0        0        0      794 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/business_event.py
--rw-r--r--   0        0        0      336 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/catalog.py
--rw-r--r--   0        0        0      611 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/channel.py
--rw-r--r--   0        0        0     2439 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/concept.py
--rw-r--r--   0        0        0      189 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/conforms_to.py
--rw-r--r--   0        0        0     1010 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/contactpoint.py
--rw-r--r--   0        0        0      436 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/cost.py
--rw-r--r--   0        0        0     2382 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/cpsvno_service.py
--rw-r--r--   0        0        0      356 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/data_distribution_service.py
--rw-r--r--   0        0        0     1644 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/dataservice.py
--rw-r--r--   0        0        0     8180 2023-02-13 12:05:09.833348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/dataset.py
--rw-r--r--   0        0        0      971 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/dcat_resource.py
--rw-r--r--   0        0        0      274 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/dct_standard.py
--rw-r--r--   0        0        0     1099 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/distribution.py
--rw-r--r--   0        0        0      803 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/event.py
--rw-r--r--   0        0        0      758 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/evidence.py
--rw-r--r--   0        0        0      349 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/format.py
--rw-r--r--   0        0        0      198 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/harvest_meta_data.py
--rw-r--r--   0        0        0     3419 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/info_model.py
--rw-r--r--   0        0        0      331 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/legal_resource.py
--rw-r--r--   0        0        0      786 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/life_event.py
--rw-r--r--   0        0        0      511 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/media_type.py
--rw-r--r--   0        0        0     1910 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/model_element.py
--rw-r--r--   0        0        0     1147 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/model_property.py
--rw-r--r--   0        0        0      405 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/opening_hours_specification.py
--rw-r--r--   0        0        0      430 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/organization.py
--rw-r--r--   0        0        0      466 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/output.py
--rw-r--r--   0        0        0      376 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/participation.py
--rw-r--r--   0        0        0     1934 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/public_service.py
--rw-r--r--   0        0        0      326 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/publisher.py
--rw-r--r--   0        0        0      206 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/qualified_attribution.py
--rw-r--r--   0        0        0      202 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/quality_annotation.py
--rw-r--r--   0        0        0      227 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/reference_data_code.py
--rw-r--r--   0        0        0      277 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/references.py
--rw-r--r--   0        0        0      412 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/requirement.py
--rw-r--r--   0        0        0      424 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/rule.py
--rw-r--r--   0        0        0      317 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/skos_concept.py
--rw-r--r--   0        0        0      271 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/subject.py
--rw-r--r--   0        0        0      191 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/temporal.py
--rw-r--r--   0        0        0     2500 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/theme.py
--rw-r--r--   0        0        0     8312 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/fdk_rdf_parser.py
--rw-r--r--   0        0        0     1400 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/__init__.py
--rw-r--r--   0        0        0     1070 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/address.py
--rw-r--r--   0        0        0     2175 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/agent.py
--rw-r--r--   0        0        0     1154 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/catalog.py
--rw-r--r--   0        0        0     1741 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/channel.py
--rw-r--r--   0        0        0    10210 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/concept.py
--rw-r--r--   0        0        0      992 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/conforms_to.py
--rw-r--r--   0        0        0     3811 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/contactpoint.py
--rw-r--r--   0        0        0     1336 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/cost.py
--rw-r--r--   0        0        0     5507 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/cpsvno_service.py
--rw-r--r--   0        0        0     1555 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/data_distribution_service.py
--rw-r--r--   0        0        0     1873 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/dataservice.py
--rw-r--r--   0        0        0     7122 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/dataset.py
--rw-r--r--   0        0        0     2841 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/dcat_resource.py
--rw-r--r--   0        0        0      979 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/dct_standard.py
--rw-r--r--   0        0        0     2134 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/distribution.py
--rw-r--r--   0        0        0     3540 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/event.py
--rw-r--r--   0        0        0     1981 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/evidence.py
--rw-r--r--   0        0        0     1064 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/format.py
--rw-r--r--   0        0        0      444 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/harvest_meta_data.py
--rw-r--r--   0        0        0     5785 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/info_model.py
--rw-r--r--   0        0        0     1047 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/legal_resource.py
--rw-r--r--   0        0        0     1853 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/media_type.py
--rw-r--r--   0        0        0     4434 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/model_element.py
--rw-r--r--   0        0        0     3439 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/model_property.py
--rw-r--r--   0        0        0     1280 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/opening_hours_specification.py
--rw-r--r--   0        0        0     2611 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/organization.py
--rw-r--r--   0        0        0     1249 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/output.py
--rw-r--r--   0        0        0      840 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/participation.py
--rw-r--r--   0        0        0     2155 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/publisher.py
--rw-r--r--   0        0        0      911 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/qualified_attribution.py
--rw-r--r--   0        0        0     1451 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/quality_annotation.py
--rw-r--r--   0        0        0      885 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/reference_data_code.py
--rw-r--r--   0        0        0     1538 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/references.py
--rw-r--r--   0        0        0     1170 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/requirement.py
--rw-r--r--   0        0        0     1247 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/rule.py
--rw-r--r--   0        0        0     1605 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/skos_concept.py
--rw-r--r--   0        0        0      965 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/subject.py
--rw-r--r--   0        0        0     2540 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/temporal.py
--rw-r--r--   0        0        0      736 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/rdf_utils/__init__.py
--rw-r--r--   0        0        0     3126 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/rdf_utils/ns.py
--rw-r--r--   0        0        0     4797 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/rdf_utils/utils.py
--rw-r--r--   0        0        0      579 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/__init__.py
--rw-r--r--   0        0        0     5973 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/extend_cpsvno_service.py
--rw-r--r--   0        0        0     2232 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/extend_dataservice.py
--rw-r--r--   0        0        0     5318 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/extend_dataset.py
--rw-r--r--   0        0        0     1030 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/extend_info_model.py
--rw-r--r--   0        0        0    11923 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/reference_data.py
--rw-r--r--   0        0        0      626 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/reference_data_client.py
--rw-r--r--   0        0        0     4904 2023-02-13 12:05:09.837348 fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/utils.py
--rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 fdk_rdf_parser-2.2.8/setup.py
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 fdk_rdf_parser-2.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1207 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/__init__.py
+-rw-r--r--   0        0        0     1646 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/__init__.py
+-rw-r--r--   0        0        0      270 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/address.py
+-rw-r--r--   0        0        0      342 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/agent.py
+-rw-r--r--   0        0        0      794 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/business_event.py
+-rw-r--r--   0        0        0      336 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/catalog.py
+-rw-r--r--   0        0        0      611 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/channel.py
+-rw-r--r--   0        0        0     2439 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/concept.py
+-rw-r--r--   0        0        0      189 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/conforms_to.py
+-rw-r--r--   0        0        0     1010 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/contactpoint.py
+-rw-r--r--   0        0        0      436 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/cost.py
+-rw-r--r--   0        0        0     2382 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/cpsvno_service.py
+-rw-r--r--   0        0        0      356 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/data_distribution_service.py
+-rw-r--r--   0        0        0     1644 2023-03-09 10:28:14.933721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/dataservice.py
+-rw-r--r--   0        0        0     8195 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/dataset.py
+-rw-r--r--   0        0        0      971 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/dcat_resource.py
+-rw-r--r--   0        0        0      274 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/dct_standard.py
+-rw-r--r--   0        0        0     1099 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/distribution.py
+-rw-r--r--   0        0        0      803 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/event.py
+-rw-r--r--   0        0        0      758 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/evidence.py
+-rw-r--r--   0        0        0      349 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/format.py
+-rw-r--r--   0        0        0      198 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/harvest_meta_data.py
+-rw-r--r--   0        0        0     3419 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/info_model.py
+-rw-r--r--   0        0        0      331 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/legal_resource.py
+-rw-r--r--   0        0        0      786 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/life_event.py
+-rw-r--r--   0        0        0      511 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/media_type.py
+-rw-r--r--   0        0        0     1910 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/model_element.py
+-rw-r--r--   0        0        0     1147 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/model_property.py
+-rw-r--r--   0        0        0      405 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/opening_hours_specification.py
+-rw-r--r--   0        0        0      430 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/organization.py
+-rw-r--r--   0        0        0      466 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/output.py
+-rw-r--r--   0        0        0      376 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/participation.py
+-rw-r--r--   0        0        0     1934 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/public_service.py
+-rw-r--r--   0        0        0      326 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/publisher.py
+-rw-r--r--   0        0        0      206 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/qualified_attribution.py
+-rw-r--r--   0        0        0      202 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/quality_annotation.py
+-rw-r--r--   0        0        0      227 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/reference_data_code.py
+-rw-r--r--   0        0        0      277 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/references.py
+-rw-r--r--   0        0        0      412 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/requirement.py
+-rw-r--r--   0        0        0      424 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/rule.py
+-rw-r--r--   0        0        0      317 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/skos_concept.py
+-rw-r--r--   0        0        0      271 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/subject.py
+-rw-r--r--   0        0        0      191 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/temporal.py
+-rw-r--r--   0        0        0     2500 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/theme.py
+-rw-r--r--   0        0        0     8298 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/fdk_rdf_parser.py
+-rw-r--r--   0        0        0     1393 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/__init__.py
+-rw-r--r--   0        0        0     1070 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/address.py
+-rw-r--r--   0        0        0     2175 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/agent.py
+-rw-r--r--   0        0        0     1154 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/catalog.py
+-rw-r--r--   0        0        0     1741 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/channel.py
+-rw-r--r--   0        0        0    10210 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/concept.py
+-rw-r--r--   0        0        0      992 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/conforms_to.py
+-rw-r--r--   0        0        0     3811 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/contactpoint.py
+-rw-r--r--   0        0        0     1336 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/cost.py
+-rw-r--r--   0        0        0     5507 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/cpsvno_service.py
+-rw-r--r--   0        0        0     1555 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/data_distribution_service.py
+-rw-r--r--   0        0        0     1873 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/dataservice.py
+-rw-r--r--   0        0        0     8502 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/dataset.py
+-rw-r--r--   0        0        0     2841 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/dcat_resource.py
+-rw-r--r--   0        0        0      979 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/dct_standard.py
+-rw-r--r--   0        0        0     2134 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/distribution.py
+-rw-r--r--   0        0        0     3540 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/event.py
+-rw-r--r--   0        0        0     1981 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/evidence.py
+-rw-r--r--   0        0        0     1064 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/format.py
+-rw-r--r--   0        0        0      444 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/harvest_meta_data.py
+-rw-r--r--   0        0        0     5785 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/info_model.py
+-rw-r--r--   0        0        0     1047 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/legal_resource.py
+-rw-r--r--   0        0        0     1853 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/media_type.py
+-rw-r--r--   0        0        0     4434 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/model_element.py
+-rw-r--r--   0        0        0     3439 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/model_property.py
+-rw-r--r--   0        0        0     1280 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/opening_hours_specification.py
+-rw-r--r--   0        0        0     2611 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/organization.py
+-rw-r--r--   0        0        0     1249 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/output.py
+-rw-r--r--   0        0        0      840 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/participation.py
+-rw-r--r--   0        0        0     2155 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/publisher.py
+-rw-r--r--   0        0        0      911 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/qualified_attribution.py
+-rw-r--r--   0        0        0     1451 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/quality_annotation.py
+-rw-r--r--   0        0        0      885 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/reference_data_code.py
+-rw-r--r--   0        0        0     1538 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/references.py
+-rw-r--r--   0        0        0     1170 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/requirement.py
+-rw-r--r--   0        0        0     1247 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/rule.py
+-rw-r--r--   0        0        0     1605 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/skos_concept.py
+-rw-r--r--   0        0        0      965 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/subject.py
+-rw-r--r--   0        0        0     2540 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/temporal.py
+-rw-r--r--   0        0        0      736 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/rdf_utils/__init__.py
+-rw-r--r--   0        0        0     3126 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/rdf_utils/ns.py
+-rw-r--r--   0        0        0     4797 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/rdf_utils/utils.py
+-rw-r--r--   0        0        0      579 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/__init__.py
+-rw-r--r--   0        0        0     5973 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/extend_cpsvno_service.py
+-rw-r--r--   0        0        0     2232 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/extend_dataservice.py
+-rw-r--r--   0        0        0     5318 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/extend_dataset.py
+-rw-r--r--   0        0        0     1030 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/extend_info_model.py
+-rw-r--r--   0        0        0    11923 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/reference_data.py
+-rw-r--r--   0        0        0      626 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/reference_data_client.py
+-rw-r--r--   0        0        0     4904 2023-03-09 10:28:14.937721 fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/utils.py
+-rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 fdk_rdf_parser-2.2.9/setup.py
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 fdk_rdf_parser-2.2.9/PKG-INFO
```

### Comparing `fdk_rdf_parser-2.2.8/pyproject.toml` & `fdk_rdf_parser-2.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fdk-rdf-parser"
-version = "2.2.8"
+version = "2.2.9"
 description = ""
 authors = ["NilsOveTen <nils.ove.tendenes@digdir.no>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 rdflib = "^6.2.0"
 isodate = "^0.6.1"
```

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/__init__.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/business_event.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/business_event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/channel.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/channel.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/concept.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/concept.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/contactpoint.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/cpsvno_service.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/cpsvno_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/dataservice.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/dataservice.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/dataset.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,17 +130,17 @@
         self.isRelatedToTransportportal = values.isRelatedToTransportportal
         self.inSeries = values.inSeries
         self.prev = values.prev
 
 
 @dataclass
 class DatasetSeries(Dataset):
-    first: Optional[str] = None
     last: Optional[str] = None
-    specialized_type: str = "dataset_series"
+    datasetsInSeries: Optional[List[str]] = None
+    specializedType: str = "datasetSeries"
 
     def add_values_from_dataset(self: Any, values: Dataset) -> None:
         self.id = values.id
         self.identifier = values.identifier
         self.title = values.title
         self.publisher = values.publisher
         self.description = values.description
```

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/dcat_resource.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/dcat_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/distribution.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/distribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/event.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/evidence.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/evidence.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/info_model.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/info_model.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/life_event.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/life_event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/model_element.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/model_element.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/model_property.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/model_property.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/public_service.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/public_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/classes/theme.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/classes/theme.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/fdk_rdf_parser.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/fdk_rdf_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 )
 from .parse_functions import (
     extend_with_associated_broader_types,
     parse_concept,
     parse_cpsvno_service,
     parse_data_service,
     parse_dataset,
-    parse_dataset_series_values,
+    parse_dataset_series,
     parse_event,
     parse_information_model,
 )
 from .rdf_utils import (
     cpsv_uri,
     cpsvno_uri,
     cv_uri,
@@ -98,15 +98,15 @@
             )
 
             dataset = Dataset()
             dataset.add_values_from_partial(values=partial_dataset)
             dataset = extend_dataset_with_reference_data(dataset, reference_data)
 
             if is_type(dcat_uri("DatasetSeries"), datasets_graph, primary_topic_uri):
-                series = parse_dataset_series_values(datasets_graph, primary_topic_uri)
+                series = parse_dataset_series(datasets_graph, primary_topic_uri)
                 series.add_values_from_dataset(values=dataset)
                 datasets[primary_topic_uri.toPython()] = series
             else:
                 datasets[primary_topic_uri.toPython()] = dataset
 
     return datasets
```

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/__init__.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .conforms_to import extract_conforms_to
 from .contactpoint import extract_contact_points
 from .cost import extract_costs
 from .cpsvno_service import parse_cpsvno_service
 from .dataservice import parse_data_service
 from .dataset import (
     parse_dataset,
-    parse_dataset_series_values,
+    parse_dataset_series,
 )
 from .dcat_resource import parse_dcat_resource
 from .dct_standard import extract_dct_standard_list
 from .distribution import extract_distributions
 from .event import (
     extend_with_associated_broader_types,
     parse_event,
```

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/address.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/address.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/agent.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/agent.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/catalog.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/catalog.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/channel.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/channel.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/concept.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/concept.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/conforms_to.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/conforms_to.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/contactpoint.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/contactpoint.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/cost.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/cost.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/cpsvno_service.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/cpsvno_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/data_distribution_service.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/data_distribution_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/dataservice.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/dataservice.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/dataset.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import logging
 from typing import (
     Dict,
     List,
+    Optional,
 )
 
 from rdflib import (
     Graph,
     URIRef,
 )
 from rdflib.namespace import (
@@ -139,23 +141,60 @@
             subject=dataset_uri,
         )
     )
 
     return dataset
 
 
-def parse_dataset_series_values(
-    datasets_graph: Graph, dataset_uri: URIRef
-) -> DatasetSeries:
+def parse_dataset_series(datasets_graph: Graph, dataset_uri: URIRef) -> DatasetSeries:
+    prev_dataset_uri = object_value(datasets_graph, dataset_uri, dcat_uri("last"))
     return DatasetSeries(
-        last=object_value(datasets_graph, dataset_uri, dcat_uri("last")),
-        first=object_value(datasets_graph, dataset_uri, dcat_uri("first")),
+        last=prev_dataset_uri,
+        datasetsInSeries=extract_datasets_in_series(
+            datasets_graph, dataset_uri.toPython(), prev_dataset_uri
+        )
+        if prev_dataset_uri
+        else None,
     )
 
 
+def extract_datasets_in_series(
+    datasets_graph: Graph, dataset_series_uri: str, last_dataset_uri: str
+) -> List[str]:
+    datasets_in_series: List[str] = [last_dataset_uri]
+    cur_dataset_uri: Optional[str] = last_dataset_uri
+
+    while prev_dataset_uri := object_value(
+        datasets_graph, URIRef(str(cur_dataset_uri)), dcat_uri("prev")
+    ):
+        # Check for circular graphs
+        if prev_dataset_uri in datasets_in_series:
+            logging.warning(
+                f"Circular linking in dataset series {dataset_series_uri}, on dataset {cur_dataset_uri}. Aborting list traversal."
+            )
+            break
+        datasets_in_series.append(prev_dataset_uri)
+        cur_dataset_uri = prev_dataset_uri
+
+    # Verify that all datasets in series are included
+    number_of_datasets_in_series = len(
+        list(
+            datasets_graph.subjects(
+                dcat_uri("inSeries"), URIRef(dataset_series_uri), unique=True
+            )
+        )
+    )
+    if len(datasets_in_series) != number_of_datasets_in_series:
+        logging.warning(
+            f"List of datasets in series {dataset_series_uri} is incomplete, linked list might be broken."
+        )
+
+    return datasets_in_series
+
+
 def extract_boolean(
     datasets_graph: Graph, dataset_uri: URIRef, predicate: URIRef
 ) -> bool:
     value = object_value(datasets_graph, dataset_uri, predicate)
     return value if value and isinstance(value, bool) else False
```

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/dcat_resource.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/dcat_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/dct_standard.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/dct_standard.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/distribution.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/distribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/event.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/event.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/evidence.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/evidence.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/format.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/format.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/info_model.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/info_model.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/legal_resource.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/legal_resource.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/media_type.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/media_type.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/model_element.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/model_element.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/model_property.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/model_property.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/opening_hours_specification.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/opening_hours_specification.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/organization.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/organization.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/output.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/output.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/participation.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/participation.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/publisher.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/publisher.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/qualified_attribution.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/qualified_attribution.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/quality_annotation.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/quality_annotation.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/reference_data_code.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/reference_data_code.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/references.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/references.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/requirement.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/requirement.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/rule.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/rule.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/skos_concept.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/skos_concept.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/subject.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/subject.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/parse_functions/temporal.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/parse_functions/temporal.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/rdf_utils/__init__.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/rdf_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/rdf_utils/ns.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/rdf_utils/ns.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/rdf_utils/utils.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/rdf_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/__init__.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/extend_cpsvno_service.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/extend_cpsvno_service.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/extend_dataservice.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/extend_dataservice.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/extend_dataset.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/extend_dataset.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/extend_info_model.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/extend_info_model.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/reference_data.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/reference_data.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/reference_data_client.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/reference_data_client.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/src/fdk_rdf_parser/reference_data/utils.py` & `fdk_rdf_parser-2.2.9/src/fdk_rdf_parser/reference_data/utils.py`

 * *Files identical despite different names*

### Comparing `fdk_rdf_parser-2.2.8/setup.py` & `fdk_rdf_parser-2.2.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 {'': ['*']}
 
 install_requires = \
 ['isodate>=0.6.1,<0.7.0', 'rdflib>=6.2.0,<7.0.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'fdk-rdf-parser',
-    'version': '2.2.8',
+    'version': '2.2.9',
     'description': '',
     'long_description': 'None',
     'author': 'NilsOveTen',
     'author_email': 'nils.ove.tendenes@digdir.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```


# Comparing `tmp/geoh5py-0.9.0rc1.tar.gz` & `tmp/geoh5py-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoh5py-0.9.0rc1.tar", max compression
+gzip compressed data, was "geoh5py-0.9.0rc2.tar", max compression
```

## Comparing `geoh5py-0.9.0rc1.tar` & `geoh5py-0.9.0rc2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0    35823 2024-04-23 21:09:09.940960 geoh5py-0.9.0rc1/COPYING
--rw-r--r--   0        0        0     7817 2024-04-23 21:09:09.940960 geoh5py-0.9.0rc1/COPYING.LESSER
--rw-r--r--   0        0        0      838 2024-04-26 16:22:09.229409 geoh5py-0.9.0rc1/geoh5py/__init__.py
--rw-r--r--   0        0        0     1574 2024-04-23 21:09:10.033237 geoh5py-0.9.0rc1/geoh5py/data/__init__.py
--rw-r--r--   0        0        0     1311 2024-04-23 21:09:10.034242 geoh5py-0.9.0rc1/geoh5py/data/blob_data.py
--rw-r--r--   0        0        0     2005 2024-04-23 21:09:10.034314 geoh5py-0.9.0rc1/geoh5py/data/boolean_data.py
--rw-r--r--   0        0        0     3756 2024-04-23 21:09:10.034314 geoh5py-0.9.0rc1/geoh5py/data/color_map.py
--rw-r--r--   0        0        0     8914 2024-04-23 21:09:50.491132 geoh5py-0.9.0rc1/geoh5py/data/data.py
--rw-r--r--   0        0        0     1138 2024-04-23 21:09:10.035431 geoh5py-0.9.0rc1/geoh5py/data/data_association_enum.py
--rw-r--r--   0        0        0    13377 2024-04-23 21:09:50.491940 geoh5py-0.9.0rc1/geoh5py/data/data_type.py
--rw-r--r--   0        0        0     1138 2024-04-23 21:09:10.035431 geoh5py-0.9.0rc1/geoh5py/data/data_unit.py
--rw-r--r--   0        0        0     1340 2024-04-23 21:09:10.036503 geoh5py-0.9.0rc1/geoh5py/data/datetime_data.py
--rw-r--r--   0        0        0     3690 2024-04-23 21:09:10.036503 geoh5py-0.9.0rc1/geoh5py/data/filename_data.py
--rw-r--r--   0        0        0     1787 2024-04-23 21:09:10.036503 geoh5py-0.9.0rc1/geoh5py/data/float_data.py
--rw-r--r--   0        0        0     1625 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc1/geoh5py/data/geometric_data_constants.py
--rw-r--r--   0        0        0     1709 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc1/geoh5py/data/integer_data.py
--rw-r--r--   0        0        0     4001 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc1/geoh5py/data/numeric_data.py
--rw-r--r--   0        0        0     1121 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc1/geoh5py/data/primitive_type_enum.py
--rw-r--r--   0        0        0     2896 2024-04-23 21:09:50.493092 geoh5py-0.9.0rc1/geoh5py/data/reference_value_map.py
--rw-r--r--   0        0        0     1531 2024-04-23 21:09:10.038674 geoh5py-0.9.0rc1/geoh5py/data/referenced_data.py
--rw-r--r--   0        0        0     5093 2024-04-23 21:09:10.038674 geoh5py-0.9.0rc1/geoh5py/data/text_data.py
--rw-r--r--   0        0        0     1573 2024-04-23 21:09:10.039753 geoh5py-0.9.0rc1/geoh5py/data/unknown_data.py
--rw-r--r--   0        0        0     4559 2024-04-23 21:09:10.039753 geoh5py-0.9.0rc1/geoh5py/data/visual_parameters.py
--rw-r--r--   0        0        0     1587 2024-04-23 21:09:10.039753 geoh5py-0.9.0rc1/geoh5py/groups/__init__.py
--rw-r--r--   0        0        0     1441 2024-04-23 21:09:10.040830 geoh5py-0.9.0rc1/geoh5py/groups/container_group.py
--rw-r--r--   0        0        0     1474 2024-04-23 21:09:10.040830 geoh5py-0.9.0rc1/geoh5py/groups/custom_group.py
--rw-r--r--   0        0        0     1797 2024-04-23 21:09:10.040830 geoh5py-0.9.0rc1/geoh5py/groups/drillhole_group.py
--rw-r--r--   0        0        0     1444 2024-04-23 21:09:10.041866 geoh5py-0.9.0rc1/geoh5py/groups/giftools_group.py
--rw-r--r--   0        0        0     7068 2024-04-23 21:09:50.493092 geoh5py-0.9.0rc1/geoh5py/groups/group.py
--rw-r--r--   0        0        0     2517 2024-04-23 21:09:10.041938 geoh5py-0.9.0rc1/geoh5py/groups/group_type.py
--rw-r--r--   0        0        0     6714 2024-04-23 21:09:10.043010 geoh5py-0.9.0rc1/geoh5py/groups/integrator_group.py
--rw-r--r--   0        0        0     1295 2024-04-23 21:09:10.043010 geoh5py-0.9.0rc1/geoh5py/groups/maps_group.py
--rw-r--r--   0        0        0     1414 2024-04-23 21:09:10.043010 geoh5py-0.9.0rc1/geoh5py/groups/notype_group.py
--rw-r--r--   0        0        0     7843 2024-04-23 21:09:50.494180 geoh5py-0.9.0rc1/geoh5py/groups/property_group.py
--rw-r--r--   0        0        0     1593 2024-04-23 21:09:10.044089 geoh5py-0.9.0rc1/geoh5py/groups/root_group.py
--rw-r--r--   0        0        0     2053 2024-04-23 21:09:10.044089 geoh5py-0.9.0rc1/geoh5py/groups/simpeg_group.py
--rw-r--r--   0        0        0     1322 2024-04-23 21:09:10.044089 geoh5py-0.9.0rc1/geoh5py/groups/survey_group.py
--rw-r--r--   0        0        0      866 2024-04-23 21:09:10.049503 geoh5py-0.9.0rc1/geoh5py/io/__init__.py
--rw-r--r--   0        0        0    17355 2024-04-23 21:09:50.495268 geoh5py-0.9.0rc1/geoh5py/io/h5_reader.py
--rw-r--r--   0        0        0    34805 2024-04-23 21:09:50.495268 geoh5py-0.9.0rc1/geoh5py/io/h5_writer.py
--rw-r--r--   0        0        0     2403 2024-04-23 21:09:10.051610 geoh5py-0.9.0rc1/geoh5py/objects/__init__.py
--rw-r--r--   0        0        0     9440 2024-04-23 21:09:10.051957 geoh5py-0.9.0rc1/geoh5py/objects/block_model.py
--rw-r--r--   0        0        0     7873 2024-04-23 21:09:50.496387 geoh5py-0.9.0rc1/geoh5py/objects/cell_object.py
--rw-r--r--   0        0        0     6300 2024-04-23 21:09:50.497531 geoh5py-0.9.0rc1/geoh5py/objects/curve.py
--rw-r--r--   0        0        0     6204 2024-04-23 21:09:10.053010 geoh5py-0.9.0rc1/geoh5py/objects/drape_model.py
--rw-r--r--   0        0        0    26674 2024-04-23 21:09:10.053010 geoh5py-0.9.0rc1/geoh5py/objects/drillhole.py
--rw-r--r--   0        0        0    21867 2024-04-23 21:09:50.498540 geoh5py-0.9.0rc1/geoh5py/objects/geo_image.py
--rw-r--r--   0        0        0    14054 2024-04-23 21:09:10.053963 geoh5py-0.9.0rc1/geoh5py/objects/grid2d.py
--rw-r--r--   0        0        0     4879 2024-04-23 21:09:10.053963 geoh5py-0.9.0rc1/geoh5py/objects/grid_object.py
--rw-r--r--   0        0        0     1957 2024-04-23 21:09:10.053963 geoh5py-0.9.0rc1/geoh5py/objects/integrator.py
--rw-r--r--   0        0        0     2921 2024-04-23 21:09:10.055218 geoh5py-0.9.0rc1/geoh5py/objects/label.py
--rw-r--r--   0        0        0     2686 2024-04-23 21:09:10.055218 geoh5py-0.9.0rc1/geoh5py/objects/notype_object.py
--rw-r--r--   0        0        0    21991 2024-04-23 21:09:50.498666 geoh5py-0.9.0rc1/geoh5py/objects/object_base.py
--rw-r--r--   0        0        0     1098 2024-04-23 21:09:10.056303 geoh5py-0.9.0rc1/geoh5py/objects/object_type.py
--rw-r--r--   0        0        0    13455 2024-04-23 21:09:50.499764 geoh5py-0.9.0rc1/geoh5py/objects/octree.py
--rw-r--r--   0        0        0     5353 2024-04-23 21:09:50.500917 geoh5py-0.9.0rc1/geoh5py/objects/points.py
--rw-r--r--   0        0        0     2588 2024-04-23 21:09:10.057382 geoh5py-0.9.0rc1/geoh5py/objects/surface.py
--rw-r--r--   0        0        0      747 2024-04-23 21:09:10.057382 geoh5py-0.9.0rc1/geoh5py/objects/surveys/__init__.py
--rw-r--r--   0        0        0    14521 2024-04-23 21:09:10.058382 geoh5py-0.9.0rc1/geoh5py/objects/surveys/direct_current.py
--rw-r--r--   0        0        0      747 2024-04-23 21:09:10.058382 geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/__init__.py
--rw-r--r--   0        0        0     3660 2024-04-23 21:09:10.058382 geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
--rw-r--r--   0        0        0     3629 2024-04-23 21:09:10.059469 geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
--rw-r--r--   0        0        0    36522 2024-04-23 21:09:10.059469 geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/base.py
--rw-r--r--   0        0        0     6925 2024-04-23 21:09:10.059469 geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/ground_fem.py
--rw-r--r--   0        0        0     6937 2024-04-23 21:09:10.060547 geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/ground_tem.py
--rw-r--r--   0        0        0     2615 2024-04-23 21:09:10.060547 geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
--rw-r--r--   0        0        0     6605 2024-04-23 21:09:10.060547 geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/tipper.py
--rw-r--r--   0        0        0     1247 2024-04-23 21:09:10.061666 geoh5py-0.9.0rc1/geoh5py/objects/surveys/magnetics.py
--rw-r--r--   0        0        0        0 2024-04-23 21:09:10.061666 geoh5py-0.9.0rc1/geoh5py/py.typed
--rw-r--r--   0        0        0     1013 2024-04-23 21:09:10.061666 geoh5py-0.9.0rc1/geoh5py/shared/__init__.py
--rw-r--r--   0        0        0     1057 2024-04-23 21:09:10.062721 geoh5py-0.9.0rc1/geoh5py/shared/concatenation/__init__.py
--rw-r--r--   0        0        0     1847 2024-04-23 21:09:10.062721 geoh5py-0.9.0rc1/geoh5py/shared/concatenation/concatenated.py
--rw-r--r--   0        0        0    25972 2024-04-23 21:09:50.500917 geoh5py-0.9.0rc1/geoh5py/shared/concatenation/concatenator.py
--rw-r--r--   0        0        0     3029 2024-04-23 21:09:10.063809 geoh5py-0.9.0rc1/geoh5py/shared/concatenation/data.py
--rw-r--r--   0        0        0    14282 2024-04-23 21:09:50.502000 geoh5py-0.9.0rc1/geoh5py/shared/concatenation/drillhole.py
--rw-r--r--   0        0        0    15847 2024-04-23 21:09:50.503139 geoh5py-0.9.0rc1/geoh5py/shared/concatenation/drillholes_group_table.py
--rw-r--r--   0        0        0     6729 2024-04-23 21:09:50.503139 geoh5py-0.9.0rc1/geoh5py/shared/concatenation/object.py
--rw-r--r--   0        0        0     5193 2024-04-23 21:09:50.504046 geoh5py-0.9.0rc1/geoh5py/shared/concatenation/property_group.py
--rw-r--r--   0        0        0      937 2024-04-23 21:09:10.066045 geoh5py-0.9.0rc1/geoh5py/shared/conversion/__init__.py
--rw-r--r--   0        0        0     4426 2024-04-23 21:09:10.067142 geoh5py-0.9.0rc1/geoh5py/shared/conversion/base.py
--rw-r--r--   0        0        0     5629 2024-04-23 21:09:50.504628 geoh5py-0.9.0rc1/geoh5py/shared/conversion/geo_image.py
--rw-r--r--   0        0        0    10840 2024-04-23 21:09:10.068311 geoh5py-0.9.0rc1/geoh5py/shared/conversion/grid2d.py
--rw-r--r--   0        0        0    10730 2024-04-23 21:09:10.068311 geoh5py-0.9.0rc1/geoh5py/shared/entity.py
--rw-r--r--   0        0        0     7630 2024-04-23 21:09:50.505726 geoh5py-0.9.0rc1/geoh5py/shared/entity_container.py
--rw-r--r--   0        0        0     8632 2024-04-23 21:09:10.069420 geoh5py-0.9.0rc1/geoh5py/shared/entity_type.py
--rw-r--r--   0        0        0     8353 2024-04-23 21:09:10.070423 geoh5py-0.9.0rc1/geoh5py/shared/exceptions.py
--rw-r--r--   0        0        0      923 2024-04-23 21:09:10.070423 geoh5py-0.9.0rc1/geoh5py/shared/merging/__init__.py
--rw-r--r--   0        0        0     7734 2024-04-23 21:09:10.071533 geoh5py-0.9.0rc1/geoh5py/shared/merging/base.py
--rw-r--r--   0        0        0     2336 2024-04-23 21:09:10.071533 geoh5py-0.9.0rc1/geoh5py/shared/merging/cell.py
--rw-r--r--   0        0        0     6105 2024-04-23 21:09:10.072628 geoh5py-0.9.0rc1/geoh5py/shared/merging/drape_model.py
--rw-r--r--   0        0        0     1845 2024-04-23 21:09:10.072628 geoh5py-0.9.0rc1/geoh5py/shared/merging/points.py
--rw-r--r--   0        0        0    21424 2024-04-23 21:09:50.506831 geoh5py-0.9.0rc1/geoh5py/shared/utils.py
--rw-r--r--   0        0        0     8847 2024-04-23 21:09:10.073740 geoh5py-0.9.0rc1/geoh5py/shared/validators.py
--rw-r--r--   0        0        0     2647 2024-04-23 21:09:10.074842 geoh5py-0.9.0rc1/geoh5py/shared/weakref_utils.py
--rw-r--r--   0        0        0      959 2024-04-23 21:09:10.074842 geoh5py-0.9.0rc1/geoh5py/ui_json/__init__.py
--rw-r--r--   0        0        0     2991 2024-04-23 21:09:10.076022 geoh5py-0.9.0rc1/geoh5py/ui_json/constants.py
--rw-r--r--   0        0        0     1983 2024-04-23 21:09:10.076022 geoh5py-0.9.0rc1/geoh5py/ui_json/descriptors.py
--rw-r--r--   0        0        0    11461 2024-04-23 21:09:10.077023 geoh5py-0.9.0rc1/geoh5py/ui_json/enforcers.py
--rw-r--r--   0        0        0    18309 2024-04-23 21:09:10.077147 geoh5py-0.9.0rc1/geoh5py/ui_json/forms.py
--rw-r--r--   0        0        0    18789 2024-04-23 21:09:50.508030 geoh5py-0.9.0rc1/geoh5py/ui_json/input_file.py
--rw-r--r--   0        0        0     4939 2024-04-26 17:53:29.560114 geoh5py-0.9.0rc1/geoh5py/ui_json/parameters.py
--rw-r--r--   0        0        0    15250 2024-04-23 21:09:50.508030 geoh5py-0.9.0rc1/geoh5py/ui_json/templates.py
--rw-r--r--   0        0        0     5076 2024-04-23 21:09:10.079354 geoh5py-0.9.0rc1/geoh5py/ui_json/ui_json.py
--rw-r--r--   0        0        0    11199 2024-04-23 21:09:50.509027 geoh5py-0.9.0rc1/geoh5py/ui_json/utils.py
--rw-r--r--   0        0        0    11402 2024-04-26 17:53:43.697719 geoh5py-0.9.0rc1/geoh5py/ui_json/validation.py
--rw-r--r--   0        0        0      852 2024-04-23 21:09:10.081557 geoh5py-0.9.0rc1/geoh5py/workspace/__init__.py
--rw-r--r--   0        0        0    51060 2024-04-23 21:09:50.511214 geoh5py-0.9.0rc1/geoh5py/workspace/workspace.py
--rw-r--r--   0        0        0     2111 2024-04-23 21:09:10.082662 geoh5py-0.9.0rc1/package.rst
--rw-r--r--   0        0        0     2355 2024-04-26 17:29:33.100894 geoh5py-0.9.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5600 2024-04-23 21:09:09.940960 geoh5py-0.9.0rc1/README.rst
--rw-r--r--   0        0        0    54566 2024-04-23 21:09:09.942022 geoh5py-0.9.0rc1/THIRD_PARTY_SOFTWARE.rst
--rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 geoh5py-0.9.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-04-23 21:09:09.940960 geoh5py-0.9.0rc2/COPYING
+-rw-r--r--   0        0        0     7817 2024-04-23 21:09:09.940960 geoh5py-0.9.0rc2/COPYING.LESSER
+-rw-r--r--   0        0        0      838 2024-05-02 19:52:20.263627 geoh5py-0.9.0rc2/geoh5py/__init__.py
+-rw-r--r--   0        0        0     1574 2024-04-23 21:09:10.033237 geoh5py-0.9.0rc2/geoh5py/data/__init__.py
+-rw-r--r--   0        0        0     1311 2024-04-23 21:09:10.034242 geoh5py-0.9.0rc2/geoh5py/data/blob_data.py
+-rw-r--r--   0        0        0     2005 2024-04-23 21:09:10.034314 geoh5py-0.9.0rc2/geoh5py/data/boolean_data.py
+-rw-r--r--   0        0        0     3756 2024-04-23 21:09:10.034314 geoh5py-0.9.0rc2/geoh5py/data/color_map.py
+-rw-r--r--   0        0        0     8914 2024-04-23 21:09:50.491132 geoh5py-0.9.0rc2/geoh5py/data/data.py
+-rw-r--r--   0        0        0     1138 2024-04-23 21:09:10.035431 geoh5py-0.9.0rc2/geoh5py/data/data_association_enum.py
+-rw-r--r--   0        0        0    13377 2024-04-23 21:09:50.491940 geoh5py-0.9.0rc2/geoh5py/data/data_type.py
+-rw-r--r--   0        0        0     1138 2024-04-23 21:09:10.035431 geoh5py-0.9.0rc2/geoh5py/data/data_unit.py
+-rw-r--r--   0        0        0     1340 2024-04-23 21:09:10.036503 geoh5py-0.9.0rc2/geoh5py/data/datetime_data.py
+-rw-r--r--   0        0        0     3690 2024-04-23 21:09:10.036503 geoh5py-0.9.0rc2/geoh5py/data/filename_data.py
+-rw-r--r--   0        0        0     1787 2024-04-23 21:09:10.036503 geoh5py-0.9.0rc2/geoh5py/data/float_data.py
+-rw-r--r--   0        0        0     1625 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc2/geoh5py/data/geometric_data_constants.py
+-rw-r--r--   0        0        0     1709 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc2/geoh5py/data/integer_data.py
+-rw-r--r--   0        0        0     4001 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc2/geoh5py/data/numeric_data.py
+-rw-r--r--   0        0        0     1121 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc2/geoh5py/data/primitive_type_enum.py
+-rw-r--r--   0        0        0     2896 2024-04-23 21:09:50.493092 geoh5py-0.9.0rc2/geoh5py/data/reference_value_map.py
+-rw-r--r--   0        0        0     1531 2024-04-23 21:09:10.038674 geoh5py-0.9.0rc2/geoh5py/data/referenced_data.py
+-rw-r--r--   0        0        0     5093 2024-04-23 21:09:10.038674 geoh5py-0.9.0rc2/geoh5py/data/text_data.py
+-rw-r--r--   0        0        0     1573 2024-04-23 21:09:10.039753 geoh5py-0.9.0rc2/geoh5py/data/unknown_data.py
+-rw-r--r--   0        0        0     4559 2024-04-23 21:09:10.039753 geoh5py-0.9.0rc2/geoh5py/data/visual_parameters.py
+-rw-r--r--   0        0        0     1587 2024-04-23 21:09:10.039753 geoh5py-0.9.0rc2/geoh5py/groups/__init__.py
+-rw-r--r--   0        0        0     1441 2024-04-23 21:09:10.040830 geoh5py-0.9.0rc2/geoh5py/groups/container_group.py
+-rw-r--r--   0        0        0     1474 2024-04-23 21:09:10.040830 geoh5py-0.9.0rc2/geoh5py/groups/custom_group.py
+-rw-r--r--   0        0        0     1797 2024-04-23 21:09:10.040830 geoh5py-0.9.0rc2/geoh5py/groups/drillhole_group.py
+-rw-r--r--   0        0        0     1444 2024-04-23 21:09:10.041866 geoh5py-0.9.0rc2/geoh5py/groups/giftools_group.py
+-rw-r--r--   0        0        0     7068 2024-04-23 21:09:50.493092 geoh5py-0.9.0rc2/geoh5py/groups/group.py
+-rw-r--r--   0        0        0     2517 2024-04-23 21:09:10.041938 geoh5py-0.9.0rc2/geoh5py/groups/group_type.py
+-rw-r--r--   0        0        0     6714 2024-04-23 21:09:10.043010 geoh5py-0.9.0rc2/geoh5py/groups/integrator_group.py
+-rw-r--r--   0        0        0     1295 2024-04-23 21:09:10.043010 geoh5py-0.9.0rc2/geoh5py/groups/maps_group.py
+-rw-r--r--   0        0        0     1414 2024-04-23 21:09:10.043010 geoh5py-0.9.0rc2/geoh5py/groups/notype_group.py
+-rw-r--r--   0        0        0     7843 2024-04-23 21:09:50.494180 geoh5py-0.9.0rc2/geoh5py/groups/property_group.py
+-rw-r--r--   0        0        0     1593 2024-04-23 21:09:10.044089 geoh5py-0.9.0rc2/geoh5py/groups/root_group.py
+-rw-r--r--   0        0        0     2053 2024-04-23 21:09:10.044089 geoh5py-0.9.0rc2/geoh5py/groups/simpeg_group.py
+-rw-r--r--   0        0        0     1322 2024-04-23 21:09:10.044089 geoh5py-0.9.0rc2/geoh5py/groups/survey_group.py
+-rw-r--r--   0        0        0      866 2024-04-23 21:09:10.049503 geoh5py-0.9.0rc2/geoh5py/io/__init__.py
+-rw-r--r--   0        0        0    17355 2024-04-23 21:09:50.495268 geoh5py-0.9.0rc2/geoh5py/io/h5_reader.py
+-rw-r--r--   0        0        0    34805 2024-04-23 21:09:50.495268 geoh5py-0.9.0rc2/geoh5py/io/h5_writer.py
+-rw-r--r--   0        0        0     2403 2024-04-23 21:09:10.051610 geoh5py-0.9.0rc2/geoh5py/objects/__init__.py
+-rw-r--r--   0        0        0     9440 2024-04-23 21:09:10.051957 geoh5py-0.9.0rc2/geoh5py/objects/block_model.py
+-rw-r--r--   0        0        0     7873 2024-04-23 21:09:50.496387 geoh5py-0.9.0rc2/geoh5py/objects/cell_object.py
+-rw-r--r--   0        0        0     6300 2024-04-23 21:09:50.497531 geoh5py-0.9.0rc2/geoh5py/objects/curve.py
+-rw-r--r--   0        0        0     6204 2024-04-23 21:09:10.053010 geoh5py-0.9.0rc2/geoh5py/objects/drape_model.py
+-rw-r--r--   0        0        0    26674 2024-04-23 21:09:10.053010 geoh5py-0.9.0rc2/geoh5py/objects/drillhole.py
+-rw-r--r--   0        0        0    21867 2024-04-23 21:09:50.498540 geoh5py-0.9.0rc2/geoh5py/objects/geo_image.py
+-rw-r--r--   0        0        0    14054 2024-04-23 21:09:10.053963 geoh5py-0.9.0rc2/geoh5py/objects/grid2d.py
+-rw-r--r--   0        0        0     4879 2024-04-23 21:09:10.053963 geoh5py-0.9.0rc2/geoh5py/objects/grid_object.py
+-rw-r--r--   0        0        0     1957 2024-04-23 21:09:10.053963 geoh5py-0.9.0rc2/geoh5py/objects/integrator.py
+-rw-r--r--   0        0        0     2921 2024-04-23 21:09:10.055218 geoh5py-0.9.0rc2/geoh5py/objects/label.py
+-rw-r--r--   0        0        0     2686 2024-04-23 21:09:10.055218 geoh5py-0.9.0rc2/geoh5py/objects/notype_object.py
+-rw-r--r--   0        0        0    21991 2024-04-23 21:09:50.498666 geoh5py-0.9.0rc2/geoh5py/objects/object_base.py
+-rw-r--r--   0        0        0     1098 2024-04-23 21:09:10.056303 geoh5py-0.9.0rc2/geoh5py/objects/object_type.py
+-rw-r--r--   0        0        0    13455 2024-04-23 21:09:50.499764 geoh5py-0.9.0rc2/geoh5py/objects/octree.py
+-rw-r--r--   0        0        0     5353 2024-04-23 21:09:50.500917 geoh5py-0.9.0rc2/geoh5py/objects/points.py
+-rw-r--r--   0        0        0     2588 2024-04-23 21:09:10.057382 geoh5py-0.9.0rc2/geoh5py/objects/surface.py
+-rw-r--r--   0        0        0      747 2024-04-23 21:09:10.057382 geoh5py-0.9.0rc2/geoh5py/objects/surveys/__init__.py
+-rw-r--r--   0        0        0    14521 2024-04-23 21:09:10.058382 geoh5py-0.9.0rc2/geoh5py/objects/surveys/direct_current.py
+-rw-r--r--   0        0        0      747 2024-04-23 21:09:10.058382 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/__init__.py
+-rw-r--r--   0        0        0     3660 2024-04-23 21:09:10.058382 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
+-rw-r--r--   0        0        0     3629 2024-04-23 21:09:10.059469 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
+-rw-r--r--   0        0        0    36522 2024-04-23 21:09:10.059469 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/base.py
+-rw-r--r--   0        0        0     6925 2024-04-23 21:09:10.059469 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/ground_fem.py
+-rw-r--r--   0        0        0     6937 2024-04-23 21:09:10.060547 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/ground_tem.py
+-rw-r--r--   0        0        0     2615 2024-04-23 21:09:10.060547 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
+-rw-r--r--   0        0        0     6605 2024-04-23 21:09:10.060547 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/tipper.py
+-rw-r--r--   0        0        0     1247 2024-04-23 21:09:10.061666 geoh5py-0.9.0rc2/geoh5py/objects/surveys/magnetics.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:09:10.061666 geoh5py-0.9.0rc2/geoh5py/py.typed
+-rw-r--r--   0        0        0     1013 2024-04-23 21:09:10.061666 geoh5py-0.9.0rc2/geoh5py/shared/__init__.py
+-rw-r--r--   0        0        0     1057 2024-04-23 21:09:10.062721 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/__init__.py
+-rw-r--r--   0        0        0     1847 2024-04-23 21:09:10.062721 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/concatenated.py
+-rw-r--r--   0        0        0    25972 2024-04-23 21:09:50.500917 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/concatenator.py
+-rw-r--r--   0        0        0     3029 2024-04-23 21:09:10.063809 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/data.py
+-rw-r--r--   0        0        0    14282 2024-04-23 21:09:50.502000 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/drillhole.py
+-rw-r--r--   0        0        0    15847 2024-04-23 21:09:50.503139 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/drillholes_group_table.py
+-rw-r--r--   0        0        0     6729 2024-04-23 21:09:50.503139 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/object.py
+-rw-r--r--   0        0        0     5193 2024-04-23 21:09:50.504046 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/property_group.py
+-rw-r--r--   0        0        0      937 2024-04-23 21:09:10.066045 geoh5py-0.9.0rc2/geoh5py/shared/conversion/__init__.py
+-rw-r--r--   0        0        0     4426 2024-04-23 21:09:10.067142 geoh5py-0.9.0rc2/geoh5py/shared/conversion/base.py
+-rw-r--r--   0        0        0     5629 2024-04-23 21:09:50.504628 geoh5py-0.9.0rc2/geoh5py/shared/conversion/geo_image.py
+-rw-r--r--   0        0        0    10840 2024-04-23 21:09:10.068311 geoh5py-0.9.0rc2/geoh5py/shared/conversion/grid2d.py
+-rw-r--r--   0        0        0    10730 2024-04-23 21:09:10.068311 geoh5py-0.9.0rc2/geoh5py/shared/entity.py
+-rw-r--r--   0        0        0     7630 2024-04-23 21:09:50.505726 geoh5py-0.9.0rc2/geoh5py/shared/entity_container.py
+-rw-r--r--   0        0        0     8632 2024-04-23 21:09:10.069420 geoh5py-0.9.0rc2/geoh5py/shared/entity_type.py
+-rw-r--r--   0        0        0     8353 2024-04-23 21:09:10.070423 geoh5py-0.9.0rc2/geoh5py/shared/exceptions.py
+-rw-r--r--   0        0        0      923 2024-04-23 21:09:10.070423 geoh5py-0.9.0rc2/geoh5py/shared/merging/__init__.py
+-rw-r--r--   0        0        0     7734 2024-04-23 21:09:10.071533 geoh5py-0.9.0rc2/geoh5py/shared/merging/base.py
+-rw-r--r--   0        0        0     2336 2024-04-23 21:09:10.071533 geoh5py-0.9.0rc2/geoh5py/shared/merging/cell.py
+-rw-r--r--   0        0        0     6105 2024-04-23 21:09:10.072628 geoh5py-0.9.0rc2/geoh5py/shared/merging/drape_model.py
+-rw-r--r--   0        0        0     1845 2024-04-23 21:09:10.072628 geoh5py-0.9.0rc2/geoh5py/shared/merging/points.py
+-rw-r--r--   0        0        0    21424 2024-04-23 21:09:50.506831 geoh5py-0.9.0rc2/geoh5py/shared/utils.py
+-rw-r--r--   0        0        0     8847 2024-04-23 21:09:10.073740 geoh5py-0.9.0rc2/geoh5py/shared/validators.py
+-rw-r--r--   0        0        0     2647 2024-04-23 21:09:10.074842 geoh5py-0.9.0rc2/geoh5py/shared/weakref_utils.py
+-rw-r--r--   0        0        0      959 2024-04-23 21:09:10.074842 geoh5py-0.9.0rc2/geoh5py/ui_json/__init__.py
+-rw-r--r--   0        0        0     2991 2024-04-23 21:09:10.076022 geoh5py-0.9.0rc2/geoh5py/ui_json/constants.py
+-rw-r--r--   0        0        0     1983 2024-04-23 21:09:10.076022 geoh5py-0.9.0rc2/geoh5py/ui_json/descriptors.py
+-rw-r--r--   0        0        0    11461 2024-04-23 21:09:10.077023 geoh5py-0.9.0rc2/geoh5py/ui_json/enforcers.py
+-rw-r--r--   0        0        0    18309 2024-04-23 21:09:10.077147 geoh5py-0.9.0rc2/geoh5py/ui_json/forms.py
+-rw-r--r--   0        0        0    18789 2024-04-23 21:09:50.508030 geoh5py-0.9.0rc2/geoh5py/ui_json/input_file.py
+-rw-r--r--   0        0        0     4939 2024-04-26 17:53:29.560114 geoh5py-0.9.0rc2/geoh5py/ui_json/parameters.py
+-rw-r--r--   0        0        0    15250 2024-04-23 21:09:50.508030 geoh5py-0.9.0rc2/geoh5py/ui_json/templates.py
+-rw-r--r--   0        0        0     5076 2024-04-23 21:09:10.079354 geoh5py-0.9.0rc2/geoh5py/ui_json/ui_json.py
+-rw-r--r--   0        0        0    11199 2024-04-23 21:09:50.509027 geoh5py-0.9.0rc2/geoh5py/ui_json/utils.py
+-rw-r--r--   0        0        0    11402 2024-04-26 17:53:43.697719 geoh5py-0.9.0rc2/geoh5py/ui_json/validation.py
+-rw-r--r--   0        0        0      852 2024-04-23 21:09:10.081557 geoh5py-0.9.0rc2/geoh5py/workspace/__init__.py
+-rw-r--r--   0        0        0    51060 2024-04-23 21:09:50.511214 geoh5py-0.9.0rc2/geoh5py/workspace/workspace.py
+-rw-r--r--   0        0        0     2111 2024-04-23 21:09:10.082662 geoh5py-0.9.0rc2/package.rst
+-rw-r--r--   0        0        0     2432 2024-05-02 19:52:20.268477 geoh5py-0.9.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5600 2024-04-23 21:09:09.940960 geoh5py-0.9.0rc2/README.rst
+-rw-r--r--   0        0        0    54566 2024-04-23 21:09:09.942022 geoh5py-0.9.0rc2/THIRD_PARTY_SOFTWARE.rst
+-rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 geoh5py-0.9.0rc2/PKG-INFO
```

### Comparing `geoh5py-0.9.0rc1/COPYING` & `geoh5py-0.9.0rc2/COPYING`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/COPYING.LESSER` & `geoh5py-0.9.0rc2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 # flake8: noqa
 
-__version__ = "0.9.0-rc.1"
+__version__ = "0.9.0-rc.2"
 
 from geoh5py.workspace import Workspace
```

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/data/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/blob_data.py` & `geoh5py-0.9.0rc2/geoh5py/data/blob_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/boolean_data.py` & `geoh5py-0.9.0rc2/geoh5py/data/boolean_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/color_map.py` & `geoh5py-0.9.0rc2/geoh5py/data/color_map.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/data.py` & `geoh5py-0.9.0rc2/geoh5py/data/data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/data_association_enum.py` & `geoh5py-0.9.0rc2/geoh5py/data/data_association_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/data_type.py` & `geoh5py-0.9.0rc2/geoh5py/data/data_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/data_unit.py` & `geoh5py-0.9.0rc2/geoh5py/data/data_unit.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/datetime_data.py` & `geoh5py-0.9.0rc2/geoh5py/data/datetime_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/filename_data.py` & `geoh5py-0.9.0rc2/geoh5py/data/filename_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/float_data.py` & `geoh5py-0.9.0rc2/geoh5py/data/float_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/geometric_data_constants.py` & `geoh5py-0.9.0rc2/geoh5py/data/geometric_data_constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/integer_data.py` & `geoh5py-0.9.0rc2/geoh5py/data/integer_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/numeric_data.py` & `geoh5py-0.9.0rc2/geoh5py/data/numeric_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/primitive_type_enum.py` & `geoh5py-0.9.0rc2/geoh5py/data/primitive_type_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/reference_value_map.py` & `geoh5py-0.9.0rc2/geoh5py/data/reference_value_map.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/referenced_data.py` & `geoh5py-0.9.0rc2/geoh5py/data/referenced_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/text_data.py` & `geoh5py-0.9.0rc2/geoh5py/data/text_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/unknown_data.py` & `geoh5py-0.9.0rc2/geoh5py/data/unknown_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/data/visual_parameters.py` & `geoh5py-0.9.0rc2/geoh5py/data/visual_parameters.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/container_group.py` & `geoh5py-0.9.0rc2/geoh5py/groups/container_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/custom_group.py` & `geoh5py-0.9.0rc2/geoh5py/groups/custom_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/drillhole_group.py` & `geoh5py-0.9.0rc2/geoh5py/groups/drillhole_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/giftools_group.py` & `geoh5py-0.9.0rc2/geoh5py/groups/giftools_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/group.py` & `geoh5py-0.9.0rc2/geoh5py/groups/group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/group_type.py` & `geoh5py-0.9.0rc2/geoh5py/groups/group_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/integrator_group.py` & `geoh5py-0.9.0rc2/geoh5py/groups/integrator_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/maps_group.py` & `geoh5py-0.9.0rc2/geoh5py/groups/maps_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/notype_group.py` & `geoh5py-0.9.0rc2/geoh5py/groups/notype_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/property_group.py` & `geoh5py-0.9.0rc2/geoh5py/groups/property_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/root_group.py` & `geoh5py-0.9.0rc2/geoh5py/groups/root_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/simpeg_group.py` & `geoh5py-0.9.0rc2/geoh5py/groups/simpeg_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/groups/survey_group.py` & `geoh5py-0.9.0rc2/geoh5py/groups/survey_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/io/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/io/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/io/h5_reader.py` & `geoh5py-0.9.0rc2/geoh5py/io/h5_reader.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/io/h5_writer.py` & `geoh5py-0.9.0rc2/geoh5py/io/h5_writer.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/block_model.py` & `geoh5py-0.9.0rc2/geoh5py/objects/block_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/cell_object.py` & `geoh5py-0.9.0rc2/geoh5py/objects/cell_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/curve.py` & `geoh5py-0.9.0rc2/geoh5py/objects/curve.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/drape_model.py` & `geoh5py-0.9.0rc2/geoh5py/objects/drape_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/drillhole.py` & `geoh5py-0.9.0rc2/geoh5py/objects/drillhole.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/geo_image.py` & `geoh5py-0.9.0rc2/geoh5py/objects/geo_image.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/grid2d.py` & `geoh5py-0.9.0rc2/geoh5py/objects/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/grid_object.py` & `geoh5py-0.9.0rc2/geoh5py/objects/grid_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/integrator.py` & `geoh5py-0.9.0rc2/geoh5py/objects/integrator.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/label.py` & `geoh5py-0.9.0rc2/geoh5py/objects/label.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/notype_object.py` & `geoh5py-0.9.0rc2/geoh5py/objects/notype_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/object_base.py` & `geoh5py-0.9.0rc2/geoh5py/objects/object_base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/object_type.py` & `geoh5py-0.9.0rc2/geoh5py/objects/object_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/octree.py` & `geoh5py-0.9.0rc2/geoh5py/objects/octree.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/points.py` & `geoh5py-0.9.0rc2/geoh5py/objects/points.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/surface.py` & `geoh5py-0.9.0rc2/geoh5py/objects/surface.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/surveys/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/objects/surveys/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/surveys/direct_current.py` & `geoh5py-0.9.0rc2/geoh5py/objects/surveys/direct_current.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/airborne_fem.py` & `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/airborne_fem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/airborne_tem.py` & `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/airborne_tem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/base.py` & `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/ground_fem.py` & `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/ground_fem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/ground_tem.py` & `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/ground_tem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py` & `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/surveys/electromagnetics/tipper.py` & `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/tipper.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/objects/surveys/magnetics.py` & `geoh5py-0.9.0rc2/geoh5py/objects/surveys/magnetics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/concatenation/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/concatenation/concatenated.py` & `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/concatenated.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/concatenation/concatenator.py` & `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/concatenator.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/concatenation/data.py` & `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/concatenation/drillhole.py` & `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/drillhole.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/concatenation/drillholes_group_table.py` & `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/drillholes_group_table.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/concatenation/object.py` & `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/concatenation/property_group.py` & `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/property_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/conversion/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/shared/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/conversion/base.py` & `geoh5py-0.9.0rc2/geoh5py/shared/conversion/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/conversion/geo_image.py` & `geoh5py-0.9.0rc2/geoh5py/shared/conversion/geo_image.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/conversion/grid2d.py` & `geoh5py-0.9.0rc2/geoh5py/shared/conversion/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/entity.py` & `geoh5py-0.9.0rc2/geoh5py/shared/entity.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/entity_container.py` & `geoh5py-0.9.0rc2/geoh5py/shared/entity_container.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/entity_type.py` & `geoh5py-0.9.0rc2/geoh5py/shared/entity_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/exceptions.py` & `geoh5py-0.9.0rc2/geoh5py/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/merging/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/shared/merging/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/merging/base.py` & `geoh5py-0.9.0rc2/geoh5py/shared/merging/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/merging/cell.py` & `geoh5py-0.9.0rc2/geoh5py/shared/merging/cell.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/merging/drape_model.py` & `geoh5py-0.9.0rc2/geoh5py/shared/merging/drape_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/merging/points.py` & `geoh5py-0.9.0rc2/geoh5py/shared/merging/points.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/utils.py` & `geoh5py-0.9.0rc2/geoh5py/shared/utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/validators.py` & `geoh5py-0.9.0rc2/geoh5py/shared/validators.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/shared/weakref_utils.py` & `geoh5py-0.9.0rc2/geoh5py/shared/weakref_utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/ui_json/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/ui_json/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/ui_json/constants.py` & `geoh5py-0.9.0rc2/geoh5py/ui_json/constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/ui_json/descriptors.py` & `geoh5py-0.9.0rc2/geoh5py/ui_json/descriptors.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/ui_json/enforcers.py` & `geoh5py-0.9.0rc2/geoh5py/ui_json/enforcers.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/ui_json/forms.py` & `geoh5py-0.9.0rc2/geoh5py/ui_json/forms.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/ui_json/input_file.py` & `geoh5py-0.9.0rc2/geoh5py/ui_json/input_file.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/ui_json/parameters.py` & `geoh5py-0.9.0rc2/geoh5py/ui_json/parameters.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/ui_json/templates.py` & `geoh5py-0.9.0rc2/geoh5py/ui_json/templates.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/ui_json/ui_json.py` & `geoh5py-0.9.0rc2/geoh5py/ui_json/ui_json.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/ui_json/utils.py` & `geoh5py-0.9.0rc2/geoh5py/ui_json/utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/ui_json/validation.py` & `geoh5py-0.9.0rc2/geoh5py/ui_json/validation.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/workspace/__init__.py` & `geoh5py-0.9.0rc2/geoh5py/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/geoh5py/workspace/workspace.py` & `geoh5py-0.9.0rc2/geoh5py/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/package.rst` & `geoh5py-0.9.0rc2/package.rst`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/pyproject.toml` & `geoh5py-0.9.0rc2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 [tool.poetry]
 name = "geoh5py"
-version = "0.9.0-rc.1"
+version = "0.9.0-rc.2"
 license = "LGPL-3.0-or-later"
 description = "Python API for geoh5, an open file format for geoscientific data"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/geoh5py"
-documentation = "https://geoh5py.readthedocs.io/en/latest/"
-homepage = "https://mirageoscience.com"
+maintainers = [
+    "Benjamin Kary <benjamink@mirageoscience.com>",
+    "Dominique Fournier <dominiquef@mirageoscience.com>",
+    "Matthieu Cedou <matthieuc@mirageoscience.com>",
+]
+documentation = "https://mirageoscience-geoh5py.readthedocs-hosted.com/"
+homepage = "https://www.mirageoscience.com/mining-industry-software/python-integration/"
 readme = "package.rst"
 keywords = ["geology", "geophysics", "data", "interoperability"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "Natural Language :: English",
@@ -28,15 +33,15 @@
     "COPYING.LESSER",
     "LICENSE",
     "README.rst",
     "THIRD_PARTY_SOFTWARE.rst",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.11"
+python = "^3.9,<3.11"
 
 h5py = "^3.2.1"
 numpy = "!=1.19.4, ~1.23.5"
 Pillow = "~10.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
@@ -50,20 +55,15 @@
 sphinx-autodoc-typehints = "^1.10"
 sphinx-rtd-theme = "^0.4.3"
 tomli = "*"
 
 [tool.poetry.extras]
 
 [tool.isort]
-# settings for compatibility between ``isort`` and ``black`` formatting
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-line_length = 88
+profile = "black"
 
 [tool.black]
 # defaults are just fine
 
 [tool.mypy]
 warn_unused_configs = true
 ignore_missing_imports = true
```

### Comparing `geoh5py-0.9.0rc1/README.rst` & `geoh5py-0.9.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/THIRD_PARTY_SOFTWARE.rst` & `geoh5py-0.9.0rc2/THIRD_PARTY_SOFTWARE.rst`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc1/PKG-INFO` & `geoh5py-0.9.0rc2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: geoh5py
-Version: 0.9.0rc1
+Version: 0.9.0rc2
 Summary: Python API for geoh5, an open file format for geoscientific data
-Home-page: https://mirageoscience.com
+Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: LGPL-3.0-or-later
 Keywords: geology,geophysics,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
-Requires-Python: >=3.8,<3.11
+Maintainer: Benjamin Kary
+Maintainer-email: benjamink@mirageoscience.com
+Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Pillow (>=10.1.0,<10.2.0)
 Requires-Dist: h5py (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
-Project-URL: Documentation, https://geoh5py.readthedocs.io/en/latest/
+Project-URL: Documentation, https://mirageoscience-geoh5py.readthedocs-hosted.com/
 Project-URL: Repository, https://github.com/MiraGeoscience/geoh5py
 Description-Content-Type: text/x-rst
 
 geoh5py: Python API for geoh5. An open file format for geoscientific data
 ==========================================================================
 
 The **geoh5py** library has been created for the manipulation and storage of a wide range of
```


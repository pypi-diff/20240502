# Comparing `tmp/spatialdata_plot-0.2.1.tar.gz` & `tmp/spatialdata_plot-0.2.2.tar.gz`

## Comparing `spatialdata_plot-0.2.1.tar` & `spatialdata_plot-0.2.2.tar`

### file list

```diff
@@ -1,149 +1,150 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/.codecov.yaml
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/.cruft.json
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/.editorconfig
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/.flake8
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/.mypy.ini
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/.readthedocs.yaml
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/_version.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/pyproject.toml.rej
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/.github/codecov.yml
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/.github/workflows/build.yaml
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/Makefile
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/changelog.md
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/conf.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/conf.py.rej
--rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/contributing.md
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/index.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/index.md.rej
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/plotting.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/preprocessing.rst
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/references.md
--rw-r--r--   0        0        0  1810880 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/spatialdata-plot.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/_static/.gitkeep
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/_static/css/custom.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0    15163 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/docs/notebooks/preprocessing.ipynb
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/src/spatialdata_plot/__init__.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/src/spatialdata_plot/_accessor.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/src/spatialdata_plot/_logging.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/src/spatialdata_plot/pl/__init__.py
--rw-r--r--   0        0        0    38047 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/src/spatialdata_plot/pl/basic.py
--rw-r--r--   0        0        0    31384 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/src/spatialdata_plot/pl/render.py
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/src/spatialdata_plot/pl/render_params.py
--rw-r--r--   0        0        0    74846 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/src/spatialdata_plot/pl/utils.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/src/spatialdata_plot/pp/__init__.py
--rw-r--r--   0        0        0    13041 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/src/spatialdata_plot/pp/basic.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/src/spatialdata_plot/pp/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0    16976 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/test_image.py
--rw-r--r--   0        0        0     5567 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/test_pp.py
--rw-r--r--   0        0        0    24002 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Extent_correct_plot_after_transformations.png
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Extent_extent_calculation_respects_element_selection_circles.png
--rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Extent_extent_calculation_respects_element_selection_circles_and_polygons.png
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Extent_extent_calculation_respects_element_selection_polygons.png
--rw-r--r--   0        0        0    38467 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Extent_extent_of_img_full_canvas.png
--rw-r--r--   0        0        0    32359 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Extent_extent_of_img_is_correct_after_spatial_query.png
--rw-r--r--   0        0        0    39864 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Extent_extent_of_partial_canvas_on_full_canvas.png
--rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Extent_extent_of_points_partial_canvas.png
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Extent_extent_of_polygons_is_correct_after_spatial_query.png
--rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Extent_extent_of_polygons_on_img_is_correct_after_spatial_query.png
--rw-r--r--   0        0        0    48839 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_do_rasterization.png
--rw-r--r--   0        0        0    44800 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_normalize_image.png
--rw-r--r--   0        0        0    32781 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_pass_cmap.png
--rw-r--r--   0        0        0    32593 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_pass_cmap_list.png
--rw-r--r--   0        0        0    32435 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_pass_cmap_to_each_channel.png
--rw-r--r--   0        0        0    27365 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_pass_cmap_to_single_channel.png
--rw-r--r--   0        0        0    36294 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_pass_color_to_each_channel.png
--rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_pass_color_to_single_channel.png
--rw-r--r--   0        0        0    32781 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_pass_str_cmap.png
--rw-r--r--   0        0        0    32593 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_pass_str_cmap_list.png
--rw-r--r--   0        0        0    26641 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_render_a_single_channel_from_image.png
--rw-r--r--   0        0        0    35235 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_render_given_scale_of_multiscale_image.png
--rw-r--r--   0        0        0    38467 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_render_image.png
--rw-r--r--   0        0        0    35384 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_render_multiscale_image.png
--rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_render_two_channels_from_image.png
--rw-r--r--   0        0        0    18929 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_stack_render_images.png
--rw-r--r--   0        0        0    50141 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Images_can_stop_rasterization_with_scale_full.png
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Labels_can_color_labels.png
--rw-r--r--   0        0        0    14178 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Labels_can_color_labels_by_continuous_variable.png
--rw-r--r--   0        0        0    39660 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Labels_can_do_rasterization.png
--rw-r--r--   0        0        0    15412 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Labels_can_render_given_scale_of_multiscale_labels.png
--rw-r--r--   0        0        0    14410 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Labels_can_render_labels.png
--rw-r--r--   0        0        0    12564 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Labels_can_render_multiscale_labels.png
--rw-r--r--   0        0        0    20535 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Labels_can_stack_render_labels.png
--rw-r--r--   0        0        0    37071 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Labels_can_stop_rasterization_with_scale_full.png
--rw-r--r--   0        0        0    17865 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Labels_label_categorical_color.png
--rw-r--r--   0        0        0    22746 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Labels_multiscale_label_categorical_color.png
--rw-r--r--   0        0        0    16629 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_affine.png
--rw-r--r--   0        0        0    17239 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_composition.png
--rw-r--r--   0        0        0    36378 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_inverse.png
--rw-r--r--   0        0        0    40028 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_mapaxis.png
--rw-r--r--   0        0        0    36378 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_overlay.png
--rw-r--r--   0        0        0    27226 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_rotation.png
--rw-r--r--   0        0        0    19966 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_scale.png
--rw-r--r--   0        0        0    44855 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_split.png
--rw-r--r--   0        0        0    25109 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_translation.png
--rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Points_can_filter_with_groups.png
--rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Points_can_render_points.png
--rw-r--r--   0        0        0    15262 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Points_can_stack_render_points.png
--rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Points_color_recognises_actual_color_as_color.png
--rw-r--r--   0        0        0    10913 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Points_coloring_with_cmap.png
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Points_coloring_with_palette.png
--rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Points_points_categorical_color.png
--rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Points_points_coercable_categorical_color.png
--rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_color_from_geodataframe.png
--rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_color_two_queried_shapes_elements_by_annotation.png
--rw-r--r--   0        0        0    10991 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_color_two_shapes_elements_by_annotation.png
--rw-r--r--   0        0        0     7641 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_filter_with_groups.png
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_plot_queried_with_annotation_despite_random_shuffling.png
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_plot_shapes_after_spatial_query.png
--rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_plot_with_annotation_despite_random_shuffling.png
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_circles.png
--rw-r--r--   0        0        0     8802 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_circles_with_colored_outline.png
--rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_circles_with_default_outline_width.png
--rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_circles_with_outline.png
--rw-r--r--   0        0        0    10042 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_circles_with_specified_outline_width.png
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_empty_geometry.png
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_multipolygons.png
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_polygons.png
--rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_polygons_with_outline.png
--rw-r--r--   0        0        0     7857 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_polygons_with_rgb_colored_outline.png
--rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_polygons_with_rgba_colored_outline.png
--rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_polygons_with_str_colored_outline.png
--rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_scale_shapes.png
--rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_can_stack_render_shapes.png
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_color_recognises_actual_color_as_color.png
--rw-r--r--   0        0        0     7772 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_colorbar_can_be_normalised.png
--rw-r--r--   0        0        0     8195 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_colorbar_respects_input_limits.png
--rw-r--r--   0        0        0     8980 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_coloring_with_palette.png
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_shapes_categorical_color.png
--rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Shapes_shapes_coercable_categorical_color.png
--rw-r--r--   0        0        0    22662 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Show_pad_extent_adds_padding.png
--rw-r--r--   0        0        0    40469 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Upstream_can_render_transformations_raccoon_mapaxis.png
--rw-r--r--   0        0        0    36658 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Upstream_can_render_transformations_raccoon_overlay.png
--rw-r--r--   0        0        0    20205 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/_images/Upstream_can_render_transformations_raccoon_scale.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/pl/__init__.py
--rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/pl/test_get_extent.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/pl/test_render.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/pl/test_render_images.py
--rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/pl/test_render_labels.py
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/pl/test_render_points.py
--rw-r--r--   0        0        0    14593 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/pl/test_render_shapes.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/pl/test_show.py
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/pl/test_upstream_plots.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/pl/test_utils.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/tests/pp/test_basic.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/LICENSE
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/README.md
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/.codecov.yaml
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/.cruft.json
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/.editorconfig
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/.flake8
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/.mypy.ini
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/_version.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/pyproject.toml.rej
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/.github/codecov.yml
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/Makefile
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/changelog.md
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/conf.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/conf.py.rej
+-rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/contributing.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/index.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/index.md.rej
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/plotting.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/preprocessing.rst
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/references.md
+-rw-r--r--   0        0        0  1810880 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/spatialdata-plot.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/_static/css/custom.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0    15163 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/docs/notebooks/preprocessing.ipynb
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/src/spatialdata_plot/__init__.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/src/spatialdata_plot/_accessor.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/src/spatialdata_plot/_logging.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/src/spatialdata_plot/pl/__init__.py
+-rw-r--r--   0        0        0    43287 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/src/spatialdata_plot/pl/basic.py
+-rw-r--r--   0        0        0    31650 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/src/spatialdata_plot/pl/render.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/src/spatialdata_plot/pl/render_params.py
+-rw-r--r--   0        0        0    79869 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/src/spatialdata_plot/pl/utils.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/src/spatialdata_plot/pp/__init__.py
+-rw-r--r--   0        0        0    13041 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/src/spatialdata_plot/pp/basic.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/src/spatialdata_plot/pp/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0    16928 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/test_image.py
+-rw-r--r--   0        0        0     5567 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/test_pp.py
+-rw-r--r--   0        0        0    24002 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Extent_correct_plot_after_transformations.png
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Extent_extent_calculation_respects_element_selection_circles.png
+-rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Extent_extent_calculation_respects_element_selection_circles_and_polygons.png
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Extent_extent_calculation_respects_element_selection_polygons.png
+-rw-r--r--   0        0        0    38467 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Extent_extent_of_img_full_canvas.png
+-rw-r--r--   0        0        0    32359 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Extent_extent_of_img_is_correct_after_spatial_query.png
+-rw-r--r--   0        0        0    39864 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Extent_extent_of_partial_canvas_on_full_canvas.png
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Extent_extent_of_points_partial_canvas.png
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Extent_extent_of_polygons_is_correct_after_spatial_query.png
+-rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Extent_extent_of_polygons_on_img_is_correct_after_spatial_query.png
+-rw-r--r--   0        0        0    48839 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_do_rasterization.png
+-rw-r--r--   0        0        0    44800 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_normalize_image.png
+-rw-r--r--   0        0        0    32781 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_pass_cmap.png
+-rw-r--r--   0        0        0    32593 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_pass_cmap_list.png
+-rw-r--r--   0        0        0    32435 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_pass_cmap_to_each_channel.png
+-rw-r--r--   0        0        0    27365 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_pass_cmap_to_single_channel.png
+-rw-r--r--   0        0        0    36294 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_pass_color_to_each_channel.png
+-rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_pass_color_to_single_channel.png
+-rw-r--r--   0        0        0    32781 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_pass_str_cmap.png
+-rw-r--r--   0        0        0    32593 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_pass_str_cmap_list.png
+-rw-r--r--   0        0        0    26641 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_render_a_single_channel_from_image.png
+-rw-r--r--   0        0        0    35235 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_render_given_scale_of_multiscale_image.png
+-rw-r--r--   0        0        0    38467 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_render_image.png
+-rw-r--r--   0        0        0    35384 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_render_multiscale_image.png
+-rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_render_two_channels_from_image.png
+-rw-r--r--   0        0        0    18929 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_stack_render_images.png
+-rw-r--r--   0        0        0    50141 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Images_can_stop_rasterization_with_scale_full.png
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Labels_can_color_labels.png
+-rw-r--r--   0        0        0    14178 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Labels_can_color_labels_by_continuous_variable.png
+-rw-r--r--   0        0        0    39660 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Labels_can_do_rasterization.png
+-rw-r--r--   0        0        0    15412 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Labels_can_render_given_scale_of_multiscale_labels.png
+-rw-r--r--   0        0        0    14410 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Labels_can_render_labels.png
+-rw-r--r--   0        0        0    12564 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Labels_can_render_multiscale_labels.png
+-rw-r--r--   0        0        0    20535 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Labels_can_stack_render_labels.png
+-rw-r--r--   0        0        0    37071 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Labels_can_stop_rasterization_with_scale_full.png
+-rw-r--r--   0        0        0    17865 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Labels_label_categorical_color.png
+-rw-r--r--   0        0        0    22746 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Labels_multiscale_label_categorical_color.png
+-rw-r--r--   0        0        0    16629 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_affine.png
+-rw-r--r--   0        0        0    17239 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_composition.png
+-rw-r--r--   0        0        0    36378 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_inverse.png
+-rw-r--r--   0        0        0    40028 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_mapaxis.png
+-rw-r--r--   0        0        0    36378 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_overlay.png
+-rw-r--r--   0        0        0    27226 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_rotation.png
+-rw-r--r--   0        0        0    19966 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_scale.png
+-rw-r--r--   0        0        0    44855 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_split.png
+-rw-r--r--   0        0        0    25109 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_translation.png
+-rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Points_can_filter_with_groups.png
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Points_can_filter_with_groups_default_palette.png
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Points_can_render_points.png
+-rw-r--r--   0        0        0    15262 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Points_can_stack_render_points.png
+-rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Points_color_recognises_actual_color_as_color.png
+-rw-r--r--   0        0        0    10913 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Points_coloring_with_cmap.png
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Points_coloring_with_palette.png
+-rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Points_points_categorical_color.png
+-rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Points_points_coercable_categorical_color.png
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_color_from_geodataframe.png
+-rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_color_two_queried_shapes_elements_by_annotation.png
+-rw-r--r--   0        0        0    10991 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_color_two_shapes_elements_by_annotation.png
+-rw-r--r--   0        0        0     7641 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_filter_with_groups.png
+-rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_plot_queried_with_annotation_despite_random_shuffling.png
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_plot_shapes_after_spatial_query.png
+-rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_plot_with_annotation_despite_random_shuffling.png
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_circles.png
+-rw-r--r--   0        0        0     8802 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_circles_with_colored_outline.png
+-rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_circles_with_default_outline_width.png
+-rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_circles_with_outline.png
+-rw-r--r--   0        0        0    10042 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_circles_with_specified_outline_width.png
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_empty_geometry.png
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_multipolygons.png
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_polygons.png
+-rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_polygons_with_outline.png
+-rw-r--r--   0        0        0     7857 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_polygons_with_rgb_colored_outline.png
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_polygons_with_rgba_colored_outline.png
+-rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_polygons_with_str_colored_outline.png
+-rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_scale_shapes.png
+-rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_can_stack_render_shapes.png
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_color_recognises_actual_color_as_color.png
+-rw-r--r--   0        0        0     7772 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_colorbar_can_be_normalised.png
+-rw-r--r--   0        0        0     8195 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_colorbar_respects_input_limits.png
+-rw-r--r--   0        0        0     8980 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_coloring_with_palette.png
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_shapes_categorical_color.png
+-rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Shapes_shapes_coercable_categorical_color.png
+-rw-r--r--   0        0        0    22662 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Show_pad_extent_adds_padding.png
+-rw-r--r--   0        0        0    40469 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Upstream_can_render_transformations_raccoon_mapaxis.png
+-rw-r--r--   0        0        0    36658 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Upstream_can_render_transformations_raccoon_overlay.png
+-rw-r--r--   0        0        0    20205 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/_images/Upstream_can_render_transformations_raccoon_scale.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/pl/__init__.py
+-rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/pl/test_get_extent.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/pl/test_render.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/pl/test_render_images.py
+-rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/pl/test_render_labels.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/pl/test_render_points.py
+-rw-r--r--   0        0        0    14593 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/pl/test_render_shapes.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/pl/test_show.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/pl/test_upstream_plots.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/pl/test_utils.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/tests/pp/test_basic.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/README.md
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6789 2020-02-02 00:00:00.000000 spatialdata_plot-0.2.2/PKG-INFO
```

### Comparing `spatialdata_plot-0.2.1/.cruft.json` & `spatialdata_plot-0.2.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/.flake8` & `spatialdata_plot-0.2.2/.flake8`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/.mypy.ini` & `spatialdata_plot-0.2.2/.mypy.ini`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/.pre-commit-config.yaml` & `spatialdata_plot-0.2.2/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -23,11 +23,11 @@
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.9.0
     hooks:
       - id: mypy
         additional_dependencies: [numpy, types-requests]
         exclude: tests/|docs/
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.4
+    rev: v0.3.5
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
```

### Comparing `spatialdata_plot-0.2.1/CHANGELOG.md` & `spatialdata_plot-0.2.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 
 The format is based on [Keep a Changelog][],
 and this project adheres to [Semantic Versioning][].
 
 [keep a changelog]: https://keepachangelog.com/en/1.0.0/
 [semantic versioning]: https://semver.org/spec/v2.0.0.html
 
+## [0.2.2] - 2024-05-02
+
+### Fixed
+
+-   Fixed `fill_alpha` ignoring `alpha` channel from custom cmap
+
+## [0.2.1] - 2024-03-26
+
+### Minor
+
+-   Adjusted GitHub worklows
+
 ## [0.2.0] - 2024-03-24
 
 ### Added
 
 -   Support for plotting multiple tables @melonora
 
 ### Fixed
```

### Comparing `spatialdata_plot-0.2.1/pyproject.toml.rej` & `spatialdata_plot-0.2.2/pyproject.toml.rej`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/.github/workflows/build.yaml` & `spatialdata_plot-0.2.2/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/.github/workflows/release.yaml` & `spatialdata_plot-0.2.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/.github/workflows/test.yaml` & `spatialdata_plot-0.2.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/docs/Makefile` & `spatialdata_plot-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/docs/conf.py` & `spatialdata_plot-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/docs/conf.py.rej` & `spatialdata_plot-0.2.2/docs/conf.py.rej`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/docs/contributing.md` & `spatialdata_plot-0.2.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/docs/references.bib` & `spatialdata_plot-0.2.2/docs/references.bib`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/docs/spatialdata-plot.png` & `spatialdata_plot-0.2.2/docs/spatialdata-plot.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/docs/_templates/autosummary/class.rst` & `spatialdata_plot-0.2.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/docs/extensions/typed_returns.py` & `spatialdata_plot-0.2.2/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/docs/notebooks/preprocessing.ipynb` & `spatialdata_plot-0.2.2/docs/notebooks/preprocessing.ipynb`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/src/spatialdata_plot/_accessor.py` & `spatialdata_plot-0.2.2/src/spatialdata_plot/_accessor.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/src/spatialdata_plot/_logging.py` & `spatialdata_plot-0.2.2/src/spatialdata_plot/_logging.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/src/spatialdata_plot/pl/basic.py` & `spatialdata_plot-0.2.2/src/spatialdata_plot/pl/basic.py`

 * *Files 17% similar despite different names*

```diff
@@ -146,18 +146,18 @@
         sdata.plotting_tree = self._sdata.plotting_tree if hasattr(self._sdata, "plotting_tree") else OrderedDict()
 
         return sdata
 
     def render_shapes(
         self,
         elements: list[str] | str | None = None,
-        color: str | None = None,
+        color: list[str | None] | str | None = None,
         fill_alpha: float | int = 1.0,
-        groups: list[list[str | None]] | list[str] | str | None = None,
-        palette: list[list[str | None]] | list[str] | str | None = None,
+        groups: list[list[str | None]] | list[str | None] | str | None = None,
+        palette: list[list[str | None]] | list[str | None] | str | None = None,
         na_color: ColorLike | None = "lightgrey",
         outline: bool = False,
         outline_width: float | int = 1.5,
         outline_color: str | list[float] = "#000000ff",
         outline_alpha: float | int = 1.0,
         cmap: Colormap | str | None = None,
         norm: bool | Normalize = False,
@@ -169,25 +169,37 @@
         Render shapes elements in SpatialData.
 
         Parameters
         ----------
         elements : list[str] | str | None, optional
             The name(s) of the shapes element(s) to render. If `None`, all shapes
             elements in the `SpatialData` object will be used.
-        color : Colorlike | str | None, optional
-            Can either be a color-like or a key in :attr:`sdata.table.obs`. The latter
-            can be used to color by categorical or continuous variables.
+        color : list[str | None] | str | None
+            Can either be string(s) representing a color-like or key(s) in :attr:`sdata.table.obs`. The latter
+            can be used to color by categorical or continuous variables. If provided as a list, the length of the list
+            must match the number of elements that will be plotted. Otherwise, if possible the color will be broadcasted
+            to all elements. For this, the table in which the color key is found must
+            annotate the respective element (region must be set to the specific element). If the color column is found
+            in multiple locations, please provide the table_name to be used for the element.
         fill_alpha : float | int, default 1.0
-            Alpha value for the fill of shapes.
-        groups : list[str] | str | None, optional
+            Alpha value for the fill of shapes. If the alpha channel is present in a cmap passed by the
+            user, this value will multiply the value present in the cmap.
+        groups : list[list[str | None]] | list[str | None] | str | None
             When using `color` and the key represents discrete labels, `groups`
-            can be used to show only a subset of them. Other values are set to NA.
-        palette : list[str] | str | None, optional
+            can be used to show only a subset of them. Other values are set to NA. In general the case of a list of
+            lists means that there is one list per element to be plotted in the list and this list can contain multiple
+            discrete labels to be visualized. If not provided as list of lists, broadcasting behaviour is attempted
+            (use the same values for all elements).
+        palette : list[list[str | None]] | list[str | None] | str | None
             Palette for discrete annotations. List of valid color names that should be
-            used for the categories. Must match the number of groups.
+            used for the categories. Must match the number of groups. Similarly to groups, in the case of a list of
+            lists means that there is one list per element to be plotted in the list and this list can contain multiple
+            palettes (one per group) to be visualized. If not provided as list of lists, broadcasting behaviour is
+            attempted (use the same values for all elements). If groups is provided but not palette, palette is set to
+            default "lightgray".
         na_color : str | list[float] | None, default "lightgrey"
             Color to be used for NAs values, if present. Can either be a named color
             ("red"), a hex representation ("#000000ff") or a list of floats that
             represent RGB/RGBA values (1.0, 0.0, 0.0, 1.0). When None, the values won't
             be shown.
         outline : bool, default False
             If `True`, a border around the shape elements is plotted.
@@ -268,18 +280,18 @@
         )
 
         return sdata
 
     def render_points(
         self,
         elements: list[str] | str | None = None,
-        color: list[str] | str | None = None,
+        color: list[str | None] | str | None = None,
         alpha: float | int = 1.0,
-        groups: list[list[str | None]] | list[str] | str | None = None,
-        palette: list[list[str | None]] | list[str] | str | None = None,
+        groups: list[list[str | None]] | list[str | None] | str | None = None,
+        palette: list[list[str | None]] | list[str | None] | str | None = None,
         na_color: ColorLike | None = "lightgrey",
         cmap: Colormap | str | None = None,
         norm: None | Normalize = None,
         size: float | int = 1.0,
         table_name: list[str] | str | None = None,
         **kwargs: Any,
     ) -> sd.SpatialData:
@@ -287,25 +299,36 @@
         Render points elements in SpatialData.
 
         Parameters
         ----------
         elements : list[str] | str | None, optional
             The name(s) of the points element(s) to render. If `None`, all points
             elements in the `SpatialData` object will be used.
-        color : Colorlike | str | None, optional
-            Can either be a color-like or a key in :attr:`sdata.table.obs`. The latter
-            can be used to color by categorical or continuous variables.
+        color : list[str | None] | str | None
+            Can either be string(s) representing a color-like or key(s) in :attr:`sdata.table.obs`. The latter
+            can be used to color by categorical or continuous variables. If provided as a list, the length of the list
+            must match the number of elements that will be plotted. Otherwise, if possible the color will be broadcasted
+            to all elements. For this, the table in which the color key is found must
+            annotate the respective element (region must be set to the specific element). If the color column is found
+            in multiple locations, please provide the table_name to be used for the element.
         alpha : float | int, default 1.0
             Alpha value for the points.
-        groups : list[str] | str | None, optional
+        groups : list[list[str | None]] | list[str | None] | str | None
             When using `color` and the key represents discrete labels, `groups`
-            can be used to show only a subset of them. Other values are set to NA.
-        palette : list[str] | str | None, optional
+            can be used to show only a subset of them. Other values are set to NA. In general the case of a list of
+            lists means that there is one list per element to be plotted in the list and this list can contain multiple
+            discrete labels to be visualized. If not provided as list of lists, broadcasting behaviour is attempted
+            (use the same values for all elements). If groups is provided but not palette, palette is set to
+            default "lightgray".
+        palette : list[list[str | None]] | list[str | None] | str | None
             Palette for discrete annotations. List of valid color names that should be
-            used for the categories. Must match the number of groups.
+            used for the categories. Must match the number of groups. Similarly to groups, in the case of a list of
+            lists means that there is one list per element to be plotted in the list and this list can contain multiple
+            palettes (one per group) to be visualized. If not provided as list of lists, broadcasting behaviour is
+            attempted (use the same values for all elements).
         na_color : str | list[float] | None, default "lightgrey"
             Color to be used for NAs values, if present. Can either be a named color
             ("red"), a hex representation ("#000000ff") or a list of floats that
             represent RGB/RGBA values (1.0, 0.0, 0.0, 1.0). When None, the values won't
             be shown.
         cmap : Colormap | str | None, optional
             Colormap for discrete or continuous annotations using 'color', see
@@ -370,15 +393,15 @@
     def render_images(
         self,
         elements: list[str] | str | None = None,
         channel: list[str] | list[int] | str | int | None = None,
         cmap: list[Colormap] | Colormap | str | None = None,
         norm: Normalize | None = None,
         na_color: ColorLike | None = (0.0, 0.0, 0.0, 0.0),
-        palette: list[str] | str | None = None,
+        palette: list[list[str | None]] | list[str | None] | str | None = None,
         alpha: float | int = 1.0,
         quantiles_for_norm: tuple[float | None, float | None] | None = None,
         scale: list[str] | str | None = None,
         **kwargs: Any,
     ) -> sd.SpatialData:
         """
         Render image elements in SpatialData.
@@ -396,14 +419,19 @@
             Colormap or list of colormaps for continuous annotations, see :class:`matplotlib.colors.Colormap`.
             Each colormap applies to a corresponding channel.
         norm : Normalize | None, optional
             Colormap normalization for continuous annotations, see :class:`matplotlib.colors.Normalize`.
             Applies to all channels if set.
         na_color : ColorLike | None, default (0.0, 0.0, 0.0, 0.0)
             Color to be used for NA values. Accepts color-like values (string, hex, RGB(A)).
+        palette : list[list[str | None]] | list[str | None] | str | None
+            Palette to color images. In the case of a list of
+            lists means that there is one list per element to be plotted in the list and this list contains the string
+            indicating the palette to be used. If not provided as list of lists, broadcasting behaviour is
+            attempted (use the same values for all elements).
         alpha : float | int, default 1.0
             Alpha value for the images. Must be a numeric between 0 and 1.
         quantiles_for_norm : tuple[float | None, float | None] | None, optional
             Optional pair of floats (pmin < pmax, 0-100) which will be used for quantile normalization.
         scale : list[str] | str | None, optional
             Influences the resolution of the rendering. Possibilities include:
                 1) `None` (default): The image is rasterized to fit the canvas size. For
@@ -471,19 +499,19 @@
         )
 
         return sdata
 
     def render_labels(
         self,
         elements: list[str] | str | None = None,
-        color: list[str] | str | None = None,
-        groups: list[list[str | None]] | list[str] | str | None = None,
+        color: list[str | None] | str | None = None,
+        groups: list[list[str | None]] | list[str | None] | str | None = None,
         contour_px: int = 3,
         outline: bool = False,
-        palette: list[list[str | None]] | list[str] | str | None = None,
+        palette: list[list[str | None]] | list[str | None] | str | None = None,
         cmap: Colormap | str | None = None,
         norm: Normalize | None = None,
         na_color: ColorLike | None = (0.0, 0.0, 0.0, 0.0),
         outline_alpha: float | int = 1.0,
         fill_alpha: float | int = 0.3,
         scale: list[str] | str | None = None,
         table_name: list[str] | str | None = None,
@@ -493,27 +521,39 @@
         Render labels elements in SpatialData.
 
         Parameters
         ----------
         elements : list[str] | str | None, optional
             The name(s) of the label element(s) to render. If `None`, all label
             elements in the `SpatialData` object will be used.
-        color : str | None, optional
-            Key for annotations in :attr:`anndata.AnnData.obs` or variables/genes.
-        groups : list[str] | str | None, optional
+        color : list[str | None] | str | None
+            Can either be string(s) representing a color-like or key(s) in :attr:`sdata.table.obs`. The latter
+            can be used to color by categorical or continuous variables. If provided as a list, the length of the list
+            must match the number of elements that will be plotted. Otherwise, if possible the color will be broadcasted
+            to all elements. For this, the table in which the color key is found must
+            annotate the respective element (region must be set to the specific element). If the color column is found
+            in multiple locations, please provide the table_name to be used for the element.
+        groups : list[list[str | None]] | list[str | None] | str | None
             When using `color` and the key represents discrete labels, `groups`
-            can be used to show only a subset of them. Other values are set to NA.
+            can be used to show only a subset of them. Other values are set to NA. In general the case of a list of
+            lists means that there is one list per element to be plotted in the list and this list can contain multiple
+            discrete labels to be visualized. If not provided as list of lists, broadcasting behaviour is attempted
+            (use the same values for all elements).
+        palette : list[list[str | None]] | list[str | None] | str | None
+            Palette for discrete annotations. List of valid color names that should be
+            used for the categories. Must match the number of groups. Similarly to groups, in the case of a list of
+            lists means that there is one list per element to be plotted in the list and this list can contain multiple
+            palettes (one per group) to be visualized. If not provided as list of lists, broadcasting behaviour is
+            attempted (use the same values for all elements). If groups is provided but not palette, palette is set to
+            default "lightgray".
         contour_px : int, default 3
             Draw contour of specified width for each segment. If `None`, fills
             entire segment, see :func:`skimage.morphology.erosion`.
         outline : bool, default False
             Whether to plot boundaries around segmentation masks.
-        palette : list[str] | str | None, optional
-            Palette for discrete annotations. List of valid color names that should be
-            used for the categories. Must match the number of groups.
         cmap : Colormap | str | None, optional
             Colormap for continuous annotations, see :class:`matplotlib.colors.Colormap`.
         norm : Normalize | None, optional
             Colormap normalization for continuous annotations, see :class:`matplotlib.colors.Normalize`.
         na_color : ColorLike | None, optional
             Color to be used for NAs values, if present.
         outline_alpha : float | int, default 1.0
@@ -525,14 +565,18 @@
                 1) None (default). The image is rasterized to fit the canvas size. For multiscale images, the best scale
                 is selected before the rasterization step.
                 2) Name of one of the scales in the multiscale image to be rendered. This scale is rendered as it is
                 (exception: a dpi is specified in `show()`. Then the image is rasterized to fit the canvas and dpi).
                 3) "full": render the full image without rasterization. In the case of a multiscale image, the scale
                 with the highest resolution is selected. This can lead to long computing times for large images!
                 4) List that is matched to the list of elements (can contain `None`, scale names or "full").
+        table_name:
+            Name of the table(s) containing the color(s) columns. If one name is given than the table is used for each
+            spatial element to be plotted if the table annotates it. If multiple names are given in a list than the
+            length must be equal to the number of spatial elements being plotted.
         kwargs
             Additional arguments to be passed to cmap and norm.
 
         Returns
         -------
         None
         """
@@ -558,14 +602,15 @@
         n_steps = len(sdata.plotting_tree.keys())
         cmap_params = _prepare_cmap_norm(
             cmap=cmap,
             norm=norm,
             na_color=na_color,  # type: ignore[arg-type]
             **kwargs,
         )
+
         sdata.plotting_tree[f"{n_steps+1}_render_labels"] = LabelsRenderParams(
             elements=params_dict["elements"],
             color=params_dict["color"],
             groups=params_dict["groups"],
             contour_px=contour_px,
             outline=outline,
             cmap_params=cmap_params,
@@ -618,14 +663,20 @@
             Resolution of the plot in dots per inch (as in matplotlib).
             If None, the default of matplotlib is used (100.0).
         ax :
             Matplotlib axes object to plot on. If None, a new figure is created.
             Works only if there is one image in the SpatialData object.
         ncols :
             Number of columns in the figure. Default is 4.
+        return_ax :
+            Whether to return the axes object created. False by default.
+        colorbar :
+            Whether to plot the colorbar. True by default.
+        title :
+            The title of the plot. If not provided the plot will have the name of the coordinate system as title.
 
         Returns
         -------
         sd.SpatialData
             A SpatialData object.
         """
         # copy the SpatialData object so we don't modify the original
```

### Comparing `spatialdata_plot-0.2.1/src/spatialdata_plot/pl/render.py` & `spatialdata_plot-0.2.2/src/spatialdata_plot/pl/render.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     _get_linear_colormap,
     _is_coercable_to_float,
     _map_color_seg,
     _maybe_set_colors,
     _multiscale_to_spatial_image,
     _normalize,
     _rasterize_if_necessary,
+    _return_list_list_str_none,
+    _return_list_str_none,
     _set_color_source_vec,
     to_hex,
 )
 
 _Normalize = Union[Normalize, abc.Sequence[Normalize]]
 
 
@@ -58,25 +60,30 @@
     ax: matplotlib.axes.SubplotBase,
     fig_params: FigParams,
     scalebar_params: ScalebarParams,
     legend_params: LegendParams,
 ) -> None:
     elements = render_params.elements
     element_table_mapping = render_params.element_table_mapping
+    cols_for_color = _return_list_str_none(render_params.col_for_color)
+    colors = _return_list_str_none(render_params.color)
+    groups = _return_list_list_str_none(render_params.groups)
+    palettes = _return_list_list_str_none(render_params.palette)
 
+    assert isinstance(element_table_mapping, dict)
     sdata_filt = sdata.filter_by_coordinate_system(
         coordinate_system=coordinate_system,
         filter_tables=any(value is not None for value in element_table_mapping.values()),
     )
 
     if elements is None:
         elements = list(sdata_filt.shapes.keys())
 
     for index, e in enumerate(elements):
-        col_for_color = render_params.col_for_color[index]
+        col_for_color = cols_for_color[index]
         shapes = sdata.shapes[e]
 
         table_name = element_table_mapping.get(e)
         if table_name is None:
             table = None
         else:
             _, region_key, _ = get_table_keys(sdata[table_name])
@@ -100,21 +107,21 @@
         # get color vector (categorical or continuous)
         color_source_vector, color_vector, _ = _set_color_source_vec(
             sdata=sdata_filt,
             element=sdata_filt.shapes[e],
             element_index=index,
             element_name=e,
             value_to_plot=col_for_color,
-            groups=render_params.groups[index] if render_params.groups[index][0] is not None else None,
+            groups=groups[index] if groups[index][0] is not None else None,
             palette=(
-                render_params.palette[index] if render_params.palette is not None else None
+                palettes[index] if palettes is not None else None
             ),  # and render_params.palette[index][0] is not None
-            na_color=render_params.color[index] or render_params.cmap_params.na_color,
+            na_color=colors[index] or render_params.cmap_params.na_color,
             cmap_params=render_params.cmap_params,
-            table_name=table_name,
+            table_name=cast(str, table_name),
         )
 
         values_are_categorical = color_source_vector is not None
 
         # color_source_vector is None when the values aren't categorical
         if values_are_categorical and render_params.transfunc is not None:
             color_vector = render_params.transfunc(color_vector)
@@ -122,20 +129,16 @@
         norm = copy(render_params.cmap_params.norm)
 
         if len(color_vector) == 0:
             color_vector = [render_params.cmap_params.na_color]
 
         # filter by `groups`
 
-        if (
-            isinstance(render_params.groups, list)
-            and render_params.groups[index][0] is not None
-            and color_source_vector is not None
-        ):
-            mask = color_source_vector.isin(render_params.groups[index])
+        if isinstance(groups, list) and groups[index][0] is not None and color_source_vector is not None:
+            mask = color_source_vector.isin(groups[index])
             shapes = shapes[mask]
             shapes = shapes.reset_index()
             color_source_vector = color_source_vector[mask]
             color_vector = color_vector[mask]
         shapes = gpd.GeoDataFrame(shapes, geometry="geometry")
 
         _cax = _get_collection_shape(
@@ -173,19 +176,19 @@
         else:
             palette = ListedColormap(dict.fromkeys(color_vector[~pd.Categorical(color_source_vector).isnull()]))
 
         if not (
             len(set(color_vector)) == 1 and list(set(color_vector))[0] == to_hex(render_params.cmap_params.na_color)
         ):
             # necessary in case different shapes elements are annotated with one table
-            if color_source_vector is not None and render_params.col_for_color[index] is not None:
+            if color_source_vector is not None and col_for_color is not None:
                 color_source_vector = color_source_vector.remove_unused_categories()
 
             # False if user specified color-like with 'color' parameter
-            colorbar = False if render_params.col_for_color[index] is None else legend_params.colorbar
+            colorbar = False if cols_for_color[index] is None else legend_params.colorbar
 
             _ = _decorate_axs(
                 ax=ax,
                 cax=cax,
                 fig_params=fig_params,
                 adata=table,
                 value_to_plot=col_for_color,
@@ -211,30 +214,36 @@
     ax: matplotlib.axes.SubplotBase,
     fig_params: FigParams,
     scalebar_params: ScalebarParams,
     legend_params: LegendParams,
 ) -> None:
     elements = render_params.elements
     element_table_mapping = render_params.element_table_mapping
+    cols_for_color = _return_list_str_none(render_params.col_for_color)
+    groups = _return_list_list_str_none(render_params.groups)
+    palettes = _return_list_list_str_none(render_params.palette)
+    colors = _return_list_str_none(render_params.color)
+    # Purely for mypy
+    assert isinstance(element_table_mapping, dict)
 
     sdata_filt = sdata.filter_by_coordinate_system(
         coordinate_system=coordinate_system,
         filter_tables=any(value is not None for value in element_table_mapping.values()),
     )
 
     if elements is None:
         elements = list(sdata_filt.points.keys())
 
     for index, e in enumerate(elements):
         points = sdata.points[e]
-        col_for_color = render_params.col_for_color[index]
+        col_for_color = cols_for_color[index]
         table_name = element_table_mapping.get(e)
 
         coords = ["x", "y"]
-        # if col_for_color is not None:
+
         if (
             col_for_color is not None
             and col_for_color not in points.columns
             and col_for_color not in sdata_filt[table_name].obs.columns
         ):
             # no error in case there are multiple elements, but onyl some have color key
             msg = f"Color key '{col_for_color}' for element '{e}' not been found, using default colors."
@@ -253,16 +262,16 @@
                     stacklevel=2,
                 )
                 sdata_filt[table_name].obs[col_for_color] = sdata_filt[table_name].obs[col_for_color].astype("category")
         else:
             coords += [col_for_color]
             points = points[coords].compute()
 
-        if render_params.groups[index][0] is not None and col_for_color is not None:
-            points = points[points[col_for_color].isin(render_params.groups[index])]
+        if groups[index][0] is not None and col_for_color is not None:
+            points = points[points[col_for_color].isin(groups[index])]
 
         # we construct an anndata to hack the plotting functions
         if table_name is None:
             adata = AnnData(
                 X=points[["x", "y"]].values, obs=points[coords].reset_index(), dtype=points[["x", "y"]].values.dtype
             )
         else:
@@ -281,32 +290,30 @@
             cols = sc.get.obs_df(adata, col_for_color)
             # maybe set color based on type
             if isinstance(cols.dtype, pd.CategoricalDtype):
                 _maybe_set_colors(
                     source=adata,
                     target=adata,
                     key=col_for_color,
-                    palette=render_params.palette[index] if render_params.palette[index][0] is not None else None,
+                    palette=palettes[index] if palettes[index][0] is not None else None,
                 )
 
         # when user specified a single color, we overwrite na with it
         default_color = (
-            render_params.color[index]
-            if col_for_color is None and render_params.color[index] is not None
-            else render_params.cmap_params.na_color
+            colors[index] if col_for_color is None and colors[index] is not None else render_params.cmap_params.na_color
         )
 
         color_source_vector, color_vector, _ = _set_color_source_vec(
             sdata=sdata_filt,
             element=points,
             element_index=index,
             element_name=e,
-            value_to_plot=render_params.col_for_color[index],
-            groups=render_params.groups[index] if render_params.groups[index][0] is not None else None,
-            palette=render_params.palette[index] if render_params.palette[index][0] is not None else None,
+            value_to_plot=col_for_color,
+            groups=groups[index] if groups[index][0] is not None else None,
+            palette=palettes[index] if palettes[index][0] is not None else None,
             na_color=default_color,
             cmap_params=render_params.cmap_params,
             table_name=cast(str, table_name),
         )
 
         # color_source_vector is None when the values aren't categorical
         if color_source_vector is None and render_params.transfunc is not None:
@@ -323,30 +330,29 @@
             s=render_params.size,
             c=color_vector,
             rasterized=sc_settings._vector_friendly,
             cmap=render_params.cmap_params.cmap,
             norm=norm,
             alpha=render_params.alpha,
             transform=trans,
-            # **kwargs,
         )
         cax = ax.add_collection(_cax)
 
         if len(set(color_vector)) != 1 or list(set(color_vector))[0] != to_hex(render_params.cmap_params.na_color):
             if color_source_vector is None:
                 palette = ListedColormap(dict.fromkeys(color_vector))
             else:
                 palette = ListedColormap(dict.fromkeys(color_vector[~pd.Categorical(color_source_vector).isnull()]))
 
             _ = _decorate_axs(
                 ax=ax,
                 cax=cax,
                 fig_params=fig_params,
                 adata=adata,
-                value_to_plot=render_params.col_for_color,
+                value_to_plot=col_for_color,
                 color_source_vector=color_source_vector,
                 palette=palette,
                 alpha=render_params.alpha,
                 na_color=render_params.cmap_params.na_color,
                 legend_fontsize=legend_params.legend_fontsize,
                 legend_fontweight=legend_params.legend_fontweight,
                 legend_loc=legend_params.legend_loc,
@@ -365,14 +371,15 @@
     ax: matplotlib.axes.SubplotBase,
     fig_params: FigParams,
     scalebar_params: ScalebarParams,
     legend_params: LegendParams,
     rasterize: bool,
 ) -> None:
     elements = render_params.elements
+    palettes = _return_list_list_str_none(render_params.palette)
 
     sdata_filt = sdata.filter_by_coordinate_system(
         coordinate_system=coordinate_system,
         filter_tables=False,
     )
 
     if elements is None:
@@ -441,19 +448,19 @@
                 layer = _normalize(
                     layer, pmin=render_params.quantiles_for_norm[0], pmax=render_params.quantiles_for_norm[1], clip=True
                 )
 
             if render_params.cmap_params.norm is not None:  # type: ignore[attr-defined]
                 layer = render_params.cmap_params.norm(layer)  # type: ignore[attr-defined]
 
-            if isinstance(render_params.palette, list):
-                if render_params.palette[i][0] is None:
+            if isinstance(palettes, list):
+                if palettes[i][0] is None:
                     cmap = render_params.cmap_params.cmap  # type: ignore[attr-defined]
                 else:
-                    cmap = _get_linear_colormap(render_params.palette[i], "k")[0]  # type: ignore[arg-type]
+                    cmap = _get_linear_colormap(palettes[i], "k")[0]  # type: ignore[arg-type]
 
             # Overwrite alpha in cmap: https://stackoverflow.com/a/10127675
             cmap._init()
             cmap._lut[:, -1] = render_params.alpha
 
             im = ax.imshow(
                 layer,
@@ -479,20 +486,16 @@
                     if render_params.cmap_params.norm is not None:
                         layers[c] = render_params.cmap_params.norm(layers[c])
                 else:
                     if render_params.cmap_params[ch_index].norm is not None:
                         layers[c] = render_params.cmap_params[ch_index].norm(layers[c])
 
             # 2A) Image has 3 channels, no palette info, and no/only one cmap was given
-            if isinstance(render_params.palette, list):
-                if (
-                    n_channels == 3
-                    and render_params.palette[i][0] is None
-                    and not isinstance(render_params.cmap_params, list)
-                ):
+            if isinstance(palettes, list):
+                if n_channels == 3 and palettes[i][0] is None and not isinstance(render_params.cmap_params, list):
                     if render_params.cmap_params.is_default:  # -> use RGB
                         stacked = np.stack([layers[c] for c in channels], axis=-1)
                     else:  # -> use given cmap for each channel
                         channel_cmaps = [render_params.cmap_params.cmap] * n_channels
                         # Apply cmaps to each channel, add up and normalize to [0, 1]
                         stacked = (
                             np.stack([channel_cmaps[ind](layers[ch]) for ind, ch in enumerate(channels)], 0).sum(0)
@@ -512,15 +515,15 @@
                     im = ax.imshow(
                         stacked,
                         alpha=render_params.alpha,
                     )
                     im.set_transform(trans_data)
 
                 # 2B) Image has n channels, no palette/cmap info -> sample n categorical colors
-                elif render_params.palette[i][0] is None and not got_multiple_cmaps:
+                elif palettes[i][0] is None and not got_multiple_cmaps:
                     # overwrite if n_channels == 2 for intuitive result
                     if n_channels == 2:
                         seed_colors = ["#ff0000ff", "#00ff00ff"]
                     else:
                         seed_colors = _get_colors_for_categorical_obs(list(range(n_channels)))
 
                     channel_cmaps = [_get_linear_colormap([c], "k")[0] for c in seed_colors]
@@ -534,33 +537,33 @@
                     im = ax.imshow(
                         colored,
                         alpha=render_params.alpha,
                     )
                     im.set_transform(trans_data)
 
                 # 2C) Image has n channels and palette info
-                elif render_params.palette[i][0] is not None and not got_multiple_cmaps:
-                    if len(render_params.palette[i]) != n_channels:
+                elif palettes[i][0] is not None and not got_multiple_cmaps:
+                    if len(palettes[i]) != n_channels:
                         raise ValueError("If 'palette' is provided, its length must match the number of channels.")
 
-                    channel_cmaps = [_get_linear_colormap([c], "k")[0] for c in render_params.palette[i]]
+                    channel_cmaps = [_get_linear_colormap([c], "k")[0] for c in palettes[i] if isinstance(c, str)]
 
                     # Apply cmaps to each channel and add up
                     colored = np.stack([channel_cmaps[i](layers[c]) for i, c in enumerate(channels)], 0).sum(0)
 
                     # Remove alpha channel so we can overwrite it from render_params.alpha
                     colored = colored[:, :, :3]
 
                     im = ax.imshow(
                         colored,
                         alpha=render_params.alpha,
                     )
                     im.set_transform(trans_data)
 
-                elif render_params.palette[i][0] is None and got_multiple_cmaps:
+                elif palettes[i][0] is None and got_multiple_cmaps:
                     channel_cmaps = [cp.cmap for cp in render_params.cmap_params]  # type: ignore[union-attr]
 
                     # Apply cmaps to each channel, add up and normalize to [0, 1]
                     colored = (
                         np.stack([channel_cmaps[ind](layers[ch]) for ind, ch in enumerate(channels)], 0).sum(0)
                         / n_channels
                     )
@@ -570,15 +573,15 @@
 
                     im = ax.imshow(
                         colored,
                         alpha=render_params.alpha,
                     )
                     im.set_transform(trans_data)
 
-                elif render_params.palette[i][0] is not None and got_multiple_cmaps:
+                elif palettes[i][0] is not None and got_multiple_cmaps:
                     raise ValueError("If 'palette' is provided, 'cmap' must be None.")
 
 
 def _render_labels(
     sdata: sd.SpatialData,
     render_params: LabelsRenderParams,
     coordinate_system: str,
@@ -586,14 +589,17 @@
     fig_params: FigParams,
     scalebar_params: ScalebarParams,
     legend_params: LegendParams,
     rasterize: bool,
 ) -> None:
     elements = render_params.elements
     element_table_mapping = cast(dict[str, str], render_params.element_table_mapping)
+    palettes = _return_list_list_str_none(render_params.palette)
+    colors = _return_list_str_none(render_params.color)
+    groups = _return_list_list_str_none(render_params.groups)
 
     if render_params.outline is False:
         render_params.outline_alpha = 0
 
     sdata_filt = sdata.filter_by_coordinate_system(
         coordinate_system=coordinate_system,
         filter_tables=any(value is not None for value in element_table_mapping.values()),
@@ -602,15 +608,15 @@
     if elements is None:
         elements = list(sdata_filt.labels.keys())
 
     for i, e in enumerate(elements):
         label = sdata_filt.labels[e]
         extent = get_extent(label, coordinate_system=coordinate_system)
         scale = render_params.scale[i] if isinstance(render_params.scale, list) else render_params.scale
-        color = render_params.color[i]
+        color = colors[i]
 
         # get best scale out of multiscale label
         if isinstance(label, MultiscaleSpatialImage):
             label = _multiscale_to_spatial_image(
                 multiscale_image=label,
                 dpi=fig_params.fig.dpi,
                 width=fig_params.fig.get_size_inches()[0],
@@ -647,16 +653,16 @@
 
         color_source_vector, color_vector, categorical = _set_color_source_vec(
             sdata=sdata_filt,
             element=label,
             element_index=i,
             element_name=e,
             value_to_plot=color,
-            groups=render_params.groups[i],
-            palette=render_params.palette[i],
+            groups=groups[i],  # if isinstance(groups, list) else None,
+            palette=palettes[i],
             na_color=render_params.cmap_params.na_color,
             cmap_params=render_params.cmap_params,
             table_name=cast(str, table_name),
         )
 
         if (render_params.fill_alpha != render_params.outline_alpha) and render_params.contour_px is not None:
             # First get the labels infill and plot them
@@ -667,25 +673,14 @@
                 color_source_vector=color_source_vector,
                 cmap_params=render_params.cmap_params,
                 seg_erosionpx=None,
                 seg_boundaries=render_params.outline,
                 na_color=render_params.cmap_params.na_color,
             )
 
-            _cax = ax.imshow(
-                labels_infill,
-                rasterized=True,
-                cmap=None if categorical else render_params.cmap_params.cmap,
-                norm=None if categorical else render_params.cmap_params.norm,
-                alpha=render_params.fill_alpha,
-                origin="lower",
-            )
-            _cax.set_transform(trans_data)
-            cax = ax.add_image(_cax)
-
             # Then overlay the contour
             labels_contour = _map_color_seg(
                 seg=label.values,
                 cell_id=instance_id,
                 color_vector=color_vector,
                 color_source_vector=color_source_vector,
                 cmap_params=render_params.cmap_params,
@@ -698,14 +693,24 @@
                 labels_contour,
                 rasterized=True,
                 cmap=None if categorical else render_params.cmap_params.cmap,
                 norm=None if categorical else render_params.cmap_params.norm,
                 alpha=render_params.outline_alpha,
                 origin="lower",
             )
+            _cax = ax.imshow(
+                labels_infill,
+                rasterized=True,
+                cmap=None if categorical else render_params.cmap_params.cmap,
+                norm=None if categorical else render_params.cmap_params.norm,
+                alpha=render_params.fill_alpha,
+                origin="lower",
+            )
+            _cax.set_transform(trans_data)
+            cax = ax.add_image(_cax)
         else:
             # Default: no alpha, contour = infill
             label = _map_color_seg(
                 seg=label.values,
                 cell_id=instance_id,
                 color_vector=color_vector,
                 color_source_vector=color_source_vector,
@@ -729,15 +734,15 @@
         _ = _decorate_axs(
             ax=ax,
             cax=cax,
             fig_params=fig_params,
             adata=table,
             value_to_plot=color,
             color_source_vector=color_source_vector,
-            palette=render_params.palette[i],
+            palette=palettes[i],
             alpha=render_params.fill_alpha,
             na_color=render_params.cmap_params.na_color,
             legend_fontsize=legend_params.legend_fontsize,
             legend_fontweight=legend_params.legend_fontweight,
             legend_loc=legend_params.legend_loc,
             legend_fontoutline=legend_params.legend_fontoutline,
             na_in_legend=legend_params.na_in_legend,
```

### Comparing `spatialdata_plot-0.2.1/src/spatialdata_plot/pl/render_params.py` & `spatialdata_plot-0.2.2/src/spatialdata_plot/pl/render_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -67,64 +67,64 @@
 @dataclass
 class ShapesRenderParams:
     """Labels render parameters.."""
 
     cmap_params: CmapParams
     outline_params: OutlineParams
     elements: str | Sequence[str] | None = None
-    color: str | None = None
+    color: list[str | None] | str | None = None
     col_for_color: str | None = None
-    groups: str | Sequence[str] | None = None
+    groups: str | list[list[str | None]] | list[str | None] | None = None
     contour_px: int | None = None
-    palette: ListedColormap | str | None = None
+    palette: ListedColormap | list[list[str | None]] | list[str | None] | None = None
     outline_alpha: float = 1.0
     fill_alpha: float = 0.3
     scale: float = 1.0
     transfunc: Callable[[float], float] | None = None
-    element_table_mapping: dict[str, set[str] | str] | str | list[str] | None = None
+    element_table_mapping: dict[str, set[str | None] | str | None] | str | list[str] | None = None
 
 
 @dataclass
 class PointsRenderParams:
     """Points render parameters.."""
 
     cmap_params: CmapParams
-    elements: str | Sequence[str] | None = None
-    color: str | None = None
-    col_for_color: str | None = None
-    groups: str | Sequence[str] | None = None
-    palette: ListedColormap | str | None = None
+    elements: str | list[str] | None = None
+    color: list[str | None] | str | None = None
+    col_for_color: list[str | None] | str | None = None
+    groups: str | list[list[str | None]] | list[str | None] | None = None
+    palette: ListedColormap | list[list[str | None]] | list[str | None] | None = None
     alpha: float = 1.0
     size: float = 1.0
     transfunc: Callable[[float], float] | None = None
-    element_table_mapping: dict[str, set[str] | str] | str | list[str] | None = None
+    element_table_mapping: dict[str, set[str | None] | str | None] | str | list[str] | None = None
 
 
 @dataclass
 class ImageRenderParams:
     """Labels render parameters.."""
 
     cmap_params: list[CmapParams] | CmapParams
     elements: str | Sequence[str] | None = None
     channel: list[str] | list[int] | int | str | None = None
-    palette: ListedColormap | str | None = None
+    palette: ListedColormap | list[list[str | None]] | list[str | None] | None = None
     alpha: float = 1.0
     quantiles_for_norm: tuple[float | None, float | None] = (None, None)
     scale: str | list[str] | None = None
 
 
 @dataclass
 class LabelsRenderParams:
     """Labels render parameters.."""
 
     cmap_params: CmapParams
     elements: str | Sequence[str] | None = None
     color: list[str | None] | str | None = None
-    groups: str | Sequence[str] | None = None
+    groups: str | list[list[str | None]] | list[str | None] | None = None
     contour_px: int | None = None
     outline: bool = False
-    palette: ListedColormap | str | None = None
+    palette: ListedColormap | list[list[str | None]] | list[str | None] | None = None
     outline_alpha: float = 1.0
     fill_alpha: float = 0.4
     transfunc: Callable[[float], float] | None = None
     scale: str | list[str] | None = None
-    element_table_mapping: dict[str, set[str] | str] | str | list[str] | None = None
+    element_table_mapping: dict[str, set[str | None] | str | None] | str | list[str] | None = None
```

### Comparing `spatialdata_plot-0.2.1/src/spatialdata_plot/pl/utils.py` & `spatialdata_plot-0.2.2/src/spatialdata_plot/pl/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import warnings
 from collections import defaultdict
 from collections.abc import Iterable, Mapping, Sequence
 from copy import copy
 from functools import partial
 from pathlib import Path
 from types import MappingProxyType
-from typing import Any, Literal, Union, cast
+from typing import Any, Literal, Union
 
 import matplotlib
 import matplotlib.patches as mpatches
 import matplotlib.patches as mplp
 import matplotlib.path as mpath
 import matplotlib.pyplot as plt
 import multiscale_spatial_image as msi
@@ -202,30 +202,43 @@
     -------
     - PatchCollection: Collection of patches for rendering.
     """
     cmap = kwargs["cmap"]
 
     try:
         # fails when numeric
-        fill_c = ColorConverter().to_rgba_array(c)
+        if len(c.shape) == 1 and c.shape[0] in [3, 4] and c.shape[0] == len(shapes) and c.dtype == float:
+            if norm is None:
+                c = cmap(c)
+            else:
+                try:
+                    norm = colors.Normalize(vmin=min(c), vmax=max(c))
+                except ValueError as e:
+                    raise ValueError(
+                        "Could not convert values in the `color` column to float, if `color` column represents"
+                        " categories, set the column to categorical dtype."
+                    ) from e
+                c = cmap(norm(c))
+        else:
+            fill_c = ColorConverter().to_rgba_array(c)
     except ValueError:
         if norm is None:
             c = cmap(c)
         else:
             try:
                 norm = colors.Normalize(vmin=min(c), vmax=max(c))
             except ValueError as e:
                 raise ValueError(
                     "Could not convert values in the `color` column to float, if `color` column represents"
                     " categories, set the column to categorical dtype."
                 ) from e
             c = cmap(norm(c))
 
     fill_c = ColorConverter().to_rgba_array(c)
-    fill_c[..., -1] = render_params.fill_alpha
+    fill_c[..., -1] *= render_params.fill_alpha
 
     if render_params.outline_params.outline:
         outline_c = ColorConverter().to_rgba_array(render_params.outline_params.outline_color)
         outline_c[..., -1] = render_params.outline_alpha
         outline_c = outline_c.tolist()
     else:
         outline_c = [None]
@@ -591,28 +604,28 @@
         palette = [to_hex(palette(x, alpha=alpha)) for x in color_idx]  # type: ignore[attr-defined]
     else:
         raise TypeError(f"Palette is {type(palette)} but should be string or list.")
 
     return palette[:len_cat]  # type: ignore[return-value]
 
 
-def _locate_points_value_in_table(value_key: str, sdata: SpatialData, element_name: str, table_name: str):
+def _locate_points_value_in_table(value_key: str, sdata: SpatialData, table_name: str) -> _ValueOrigin:
     table = sdata[table_name]
 
     if value_key in table.obs.columns:
         value = table.obs[value_key]
         is_categorical = isinstance(value.dtype, CategoricalDtype)
         return _ValueOrigin(origin="obs", is_categorical=is_categorical, value_key=value_key)
 
     is_categorical = False
     return _ValueOrigin(origin="var", is_categorical=is_categorical, value_key=value_key)
 
 
 # TODO consider move to relational query in spatialdata
-def get_values_point_table(sdata: SpatialData, origin: _ValueOrigin, table_name: str):
+def get_values_point_table(sdata: SpatialData, origin: _ValueOrigin, table_name: str) -> pd.Series:
     """Get a particular column stored in _ValueOrigin from the table in the spatialdata object."""
     table = sdata[table_name]
     if origin.origin == "obs":
         return table.obs[origin.value_key]
     if origin.origin == "var":
         return table[:, table.var_names.isin([origin.value_key])].X.copy()
     raise ValueError(f"Color column `{origin.value_key}` not found in table {table_name}")
@@ -620,32 +633,30 @@
 
 def _set_color_source_vec(
     sdata: sd.SpatialData,
     element: SpatialElement | None,
     element_index: int,
     value_to_plot: str | None,
     element_name: list[str] | str | None = None,
-    groups: Sequence[str] | str | None = None,
-    palette: str | list[str] | None = None,
+    groups: Sequence[str | None] | str | None = None,
+    palette: list[str | None] | None = None,
     na_color: str | tuple[float, ...] | None = None,
     cmap_params: CmapParams | None = None,
     table_name: str | None = None,
 ) -> tuple[ArrayLike | pd.Series | None, ArrayLike, bool]:
     if value_to_plot is None:
         color = np.full(len(element), to_hex(na_color))  # type: ignore[arg-type]
         return color, color, False
 
     model = get_model(sdata[element_name])
 
     # Figure out where to get the color from
     origins = _locate_value(value_key=value_to_plot, sdata=sdata, element_name=element_name, table_name=table_name)
     if model == PointsModel and table_name is not None:
-        origin = _locate_points_value_in_table(
-            value_key=value_to_plot, sdata=sdata, element_name=element_name, table_name=table_name
-        )
+        origin = _locate_points_value_in_table(value_key=value_to_plot, sdata=sdata, table_name=table_name)
         if origin is not None:
             origins.append(origin)
 
     if len(origins) > 1:
         raise ValueError(
             f"Color key '{value_to_plot}' for element '{element_name}' been found in multiple locations: {origins}."
         )
@@ -669,33 +680,40 @@
         color_source_vector = pd.Categorical(color_source_vector)  # convert, e.g., `pd.Series`
         categories = color_source_vector.categories
 
         if groups is not None and groups[0] is not None:
             color_source_vector = color_source_vector.remove_categories(categories.difference(groups))
             categories = groups
 
+        palette_input: list[str] | str | None
         if groups is not None and groups[0] is not None:
             if isinstance(palette, list):
-                palette_input = palette[0] if palette[0] is None else palette
+                palette_input = (
+                    palette[0]
+                    if palette[0] is None
+                    else [color_palette for color_palette in palette if isinstance(color_palette, str)]
+                )
         elif palette is not None and isinstance(palette, list):
             palette_input = palette[0]
+
         else:
             palette_input = palette
 
         color_map = dict(
             zip(categories, _get_colors_for_categorical_obs(categories, palette_input, cmap_params=cmap_params))
         )
 
         if color_map is None:
             raise ValueError("Unable to create color palette.")
 
         # do not rename categories, as colors need not be unique
         color_vector = color_source_vector.map(color_map)
         if color_vector.isna().any():
-            color_vector = color_vector.add_categories([to_hex(na_color)])
+            if na_cat_color := to_hex(na_color) not in color_vector.categories:
+                color_vector = color_vector.add_categories([na_cat_color])
             color_vector = color_vector.fillna(to_hex(na_color))
 
         return color_source_vector, color_vector, True
 
     logger.warning(f"Color key '{value_to_plot}' for element '{element_name}' not been found, using default colors.")
     color = np.full(sdata[table_name].n_obs, to_hex(na_color))
     return color, color, False
@@ -1347,19 +1365,21 @@
     render_elements
         The list of names of SpatialElements to be rendered.
 
     Returns
     -------
     The updated render parameters.
     """
-    element_table_mapping: dict[str, set[str]] = defaultdict(set)
+    element_table_mapping: dict[str, set[str | None] | str | None] = defaultdict(set)
+
     if not params.element_table_mapping:
         for element_name in render_elements:
-            element_table_mapping[element_name].update(_get_element_annotators(sdata, element_name))
-    else:
+            if isinstance(mapping := element_table_mapping[element_name], set):
+                mapping.update(_get_element_annotators(sdata, element_name))
+    elif isinstance(params.element_table_mapping, (list, str)):
         table_names: list[str] = (
             [params.element_table_mapping]
             if isinstance(params.element_table_mapping, str)
             else params.element_table_mapping
         )
         if len(table_names) == 1:
             for element_name in render_elements:
@@ -1375,64 +1395,79 @@
             ), "If specifying a list of table names, the length must be equal to number of elements to be plotted"
             for index, table_name in enumerate(table_names):
                 element = render_elements[index]
                 if element not in sdata[table_name].uns[TableModel.ATTRS_KEY][TableModel.REGION_KEY]:
                     warnings.warn(
                         f"The element '{element}' is not annotated by table '{table_name}'", UserWarning, stacklevel=2
                     )
-                element_table_mapping[element].add(table_name)
+                if isinstance(mapping := element_table_mapping[element], set):
+                    mapping.add(table_name)
+    assert isinstance(element_table_mapping, dict)
     params.element_table_mapping = element_table_mapping
     return params
 
 
 def _update_element_table_mapping_label_colors(
     sdata: SpatialData, params: LabelsRenderParams | PointsRenderParams | ShapesRenderParams, render_elements: list[str]
 ) -> ImageRenderParams | LabelsRenderParams | PointsRenderParams | ShapesRenderParams:
-    element_table_mapping = params.element_table_mapping
+    element_table_mapping: dict[str, set[str | None] | str | None] | str | list[str] | None = (
+        params.element_table_mapping
+    )
+
+    assert isinstance(element_table_mapping, dict)
 
     # If one color column check presence for each table annotating the specific element
     if isinstance(params.color, list) and len(params.color) == 1:
         params.color = params.color * len(render_elements)
         for element_name in render_elements:
-            for table_name in element_table_mapping[element_name].copy():
-                if (
-                    params.color[0] not in sdata[table_name].obs.columns
-                    and params.color[0] not in sdata[table_name].var_names
-                ):
-                    element_table_mapping[element_name].remove(table_name)
-    if len(params.color) > 1:
+            if isinstance(mapping := element_table_mapping[element_name], set):
+                table_names = mapping.copy()
+                for table_name in table_names:
+                    if (
+                        params.color[0] not in sdata[table_name].obs.columns
+                        and params.color[0] not in sdata[table_name].var_names
+                    ):
+                        mapping.remove(table_name)
+    if isinstance(params.color, list) and len(params.color) > 1:
         assert len(params.color) == len(
             render_elements
         ), "Either one color should be given or the length should be equal to the number of elements being plotted."
         for index, element_name in enumerate(render_elements):
-            if len(element_table_mapping[element_name]) != 0:
-                for table_name in element_table_mapping[element_name].copy():
+            if isinstance(mapping := element_table_mapping[element_name], set) and len(mapping) != 0:
+                for table_name in mapping.copy():
                     if (
                         params.color[index] not in sdata[table_name].obs.columns
                         and params.color[index] not in sdata[table_name].var_names
                     ):
-                        element_table_mapping[element_name].remove(table_name)
+                        mapping.remove(table_name)
             else:
                 params.color[index] = None
 
     # We only want one table containing the color column per element
+    # table_set: set[str | None]
     for element_name, table_set in element_table_mapping.items():
-        if len(table_set) > 1:
+        if isinstance(table_set, set) and len(table_set) > 1:
             raise ValueError(f"Multiple tables with color columns found for the element {element_name}")
-        element_table_mapping[element_name] = next(iter(table_set)) if len(table_set) != 0 else None
+        if isinstance(table_set, set):
+            element_table_mapping[element_name] = next(iter(table_set)) if len(table_set) != 0 else None
 
     params.element_table_mapping = element_table_mapping
     return params
 
 
 def _validate_colors_element_table_mapping_points_shapes(
     sdata: SpatialData, params: PointsRenderParams | ShapesRenderParams, render_elements: list[str]
 ) -> PointsRenderParams | ShapesRenderParams:
-    element_table_mapping = cast(dict, params.element_table_mapping)
-    if len(params.color) == 1:
+    element_table_mapping: dict[str, set[str | None] | str | None] | str | list[str] | None = (
+        params.element_table_mapping
+    )
+
+    assert isinstance(element_table_mapping, dict)
+
+    if isinstance(params.color, list) and len(params.color) == 1 and isinstance(params.col_for_color, list):
         color = params.color[0]
         col_color = params.col_for_color[0]
         # This means that we are dealing with colors that are color like
         if color is not None:
             params.color = [color] * len(render_elements)
             params.col_for_color = [None] * len(render_elements)
         else:
@@ -1440,58 +1475,62 @@
                 params.color = [None] * len(render_elements)
                 params.col_for_color = []
                 for element_name in render_elements:
                     if col_color in sdata[element_name].columns:
                         params.col_for_color.append(col_color)
                         element_table_mapping[element_name] = set()
                     else:
-                        if len(element_table_mapping[element_name].copy()) != 0:
-                            for table_name in element_table_mapping[element_name].copy():
+                        if isinstance(table_set := element_table_mapping[element_name], set) and len(table_set) != 0:
+                            for table_name in table_set.copy():
                                 if (
                                     col_color not in sdata[table_name].obs.columns
                                     and col_color not in sdata[table_name].var_names
                                 ):
-                                    element_table_mapping[element_name].remove(table_name)
+                                    table_set.remove(table_name)
                                     params.col_for_color.append(None)
                                 else:
                                     params.col_for_color.append(col_color)
                         else:
                             params.col_for_color.append(None)
             else:
                 params.color = [None] * len(render_elements)
                 params.col_for_color = [None] * len(render_elements)
     else:
-        if len(params.color) != len(render_elements):
+        if isinstance(params.color, list) and len(params.color) != len(render_elements):
             warnings.warn(
                 "The number of given colors and elements to render is not equal. "
                 "Either provide one color or a list with one color for each element. skipping",
                 UserWarning,
                 stacklevel=2,
             )
             params.color = [None] * len(render_elements)
             params.col_for_color = [None] * len(render_elements)
         else:
+            assert isinstance(params.color, list)
+            assert isinstance(params.col_for_color, list)
             for index, color in enumerate(params.color):
                 if color is None:
                     element_name = render_elements[index]
                     col_color = params.col_for_color[index]
-                    for table_name in element_table_mapping[element_name].copy():
-                        if (
-                            col_color not in sdata[table_name].obs.columns
-                            and col_color not in sdata[table_name].var_names
-                            and col_color not in sdata[element_name].columns
-                        ):
-                            element_table_mapping[element_name].remove(table_name)
+                    if isinstance(mapping := element_table_mapping[element_name], set):
+                        for table_name in mapping.copy():
+                            if (
+                                col_color not in sdata[table_name].obs.columns
+                                and col_color not in sdata[table_name].var_names
+                                and col_color not in sdata[element_name].columns
+                            ):
+                                mapping.remove(table_name)
     for index, element_name in enumerate(render_elements):
         # We only want one table value per element and only when there is a color column in the table
         if isinstance(params.col_for_color, list) and params.col_for_color[index] is not None:
             table_set = element_table_mapping[element_name]
-            if len(table_set) > 1:
+            if isinstance(table_set, set) and len(table_set) > 1:
                 raise ValueError(f"More than one table found with color column {params.col_for_color[index]}.")
-            element_table_mapping[element_name] = next(iter(table_set)) if len(table_set) != 0 else None
+            if isinstance(tables := table_set, set):
+                element_table_mapping[element_name] = next(iter(tables)) if len(tables) != 0 else None
             if element_table_mapping[element_name] is None:
                 warnings.warn(
                     f"No table found with color column {params.col_for_color[index]} to render {element_name}",
                     UserWarning,
                     stacklevel=2,
                 )
         else:
@@ -1602,26 +1641,26 @@
 
 def _validate_render_params(
     element_type: str,
     sdata: sd.SpatialData,
     alpha: float | int | None = None,
     channel: list[str] | list[int] | str | int | None = None,
     cmap: list[Colormap] | Colormap | str | None = None,
-    color: list[str] | str | None = None,
+    color: list[str | None] | str | None = None,
     contour_px: int | None = None,
     elements: list[str] | str | None = None,
     fill_alpha: float | int | None = None,
-    groups: list[list[str | None]] | list[str] | str | None = None,
+    groups: str | list[list[str | None]] | list[str | None] | None = None,
     na_color: ColorLike | None = None,
     norm: Normalize | bool | None = None,
     outline: bool | None = None,
     outline_alpha: float | int | None = None,
     outline_color: str | list[float] | None = None,
     outline_width: float | int | None = None,
-    palette: list[list[str | None]] | list[str] | str | None = None,
+    palette: list[list[str | None]] | list[str | None] | str | None = None,
     quantiles_for_norm: tuple[float | None, float | None] | None = None,
     scale: float | int | list[str] | str | None = None,
     size: float | int | None = None,
 ) -> dict[str, Any]:
     params_dict: dict[str, Any] = {}
     if elements is not None:
         if not isinstance(elements, (list, str)):
@@ -1632,69 +1671,98 @@
         if any(e not in sdata_elements for e in elements):
             raise ValueError(
                 f"Not all specified {element_type} elements were found. Available elements are: "
                 f"`{'`, `'.join(sdata_elements.keys())}`"
             )
     params_dict["elements"] = elements
 
+    groups_overwrite: list[list[str]] | None = None
     if groups is not None and element_type != "images":
         if not isinstance(groups, (list, str)):
             raise TypeError("Parameter 'groups' must be a string or a list of strings.")
         if isinstance(groups, str):
-            groups = [[groups]]
+            groups_overwrite = [[groups]]
         elif not isinstance(groups[0], list):
-            if not all(isinstance(g, str) for g in groups):
+            if all(isinstance(g, str) for g in groups):
+                groups_overwrite = [[group for group in groups if isinstance(group, str)]]
+            else:
                 raise TypeError("All items in single 'groups' list must be strings.")
-            groups = [groups]
+
         else:
-            if not all(isinstance(g, str) or g is None for group in groups for g in group):
+            if not all(
+                (
+                    isinstance(group, list) and all(isinstance(g, (str, type(None))) for g in group)
+                    if group is not None
+                    else True
+                )
+                for group in groups
+            ):
                 raise TypeError("All items in lists within lists of 'groups' must be strings or None.")
 
-    params_dict["groups"] = groups
+    params_dict["groups"] = groups_overwrite
+
+    palette_overwrite: list[list[str]] | None = None
+    if groups_overwrite is not None and palette is None:
+        warnings.warn(
+            "Groups is specified but palette is not. Setting palette to default 'lightgray'", UserWarning, stacklevel=2
+        )
+        palette_overwrite = [["lightgray" for _ in range(len(groups_sublist))] for groups_sublist in groups_overwrite]
 
     if palette is not None:
         if not isinstance(palette, (list, str)):
             raise TypeError("Parameter 'palette' must be a string or a list of strings.")
         if isinstance(palette, str):
-            palette = [[palette]]
+            palette_overwrite = [[palette]]
         elif not isinstance(palette[0], list):
             if not all(isinstance(pal, str) for pal in palette):
                 raise TypeError("All items in single 'palette' list must be strings.")
-            palette = [palette]
+            palette_overwrite = [[pal for pal in palette if isinstance(pal, str)]]
         else:
-            if not all(isinstance(p, str) or p is None for pal in palette for p in pal):
+            if not all(
+                (
+                    isinstance(pal, list) and all(isinstance(p, (str, type(None))) for p in pal)
+                    if pal is not None
+                    else True
+                )
+                for pal in palette
+            ):
                 raise TypeError("All items in lists within lists of 'groups' must be strings.")
 
         if element_type in ["shapes", "points", "labels"]:
-            if groups is None:
+            if groups_overwrite is None:
                 raise ValueError("When specifying 'palette', 'groups' must also be specified.")
-            if len(groups) != len(palette):
+            if (
+                groups_overwrite is not None
+                and palette_overwrite is not None
+                and len(groups_overwrite) != len(palette_overwrite)
+            ):
                 raise ValueError(
-                    f"The length of 'palette' and 'groups' must be the same, length is {len(palette)} and"
-                    f"{len(groups)} respectively."
+                    f"The length of 'palette' and 'groups' must be the same, length is {len(palette_overwrite)} and"
+                    f"{len(groups_overwrite)} respectively."
                 )
-            for index, sublist in enumerate(groups):
-                if not len(sublist) == len(palette[index]):
-                    raise ValueError("Not all nested lists in `groups` and `palette` are of equal length.")
-                if (
-                    not len(g_set := {type(el) for el in sublist})
-                    == len(p_set := {type(pal) for pal in palette[index]})
-                    == 1
-                ):
-                    raise ValueError(
-                        "Mixed dtypes found in sublists of `groups` and/or `palette`. Must be either all"
-                        "`str` or `None`."
-                    )
-                if g_set != p_set:
-                    raise ValueError(
-                        "Sublists with same index in `groups` and `palette` must contain elements of the "
-                        "same dtype, either both `str` or `None`."
-                    )
+            if palette_overwrite is not None:
+                for index, sublist in enumerate(groups_overwrite):
+                    if not len(sublist) == len(palette_overwrite[index]):
+                        raise ValueError("Not all nested lists in `groups` and `palette` are of equal length.")
+                    if (
+                        not len(g_set := {type(el) for el in sublist})
+                        == len(p_set := {type(pal) for pal in palette_overwrite[index]})
+                        == 1
+                    ):
+                        raise ValueError(
+                            "Mixed dtypes found in sublists of `groups` and/or `palette`. Must be either all"
+                            "`str` or `None`."
+                        )
+                    if g_set != p_set:
+                        raise ValueError(
+                            "Sublists with same index in `groups` and `palette` must contain elements of the "
+                            "same dtype, either both `str` or `None`."
+                        )
 
-    params_dict["palette"] = palette
+    params_dict["palette"] = palette_overwrite
 
     if cmap is not None:
         if element_type == "images":
             if not isinstance(cmap, (list, Colormap, str)):
                 raise TypeError("Parameter 'cmap' must be a string, a Colormap, or a list of these types.")
             if isinstance(cmap, list) and not all(isinstance(c, (Colormap, str)) for c in cmap):
                 raise TypeError("Each item in 'cmap' list must be a string or a Colormap.")
@@ -1739,48 +1807,51 @@
             raise TypeError("Parameter 'outline_width' must be numeric.")
         if outline_width < 0:
             raise ValueError("Parameter 'outline_width' cannot be negative.")
 
         if not colors.is_color_like(outline_color):
             raise TypeError("Parameter 'outline_color' must be color-like.")
 
+    color_overwrite: list[str | None] = []
+    col_for_color: list[str | None]
     if element_type in ["points", "shapes"]:
-        if color is not None:
+        if isinstance(color, (str, list)):
             if not isinstance(color, list):
                 if colors.is_color_like(color):
                     logger.info("Value for parameter 'color' appears to be a color, using it as such.")
-                    color = [color]
+                    color_overwrite = [color]
                     col_for_color = [None]
                 else:
                     if not isinstance(color, str):
                         raise TypeError(
                             "Parameter 'color' must be a string indicating which color "
                             + "in sdata.table to use for coloring the shapes."
                         )
                     col_for_color = [color]
-                    color = [None]
+                    color_overwrite = [None]
             else:
                 col_for_color = []
-                for index, c in enumerate(color):
+                for c in color:
                     if colors.is_color_like(c):
                         logger.info(f"Value `{c}` in list 'color' appears to be a color, using it as such.")
-                        color[index] = c
+                        color_overwrite.append(c)
                         col_for_color.append(None)
                     else:
                         if not isinstance(c, str):
                             raise TypeError(
                                 f"Value `{c}` in list Parameter 'color' must be a string indicating which color "
                                 + "in sdata.table to use for coloring the shapes or should be color-like."
                             )
                         col_for_color.append(c)
-                        color[index] = None
+                        color_overwrite.append(None)
         else:
-            color = [color]
+            color_overwrite = [color]
             col_for_color = [None]
-        params_dict["color"] = color
+
+        params_dict["color"] = color_overwrite
         params_dict["col_for_color"] = col_for_color
 
     if element_type == "points":
         if not isinstance(size, (float, int)):
             raise TypeError("Parameter 'size' must be numeric.")
         if size < 0:
             raise ValueError("Parameter 'size' must be a positive number.")
@@ -1835,71 +1906,107 @@
     return params_dict
 
 
 def _match_length_elements_groups_palette(
     params: ImageRenderParams | LabelsRenderParams | PointsRenderParams | ShapesRenderParams,
     render_elements: list[str],
     image: bool = False,
-):
+) -> ImageRenderParams | LabelsRenderParams | PointsRenderParams | ShapesRenderParams:
     if image and isinstance(params, ImageRenderParams):
         if params.palette is None:
             params.palette = [[None] for _ in range(len(render_elements))]
         else:
             params.palette = [params.palette[0] for _ in range(len(render_elements))]
-    else:
+    elif not isinstance(params, ImageRenderParams):
         groups = params.groups
         palette = params.palette
+
+        groups_elements: list[list[str | None]] | None = None
+        palette_elements: list[list[str | None]] | None = None
         # We already checked before that length of groups and palette is the same
         if groups is not None:
             if len(groups) == 1:
-                params.groups = [groups[0] for _ in range(len(render_elements))]
+                groups_elements = [groups[0] for _ in range(len(render_elements)) if isinstance(groups[0], list)]
                 if palette is not None:
-                    params.palette = [palette[0] for _ in range(len(render_elements))]
+                    palette_elements = [palette[0] for _ in range(len(render_elements)) if isinstance(palette[0], list)]
                 else:
-                    params.palette = [[None] for _ in range(len(render_elements))]
+                    palette_elements = [[None] for _ in range(len(render_elements))]
             else:
                 if len(groups) != len(render_elements):
                     raise ValueError(
                         "Multiple groups and palettes are given but the number is not the same as the number "
                         "of elements to be rendered."
                     )
         else:
-            params.groups = [[None] for _ in range(len(render_elements))]
-            params.palette = [[None] for _ in range(len(render_elements))]
+            groups_elements = [[None] for _ in range(len(render_elements))]
+            palette_elements = [[None] for _ in range(len(render_elements))]
+        params.palette = palette_elements
+        params.groups = groups_elements
 
     return params
 
 
 def _get_wanted_render_elements(
-    sdata, sdata_wanted_elements, params, cs, element_type: Literal["images", "labels", "points", "shapes"]
-):
+    sdata: SpatialData,
+    sdata_wanted_elements: list[str],
+    params: ImageRenderParams | LabelsRenderParams | PointsRenderParams | ShapesRenderParams,
+    cs: str,
+    element_type: Literal["images", "labels", "points", "shapes"],
+) -> tuple[list[str], list[str], bool]:
     wants_elements = True
     if element_type in ["images", "labels", "points", "shapes"]:  # Prevents eval security risk
         wanted_elements = params.elements if params.elements is not None else list(getattr(sdata, element_type).keys())
 
         wanted_elements_on_cs = [
             element for element in wanted_elements if cs in set(get_transformation(sdata[element], get_all=True).keys())
         ]
 
         sdata_wanted_elements.extend(wanted_elements_on_cs)
         return sdata_wanted_elements, wanted_elements_on_cs, wants_elements
 
     raise ValueError(f"Unknown element type {element_type}")
 
 
-def _update_params(sdata, params, wanted_elements_on_cs, element_type: Literal["images", "labels", "points", "shapes"]):
-    if element_type in ["labels", "points", "shapes"] and wanted_elements_on_cs:
+def _update_params(
+    sdata: SpatialData,
+    params: ImageRenderParams | LabelsRenderParams | PointsRenderParams | ShapesRenderParams,
+    wanted_elements_on_cs: list[str],
+    element_type: Literal["images", "labels", "points", "shapes"],
+) -> ImageRenderParams | LabelsRenderParams | PointsRenderParams | ShapesRenderParams:
+    if isinstance(params, (LabelsRenderParams, PointsRenderParams, ShapesRenderParams)) and wanted_elements_on_cs:
         params = _create_initial_element_table_mapping(sdata, params, wanted_elements_on_cs)
-        if element_type == "labels":
+        if isinstance(params, LabelsRenderParams):
             params = _update_element_table_mapping_label_colors(sdata, params, wanted_elements_on_cs)
-        else:
+        if isinstance(params, (PointsRenderParams, ShapesRenderParams)):
             params = _validate_colors_element_table_mapping_points_shapes(sdata, params, wanted_elements_on_cs)
 
-    # if params.palette is None:
-    #     params.palette = [[None] for _ in wanted_elements_on_cs]
     image_flag = element_type == "images"
     return _match_length_elements_groups_palette(params, wanted_elements_on_cs, image=image_flag)
 
 
-def _is_coercable_to_float(series):
+def _is_coercable_to_float(series: pd.Series) -> bool:
     numeric_series = pd.to_numeric(series, errors="coerce")
     return not numeric_series.isnull().any()
+
+
+def _return_list_str_none(parameter: list[str | None] | str | None) -> list[str | None]:
+    """Force mypy to recognize list of string and None."""
+    if isinstance(parameter, list) and all(isinstance(item, (str, type(None))) for item in parameter):
+        checked_parameter = parameter
+    else:
+        checked_parameter = [None]
+    return checked_parameter
+
+
+def _return_list_list_str_none(
+    parameter: str | list[list[str | None]] | list[str | None] | None,
+) -> list[list[str | None]]:
+    if not isinstance(parameter, list):
+        return [[None]]
+
+    if all(
+        isinstance(sublist, list) and all(isinstance(inner_item, (str, type(None))) for inner_item in sublist)
+        for sublist in parameter
+    ):
+        return [list(sublist) for sublist in parameter if isinstance(sublist, list)]
+
+    return [[None]]
```

### Comparing `spatialdata_plot-0.2.1/src/spatialdata_plot/pp/basic.py` & `spatialdata_plot-0.2.2/src/spatialdata_plot/pp/basic.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/src/spatialdata_plot/pp/utils.py` & `spatialdata_plot-0.2.2/src/spatialdata_plot/pp/utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/conftest.py` & `spatialdata_plot-0.2.2/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,14 @@
             points=_get_points(),
             table=_get_table("sample1"),
         )
     elif request.param == "empty":
         s = SpatialData()
     else:
         s = request.getfixturevalue(request.param)
-    # print(f"request.param = {request.param}")
     return s
 
 
 def _get_images() -> dict[str, Union[SpatialImage, MultiscaleSpatialImage]]:
     out = {}
     dims_2d = ("c", "y", "x")
     dims_3d = ("z", "y", "x", "c")
```

### Comparing `spatialdata_plot-0.2.1/tests/test_pp.py` & `spatialdata_plot-0.2.2/tests/test_pp.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Extent_correct_plot_after_transformations.png` & `spatialdata_plot-0.2.2/tests/_images/Extent_correct_plot_after_transformations.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Extent_extent_calculation_respects_element_selection_circles.png` & `spatialdata_plot-0.2.2/tests/_images/Extent_extent_calculation_respects_element_selection_circles.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Extent_extent_calculation_respects_element_selection_circles_and_polygons.png` & `spatialdata_plot-0.2.2/tests/_images/Extent_extent_calculation_respects_element_selection_circles_and_polygons.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Extent_extent_calculation_respects_element_selection_polygons.png` & `spatialdata_plot-0.2.2/tests/_images/Extent_extent_calculation_respects_element_selection_polygons.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Extent_extent_of_img_full_canvas.png` & `spatialdata_plot-0.2.2/tests/_images/Extent_extent_of_img_full_canvas.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Extent_extent_of_img_is_correct_after_spatial_query.png` & `spatialdata_plot-0.2.2/tests/_images/Extent_extent_of_img_is_correct_after_spatial_query.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Extent_extent_of_partial_canvas_on_full_canvas.png` & `spatialdata_plot-0.2.2/tests/_images/Extent_extent_of_partial_canvas_on_full_canvas.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Extent_extent_of_points_partial_canvas.png` & `spatialdata_plot-0.2.2/tests/_images/Extent_extent_of_points_partial_canvas.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Extent_extent_of_polygons_is_correct_after_spatial_query.png` & `spatialdata_plot-0.2.2/tests/_images/Extent_extent_of_polygons_is_correct_after_spatial_query.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Extent_extent_of_polygons_on_img_is_correct_after_spatial_query.png` & `spatialdata_plot-0.2.2/tests/_images/Extent_extent_of_polygons_on_img_is_correct_after_spatial_query.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_do_rasterization.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_do_rasterization.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_normalize_image.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_normalize_image.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_pass_cmap.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_pass_cmap.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_pass_cmap_list.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_pass_cmap_list.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_pass_cmap_to_each_channel.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_pass_cmap_to_each_channel.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_pass_cmap_to_single_channel.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_pass_cmap_to_single_channel.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_pass_color_to_each_channel.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_pass_color_to_each_channel.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_pass_color_to_single_channel.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_pass_color_to_single_channel.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_pass_str_cmap.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_pass_str_cmap.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_pass_str_cmap_list.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_pass_str_cmap_list.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_render_a_single_channel_from_image.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_render_a_single_channel_from_image.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_render_given_scale_of_multiscale_image.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_render_given_scale_of_multiscale_image.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_render_image.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_render_image.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_render_multiscale_image.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_render_multiscale_image.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_render_two_channels_from_image.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_render_two_channels_from_image.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_stack_render_images.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_stack_render_images.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Images_can_stop_rasterization_with_scale_full.png` & `spatialdata_plot-0.2.2/tests/_images/Images_can_stop_rasterization_with_scale_full.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Labels_can_color_labels.png` & `spatialdata_plot-0.2.2/tests/_images/Labels_can_color_labels.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Labels_can_color_labels_by_continuous_variable.png` & `spatialdata_plot-0.2.2/tests/_images/Labels_can_color_labels_by_continuous_variable.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Labels_can_do_rasterization.png` & `spatialdata_plot-0.2.2/tests/_images/Labels_can_do_rasterization.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Labels_can_render_given_scale_of_multiscale_labels.png` & `spatialdata_plot-0.2.2/tests/_images/Labels_can_render_given_scale_of_multiscale_labels.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Labels_can_render_labels.png` & `spatialdata_plot-0.2.2/tests/_images/Labels_can_render_labels.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Labels_can_render_multiscale_labels.png` & `spatialdata_plot-0.2.2/tests/_images/Labels_can_render_multiscale_labels.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Labels_can_stack_render_labels.png` & `spatialdata_plot-0.2.2/tests/_images/Labels_can_stack_render_labels.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Labels_can_stop_rasterization_with_scale_full.png` & `spatialdata_plot-0.2.2/tests/_images/Labels_can_stop_rasterization_with_scale_full.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Labels_label_categorical_color.png` & `spatialdata_plot-0.2.2/tests/_images/Labels_label_categorical_color.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Labels_multiscale_label_categorical_color.png` & `spatialdata_plot-0.2.2/tests/_images/Labels_multiscale_label_categorical_color.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_affine.png` & `spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_affine.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_composition.png` & `spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_composition.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_inverse.png` & `spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_inverse.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_mapaxis.png` & `spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_mapaxis.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_overlay.png` & `spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_overlay.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_rotation.png` & `spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_rotation.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_scale.png` & `spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_scale.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_split.png` & `spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_split.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_translation.png` & `spatialdata_plot-0.2.2/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_translation.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Points_can_filter_with_groups.png` & `spatialdata_plot-0.2.2/tests/_images/Points_can_filter_with_groups.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Points_can_render_points.png` & `spatialdata_plot-0.2.2/tests/_images/Points_can_render_points.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Points_can_stack_render_points.png` & `spatialdata_plot-0.2.2/tests/_images/Points_can_stack_render_points.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Points_color_recognises_actual_color_as_color.png` & `spatialdata_plot-0.2.2/tests/_images/Points_color_recognises_actual_color_as_color.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Points_coloring_with_cmap.png` & `spatialdata_plot-0.2.2/tests/_images/Points_coloring_with_cmap.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Points_coloring_with_palette.png` & `spatialdata_plot-0.2.2/tests/_images/Points_coloring_with_palette.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Points_points_categorical_color.png` & `spatialdata_plot-0.2.2/tests/_images/Points_points_categorical_color.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Points_points_coercable_categorical_color.png` & `spatialdata_plot-0.2.2/tests/_images/Points_points_coercable_categorical_color.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_color_from_geodataframe.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_color_from_geodataframe.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_color_two_queried_shapes_elements_by_annotation.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_color_two_queried_shapes_elements_by_annotation.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_color_two_shapes_elements_by_annotation.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_color_two_shapes_elements_by_annotation.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_filter_with_groups.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_filter_with_groups.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_plot_queried_with_annotation_despite_random_shuffling.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_plot_queried_with_annotation_despite_random_shuffling.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_plot_shapes_after_spatial_query.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_plot_shapes_after_spatial_query.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_plot_with_annotation_despite_random_shuffling.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_plot_with_annotation_despite_random_shuffling.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_circles.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_circles.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_circles_with_colored_outline.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_circles_with_colored_outline.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_circles_with_default_outline_width.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_circles_with_default_outline_width.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_circles_with_outline.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_circles_with_outline.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_circles_with_specified_outline_width.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_circles_with_specified_outline_width.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_empty_geometry.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_empty_geometry.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_multipolygons.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_multipolygons.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_polygons.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_polygons.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_polygons_with_outline.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_polygons_with_outline.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_polygons_with_rgb_colored_outline.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_polygons_with_rgb_colored_outline.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_polygons_with_rgba_colored_outline.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_polygons_with_rgba_colored_outline.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_render_polygons_with_str_colored_outline.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_render_polygons_with_str_colored_outline.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_scale_shapes.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_scale_shapes.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_can_stack_render_shapes.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_can_stack_render_shapes.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_color_recognises_actual_color_as_color.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_color_recognises_actual_color_as_color.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_colorbar_can_be_normalised.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_colorbar_can_be_normalised.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_colorbar_respects_input_limits.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_colorbar_respects_input_limits.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_coloring_with_palette.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_coloring_with_palette.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_shapes_categorical_color.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_shapes_categorical_color.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Shapes_shapes_coercable_categorical_color.png` & `spatialdata_plot-0.2.2/tests/_images/Shapes_shapes_coercable_categorical_color.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Show_pad_extent_adds_padding.png` & `spatialdata_plot-0.2.2/tests/_images/Show_pad_extent_adds_padding.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Upstream_can_render_transformations_raccoon_mapaxis.png` & `spatialdata_plot-0.2.2/tests/_images/Upstream_can_render_transformations_raccoon_mapaxis.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Upstream_can_render_transformations_raccoon_overlay.png` & `spatialdata_plot-0.2.2/tests/_images/Upstream_can_render_transformations_raccoon_overlay.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/_images/Upstream_can_render_transformations_raccoon_scale.png` & `spatialdata_plot-0.2.2/tests/_images/Upstream_can_render_transformations_raccoon_scale.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/pl/test_get_extent.py` & `spatialdata_plot-0.2.2/tests/pl/test_get_extent.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/pl/test_render.py` & `spatialdata_plot-0.2.2/tests/pl/test_render.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/pl/test_render_images.py` & `spatialdata_plot-0.2.2/tests/pl/test_render_images.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/pl/test_render_labels.py` & `spatialdata_plot-0.2.2/tests/pl/test_render_labels.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/pl/test_render_points.py` & `spatialdata_plot-0.2.2/tests/pl/test_render_points.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,19 @@
         sdata_blobs.pl.render_points(elements="blobs_points").pl.show()
 
     def test_plot_can_filter_with_groups(self, sdata_blobs: SpatialData):
         sdata_blobs["table"].obs["region"] = ["blobs_points"] * sdata_blobs["table"].n_obs
         sdata_blobs["table"].uns["spatialdata_attrs"]["region"] = "blobs_points"
         sdata_blobs.pl.render_points(color="genes", groups="gene_b", palette="orange").pl.show()
 
+    def test_plot_can_filter_with_groups_default_palette(self, sdata_blobs: SpatialData):
+        sdata_blobs["table"].obs["region"] = ["blobs_points"] * sdata_blobs["table"].n_obs
+        sdata_blobs["table"].uns["spatialdata_attrs"]["region"] = "blobs_points"
+        sdata_blobs.pl.render_points(color="genes", groups="gene_b").pl.show()
+
     def test_plot_coloring_with_palette(self, sdata_blobs: SpatialData):
         sdata_blobs["table"].obs["region"] = ["blobs_points"] * sdata_blobs["table"].n_obs
         sdata_blobs["table"].uns["spatialdata_attrs"]["region"] = "blobs_points"
         sdata_blobs.pl.render_points(
             color="genes", groups=["gene_a", "gene_b"], palette=["lightgreen", "darkblue"]
         ).pl.show()
```

### Comparing `spatialdata_plot-0.2.1/tests/pl/test_render_shapes.py` & `spatialdata_plot-0.2.2/tests/pl/test_render_shapes.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/pl/test_show.py` & `spatialdata_plot-0.2.2/tests/pl/test_show.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/pl/test_upstream_plots.py` & `spatialdata_plot-0.2.2/tests/pl/test_upstream_plots.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/tests/pp/test_basic.py` & `spatialdata_plot-0.2.2/tests/pp/test_basic.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/LICENSE` & `spatialdata_plot-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/README.md` & `spatialdata_plot-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [![Tests][badge-tests]][link-tests]
 [![Documentation][badge-docs]][link-docs]
 [![Codecov][badge-codecov]][link-codecov]
 [![Documentation][badge-pypi]][link-pypi]
 [![DOI](https://zenodo.org/badge/588223127.svg)](https://zenodo.org/badge/latestdoi/588223127)
 
-[badge-tests]: https://img.shields.io/github/actions/workflow/status/scverse/spatialdata-plot/test_and_deploy.yaml?branch=main
+[badge-tests]: https://img.shields.io/github/actions/workflow/status/scverse/spatialdata-plot/test.yaml?branch=main
 [link-tests]: https://github.com/scverse/spatialdata-plot/actions/workflows/test.yml
 [badge-docs]: https://img.shields.io/readthedocs/spatialdata-plot
 [badge-codecov]: https://codecov.io/gh/scverse/spatialdata-plot/branch/main/graph/badge.svg?token=C45F3ATSVI
 [link-codecov]: https://app.codecov.io/gh/scverse/spatialdata-plot
 [badge-pypi]: https://badge.fury.io/py/spatialdata_plot.svg
 [link-pypi]: https://pypi.org/project/spatialdata-plot/
```

### Comparing `spatialdata_plot-0.2.1/pyproject.toml` & `spatialdata_plot-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.2.1/PKG-INFO` & `spatialdata_plot-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: spatialdata-plot
-Version: 0.2.1
+Version: 0.2.2
 Summary: Static plotting for spatial data.
 Project-URL: Documentation, https://spatialdata.readthedocs.io/
 Project-URL: Source, https://github.com/scverse/spatialdata-plot.git
 Project-URL: Home-page, https://github.com/scverse/spatialdata-plot.git
 Author: scverse
 Maintainer-email: scverse <tim.treis@helmholtz-munich.de>
 License: BSD 3-Clause License
@@ -68,15 +68,15 @@
 
 [![Tests][badge-tests]][link-tests]
 [![Documentation][badge-docs]][link-docs]
 [![Codecov][badge-codecov]][link-codecov]
 [![Documentation][badge-pypi]][link-pypi]
 [![DOI](https://zenodo.org/badge/588223127.svg)](https://zenodo.org/badge/latestdoi/588223127)
 
-[badge-tests]: https://img.shields.io/github/actions/workflow/status/scverse/spatialdata-plot/test_and_deploy.yaml?branch=main
+[badge-tests]: https://img.shields.io/github/actions/workflow/status/scverse/spatialdata-plot/test.yaml?branch=main
 [link-tests]: https://github.com/scverse/spatialdata-plot/actions/workflows/test.yml
 [badge-docs]: https://img.shields.io/readthedocs/spatialdata-plot
 [badge-codecov]: https://codecov.io/gh/scverse/spatialdata-plot/branch/main/graph/badge.svg?token=C45F3ATSVI
 [link-codecov]: https://app.codecov.io/gh/scverse/spatialdata-plot
 [badge-pypi]: https://badge.fury.io/py/spatialdata_plot.svg
 [link-pypi]: https://pypi.org/project/spatialdata-plot/
```


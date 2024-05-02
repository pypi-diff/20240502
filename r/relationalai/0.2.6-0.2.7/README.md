# Comparing `tmp/relationalai-0.2.6.tar.gz` & `tmp/relationalai-0.2.7.tar.gz`

## Comparing `relationalai-0.2.6.tar` & `relationalai-0.2.7.tar`

### file list

```diff
@@ -1,512 +1,515 @@
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.2.6/README.md
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 relationalai-0.2.6/.github/actions/benchmarks/action.yml
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 relationalai-0.2.6/.github/actions/end-to-end/action.yml
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 relationalai-0.2.6/.github/workflows/benchmarks.yml
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 relationalai-0.2.6/.github/workflows/end-to-end.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 relationalai-0.2.6/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/README.md
--rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/getting_started.md
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/_old/OLD_pyrel_quickstart.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/_old/metamodel.md
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/_old/python_dsl.md
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/_old/quickstart.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/README.md
--rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/cli/README.md
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/configuration/README.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Expression.md
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Property.md
--rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/README.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Context/README.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Context/enter__.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Context/exit__.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Context/iter__.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Context/model.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Context/results.md
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/ContextSelect/README.md
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/ContextSelect/add.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/ContextSelect/call__.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/ContextSelect/getattribute__.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Instance/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Instance/persist.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Instance/set.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Instance/unpersist.md
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/InstanceProperty/README.md
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/InstanceProperty/or_.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/README.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/Type.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/found.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/name.md
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/not_found.md
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/ordered_choice.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/query.md
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/read.md
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/rule.md
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/scope.md
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/union.md
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/README.md
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/add__.md
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/enter__.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/eq__.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/exit__.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/floordiv__.md
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/ge__.md
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/getattribute__.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/gt__.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/le__.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/lt__.md
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/mul__.md
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/ne__.md
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/pow__.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/radd__.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/rfloordiv__.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/rmul__.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/rpow__.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/rsub__.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/rtruediv__.md
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/sub__.md
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/truediv__.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/README.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/add.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/call__.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/extend.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/model.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/name.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/or__.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/PrimaryKey.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/README.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/Snowflake.md
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/README.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/Vars.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/alias.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/README.md
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/avg.md
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/count.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/max.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/min.md
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/rank_asc.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/rank_desc.md
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/sum.md
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/README.md
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/README.md
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/avg_degree.md
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/degree.md
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/diameter_range.md
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/distance.md
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/indegree.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/infomap.md
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/is_connected.md
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/is_reachable.md
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/is_triangle.md
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/label_propagation.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/louvain.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/max_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/max_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/min_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/min_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/num_edges.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/num_nodes.md
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/num_triangles.md
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/outdegree.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/pagerank.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/reachable_from.md
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/triangles.md
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_distance.md
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/README.md
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/add.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/call__.md
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/extend.md
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/README.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/set.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/to.md
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/Edge.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/Node.md
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/README.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/compute.md
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/fetch.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/id.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/model.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/undirected.md
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/visualize.md
--rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
--rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/README.md
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/abs.md
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/cbrt.md
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/ceil.md
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/floor.md
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/isclose.md
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/log.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/sign.md
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/sqrt.md
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/trunc_divide.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/README.md
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/concat.md
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/contains.md
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/ends_with.md
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/join.md
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/length.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/like.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/lowercase.md
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/regex_compile.md
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/regex_match.md
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/replace.md
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/split.md
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/split_part.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/uppercase.md
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/sql/README.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/faq/README.md
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/faq/engines.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/cdc.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/custom_snowflake_connection.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/emit_playground.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/found.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/fraud.ipynb
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/fraud.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/graph_algos.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/load_raw.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/nested.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/or_types.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/remote_load_csv.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/requirements.txt
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/simple.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/simple_recursion.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/simple_streamlit.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/solver.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/weighted_graph_algos.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/articles_graph/README.md
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/articles_graph/articles_graph.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/articles_graph/articles_graph_with_nlp.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/articles_graph/pyproject.toml
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/articles_graph/utils.py
--rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/articles_graph/daily_articles/04_04_2024.json
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/data/people.csv
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/data/transactions.csv
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/ev_penetration/ev_penetration.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/ev_penetration/ev_penetration_csv.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/ev_penetration/state_stats.csv
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/imdb/README.md
--rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/imdb/imdb.csv
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/imdb/imdb.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/rel/bar.rel
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/rel/foo.rel
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/rel/solver.rel
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/social-money-network/SF_pagerank.ipynb
--rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/social-money-network/Simulation-and-SF-Upload.ipynb
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/social-money-network/snowflake_pagerank.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/README.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/index.html
--rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/package-lock.json
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/package.json
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/tsconfig.json
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/vite.config.ts
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/.storybook/main.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/.storybook/preview-body.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/.storybook/preview-head.html
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/.storybook/preview.ts
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/App.styl
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/App.tsx
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/Selection.tsx
--rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/debugger_client.ts
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/index.css
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/index.tsx
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/logo.svg
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/util.styl
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/util.ts
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/ws.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/assets/favicon.png
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/EventList.styl
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/EventList.tsx
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/EventViewer.styl
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/EventViewer.tsx
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Sidebar.styl
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Sidebar.tsx
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/index.stories.tsx
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/index.styl
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/index.tsx
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/base.styl
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/base.tsx
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/index.tsx
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Accordion.stories.tsx
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Accordion.styl
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Accordion.tsx
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Breadcrumbs.styl
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Breadcrumbs.tsx
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Button.styl
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Button.tsx
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Code.styl
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Code.tsx
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Collapsible.stories.tsx
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Collapsible.styl
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Collapsible.tsx
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Field.stories.tsx
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Field.styl
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Field.tsx
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Icon.styl
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Icon.tsx
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Modal.stories.tsx
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Modal.styl
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Modal.tsx
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Tooltip.stories.tsx
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Tooltip.styl
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Tooltip.tsx
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/branch-improved.json
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/branch.json
--rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/fraud.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/index.ts
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/not_found.json
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/simple.json
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/union.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/types/json.d.ts
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/types/jsx.d.ts
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/types/mech.d.ts
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/__init__.py
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/emit.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/exec.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/fixtures.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/patch.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/util.py
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/cli/__main__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/cli/collect_failures.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/cli/collect_tests.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/cli/repro.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/cli/run_tests.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/cli/watch.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/action.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/context.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/document.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/error.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/group_limited.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/ir.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/scope.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/staged.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/task.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/test.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/harness/database.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/harness/vendor_types.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/validate/diff.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/validate/errors.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/validate/mapping.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/validate/roundtrip.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/__init__.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/compiler.py
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/debugging.py
--rw-r--r--   0        0        0    46119 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/dsl.py
--rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/errors.py
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/metagen.py
--rw-r--r--   0        0        0    27989 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/metamodel.py
--rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/rel.py
--rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/rel2.py
--rw-r--r--   0        0        0    13261 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/rel_emitter.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/rel_utils.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/analysis/mechanistic.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/analysis/whynot.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/__init__.py
--rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/azure.py
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/client.py
--rw-r--r--   0        0        0    18211 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/config.py
--rw-r--r--   0        0        0    37351 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/snowflake.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/test.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/types.py
--rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/loaders/csv.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/loaders/loader.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/loaders/types.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/std/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/std/aggregates.py
--rw-r--r--   0        0        0    18717 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/std/graphs.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/std/math.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/std/strings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/__init__.py
--rw-r--r--   0        0        0    51586 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/cli.py
--rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/cli_controls.py
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/debugger.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/debugger_server.py
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/dev.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/notes
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/util/keys.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/util/snowflake_logger.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/util/tracing_logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/conftest.py
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/util.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/benchmarks/conftest.py
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/benchmarks/test_tastybytes.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/conftest.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_graph_visualize.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_snapshots.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query0.txt
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query1.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query2.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query2.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query1.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query2.txt
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query3.txt
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query4.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query0.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query2.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query3.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query4.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query5.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query6.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query7.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query8.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query9.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query10.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query7.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query8.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query9.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/agg_ordering.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/bool.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/bottom.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/export.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/first.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/math.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/multi_valued.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/not_found.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/out_of_context.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/persist.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/smoke.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/strings.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/top.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/union.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/weighted_graphs.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/basics.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/centrality.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/community.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/connectivity.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/degree.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/distance.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/link_prediction.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/similarity.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/triangles.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/test_core.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/test_examples.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/basic/smoketest.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/found/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/test/query0.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/init-cli/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/init-cli/azure_basic.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/init-cli/common.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/roundtrip/test_document.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/roundtrip/test_task.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.6/.gitignore
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 relationalai-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/pypi/README.md
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 relationalai-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.2.7/README.md
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 relationalai-0.2.7/.github/actions/benchmarks/action.yml
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 relationalai-0.2.7/.github/actions/end-to-end/action.yml
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 relationalai-0.2.7/.github/workflows/benchmarks.yml
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 relationalai-0.2.7/.github/workflows/end-to-end.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 relationalai-0.2.7/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/README.md
+-rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/getting_started.md
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/_old/OLD_pyrel_quickstart.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/_old/metamodel.md
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/_old/python_dsl.md
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/_old/quickstart.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/README.md
+-rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/cli/README.md
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/configuration/README.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Expression.md
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Property.md
+-rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Context/README.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Context/enter__.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Context/exit__.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Context/iter__.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Context/model.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Context/results.md
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/ContextSelect/README.md
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/ContextSelect/add.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/ContextSelect/call__.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/ContextSelect/getattribute__.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Instance/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Instance/persist.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Instance/set.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Instance/unpersist.md
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/InstanceProperty/README.md
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/InstanceProperty/or_.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/README.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/Type.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/found.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/name.md
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/not_found.md
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/ordered_choice.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/query.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/read.md
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/rule.md
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/scope.md
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/union.md
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/README.md
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/add__.md
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/enter__.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/eq__.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/exit__.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/floordiv__.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/ge__.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/getattribute__.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/gt__.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/le__.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/lt__.md
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/mul__.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/ne__.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/pow__.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/radd__.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/rfloordiv__.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/rmul__.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/rpow__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/rsub__.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/rtruediv__.md
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/sub__.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/truediv__.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/README.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/add.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/call__.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/extend.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/model.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/name.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/or__.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/PrimaryKey.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/README.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/Snowflake.md
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/README.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/Vars.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/alias.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/avg.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/count.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/max.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/min.md
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/rank_asc.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/rank_desc.md
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/sum.md
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/README.md
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/README.md
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/avg_degree.md
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/degree.md
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/diameter_range.md
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/distance.md
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/indegree.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/infomap.md
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/is_connected.md
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/is_reachable.md
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/is_triangle.md
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/label_propagation.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/louvain.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/max_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/max_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/min_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/min_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/num_edges.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/num_nodes.md
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/num_triangles.md
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/outdegree.md
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/pagerank.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/reachable_from.md
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/triangles.md
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_distance.md
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/README.md
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/add.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/call__.md
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/extend.md
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/set.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/to.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/Edge.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/Node.md
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/README.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/compute.md
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/fetch.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/id.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/model.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/undirected.md
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/visualize.md
+-rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
+-rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/README.md
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/abs.md
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/cbrt.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/ceil.md
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/floor.md
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/isclose.md
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/log.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/sign.md
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/sqrt.md
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/trunc_divide.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/README.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/concat.md
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/contains.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/ends_with.md
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/join.md
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/length.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/like.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/lowercase.md
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/regex_compile.md
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/regex_match.md
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/replace.md
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/split.md
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/split_part.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/uppercase.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/sql/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/faq/README.md
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/faq/engines.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/cdc.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/custom_snowflake_connection.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/emit_playground.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/found.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/fraud.ipynb
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/fraud.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/graph_algos.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/load_raw.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/nested.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/or_types.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/remote_load_csv.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/requirements.txt
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/simple.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/simple_recursion.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/simple_streamlit.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/solver.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/weighted_graph_algos.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/articles_graph/README.md
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/articles_graph/articles_graph.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/articles_graph/articles_graph_with_nlp.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/articles_graph/pyproject.toml
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/articles_graph/utils.py
+-rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/articles_graph/daily_articles/04_04_2024.json
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/data/people.csv
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/data/transactions.csv
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/ev_penetration/ev_penetration.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/ev_penetration/ev_penetration_csv.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/ev_penetration/state_stats.csv
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/imdb/README.md
+-rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/imdb/imdb.csv
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/imdb/imdb.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/rel/bar.rel
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/rel/foo.rel
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/rel/solver.rel
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/social-money-network/SF_pagerank.ipynb
+-rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/social-money-network/Simulation-and-SF-Upload.ipynb
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/social-money-network/snowflake_pagerank.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/README.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/index.html
+-rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/package-lock.json
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/package.json
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/tsconfig.json
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/vite.config.ts
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/.storybook/main.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/.storybook/preview-body.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/.storybook/preview-head.html
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/.storybook/preview.ts
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/App.styl
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/App.tsx
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/Selection.tsx
+-rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/debugger_client.ts
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/index.css
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/index.tsx
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/logo.svg
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/util.styl
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/util.ts
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/ws.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/assets/favicon.png
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/EventList.styl
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/EventList.tsx
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/EventViewer.styl
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/EventViewer.tsx
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Sidebar.styl
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/index.stories.tsx
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/index.styl
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/index.tsx
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/base.styl
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/base.tsx
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/index.tsx
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Accordion.stories.tsx
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Accordion.styl
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Accordion.tsx
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Breadcrumbs.styl
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Breadcrumbs.tsx
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Button.styl
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Button.tsx
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Code.styl
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Code.tsx
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Collapsible.stories.tsx
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Collapsible.styl
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Collapsible.tsx
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Field.stories.tsx
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Field.styl
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Field.tsx
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Icon.styl
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Icon.tsx
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Modal.stories.tsx
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Modal.styl
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Modal.tsx
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Tooltip.stories.tsx
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Tooltip.styl
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Tooltip.tsx
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/branch-improved.json
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/branch.json
+-rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/fraud.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/index.ts
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/not_found.json
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/simple.json
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/union.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/types/json.d.ts
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/types/jsx.d.ts
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/types/mech.d.ts
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/__init__.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/emit.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/exec.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/fixtures.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/patch.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/util.py
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/cli/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/cli/collect_failures.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/cli/collect_tests.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/cli/repro.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/cli/run_tests.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/cli/watch.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/action.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/context.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/document.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/error.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/group_limited.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/ir.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/scope.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/staged.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/task.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/test.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/harness/database.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/harness/vendor_types.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/validate/diff.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/validate/errors.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/validate/mapping.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/validate/roundtrip.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/compiler.py
+-rw-r--r--   0        0        0    11634 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/debugging.py
+-rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/dsl.py
+-rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/errors.py
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/metagen.py
+-rw-r--r--   0        0        0    27989 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/metamodel.py
+-rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/rel.py
+-rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/rel2.py
+-rw-r--r--   0        0        0    13261 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/rel_emitter.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/rel_utils.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/analysis/mechanistic.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/analysis/whynot.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/__init__.py
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/azure.py
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/client.py
+-rw-r--r--   0        0        0    18211 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/config.py
+-rw-r--r--   0        0        0    37604 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/snowflake.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/types.py
+-rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/loaders/csv.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/loaders/loader.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/loaders/types.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/std/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/std/aggregates.py
+-rw-r--r--   0        0        0    18717 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/std/graphs.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/std/math.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/std/strings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/__init__.py
+-rw-r--r--   0        0        0    54404 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/cli.py
+-rw-r--r--   0        0        0    12721 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/cli_controls.py
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/debugger.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/debugger_server.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/dev.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/notes
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/util/keys.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/util/snowflake_logger.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/util/tracing_logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/conftest.py
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/util.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/benchmarks/conftest.py
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/benchmarks/test_tastybytes.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/conftest.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_graph_visualize.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_snapshots.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query1.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query0.txt
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query1.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query2.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query2.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query1.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query2.txt
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query3.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query4.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query0.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query2.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query3.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query4.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query5.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query6.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query7.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query8.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query9.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query10.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query7.txt
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query8.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query9.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/after_errors.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/agg_ordering.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/bool.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/bottom.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/export.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/first.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/multi_valued.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/not_found.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/out_of_context.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/persist.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/smoke.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/std_math.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/strings.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/top.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/union.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/weighted_graphs.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/basics.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/centrality.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/community.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/connectivity.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/degree.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/distance.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/link_prediction.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/similarity.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/triangles.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/test_core.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/test_examples.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/basic/smoketest.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/found/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/test/query0.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/init-cli/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/init-cli/azure_basic.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/init-cli/common.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/roundtrip/test_document.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/roundtrip/test_task.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 relationalai-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/pypi/README.md
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 relationalai-0.2.7/PKG-INFO
```

### Comparing `relationalai-0.2.6/README.md` & `relationalai-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/.github/actions/benchmarks/action.yml` & `relationalai-0.2.7/.github/actions/benchmarks/action.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/.github/actions/end-to-end/action.yml` & `relationalai-0.2.7/.github/actions/end-to-end/action.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/.github/workflows/benchmarks.yml` & `relationalai-0.2.7/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/.github/workflows/end-to-end.yml` & `relationalai-0.2.7/.github/workflows/end-to-end.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/.github/workflows/publish-to-pypi.yml` & `relationalai-0.2.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/.github/workflows/ruff.yml` & `relationalai-0.2.7/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/getting_started.md` & `relationalai-0.2.7/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/_old/OLD_pyrel_quickstart.md` & `relationalai-0.2.7/docs/_old/OLD_pyrel_quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/_old/metamodel.md` & `relationalai-0.2.7/docs/_old/metamodel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/_old/python_dsl.md` & `relationalai-0.2.7/docs/_old/python_dsl.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/_old/quickstart.md` & `relationalai-0.2.7/docs/_old/quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/cli/README.md` & `relationalai-0.2.7/docs/api_reference/cli/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/configuration/README.md` & `relationalai-0.2.7/docs/api_reference/configuration/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Expression.md` & `relationalai-0.2.7/docs/api_reference/python/Expression.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Property.md` & `relationalai-0.2.7/docs/api_reference/python/Property.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/README.md` & `relationalai-0.2.7/docs/api_reference/python/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Context/README.md` & `relationalai-0.2.7/docs/api_reference/python/Context/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Context/enter__.md` & `relationalai-0.2.7/docs/api_reference/python/Context/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Context/exit__.md` & `relationalai-0.2.7/docs/api_reference/python/Context/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Context/iter__.md` & `relationalai-0.2.7/docs/api_reference/python/Context/iter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Context/model.md` & `relationalai-0.2.7/docs/api_reference/python/Context/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Context/results.md` & `relationalai-0.2.7/docs/api_reference/python/Context/results.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/ContextSelect/README.md` & `relationalai-0.2.7/docs/api_reference/python/ContextSelect/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/ContextSelect/add.md` & `relationalai-0.2.7/docs/api_reference/python/ContextSelect/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/ContextSelect/call__.md` & `relationalai-0.2.7/docs/api_reference/python/ContextSelect/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/ContextSelect/getattribute__.md` & `relationalai-0.2.7/docs/api_reference/python/ContextSelect/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Instance/README.md` & `relationalai-0.2.7/docs/api_reference/python/Instance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Instance/persist.md` & `relationalai-0.2.7/docs/api_reference/python/Instance/persist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Instance/set.md` & `relationalai-0.2.7/docs/api_reference/python/Instance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Instance/unpersist.md` & `relationalai-0.2.7/docs/api_reference/python/Instance/unpersist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/InstanceProperty/README.md` & `relationalai-0.2.7/docs/api_reference/python/InstanceProperty/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/InstanceProperty/or_.md` & `relationalai-0.2.7/docs/api_reference/python/InstanceProperty/or_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Model/README.md` & `relationalai-0.2.7/docs/api_reference/python/Model/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Model/Type.md` & `relationalai-0.2.7/docs/api_reference/python/Model/Type.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Model/found.md` & `relationalai-0.2.7/docs/api_reference/python/Model/found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Model/not_found.md` & `relationalai-0.2.7/docs/api_reference/python/Model/not_found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Model/ordered_choice.md` & `relationalai-0.2.7/docs/api_reference/python/Model/ordered_choice.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Model/query.md` & `relationalai-0.2.7/docs/api_reference/python/Model/query.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Model/read.md` & `relationalai-0.2.7/docs/api_reference/python/Model/read.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Model/rule.md` & `relationalai-0.2.7/docs/api_reference/python/Model/rule.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Model/scope.md` & `relationalai-0.2.7/docs/api_reference/python/Model/scope.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Model/union.md` & `relationalai-0.2.7/docs/api_reference/python/Model/union.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/README.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/add__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/add__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/enter__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/eq__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/eq__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/exit__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/floordiv__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/floordiv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/ge__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/ge__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/getattribute__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/gt__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/gt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/le__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/le__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/lt__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/lt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/mul__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/mul__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/ne__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/ne__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/pow__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/pow__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/sub__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/sub__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Producer/truediv__.md` & `relationalai-0.2.7/docs/api_reference/python/Producer/truediv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Type/README.md` & `relationalai-0.2.7/docs/api_reference/python/Type/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Type/add.md` & `relationalai-0.2.7/docs/api_reference/python/Type/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Type/call__.md` & `relationalai-0.2.7/docs/api_reference/python/Type/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Type/extend.md` & `relationalai-0.2.7/docs/api_reference/python/Type/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/Type/or__.md` & `relationalai-0.2.7/docs/api_reference/python/Type/or__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/clients/README.md` & `relationalai-0.2.7/docs/api_reference/python/clients/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/PrimaryKey.md` & `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/PrimaryKey.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/README.md` & `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/Snowflake.md` & `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/Snowflake.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md` & `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md` & `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md` & `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md` & `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/README.md` & `relationalai-0.2.7/docs/api_reference/python/std/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/Vars.md` & `relationalai-0.2.7/docs/api_reference/python/std/Vars.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/alias.md` & `relationalai-0.2.7/docs/api_reference/python/std/alias.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/aggregates/README.md` & `relationalai-0.2.7/docs/api_reference/python/std/aggregates/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/aggregates/avg.md` & `relationalai-0.2.7/docs/api_reference/python/std/aggregates/avg.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/aggregates/count.md` & `relationalai-0.2.7/docs/api_reference/python/std/aggregates/count.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/aggregates/max.md` & `relationalai-0.2.7/docs/api_reference/python/std/aggregates/max.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/aggregates/min.md` & `relationalai-0.2.7/docs/api_reference/python/std/aggregates/min.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/aggregates/rank_asc.md` & `relationalai-0.2.7/docs/api_reference/python/std/aggregates/rank_asc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/aggregates/rank_desc.md` & `relationalai-0.2.7/docs/api_reference/python/std/aggregates/rank_desc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/aggregates/sum.md` & `relationalai-0.2.7/docs/api_reference/python/std/aggregates/sum.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/README.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/README.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/adamic_adar.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/adamic_adar.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/avg_degree.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/avg_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/avg_indegree.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/avg_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/common_neighbor.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/common_neighbor.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/degree.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/degree_centrality.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/diameter_range.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/diameter_range.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/distance.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/distance.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/indegree.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/infomap.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/infomap.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/is_connected.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/is_connected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/is_reachable.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/is_reachable.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/is_triangle.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/is_triangle.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/label_propagation.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/label_propagation.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/louvain.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/louvain.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/max_degree.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/max_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/max_indegree.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/max_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/max_outdegree.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/max_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/min_degree.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/min_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/min_indegree.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/min_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/min_outdegree.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/min_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/num_edges.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/num_edges.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/num_nodes.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/num_nodes.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/num_triangles.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/num_triangles.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/outdegree.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/pagerank.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/pagerank.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/reachable_from.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/reachable_from.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/triangles.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/triangles.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_distance.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_distance.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/README.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/add.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/call__.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/extend.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/README.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/from_.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/from_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/set.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/to.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/to.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/Edge.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/Edge.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/Node.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/Node.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/README.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/compute.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/compute.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/fetch.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/fetch.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/id.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/id.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/model.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/undirected.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/undirected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/visualize.md` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/visualize.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png` & `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/math/abs.md` & `relationalai-0.2.7/docs/api_reference/python/std/math/abs.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/math/cbrt.md` & `relationalai-0.2.7/docs/api_reference/python/std/math/cbrt.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/math/ceil.md` & `relationalai-0.2.7/docs/api_reference/python/std/math/ceil.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/math/floor.md` & `relationalai-0.2.7/docs/api_reference/python/std/math/floor.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/math/isclose.md` & `relationalai-0.2.7/docs/api_reference/python/std/math/isclose.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/math/log.md` & `relationalai-0.2.7/docs/api_reference/python/std/math/log.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/math/sign.md` & `relationalai-0.2.7/docs/api_reference/python/std/math/sign.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/math/sqrt.md` & `relationalai-0.2.7/docs/api_reference/python/std/math/sqrt.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/math/trunc_divide.md` & `relationalai-0.2.7/docs/api_reference/python/std/math/trunc_divide.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/README.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/concat.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/concat.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/contains.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/contains.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/ends_with.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/ends_with.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/join.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/join.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/length.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/length.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/like.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/like.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/lowercase.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/lowercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/regex_compile.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/regex_compile.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/regex_match.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/regex_match.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/replace.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/replace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/split.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/split.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/split_part.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/split_part.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/api_reference/python/std/strings/uppercase.md` & `relationalai-0.2.7/docs/api_reference/python/std/strings/uppercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/docs/faq/engines.md` & `relationalai-0.2.7/docs/faq/engines.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/README.md` & `relationalai-0.2.7/examples/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/cdc.py` & `relationalai-0.2.7/examples/cdc.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/custom_snowflake_connection.py` & `relationalai-0.2.7/examples/custom_snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/emit_playground.py` & `relationalai-0.2.7/examples/emit_playground.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/found.py` & `relationalai-0.2.7/examples/found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/fraud.ipynb` & `relationalai-0.2.7/examples/fraud.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/fraud.py` & `relationalai-0.2.7/examples/fraud.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/graph_algos.py` & `relationalai-0.2.7/examples/graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/nested.py` & `relationalai-0.2.7/examples/nested.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/or_types.py` & `relationalai-0.2.7/examples/or_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/remote_load_csv.py` & `relationalai-0.2.7/examples/remote_load_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/simple_recursion.py` & `relationalai-0.2.7/examples/simple_recursion.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/simple_streamlit.py` & `relationalai-0.2.7/examples/simple_streamlit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/solver.py` & `relationalai-0.2.7/examples/solver.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/weighted_graph_algos.py` & `relationalai-0.2.7/examples/weighted_graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/articles_graph/README.md` & `relationalai-0.2.7/examples/articles_graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/articles_graph/articles_graph.py` & `relationalai-0.2.7/examples/articles_graph/articles_graph.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/articles_graph/articles_graph_with_nlp.py` & `relationalai-0.2.7/examples/articles_graph/articles_graph_with_nlp.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/articles_graph/utils.py` & `relationalai-0.2.7/examples/articles_graph/utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/articles_graph/daily_articles/04_04_2024.json` & `relationalai-0.2.7/examples/articles_graph/daily_articles/04_04_2024.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/data/people.csv` & `relationalai-0.2.7/examples/data/people.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/data/transactions.csv` & `relationalai-0.2.7/examples/data/transactions.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/ev_penetration/ev_penetration.py` & `relationalai-0.2.7/examples/ev_penetration/ev_penetration.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/ev_penetration/ev_penetration_csv.py` & `relationalai-0.2.7/examples/ev_penetration/ev_penetration_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/ev_penetration/state_stats.csv` & `relationalai-0.2.7/examples/ev_penetration/state_stats.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/imdb/README.md` & `relationalai-0.2.7/examples/imdb/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/imdb/imdb.csv` & `relationalai-0.2.7/examples/imdb/imdb.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/imdb/imdb.py` & `relationalai-0.2.7/examples/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/rel/solver.rel` & `relationalai-0.2.7/examples/rel/solver.rel`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/social-money-network/SF_pagerank.ipynb` & `relationalai-0.2.7/examples/social-money-network/SF_pagerank.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/social-money-network/Simulation-and-SF-Upload.ipynb` & `relationalai-0.2.7/examples/social-money-network/Simulation-and-SF-Upload.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/examples/social-money-network/snowflake_pagerank.py` & `relationalai-0.2.7/examples/social-money-network/snowflake_pagerank.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/package-lock.json` & `relationalai-0.2.7/frontend/debugger/package-lock.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/package.json` & `relationalai-0.2.7/frontend/debugger/package.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/tsconfig.json` & `relationalai-0.2.7/frontend/debugger/tsconfig.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/vite.config.ts` & `relationalai-0.2.7/frontend/debugger/vite.config.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/.storybook/main.ts` & `relationalai-0.2.7/frontend/debugger/.storybook/main.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/App.styl` & `relationalai-0.2.7/frontend/debugger/src/App.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/App.tsx` & `relationalai-0.2.7/frontend/debugger/src/App.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/Selection.tsx` & `relationalai-0.2.7/frontend/debugger/src/Selection.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/debugger_client.ts` & `relationalai-0.2.7/frontend/debugger/src/debugger_client.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/index.tsx` & `relationalai-0.2.7/frontend/debugger/src/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/logo.svg` & `relationalai-0.2.7/frontend/debugger/src/logo.svg`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/util.styl` & `relationalai-0.2.7/frontend/debugger/src/util.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/util.ts` & `relationalai-0.2.7/frontend/debugger/src/util.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/assets/favicon.png` & `relationalai-0.2.7/frontend/debugger/src/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/EventList.styl` & `relationalai-0.2.7/frontend/debugger/src/components/EventList.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/EventList.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/EventList.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/EventViewer.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/EventViewer.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Sidebar.styl` & `relationalai-0.2.7/frontend/debugger/src/components/Sidebar.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Sidebar.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/ScopeProvider.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/ScopeProvider.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/index.stories.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/index.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/index.styl` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/index.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/index.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/base.styl` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/base.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/base.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/base.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/index.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Accordion.stories.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Accordion.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Accordion.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Accordion.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Breadcrumbs.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Breadcrumbs.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Button.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Button.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Code.styl` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Code.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Code.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Code.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Collapsible.stories.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Collapsible.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Collapsible.styl` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Collapsible.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Collapsible.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Collapsible.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Field.stories.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Field.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Field.styl` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Field.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Field.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Field.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Icon.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Icon.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Modal.stories.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Modal.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Modal.styl` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Modal.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Modal.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Modal.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Tooltip.stories.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Tooltip.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Tooltip.styl` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Tooltip.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/components/ui/Tooltip.tsx` & `relationalai-0.2.7/frontend/debugger/src/components/ui/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/fixtures/branch-improved.json` & `relationalai-0.2.7/frontend/debugger/src/fixtures/branch-improved.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/fixtures/branch.json` & `relationalai-0.2.7/frontend/debugger/src/fixtures/branch.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/fixtures/fraud.json` & `relationalai-0.2.7/frontend/debugger/src/fixtures/fraud.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/fixtures/not_found.json` & `relationalai-0.2.7/frontend/debugger/src/fixtures/not_found.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/fixtures/simple.json` & `relationalai-0.2.7/frontend/debugger/src/fixtures/simple.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/fixtures/union.json` & `relationalai-0.2.7/frontend/debugger/src/fixtures/union.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/frontend/debugger/src/types/mech.d.ts` & `relationalai-0.2.7/frontend/debugger/src/types/mech.d.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/README.md` & `relationalai-0.2.7/src/gentest/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/emit.py` & `relationalai-0.2.7/src/gentest/emit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/exec.py` & `relationalai-0.2.7/src/gentest/exec.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/fixtures.py` & `relationalai-0.2.7/src/gentest/fixtures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/patch.py` & `relationalai-0.2.7/src/gentest/patch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/util.py` & `relationalai-0.2.7/src/gentest/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/cli/__main__.py` & `relationalai-0.2.7/src/gentest/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/cli/collect_failures.py` & `relationalai-0.2.7/src/gentest/cli/collect_failures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/cli/collect_tests.py` & `relationalai-0.2.7/src/gentest/cli/collect_tests.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/cli/repro.py` & `relationalai-0.2.7/src/gentest/cli/repro.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/cli/watch.py` & `relationalai-0.2.7/src/gentest/cli/watch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/gen/action.py` & `relationalai-0.2.7/src/gentest/gen/action.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/gen/context.py` & `relationalai-0.2.7/src/gentest/gen/context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/gen/document.py` & `relationalai-0.2.7/src/gentest/gen/document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/gen/group_limited.py` & `relationalai-0.2.7/src/gentest/gen/group_limited.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/gen/ir.py` & `relationalai-0.2.7/src/gentest/gen/ir.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/gen/scope.py` & `relationalai-0.2.7/src/gentest/gen/scope.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/gen/task.py` & `relationalai-0.2.7/src/gentest/gen/task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/gen/test.py` & `relationalai-0.2.7/src/gentest/gen/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/harness/database.py` & `relationalai-0.2.7/src/gentest/harness/database.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/validate/diff.py` & `relationalai-0.2.7/src/gentest/validate/diff.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/validate/errors.py` & `relationalai-0.2.7/src/gentest/validate/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/validate/mapping.py` & `relationalai-0.2.7/src/gentest/validate/mapping.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/gentest/validate/roundtrip.py` & `relationalai-0.2.7/src/gentest/validate/roundtrip.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/__init__.py` & `relationalai-0.2.7/src/relationalai/__init__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/compiler.py` & `relationalai-0.2.7/src/relationalai/compiler.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/debugging.py` & `relationalai-0.2.7/src/relationalai/debugging.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,19 +95,19 @@
         "span": span,
     })
     return span
 
 def span_end(span):
     if not DEBUG:
         return
-    
+
     global TIP_SPAN
     TIP_SPAN = span.parent
     span.mark_finished()
-    
+
     logger.debug({
         "event": "span_end",
         "id": str(span.id),
         "end_timestamp": span.end_timestamp,
         "end_attrs": span.end_attrs,
     })
 
@@ -118,21 +118,21 @@
         self.type = type
         self.attrs = attrs
         # additional attributes added during the lifetime of the span
         self.end_attrs = {}
         # Would use `datetime.datetime.now(datetime.UTC)`, but it only works in 3.11.
         self.start_timestamp = datetime.datetime.utcnow()
         self.end_timestamp = None
-    
+
     def mark_finished(self):
         self.end_timestamp = datetime.datetime.utcnow()
-    
+
     def __setitem__(self, key, value):
         self.end_attrs[key] = value
-    
+
     def to_json(self):
         return {
             "type": self.type,
             "id": str(self.id),
             "parent_id": str(self.parent.id) if self.parent else None,
             "start_timestamp": self.start_timestamp.isoformat(),
             "end_timestamp": None if self.end_timestamp is None else self.end_timestamp.isoformat(),
@@ -218,21 +218,32 @@
     def __init__(self):
         self.dirty_cells = set()
         try:
             from IPython import get_ipython # type: ignore
             self.ipython = get_ipython()
             if self.ipython:
                 self.ipython.events.register('pre_run_cell', self.pre_run_cell)
+                self.ipython.events.register('post_run_cell', self.post_run_cell)
                 self.dirty_cells.add(self.cell())
         except ImportError:
             self.ipython = None
 
     def pre_run_cell(self, info):
         self.dirty_cells.add(info.cell_id)
 
+    def post_run_cell(self, result):
+        try:
+            from . import dsl
+            graph = dsl.get_graph()
+            if graph._temp_is_active():
+                graph._flush_temp()
+                graph._restore_temp()
+        except Exception:
+            return
+
     def cell_content(self):
         if self.ipython:
             last_input = self.ipython.user_ns['In'][-1]
             return (last_input, f"In[{len(self.ipython.user_ns['In'])}]")
         return ("", "")
 
     def is_colab(self):
```

### Comparing `relationalai-0.2.6/src/relationalai/dsl.py` & `relationalai-0.2.7/src/relationalai/dsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     def __rsub__(self, other):
         return self._wrapped_op(Builtins.minus, other, self)
 
     def __truediv__(self, other):
         return self._wrapped_op(Builtins.div, self, other)
     def __rtruediv__(self, other):
         return self._wrapped_op(Builtins.div, other, self)
-    
+
     def __floordiv__(self, other):
         return self._wrapped_op(Builtins.floor_div, self, other)
     def __rfloordiv__(self, other):
         return self._wrapped_op(Builtins.floor_div, other, self)
 
     def __pow__(self, other):
         return self._wrapped_op(Builtins.pow, self, other)
@@ -673,14 +673,15 @@
 #--------------------------------------------------
 
 class Expression(Producer):
     def __init__(self, graph:'Graph', op:mType|Task, args:List[Any]):
 
         super().__init__(graph, [])
         self._var = None
+        self._context = graph._stack.active()
 
         # For calls to tasks with known signatures, normalize their arguments by
         # throwing on missing inputs or constructing vars for missing outputs
         if op.properties and not op.isa(Builtins.Anonymous):
             for prop, arg in zip_longest(op.properties, args):
                 if arg is None:
                     if prop.is_input:
@@ -700,14 +701,16 @@
         raise Exception("Expressions can't be called")
 
     def _use_var(self):
         if not self._var:
             self._var = Var(Builtins.Unknown)
             prop = build.property_named("result", self._expr.types)
             self._expr.append(prop, self._var)
+        if not self._graph._stack.contains(self._context):
+            Errors.variable_out_of_context(Errors.call_source(), self._var.name or "a result")
 
     def _make_sub(self, name: str, existing=None):
         if existing is not None and existing._instance._context is self._graph._stack.active():
             return existing
         return getattr(Instance(self._graph, ActionType.Get, [self], {}), name)
 
 #--------------------------------------------------
@@ -1061,15 +1064,15 @@
 #--------------------------------------------------
 # Graph
 #--------------------------------------------------
 
 locals = threading.local()
 locals.graph_stack = []
 
-def get_graph():
+def get_graph() -> 'Graph':
     _ensure_stack()
     if not len(locals.graph_stack):
         raise Exception("Outside of a model context")
     return locals.graph_stack[-1]
 
 def _ensure_stack():
     if not hasattr(locals, "graph_stack"):
@@ -1103,32 +1106,43 @@
         _ensure_stack().append(self)
         self._stack.push(self._temp_rule)
 
     #--------------------------------------------------
     # Rule stack
     #--------------------------------------------------
 
-    def _push(self, item):
-        _ensure_stack().append(self)
+    def _flush_temp(self):
         if self._temp_rule:
             self._pop(self._temp_rule, is_temp=True)
             if not len(_ensure_stack()):
                 _ensure_stack().append(self)
             self._temp_rule = None
+
+    def _restore_temp(self):
+        self._temp_rule = Context(self)
+        _ensure_stack().append(self)
+        self._stack.push(self._temp_rule)
+
+    def _temp_is_active(self):
+        return self._temp_rule and len(self._stack.items) > 1
+
+    def _push(self, item):
+        _ensure_stack().append(self)
+        self._flush_temp()
         self._stack.push(item)
 
     def _pop(self, item, exec=True, is_temp=False):
         _ensure_stack().pop()
         task = self._stack.pop(item)
-        if exec and task:
-            self._exec(item, task)
-        if not is_temp and not len(self._stack.stack):
-            self._temp_rule = Context(self)
-            _ensure_stack().append(self)
-            self._stack.push(self._temp_rule)
+        try:
+            if exec and task:
+                self._exec(item, task)
+        finally:
+            if not is_temp and not len(self._stack.stack):
+                self._restore_temp()
 
     def _action(self, action:Action|List[Action]):
         if isinstance(action, list):
             for a in action:
                 self._action(a)
             return
         self._stack.items.append(action)
```

### Comparing `relationalai-0.2.6/src/relationalai/errors.py` & `relationalai-0.2.7/src/relationalai/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/metagen.py` & `relationalai-0.2.7/src/relationalai/metagen.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/metamodel.py` & `relationalai-0.2.7/src/relationalai/metamodel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/rel.py` & `relationalai-0.2.7/src/relationalai/rel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/rel2.py` & `relationalai-0.2.7/src/relationalai/rel2.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/rel_emitter.py` & `relationalai-0.2.7/src/relationalai/rel_emitter.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/rel_utils.py` & `relationalai-0.2.7/src/relationalai/rel_utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/analysis/mechanistic.py` & `relationalai-0.2.7/src/relationalai/analysis/mechanistic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/analysis/whynot.py` & `relationalai-0.2.7/src/relationalai/analysis/whynot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/clients/azure.py` & `relationalai-0.2.7/src/relationalai/clients/azure.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 #--------------------------------------------------
 # Constants
 #--------------------------------------------------
 
 UNIXEPOCH = 62135683200000
 MILLISECONDS_PER_DAY = 24 * 60 * 60 * 1000
+VALID_ENGINE_STATES = ["REQUESTED", "PROVISIONED", "PROVISIONING"]
 
 #--------------------------------------------------
 # Resources
 #--------------------------------------------------
 
 class Resources(ResourceProvider):
     def __init__(self, profile:str|None=None, config:Config|None=None):
@@ -50,20 +51,23 @@
     def get_version(self):
         raise Exception("Azure version not available")
 
     #--------------------------------------------------
     # Engines
     #--------------------------------------------------
 
-    def list_engines(self):
-        return api.list_engines(self._api_ctx())
+    def list_engines(self, state:str|None = None):
+        return api.list_engines(self._api_ctx(), state)
 
     def get_engine(self, name:str):
         return api.get_engine(self._api_ctx(), name)
 
+    def is_valid_engine_state(self, state:str):
+        return state in VALID_ENGINE_STATES
+
     def create_engine(self, name:str, size:str, pool:str=""):
         with debugging.span("create_engine", name=name, size=size):
             return api.create_engine_wait(self._api_ctx(), name, size)
 
     def delete_engine(self, name:str):
         return api.delete_engine(self._api_ctx(), name)
```

### Comparing `relationalai-0.2.6/src/relationalai/clients/client.py` & `relationalai-0.2.7/src/relationalai/clients/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,22 +91,26 @@
         pass
 
     #--------------------------------------------------
     # Engines
     #--------------------------------------------------
 
     @abstractmethod
-    def list_engines(self) -> List[Any]:
+    def list_engines(self, state: str|None = None) -> List[Any]:
         pass
 
     @abstractmethod
     def get_engine(self, name: str):
         pass
 
     @abstractmethod
+    def is_valid_engine_state(self, name: str):
+        pass
+
+    @abstractmethod
     def create_engine(self, name: str, size: str, pool:str=""):
         pass
 
     @abstractmethod
     def delete_engine(self, name: str):
         pass
```

### Comparing `relationalai-0.2.6/src/relationalai/clients/config.py` & `relationalai-0.2.7/src/relationalai/clients/config.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/clients/snowflake.py` & `relationalai-0.2.7/src/relationalai/clients/snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 #--------------------------------------------------
 # Constants
 #--------------------------------------------------
 
 USE_EXEC_ASYNC = True
 VALID_POOL_STATUS = ["ACTIVE", "IDLE", "SUSPENDED"]
+VALID_ENGINE_STATES = ["READY", "PENDING"]
 COMPUTE_POOL_MAP = {
     "STANDARD_1": "XS",
     "CPU_X64_XS": "XS",
     "CPU_X64_S": "XS",
     "CPU_X64_M": "S",
     "HIGHMEM_X64_S": "M",
     "HIGH_MEMORY_4": "L",
@@ -127,15 +128,15 @@
             )
         except Exception as e:
             orig_message = str(e).lower()
             rai_app = self.config.get("rai_app_name", "")
             if re.search(f"database '{rai_app}' does not exist or not authorized.".lower(), orig_message):
                 print("\n")
                 Errors.snowflake_app_missing(rai_app)
-            elif re.search(r"JavaScript execution error", orig_message):
+            elif re.search(r"javascript execution error", orig_message):
                 match = re.search(r"\"message\":\"(.*)\"", orig_message)
                 if match:
                     message = match.group(1)
                     if "engine was deleted" in message or "engine not found" in message:
                         Errors.engine_not_found(self.config.get('engine', "Unknown"), message)
                     else:
                         raise RAIException(message) from None
@@ -145,30 +146,35 @@
     def reset(self):
         self._conn = None
 
     #--------------------------------------------------
     # Engines
     #--------------------------------------------------
 
-    def list_engines(self):
-        results = self._exec(f"select NAME, SIZE, STATUS from {APP_NAME}.api.engines")
+    def list_engines(self, state: str|None = None):
+        where_clause = f"WHERE STATUS = '{state}'" if state else ""
+        statement = f"select NAME, SIZE, STATUS from {APP_NAME}.api.engines {where_clause}"
+        results = self._exec(statement)
         if not results:
             return []
         return [{"name":name, "size":size, "state":state}
                 for (name, size, state) in results.fetchall()]
 
     def get_engine(self, name:str):
         results = self._exec(f"select NAME, SIZE, STATUS from {APP_NAME}.api.engines WHERE NAME='{name}'")
         if not results:
             return None
         engine = results.fetchone()
         if not engine:
             return None
         return {"name": engine[0], "size": engine[1], "state": engine[2]}
 
+    def is_valid_engine_state(self, state:str):
+        return state in VALID_ENGINE_STATES
+
     def create_engine(self, name:str, size:str, pool:str = ""):
         if not pool:
             raise ValueError("Pool is required")
         try:
             with debugging.span("create_engine", name=name, size=size, pool=pool):
                 self._exec(f"call {APP_NAME}.api.create_engine('{name}', '{pool}', '{size}');")
         except Exception as e:
@@ -482,15 +488,15 @@
             with pa.ipc.open_stream(file_content) as reader:
                 schema = reader.schema
                 batches = [batch for batch in reader]
                 table = pa.Table.from_batches(batches=batches, schema=schema)
                 results.append({"relationId": file_name, "table": table})
 
         return results
-    
+
     def _download_results(self, artifact_urls, txn_id):
         with debugging.span("download_results"):
             # Fetch artifacts
             artifacts = self._fetch_exec_async_artifacts(artifact_urls)
 
             # Parse metadata from the artifacts
             meta = _parse_metadata_proto(artifacts["metadata.proto"])
@@ -537,15 +543,15 @@
                     poll_with_specified_overhead(lambda: self._check_exec_async_status(txn_id), 0.2)
 
             self._pending_transactions.remove(txn_id)
 
             with debugging.span("fetch"):
                 # List the result artifacts (and the URLs to retrieve them)
                 artifact_urls = self._list_exec_async_artifacts(txn_id)
-                
+
                 return self._download_results(artifact_urls, txn_id)
 
     # Copied directly from azure.py
     def _has_errors(self, results):
         if len(results.problems):
             for problem in results.problems:
                 if problem['is_error'] or problem['is_exception']:
```

### Comparing `relationalai-0.2.6/src/relationalai/clients/test.py` & `relationalai-0.2.7/src/relationalai/clients/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/clients/types.py` & `relationalai-0.2.7/src/relationalai/clients/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/loaders/csv.py` & `relationalai-0.2.7/src/relationalai/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/loaders/loader.py` & `relationalai-0.2.7/src/relationalai/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/loaders/types.py` & `relationalai-0.2.7/src/relationalai/loaders/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/std/aggregates.py` & `relationalai-0.2.7/src/relationalai/std/aggregates.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/std/graphs.py` & `relationalai-0.2.7/src/relationalai/std/graphs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/std/math.py` & `relationalai-0.2.7/src/relationalai/std/math.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/std/strings.py` & `relationalai-0.2.7/src/relationalai/std/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/tools/cli.py` & `relationalai-0.2.7/src/relationalai/tools/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     ConfigFile,
     all_configs_including_legacy,
     get_from_snowflake_connections_toml,
     azure_default_props,
     snowflake_default_props,
 )
 from InquirerPy.base.control import Choice
+from InquirerPy.validator import ValidationError
 
 import os
 import sys
 import click
 from pathlib import Path
 from .cli_controls import divider, Spinner
 from . import cli_controls as controls
@@ -124,20 +125,40 @@
         rich.print("[yellow bold]No configuration file found.")
         rich.print("To create one, run: [green bold]rai init[/green bold]")
         divider()
         sys.exit(1)
     return cfg
 
 #--------------------------------------------------
-# Validators
+# Validation
 #--------------------------------------------------
 
+EMPTY_STRING_REGEX = re.compile(r'^\S+$')
 ENGINE_NAME_REGEX = re.compile(r'^[a-zA-Z]\w{2,}$')
 ENGINE_NAME_ERROR = "Min 3 chars, start with letter, only letters, numbers, underscores allowed."
 
+def engine_name_validator(cfg:config.Config, name:str):
+    if not ENGINE_NAME_REGEX.match(name):
+        raise ValidationError(message=ENGINE_NAME_ERROR)
+
+    try:
+        provider = get_resource_provider(None, cfg)
+        engine = provider.get_engine(name)
+        if engine and provider.is_valid_engine_state(engine['state']):
+            raise ValidationError(message=f"Engine '{name}' already exists")
+        return True
+    except Exception as e:
+        raise ValidationError(message=f"{e}")
+
+def validate_engine_name(cfg:config.Config, name:str):
+    try:
+        return engine_name_validator(cfg, name)
+    except ValidationError as e:
+        return e.message
+
 #--------------------------------------------------
 # Custom help printer
 #--------------------------------------------------
 
 class RichGroup(click.Group):
     def format_help(self, ctx: Context, formatter: HelpFormatter) -> None:
         global PROFILE
@@ -294,24 +315,43 @@
     else:
         return account_or_url
 
 def snowflake_flow(cfg:config.Config):
     pyrel_config = check_original_config_flow(cfg, "snowflake")
     if not pyrel_config:
         check_snowflake_connections_flow(cfg)
+
     # get account info
-    user = controls.text("SnowSQL user:", default=cfg.get("user", ""))
+    user = controls.text(
+        "SnowSQL user:",
+        default=cfg.get("user", ""),
+        validator=EMPTY_STRING_REGEX.match,
+        invalid_message="User is required"
+    )
     cfg.set("user", user)
-    password = controls.password("SnowSQL password:", default=cfg.get("password", ""))
+
+    password = controls.password(
+        "SnowSQL password:",
+        default=cfg.get("password", ""),
+        validator=EMPTY_STRING_REGEX.match,
+        invalid_message="Password is required"
+    )
     cfg.set("password", password)
+
     rich.print("\n[dim]  Note: Account ID should look like: myorg-account123")
     rich.print("[dim]  Details: https://docs.snowflake.com/en/user-guide/admin-account-identifier\n")
     rich.print("[dim]  Alternatively, you can log in to Snowsight, copy the URL, and paste it here.")
     rich.print("[dim]  Example: https://app.snowflake.com/myorg/account123/worksheets\n")
-    account_or_url = controls.text("Snowflake account:", default=cfg.get("account", ""))
+
+    account_or_url = controls.text(
+        "Snowflake account:",
+        default=cfg.get("account", ""),
+        validator=EMPTY_STRING_REGEX.match,
+        invalid_message="Account is required"
+    )
     account = account_from_url(account_or_url)
     if "." in account:
         rich.print("\n[yellow] Your Account ID should not contain a period (.) character.")
         corrected_account = account.replace(".", "-")
         use_replacement = controls.confirm(f"Use '{corrected_account}' instead", default=True)
         if use_replacement:
             account = corrected_account
@@ -377,73 +417,80 @@
     if not profile:
         return
     cfg.profile = profile
     cfg.update(sf_config[profile])
     return True
 
 def role_flow(provider:ResourceProvider, cfg:config.Config):
-    role = controls.fuzzy_with_refetch(
+    result = controls.fuzzy_with_refetch(
             "Select a role:",
             "roles",
             lambda: [r["name"] for r in cast(snowflake.Resources, provider).list_roles()],
             default=cfg.get("role", None),
         )
+    if isinstance(result, Exception):
+        return
+    else:
+        role = result
     cfg.set("role", role or FIELD_PLACEHOLDER)
     provider.reset()
 
 def warehouse_flow(provider:ResourceProvider, cfg:config.Config):
-    warehouse = controls.fuzzy_with_refetch(
+    result = controls.fuzzy_with_refetch(
             "Select a warehouse:",
             "warehouses",
             lambda: [w["name"] for w in cast(snowflake.Resources, provider).list_warehouses()],
             default=cfg.get("warehouse", None),
         )
+    if not result or isinstance(result, Exception):
+        return
+    else:
+        warehouse = result
     cfg.set("warehouse", warehouse or FIELD_PLACEHOLDER)
 
 def rai_app_flow(provider:ResourceProvider, cfg:config.Config):
-    app = controls.fuzzy_with_refetch(
+    result = controls.fuzzy_with_refetch(
             "Select RelationalAI app name:",
             "apps",
             lambda: [w["name"] for w in cast(snowflake.Resources, provider).list_apps()],
             default=cfg.get("rai_app_name", None),
         )
+    if not result or isinstance(result, Exception):
+        return
+    else:
+        app = result
     cfg.set("rai_app_name", app or FIELD_PLACEHOLDER)
     provider.reset()
 
 def spcs_flow(provider: ResourceProvider, cfg: config.Config):
-
     role_flow(provider, cfg)
     warehouse_flow(provider, cfg)
     rai_app_flow(provider, cfg)
 
 def engine_flow(provider:ResourceProvider, cfg:config.Config):
-    engine = controls.fuzzy_with_refetch(
+    app_name = cfg.get("rai_app_name", None)
+    if not app_name:
+        rich.print("[yellow]App name is required for engine selection. Skipping step.\n")
+        return
+    warehouse = cfg.get("warehouse", None)
+    if not warehouse:
+        rich.print("[yellow]Warehouse is required for engine selection. Skipping step.\n")
+        return
+    result = controls.fuzzy_with_refetch(
         "Select an engine:",
         "engines",
         lambda: ["Create a new engine"] + [engine.get("name") for engine in provider.list_engines()],
         default=cfg.get("engine", None),
     )
-    if engine == "Create a new engine":
-        engine = controls.text("Engine name:", validator=ENGINE_NAME_REGEX.match, invalid_message=ENGINE_NAME_ERROR)
-        engine_size = controls.fuzzy("Engine size:", choices=ENGINE_SIZES)
-        engine_pool = ""
-        if cfg.get("platform") == "snowflake":
-            provider = cast(snowflake.Resources, provider)
-            engine_pool = controls.fuzzy_with_refetch(
-                "Compute pool:",
-                "compute pools",
-                provider.list_valid_compute_pools_by_engine_size,
-                engine_size,
-            )
-        rich.print("")
-        with Spinner(f"Creating '{engine}' engine... (this may take several minutes)", f"Engine '{engine}' created"):
-            try:
-                provider.create_engine(engine, engine_size, engine_pool)
-            except Exception as e:
-                raise Exception(f"Error creating engine: {e}")
+    if not result or isinstance(result, Exception):
+        return
+    else:
+        engine = result
+    if result == "Create a new engine":
+        engine = create_engine_flow(cfg)
         rich.print("")
     cfg.set("engine", engine or FIELD_PLACEHOLDER)
 
 def gitignore_flow():
     current_dir = Path.cwd()
     prev_dir = None
     while current_dir != prev_dir:
@@ -704,20 +751,21 @@
     deb.main(port)
 
 #--------------------------------------------------
 # Engine list
 #--------------------------------------------------
 
 @cli.command(name="engines:list", help="List all engines")
-def engines_list():
+@click.option("--state", help="Filter by engine state")
+def engines_list(state:str|None=None):
     divider(flush=True)
     ensure_config()
     with Spinner("Fetching engines"):
         try:
-            engines = get_resource_provider().list_engines()
+            engines = get_resource_provider().list_engines(state)
         except Exception as e:
             rich.print(f"\n\n[yellow]Error fetching engines: {e}")
             exit(1)
 
     if len(engines):
         table = Table(show_header=True, border_style="dim", header_style="bold", box=rich_box.SIMPLE_HEAD)
         table.add_column("Name")
@@ -761,44 +809,90 @@
 
     divider()
 
 #--------------------------------------------------
 # Engine create
 #--------------------------------------------------
 
-@cli.command(name="engines:create", help="Create a new engine")
-@click.option("--name", help="Name of the engine")
-@click.option("--size", type=click.Choice(ENGINE_SIZES, case_sensitive=False), help="Size of the engine")
-def engines_create(name, size):
-    divider(flush=True)
-    ensure_config()
-    name = controls.prompt("Engine name?", name, validator=ENGINE_NAME_REGEX.match, invalid_message=ENGINE_NAME_ERROR, newline=True)
+def create_engine_flow(cfg:config.Config, name=None, size=None, pool=None):
+    provider = get_resource_provider(None, cfg)
+    is_snowflake = provider.config.get("platform") == "snowflake"
+    is_interactive = name is None or size is None or (is_snowflake and pool is None)
+
+    if not name:
+        name = controls.prompt(
+            "Engine name:",
+            name,
+            validator=lambda e: engine_name_validator(cfg, e),
+            newline=True
+        )
+    else:
+        is_name_valid = validate_engine_name(cfg, name)
+        if isinstance(is_name_valid, str):
+            rich.print(f"[yellow]{is_name_valid}")
+            return None
+
     if not size:
         size = controls.fuzzy("Engine size:", choices=ENGINE_SIZES)
         rich.print("")
-    provider = get_resource_provider()
 
-    if provider.config.get("platform") == "snowflake":
+    if is_snowflake:
         provider = cast(snowflake.Resources, provider)
-        pool = controls.fuzzy_with_refetch(
-            "Compute pool:",
-            "compute pools",
-            provider.list_valid_compute_pools_by_engine_size,
-            size,
-        )
+        if not pool:
+            result = controls.fuzzy_with_refetch(
+                "Compute pool:",
+                "compute pools",
+                provider.list_valid_compute_pools_by_engine_size,
+                size,
+            )
+            if isinstance(result, Exception):
+                return None
+            else:
+                pool = result
+        if is_interactive and not pool:
+            redo = controls.confirm("Would you like to choose a different engine size?", default=True)
+            rich.print("")
+            if redo:
+                return create_engine_flow(cfg, name)
+            else:
+                return None
     else:
         pool = ""
 
-    with Spinner(f"Creating '{name}' engine... (this may take several minutes)", f"Engine '{name}' created!"):
+    create_exception = None
+
+    with Spinner(
+        f"Creating '{name}' engine... (this may take several minutes)",
+        f"Engine '{name}' created!",
+        failed_message="Error:"
+    ):
         try:
             provider.create_engine(name, size, pool)
         except Exception as e:
-            rich.print(f"\n\n[yellow]Error creating engine: {e}")
-            divider()
-            exit(1)
+            create_exception = e
+            # We do not want to print the success context message if the engine creation fails
+            # Since we are raising here and passing a "fail_message", the spinner will print the actual error message
+            raise e
+    if isinstance(create_exception, Exception):
+        if is_interactive and "does not exist" in f"{create_exception}".lower():
+            rich.print("")
+            redo = controls.confirm("Would you like to choose a different compute pool?", default=True)
+            rich.print("")
+            if redo:
+                return create_engine_flow(cfg, name, size)
+    return name
+
+@cli.command(name="engines:create", help="Create a new engine")
+@click.option("--name", help="Name of the engine")
+@click.option("--size", type=click.Choice(ENGINE_SIZES, case_sensitive=False), help="Size of the engine")
+@click.option("--pool", help="Compute pool name. Note: Snowflake platform only.")
+def engines_create(name, size, pool):
+    divider(flush=True)
+    cfg = ensure_config()
+    create_engine_flow(cfg, name, size, pool)
     divider()
 
 #--------------------------------------------------
 # Engine delete
 #--------------------------------------------------
 
 @cli.command(name="engines:delete", help="Delete an engine")
@@ -808,15 +902,16 @@
     ensure_config()
     if not name:
         name = controls.fuzzy_with_refetch(
             "Select an engine:",
             "engines",
             lambda: [engine["name"] for engine in get_resource_provider().list_engines()],
         )
-
+        if not name or isinstance(name, Exception):
+            return
     with Spinner(f"Deleting '{name}' engine", f"Engine '{name}' deleted!"):
         try:
             get_resource_provider().delete_engine(name)
         except Exception as e:
             rich.print(f"\n\n[yellow]Error deleting engine: {e}")
     divider()
```

### Comparing `relationalai-0.2.6/src/relationalai/tools/cli_controls.py` & `relationalai-0.2.7/src/relationalai/tools/cli_controls.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     if value:
         return value
     try:
         result:str = inquirer.text(
             message,
             validate=validator,
             invalid_message=invalid_message,
-            keybindings=default_bindings
+            keybindings=default_bindings,
         ).execute()
     except KeyboardInterrupt:
         abort()
         raise Exception("Unreachable")
     if newline:
         rich.print("")
     return result
@@ -145,58 +145,74 @@
         if scroll_to_ix is not None:
             prompt.content_control.selected_choice_index = scroll_to_ix
         return prompt.execute()
     except KeyboardInterrupt:
         return abort()
 
 def fuzzy_with_refetch(prompt: str, type: str, fn: callable = None, *args, **kwargs):
+    exception = None
     with Spinner(f"Fetching {type}", f"Fetched {type}"):
         try:
             items = fn(*args)
         except Exception as e:
-            rich.print(f"\n\n[yellow]Error fetching {type}: {e}")
-            exit(1)
+            exception = e
+    if exception is not None:
+        rich.print(f"\n[red]Error fetching {type}: {exception}\n")
+        return exception
     if len(items) == 0:
         rich.print(f"\n[yellow]No valid {type} found\n")
-        exit(1)
+        return None
 
     items.insert(0, REFETCH)
 
     passed_default = kwargs.get("default", None)
-    default = get_default(passed_default, items)
+    passed_mandatory = kwargs.get("mandatory", False)
 
     rich.print("")
-    result = fuzzy(prompt, items, default=default)
+    result = fuzzy(
+        prompt,
+        items,
+        default=get_default(passed_default, items),
+        mandatory=passed_mandatory
+    )
     rich.print("")
 
     while result == REFETCH:
-        result = fuzzy_with_refetch(prompt, type, fn, default=passed_default, *args)
+        result = fuzzy_with_refetch(prompt, type, fn, *args, **kwargs)
     return result
 
 def confirm(message:str, default:bool = False) -> bool:
     try:
         return inquirer.confirm(message, default=default, keybindings=default_bindings).execute()
     except KeyboardInterrupt:
         return abort()
 
 def text(message:str, default:str|None = None, validator:callable = None, invalid_message:str|None = None) -> str:
+    if validator and not invalid_message:
+        invalid_message = "Invalid input"
     try:
         return inquirer.text(
             message,
             default=default or "",
             keybindings=default_bindings,
             validate=validator,
             invalid_message=invalid_message
         ).execute()
     except KeyboardInterrupt:
         return abort()
 
-def password(message:str, default:str|None = None) -> str:
+def password(message:str, default:str|None = None, validator:callable = None, invalid_message:str|None = None) -> str:
     try:
-        return inquirer.secret(message, default=default or "", keybindings=default_bindings).execute()
+        return inquirer.secret(
+            message,
+            default=default or "",
+            keybindings=default_bindings,
+            validate=validator,
+            invalid_message=invalid_message
+        ).execute()
     except KeyboardInterrupt:
         return abort()
 
 def file(message: str, start_path:Path|None = None, pattern:str|Pattern|None = None, default:str|None = None, allow_freeform=False, **kwargs) -> str|None:
     try:
         return FuzzyFile(message, start_path, allow_freeform=allow_freeform, max_height=8, border=True, style=STYLE, **kwargs).execute()
     except KeyboardInterrupt:
@@ -289,20 +305,24 @@
         self._buffer.reset()
 
 #--------------------------------------------------
 # Spinner
 #--------------------------------------------------
 
 class Spinner:
+    """Shows a spinner control while a task is running.\n
+    The finished_message will not be printed if there was an exception and the failed_message is provided.
+    """
     busy = False
     delay = 0.1
 
-    def __init__(self, message="", finished="", delay=None):
+    def __init__(self, message="", finished_message="", failed_message=None, delay=None):
         self.message = message
-        self.finished = finished
+        self.finished_message = finished_message
+        self.failed_message = failed_message
         self.spinner_generator = itertools.cycle([ "▰▱▱▱", "▰▰▱▱", "▰▰▰▱", "▰▰▰▰", "▱▰▰▰", "▱▱▰▰", "▱▱▱▰", "▱▱▱▱" ])
         if delay and float(delay):
             self.delay = delay
 
     def get_message(self):
         return rich_str(f"[magenta]{next(self.spinner_generator)} {self.message}").strip()
 
@@ -326,20 +346,23 @@
             sys.stdout.flush()
         else:
             threading.Thread(target=self.spinner_task).start()
 
     def __exit__(self, exception, value, tb):
         self.busy = False
         if exception is not None:
+            if self.failed_message is not None:
+                rich.print(f"\n\n[yellow]{self.failed_message} {value}")
+                return True
             return False
         time.sleep(self.delay)
         message = self.get_message()
         sys.stdout.write(self.get_clear(message))
-        if self.finished != "":
-            final_message = f"[green]▰▰▰▰ {self.finished}"
+        if self.finished_message != "":
+            final_message = f"[green]▰▰▰▰ {self.finished_message}"
             final_message += " " * (len(message) - len(final_message))
             rich.print(final_message)
-        elif self.finished == "":
+        elif self.finished_message == "":
             sys.stdout.write(self.get_clear(message))
             sys.stdout.write(" "*len(message.encode('utf-8')))
             sys.stdout.write(self.get_clear(message))
             sys.stdout.flush()
```

### Comparing `relationalai-0.2.6/src/relationalai/tools/debugger.py` & `relationalai-0.2.7/src/relationalai/tools/debugger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/tools/debugger_server.py` & `relationalai-0.2.7/src/relationalai/tools/debugger_server.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/tools/dev.py` & `relationalai-0.2.7/src/relationalai/tools/dev.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/util/snowflake_logger.py` & `relationalai-0.2.7/src/relationalai/util/snowflake_logger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/src/relationalai/util/tracing_logger.py` & `relationalai-0.2.7/src/relationalai/util/tracing_logger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/conftest.py` & `relationalai-0.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/util.py` & `relationalai-0.2.7/tests/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/benchmarks/conftest.py` & `relationalai-0.2.7/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/benchmarks/test_tastybytes.py` & `relationalai-0.2.7/tests/benchmarks/test_tastybytes.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/README.md` & `relationalai-0.2.7/tests/end2end/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/conftest.py` & `relationalai-0.2.7/tests/end2end/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_graph_visualize.py` & `relationalai-0.2.7/tests/end2end/test_graph_visualize.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_snapshots.py` & `relationalai-0.2.7/tests/end2end/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt` & `relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/bool.py` & `relationalai-0.2.7/tests/end2end/test_cases/bool.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/bottom.py` & `relationalai-0.2.7/tests/end2end/test_cases/bottom.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/export.py` & `relationalai-0.2.7/tests/end2end/test_cases/export.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/math.py` & `relationalai-0.2.7/tests/end2end/test_cases/std_math.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,84 +6,84 @@
 model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Point = model.Type("Point")
 
 with model.rule():
     Point.add(x=1.1, y=-1, z=0)
 
 # Check that the abs function works
-with model.query() as select:
+with model.query(tag="abs") as select:
     p = Point(y=-1)
     abs1 = std.math.abs(p.y)
     abs2 = std.math.abs(-1.0)
     select(p, abs1, abs2)
 
 # Check that the isclose function works
-with model.query() as select:
+with model.query(tag="isclose") as select:
     p = Point(z=0)
     std.math.isclose(p.z, 1e-10)
     select(p, p.z)
 
 # Check that the isclose function works with a tolerance
-with model.query() as select:
+with model.query(tag="isclose_tolerance") as select:
     p = Point(z=0)
     std.math.isclose(p.z, 1e-8, 1e-9)
     select(p, p.z)  # Should return empty dataframe
 
 # Check that the ceil function works
-with model.query() as select:
+with model.query(tag="ceil") as select:
     p = Point(x=1.1)
     ceil1 = std.math.ceil(p.x)
     ceil2 = std.math.ceil(0.5)
     select(p, ceil1, ceil2)
 
 # Check that the floor function works
-with model.query() as select:
+with model.query(tag="floor") as select:
     p = Point(x=1.1)
     floor1 = std.math.floor(p.x)
     floor2 = std.math.floor(0.5)
     select(p, floor1, floor2)
 
 # Check that the cbrt function works
-with model.query() as select:
+with model.query(tag="cbrt") as select:
     p = Point(y=-1)
     cbrt1 = std.math.cbrt(p.y)
     cbrt2 = std.math.cbrt(8)
     select(p, cbrt1, cbrt2)
 
 # Check that the sqrt function works
-with model.query() as select:
+with model.query(tag="sqrt") as select:
     p = Point(z=0)
     sqrt1 = std.math.sqrt(p.z)
     sqrt2 = std.math.sqrt(4)
     select(p, sqrt1, sqrt2)
 
 # Check that the sqrt function raises an error when given a negative number
 with pytest.raises(ValueError):
-    with model.query():
+    with model.query(tag="sqrt"):
         std.math.sqrt(-1)
 
 # Check that the log function works
-with model.query() as select:
+with model.query(tag="log") as select:
     p = Point(z=0)
     log1 = std.math.log(p.z)
     log2 = std.math.log(100, 10)
     select(p, log1, log2)
 
 # Check that the log function raises an error when given a negative number
 with pytest.raises(ValueError):
-    with model.query():
+    with model.query(tag="log"):
         std.math.log(-1)
 
 # Check that the sign function works
-with model.query() as select:
+with model.query(tag="sign") as select:
     p = Point(x=1.1, y=-1)
     sign1 = std.math.sign(p.x)
     sign2 = std.math.sign(p.y)
     sign3 = std.math.sign(0)
     select(p, sign1, sign2, sign3)
 
 # Check that the trunc_divide function works
-with model.query() as select:
+with model.query(tag="trunc_divide") as select:
     p = Point(x=1.1)
     trunc_divide1 = std.math.trunc_divide(p.x, 2)
     trunc_divide2 = std.math.trunc_divide(-5, 2)
     select(p, trunc_divide1, trunc_divide2)
```

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/multi_valued.py` & `relationalai-0.2.7/tests/end2end/test_cases/multi_valued.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/not_found.py` & `relationalai-0.2.7/tests/end2end/test_cases/not_found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/out_of_context.py` & `relationalai-0.2.7/tests/end2end/test_cases/out_of_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # pyright: reportUnusedExpression=false
 import relationalai as rai
+from relationalai.std import rel
 from relationalai.errors import RAIException
 import pytest
 
-model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
+model = rai.Model(name=globals().get("name", "test_out_of_context"), config=globals().get("config"))
 Person = model.Type("Person")
 Adult = model.Type("Adult")
 
 with model.rule():
     p = Person()
     p.age >= 18
     woop = p.woop
+    d = p.age + 10
+    v = rel.sin(3)
     p.set(Adult)
 
 with pytest.raises(RAIException):
     with model.query() as select:
         a = Adult()
         p.foo
         select(a)
@@ -24,7 +27,18 @@
         a = Adult()
         select(a, a.name, a.age, p)
 
 with pytest.raises(RAIException):
     with model.query() as select:
         a = Adult()
         select(a, a.name, a.age, woop)
+
+with pytest.raises(RAIException):
+    with model.query() as select:
+        a = Adult()
+        z = d + 10
+        select(a, z)
+
+with pytest.raises(RAIException):
+    with model.query() as select:
+        a = Adult()
+        select(a, v)
```

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/persist.py` & `relationalai-0.2.7/tests/end2end/test_cases/persist.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/smoke.py` & `relationalai-0.2.7/tests/end2end/test_cases/smoke.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/strings.py` & `relationalai-0.2.7/tests/end2end/test_cases/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/top.py` & `relationalai-0.2.7/tests/end2end/test_cases/top.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/union.py` & `relationalai-0.2.7/tests/end2end/test_cases/union.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/weighted_graphs.py` & `relationalai-0.2.7/tests/end2end/test_cases/weighted_graphs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/graphs/basics.py` & `relationalai-0.2.7/tests/end2end/test_cases/graphs/basics.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/graphs/centrality.py` & `relationalai-0.2.7/tests/end2end/test_cases/graphs/centrality.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/graphs/community.py` & `relationalai-0.2.7/tests/end2end/test_cases/graphs/community.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/graphs/connectivity.py` & `relationalai-0.2.7/tests/end2end/test_cases/graphs/connectivity.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/graphs/degree.py` & `relationalai-0.2.7/tests/end2end/test_cases/graphs/degree.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 graph = std.graphs.Graph(model)
 
 with model.rule():
     r = Relationship()
     graph.Edge.add(r.from_, r.to)
 
 for algo_name in UNARY_ALGOS:
-    with model.query() as select:
+    with model.query(tag=algo_name) as select:
         algo = getattr(graph.compute, algo_name)()
         select(algo)
 
 for algo_name in BINARY_ALGOS:
-    with model.query() as select:
+    with model.query(tag=algo_name) as select:
         o = Object()
         algo = getattr(graph.compute, algo_name)(o)
         select(o, algo)
```

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/graphs/distance.py` & `relationalai-0.2.7/tests/end2end/test_cases/graphs/distance.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/graphs/link_prediction.py` & `relationalai-0.2.7/tests/end2end/test_cases/graphs/link_prediction.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/graphs/similarity.py` & `relationalai-0.2.7/tests/end2end/test_cases/graphs/similarity.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/end2end/test_cases/graphs/triangles.py` & `relationalai-0.2.7/tests/end2end/test_cases/graphs/triangles.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/init-cli/azure_basic.py` & `relationalai-0.2.7/tests/init-cli/azure_basic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/init-cli/common.py` & `relationalai-0.2.7/tests/init-cli/common.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/roundtrip/test_document.py` & `relationalai-0.2.7/tests/roundtrip/test_document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/tests/roundtrip/test_task.py` & `relationalai-0.2.7/tests/roundtrip/test_task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.6/pyproject.toml` & `relationalai-0.2.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = 'relationalai'
-version = '0.2.6'
+version = '0.2.7'
 description = 'RelationalAI Library and CLI'
 readme="docs/pypi/README.md"
 authors = [
     { name="RelationalAI", email="support@relational.ai" },
 ]
 requires-python = ">= 3.10"
 dependencies = [
     "snowflake-connector-python[secure-local-storage]",
-    "rai-sdk",
+    "rai-sdk>=0.7.4",
     "rich",
     "nicegui",
     "numpy",
     "pandas",
     "colorama",
     "inquirerpy",
     "click",
```

### Comparing `relationalai-0.2.6/PKG-INFO` & `relationalai-0.2.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: relationalai
-Version: 0.2.6
+Version: 0.2.7
 Summary: RelationalAI Library and CLI
 Author-email: RelationalAI <support@relational.ai>
 Requires-Python: >=3.10
 Requires-Dist: bytecode
 Requires-Dist: click
 Requires-Dist: colorama
 Requires-Dist: gravis
 Requires-Dist: inquirerpy
 Requires-Dist: nicegui
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
-Requires-Dist: rai-sdk
+Requires-Dist: rai-sdk>=0.7.4
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: snowflake-connector-python[secure-local-storage]
 Requires-Dist: toml
 Requires-Dist: tomlkit
 Requires-Dist: websockets
 Provides-Extra: dev
```


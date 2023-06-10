# Comparing `tmp/ultibi-0.3.2.tar.gz` & `tmp/ultibi-0.3.3.tar.gz`

## Comparing `ultibi-0.3.2.tar` & `ultibi-0.3.3.tar`

### file list

```diff
@@ -1,153 +1,153 @@
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 ultibi-0.3.2/local_dependencies/ultibi/Cargo.toml
--rw-r--r--   0     1001      123        0 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi/README.md
--rw-r--r--   0     1001      123       73 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi/src/lib.rs
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 ultibi-0.3.2/local_dependencies/ultibi_server/Cargo.toml
--rw-r--r--   0     1001      123      219 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/build.rs
--rw-r--r--   0     1001      123       35 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/api/mod.rs
--rw-r--r--   0     1001      123      743 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/api/open_api.rs
--rw-r--r--   0     1001      123     6651 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/api/routers.rs
--rw-r--r--   0     1001      123     1264 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/app.rs
--rw-r--r--   0     1001      123     2593 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/helpers.rs
--rw-r--r--   0     1001      123     1432 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/lib.rs
--rw-r--r--   0     1001      123      433 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_server/src/visual.rs
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ultibi-0.3.2/local_dependencies/frtb_engine/Cargo.toml
--rw-r--r--   0     1001      123      481 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/README.md
--rw-r--r--   0     1001      123    14931 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/Delta.csv
--rw-r--r--   0     1001      123      541 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
--rw-r--r--   0     1001      123     2160 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
--rw-r--r--   0     1001      123      159 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/hms.csv
--rw-r--r--   0     1001      123      177 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
--rw-r--r--   0     1001      123    20066 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/calc_params.rs
--rw-r--r--   0     1001      123       25 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/docs/mod.rs
--rw-r--r--   0     1001      123     1226 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/docs/optional_params.rs
--rw-r--r--   0     1001      123     1424 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/common.rs
--rw-r--r--   0     1001      123    11840 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
--rw-r--r--   0     1001      123     9483 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
--rw-r--r--   0     1001      123     7606 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/drc_weights.rs
--rw-r--r--   0     1001      123       96 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/mod.rs
--rw-r--r--   0     1001      123      787 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/totals.rs
--rw-r--r--   0     1001      123     4811 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/helpers.rs
--rw-r--r--   0     1001      123     8968 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/lib.rs
--rw-r--r--   0     1001      123     3780 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/measures.rs
--rw-r--r--   0     1001      123      188 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/prelude.rs
--rw-r--r--   0     1001      123    26516 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/risk_weights.rs
--rw-r--r--   0     1001      123     5408 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
--rw-r--r--   0     1001      123     5268 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/rrao/mod.rs
--rw-r--r--   0     1001      123     1374 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/buckets.rs
--rw-r--r--   0     1001      123    14177 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
--rw-r--r--   0     1001      123    13866 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
--rw-r--r--   0     1001      123     3699 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
--rw-r--r--   0     1001      123     7432 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
--rw-r--r--   0     1001      123    29827 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/common.rs
--rw-r--r--   0     1001      123     9793 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/common_curv.rs
--rw-r--r--   0     1001      123    19318 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
--rw-r--r--   0     1001      123    17703 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
--rw-r--r--   0     1001      123     3841 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
--rw-r--r--   0     1001      123    11803 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
--rw-r--r--   0     1001      123    15617 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
--rw-r--r--   0     1001      123    12459 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
--rw-r--r--   0     1001      123     2904 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
--rw-r--r--   0     1001      123     8782 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
--rw-r--r--   0     1001      123    15261 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
--rw-r--r--   0     1001      123    13479 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
--rw-r--r--   0     1001      123     2988 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
--rw-r--r--   0     1001      123     8063 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
--rw-r--r--   0     1001      123    17052 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
--rw-r--r--   0     1001      123    10900 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
--rw-r--r--   0     1001      123     2162 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
--rw-r--r--   0     1001      123    10428 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
--rw-r--r--   0     1001      123    14289 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
--rw-r--r--   0     1001      123    11992 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
--rw-r--r--   0     1001      123     2162 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
--rw-r--r--   0     1001      123    10166 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
--rw-r--r--   0     1001      123    14030 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
--rw-r--r--   0     1001      123    21887 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
--rw-r--r--   0     1001      123       64 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
--rw-r--r--   0     1001      123     2295 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
--rw-r--r--   0     1001      123    15657 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
--rw-r--r--   0     1001      123      221 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/mod.rs
--rw-r--r--   0     1001      123     5170 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/totals.rs
--rw-r--r--   0     1001      123    28643 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/statics.rs
--rw-r--r--   0     1001      123      753 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/totals.rs
--rw-r--r--   0     1001      123     1881 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/src/validate.rs
--rw-r--r--   0     1001      123     1756 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/tests/common/mod.rs
--rw-r--r--   0     1001      123     1486 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/tests/dependant.rs
--rw-r--r--   0     1001      123     4487 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/tests/drc.rs
--rw-r--r--   0     1001      123      420 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/tests/rrao.rs
--rw-r--r--   0     1001      123    18903 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/tests/sbm.rs
--rw-r--r--   0     1001      123      744 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/frtb_engine/tests/sbm_totals.rs
--rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 ultibi-0.3.2/local_dependencies/ultibi_core/Cargo.toml
--rw-r--r--   0     1001      123     2031 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/add_row.rs
--rw-r--r--   0     1001      123     3486 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/aggregations.rs
--rw-r--r--   0     1001      123      654 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/cache.rs
--rw-r--r--   0     1001      123     4244 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/datarequest.rs
--rw-r--r--   0     1001      123     9751 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/dataset.rs
--rw-r--r--   0     1001      123     1782 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/acquire.rs
--rw-r--r--   0     1001      123     2059 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/awss3.rs
--rw-r--r--   0     1001      123     5329 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/helpers.rs
--rw-r--r--   0     1001      123     7509 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/mod.rs
--rw-r--r--   0     1001      123      699 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/errors.rs
--rw-r--r--   0     1001      123    10956 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/execution/execute_agg.rs
--rw-r--r--   0     1001      123     4594 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
--rw-r--r--   0     1001      123      464 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/execution/mod.rs
--rw-r--r--   0     1001      123     2585 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/filters.rs
--rw-r--r--   0     1001      123       18 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/helpers/mod.rs
--rw-r--r--   0     1001      123      545 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/helpers/searches.rs
--rw-r--r--   0     1001      123      375 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/lib.rs
--rw-r--r--   0     1001      123    11996 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/measure.rs
--rw-r--r--   0     1001      123     5459 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/overrides.rs
--rw-r--r--   0     1001      123      230 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/prelude.rs
--rw-r--r--   0     1001      123       15 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/reports/mod.rs
--rw-r--r--   0     1001      123      645 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/src/reports/report.rs
--rw-r--r--   0     1001      123     1884 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/add_row.rs
--rw-r--r--   0     1001      123      741 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/agg_request.rs
--rw-r--r--   0     1001      123     1543 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/aggregations.rs
--rw-r--r--   0     1001      123        1 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/cache.rs
--rw-r--r--   0     1001      123     2067 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/common/mod.rs
--rw-r--r--   0     1001      123       95 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/data/bad_config.toml
--rw-r--r--   0     1001      123      553 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/data/bad_config2.toml
--rw-r--r--   0     1001      123      116 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/data/test_config.toml
--rw-r--r--   0     1001      123      354 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/data/testset.csv
--rw-r--r--   0     1001      123     1250 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/datasource.rs
--rw-r--r--   0     1001      123     3115 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/dependants.rs
--rw-r--r--   0     1001      123     1485 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/filters.rs
--rw-r--r--   0     1001      123        1 2023-04-25 16:53:29.000000 ultibi-0.3.2/local_dependencies/ultibi_core/tests/overrides.rs
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 ultibi-0.3.2/Cargo.toml
--rw-r--r--   0     1001      123      728 2023-04-25 16:53:29.000000 ultibi-0.3.2/.gitignore
--rw-r--r--   0     1001      123     5183 2023-04-25 16:53:29.000000 ultibi-0.3.2/LICENSE
--rw-r--r--   0     1001      123     2403 2023-04-25 16:53:29.000000 ultibi-0.3.2/Makefile
--rw-r--r--   0     1001      123     4968 2023-04-25 16:53:29.000000 ultibi-0.3.2/README.md
--rw-r--r--   0     1001      123     1559 2023-04-25 16:53:29.000000 ultibi-0.3.2/example.py
--rw-r--r--   0     1001      123     2045 2023-04-25 16:53:55.000000 ultibi-0.3.2/pyproject.toml
--rw-r--r--   0     1001      123       36 2023-04-25 16:53:29.000000 ultibi-0.3.2/requirements-lint.txt
--rw-r--r--   0     1001      123      307 2023-04-25 16:53:29.000000 ultibi-0.3.2/requirements.txt
--rw-r--r--   0     1001      123     3682 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/calculator.rs
--rw-r--r--   0     1001      123       48 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/conversions/mod.rs
--rw-r--r--   0     1001      123     3542 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/conversions/series.rs
--rw-r--r--   0     1001      123     3049 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/conversions/wrappers.rs
--rw-r--r--   0     1001      123     7737 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/dataset.rs
--rw-r--r--   0     1001      123     3303 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/errors.rs
--rw-r--r--   0     1001      123      693 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/filter.rs
--rw-r--r--   0     1001      123     1986 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/lib.rs
--rw-r--r--   0     1001      123     2521 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/measure.rs
--rw-r--r--   0     1001      123     1353 2023-04-25 16:53:29.000000 ultibi-0.3.2/src/requests.rs
--rw-r--r--   0     1001      123     1762 2023-04-25 16:53:29.000000 ultibi-0.3.2/tests/data/datasource_config.toml
--rw-r--r--   0     1001      123     4042 2023-04-25 16:53:29.000000 ultibi-0.3.2/tests/docs/run_doc_examples.py
--rw-r--r--   0     1001      123      591 2023-04-25 16:53:29.000000 ultibi-0.3.2/tests/unit/test_compute.py
--rw-r--r--   0     1001      123     1507 2023-04-25 16:53:29.000000 ultibi-0.3.2/tests/unit/test_ds.py
--rw-r--r--   0     1001      123     2658 2023-04-25 16:53:29.000000 ultibi-0.3.2/tests/unit/test_measure.py
--rw-r--r--   0     1001      123      848 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/__init__.py
--rw-r--r--   0     1001      123     1062 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/internals/__init__.py
--rw-r--r--   0     1001      123     6735 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/internals/dataset.py
--rw-r--r--   0     1001      123     3133 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/internals/filters.py
--rw-r--r--   0     1001      123     5202 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/internals/measure.py
--rw-r--r--   0     1001      123     2952 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/internals/requests.py
--rw-r--r--   0     1001      123        0 2023-04-25 16:53:29.000000 ultibi-0.3.2/ultibi/rust_module/__init__.py
--rw-r--r--   0        0        0   101994 2023-04-25 16:55:32.000000 ultibi-0.3.2/Cargo.lock
--rw-r--r--   0        0        0     5891 1970-01-01 00:00:00.000000 ultibi-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 ultibi-0.3.3/local_dependencies/ultibi_server/Cargo.toml
+-rw-r--r--   0     1001      123      219 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/build.rs
+-rw-r--r--   0     1001      123       35 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/api/mod.rs
+-rw-r--r--   0     1001      123      754 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/api/open_api.rs
+-rw-r--r--   0     1001      123     6651 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/api/routers.rs
+-rw-r--r--   0     1001      123     1264 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/app.rs
+-rw-r--r--   0     1001      123     2593 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/helpers.rs
+-rw-r--r--   0     1001      123     1432 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/lib.rs
+-rw-r--r--   0     1001      123      433 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/visual.rs
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 ultibi-0.3.3/local_dependencies/ultibi/Cargo.toml
+-rw-r--r--   0     1001      123        0 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi/README.md
+-rw-r--r--   0     1001      123       73 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi/src/lib.rs
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 ultibi-0.3.3/local_dependencies/ultibi_core/Cargo.toml
+-rw-r--r--   0     1001      123     2031 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/add_row.rs
+-rw-r--r--   0     1001      123     3486 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/aggregations.rs
+-rw-r--r--   0     1001      123      654 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/cache.rs
+-rw-r--r--   0     1001      123     4244 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/datarequest.rs
+-rw-r--r--   0     1001      123     9751 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/dataset.rs
+-rw-r--r--   0     1001      123     1782 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/acquire.rs
+-rw-r--r--   0     1001      123     2059 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/awss3.rs
+-rw-r--r--   0     1001      123     5329 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/helpers.rs
+-rw-r--r--   0     1001      123     7509 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/mod.rs
+-rw-r--r--   0     1001      123      700 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/errors.rs
+-rw-r--r--   0     1001      123    10956 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/execution/execute_agg.rs
+-rw-r--r--   0     1001      123     4594 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
+-rw-r--r--   0     1001      123      464 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/execution/mod.rs
+-rw-r--r--   0     1001      123     2663 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/filters.rs
+-rw-r--r--   0     1001      123       18 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/helpers/mod.rs
+-rw-r--r--   0     1001      123      545 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/helpers/searches.rs
+-rw-r--r--   0     1001      123      375 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/lib.rs
+-rw-r--r--   0     1001      123    11996 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/measure.rs
+-rw-r--r--   0     1001      123     5459 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/overrides.rs
+-rw-r--r--   0     1001      123      230 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/prelude.rs
+-rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/reports/mod.rs
+-rw-r--r--   0     1001      123     1178 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/reports/report.rs
+-rw-r--r--   0     1001      123     1884 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/add_row.rs
+-rw-r--r--   0     1001      123      741 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/agg_request.rs
+-rw-r--r--   0     1001      123     1543 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/aggregations.rs
+-rw-r--r--   0     1001      123        1 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/cache.rs
+-rw-r--r--   0     1001      123     2067 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/common/mod.rs
+-rw-r--r--   0     1001      123       95 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/data/bad_config.toml
+-rw-r--r--   0     1001      123      553 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/data/bad_config2.toml
+-rw-r--r--   0     1001      123      116 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/data/test_config.toml
+-rw-r--r--   0     1001      123      354 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/data/testset.csv
+-rw-r--r--   0     1001      123     1250 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/datasource.rs
+-rw-r--r--   0     1001      123     3115 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/dependants.rs
+-rw-r--r--   0     1001      123     1485 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/filters.rs
+-rw-r--r--   0     1001      123        1 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/overrides.rs
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ultibi-0.3.3/local_dependencies/frtb_engine/Cargo.toml
+-rw-r--r--   0     1001      123      481 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/README.md
+-rw-r--r--   0     1001      123    14931 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/Delta.csv
+-rw-r--r--   0     1001      123      541 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
+-rw-r--r--   0     1001      123     2160 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
+-rw-r--r--   0     1001      123      159 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/hms.csv
+-rw-r--r--   0     1001      123      177 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
+-rw-r--r--   0     1001      123    20066 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/calc_params.rs
+-rw-r--r--   0     1001      123       25 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/docs/mod.rs
+-rw-r--r--   0     1001      123     1226 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/docs/optional_params.rs
+-rw-r--r--   0     1001      123     1424 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/common.rs
+-rw-r--r--   0     1001      123    11840 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
+-rw-r--r--   0     1001      123     9483 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
+-rw-r--r--   0     1001      123     7606 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/drc_weights.rs
+-rw-r--r--   0     1001      123       96 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/mod.rs
+-rw-r--r--   0     1001      123      787 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/totals.rs
+-rw-r--r--   0     1001      123     4811 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/helpers.rs
+-rw-r--r--   0     1001      123     8968 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/lib.rs
+-rw-r--r--   0     1001      123     3780 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/measures.rs
+-rw-r--r--   0     1001      123      188 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/prelude.rs
+-rw-r--r--   0     1001      123    26516 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/risk_weights.rs
+-rw-r--r--   0     1001      123     5408 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
+-rw-r--r--   0     1001      123     5268 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/rrao/mod.rs
+-rw-r--r--   0     1001      123     1374 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/buckets.rs
+-rw-r--r--   0     1001      123    14177 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
+-rw-r--r--   0     1001      123    13866 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
+-rw-r--r--   0     1001      123     3699 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
+-rw-r--r--   0     1001      123     7432 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
+-rw-r--r--   0     1001      123    29827 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/common.rs
+-rw-r--r--   0     1001      123     9793 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/common_curv.rs
+-rw-r--r--   0     1001      123    19318 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
+-rw-r--r--   0     1001      123    17703 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
+-rw-r--r--   0     1001      123     3841 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
+-rw-r--r--   0     1001      123    11803 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
+-rw-r--r--   0     1001      123    15617 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
+-rw-r--r--   0     1001      123    12459 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
+-rw-r--r--   0     1001      123     2904 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
+-rw-r--r--   0     1001      123     8782 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
+-rw-r--r--   0     1001      123    15261 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
+-rw-r--r--   0     1001      123    13479 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
+-rw-r--r--   0     1001      123     2988 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
+-rw-r--r--   0     1001      123     8063 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
+-rw-r--r--   0     1001      123    17052 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
+-rw-r--r--   0     1001      123    10900 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
+-rw-r--r--   0     1001      123    10428 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
+-rw-r--r--   0     1001      123    14289 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
+-rw-r--r--   0     1001      123    11992 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
+-rw-r--r--   0     1001      123    10166 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
+-rw-r--r--   0     1001      123    14030 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
+-rw-r--r--   0     1001      123    21887 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
+-rw-r--r--   0     1001      123     2295 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
+-rw-r--r--   0     1001      123    15657 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
+-rw-r--r--   0     1001      123      221 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/mod.rs
+-rw-r--r--   0     1001      123     5170 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/totals.rs
+-rw-r--r--   0     1001      123    28643 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/statics.rs
+-rw-r--r--   0     1001      123      753 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/totals.rs
+-rw-r--r--   0     1001      123     1881 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/validate.rs
+-rw-r--r--   0     1001      123     1756 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/tests/common/mod.rs
+-rw-r--r--   0     1001      123     1486 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/tests/dependant.rs
+-rw-r--r--   0     1001      123     4487 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/tests/drc.rs
+-rw-r--r--   0     1001      123      420 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/tests/rrao.rs
+-rw-r--r--   0     1001      123    18903 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/tests/sbm.rs
+-rw-r--r--   0     1001      123      744 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/tests/sbm_totals.rs
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 ultibi-0.3.3/Cargo.toml
+-rw-r--r--   0     1001      123      728 2023-06-10 15:44:32.000000 ultibi-0.3.3/.gitignore
+-rw-r--r--   0     1001      123     5183 2023-06-10 15:44:32.000000 ultibi-0.3.3/LICENSE
+-rw-r--r--   0     1001      123     2403 2023-06-10 15:44:32.000000 ultibi-0.3.3/Makefile
+-rw-r--r--   0     1001      123     5565 2023-06-10 15:44:32.000000 ultibi-0.3.3/README.md
+-rw-r--r--   0     1001      123     1559 2023-06-10 15:44:32.000000 ultibi-0.3.3/example.py
+-rw-r--r--   0     1001      123     2104 2023-06-10 15:44:32.000000 ultibi-0.3.3/pyproject.toml
+-rw-r--r--   0     1001      123       36 2023-06-10 15:44:32.000000 ultibi-0.3.3/requirements-lint.txt
+-rw-r--r--   0     1001      123      307 2023-06-10 15:44:32.000000 ultibi-0.3.3/requirements.txt
+-rw-r--r--   0     1001      123     3842 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/calculator.rs
+-rw-r--r--   0     1001      123       48 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/conversions/mod.rs
+-rw-r--r--   0     1001      123     3542 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/conversions/series.rs
+-rw-r--r--   0     1001      123     3049 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/conversions/wrappers.rs
+-rw-r--r--   0     1001      123     7737 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/dataset.rs
+-rw-r--r--   0     1001      123     3303 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/errors.rs
+-rw-r--r--   0     1001      123      693 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/filter.rs
+-rw-r--r--   0     1001      123     2021 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/lib.rs
+-rw-r--r--   0     1001      123     2521 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/measure.rs
+-rw-r--r--   0     1001      123     1353 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/requests.rs
+-rw-r--r--   0     1001      123     1762 2023-06-10 15:44:32.000000 ultibi-0.3.3/tests/data/datasource_config.toml
+-rw-r--r--   0     1001      123     4042 2023-06-10 15:44:32.000000 ultibi-0.3.3/tests/docs/run_doc_examples.py
+-rw-r--r--   0     1001      123      591 2023-06-10 15:44:32.000000 ultibi-0.3.3/tests/unit/test_compute.py
+-rw-r--r--   0     1001      123     1507 2023-06-10 15:44:32.000000 ultibi-0.3.3/tests/unit/test_ds.py
+-rw-r--r--   0     1001      123     2658 2023-06-10 15:44:32.000000 ultibi-0.3.3/tests/unit/test_measure.py
+-rw-r--r--   0     1001      123      848 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/__init__.py
+-rw-r--r--   0     1001      123     1060 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/internals/__init__.py
+-rw-r--r--   0     1001      123     6733 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/internals/dataset.py
+-rw-r--r--   0     1001      123     3131 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/internals/filters.py
+-rw-r--r--   0     1001      123     5200 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/internals/measure.py
+-rw-r--r--   0     1001      123     2950 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/internals/requests.py
+-rw-r--r--   0     1001      123        0 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/rust_module/__init__.py
+-rw-r--r--   0        0        0   100879 2023-06-10 15:47:51.000000 ultibi-0.3.3/Cargo.lock
+-rw-r--r--   0        0        0     6488 1970-01-01 00:00:00.000000 ultibi-0.3.3/PKG-INFO
```

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_server/Cargo.toml` & `ultibi-0.3.3/local_dependencies/ultibi_server/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi_server"
-version= "0.3.2"
+version= "0.3.3"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_server/src/api/open_api.rs` & `ultibi-0.3.3/local_dependencies/ultibi_server/src/api/open_api.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 //! This is Work in progress
 
 use crate::api::routers;
-use ultibi_core::{filters::FilterE, AggregationRequest, add_row::AdditionalRows, overrides::Override, reports::report::Report};
+use ultibi_core::{
+    add_row::AdditionalRows, filters::FilterE, overrides::Override, reports::report::Report,
+    AggregationRequest,
+};
 use utoipa::OpenApi;
 
 #[derive(OpenApi)]
 #[openapi(
     info(
         title = "Ultima BI"
     ),
```

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_server/src/api/routers.rs` & `ultibi-0.3.3/local_dependencies/ultibi_server/src/api/routers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_server/src/app.rs` & `ultibi-0.3.3/local_dependencies/ultibi_server/src/app.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_server/src/helpers.rs` & `ultibi-0.3.3/local_dependencies/ultibi_server/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_server/src/lib.rs` & `ultibi-0.3.3/local_dependencies/ultibi_server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/Cargo.toml` & `ultibi-0.3.3/local_dependencies/frtb_engine/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "frtb_engine"
-version= "0.3.2"
+version= "0.3.3"
 edition = "2021"
 publish = false
 license-file= "LICENSE"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/Delta.csv` & `ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/Delta.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv` & `ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/data/frtb/datasource_config.toml` & `ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/calc_params.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/calc_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/docs/optional_params.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/docs/optional_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/common.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/common.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/drc_weights.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/drc_weights.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/drc/totals.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/helpers.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/lib.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/measures.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/measures.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/risk_weights.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/risk_weights.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/risk_weights_crr2.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/risk_weights_crr2.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/rrao/mod.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/rrao/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/buckets.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/buckets.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/common.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/common.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/common_curv.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/common_curv.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/delta.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/totals.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/equity/vega.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/delta.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/totals.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/fx/vega.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/delta.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/totals.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/girr/vega.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/sbm/totals.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/statics.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/statics.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/totals.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/src/validate.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/src/validate.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/tests/common/mod.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/tests/dependant.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/tests/dependant.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/tests/drc.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/tests/drc.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/tests/sbm.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/tests/sbm.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/frtb_engine/tests/sbm_totals.rs` & `ultibi-0.3.3/local_dependencies/frtb_engine/tests/sbm_totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/Cargo.toml` & `ultibi-0.3.3/local_dependencies/ultibi_core/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi_core"
-version= "0.3.2"
+version= "0.3.3"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/add_row.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/add_row.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/aggregations.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/aggregations.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/cache.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/datarequest.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/datarequest.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/dataset.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/dataset.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/acquire.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/acquire.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/awss3.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/awss3.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/helpers.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/datasource/mod.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/errors.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/errors.rs`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use polars::prelude::PolarsError;
-use thiserror::Error;
 use std::fmt::{Debug, Formatter};
+use thiserror::Error;
 
 pub type UltiResult<T> = Result<T, UltimaErr>;
 
 #[derive(Error)]
 pub enum UltimaErr {
     #[error(transparent)]
     Polars(#[from] PolarsError),
@@ -19,8 +19,8 @@
         use UltimaErr::*;
         match self {
             Polars(err) => write!(f, "{err}"),
             SerdeJson(err) => write!(f, "Couldn't serialize string. Check format. {err}"),
             Other(err) => write!(f, "BindingsError: {err}"),
         }
     }
-}
+}
```

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/execution/execute_agg.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/execution/execute_agg.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/filters.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/filters.rs`

 * *Files 6% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 #[derive(Serialize, Deserialize, Debug, Hash, Clone, Eq, PartialEq)]
 #[serde(tag = "op")]
 #[cfg_attr(feature = "openapi", derive(utoipa::ToSchema))]
 pub enum FilterE {
     /// On Same as In, but better for 1 field only
     Eq {
         field: String,
-        value: String,
+        value: Option<String>,
     },
     Neq {
         field: String,
-        value: String,
+        value: Option<String>,
     },
     In {
         field: String,
-        value: Vec<String>,
+        value: Vec<Option<String>>,
     },
     NotIn {
         field: String,
-        value: Vec<String>,
+        value: Vec<Option<String>>,
     },
 }
 
 impl FilterE {
     pub fn to_expr(&self) -> Expr {
         match self {
             FilterE::Eq { field: c, value: v } => fltr_eq(c, v),
@@ -48,35 +48,35 @@
                 field: c,
                 value: vs,
             } => fltr_not_in(c, vs),
         }
     }
 }
 
-pub(crate) fn fltr_in(c: &str, vs: &Vec<String>) -> Expr {
+pub(crate) fn fltr_in(c: &str, vs: &Vec<Option<String>>) -> Expr {
     let s = Series::new("filter", vs);
     col(c).cast(DataType::Utf8).is_in(s.lit())
 }
 
-pub(crate) fn fltr_not_in(c: &str, vs: &Vec<String>) -> Expr {
+pub(crate) fn fltr_not_in(c: &str, vs: &Vec<Option<String>>) -> Expr {
     let s = Series::new("filter", vs);
     col(c).cast(DataType::Utf8).is_in(s.lit()).not()
 }
 
-pub(crate) fn fltr_eq(c: &str, v: &str) -> Expr {
+pub(crate) fn fltr_eq(c: &str, v: &Option<String>) -> Expr {
     match v {
-        "null" => col(c).is_null(),
-        _ => col(c).cast(DataType::Utf8).eq(lit::<&str>(v)),
+        None => col(c).is_null(),
+        Some(v) => col(c).cast(DataType::Utf8).eq(lit::<&str>(v)),
     }
 }
 
-pub(crate) fn fltr_neq(c: &str, v: &str) -> Expr {
+pub(crate) fn fltr_neq(c: &str, v: &Option<String>) -> Expr {
     match v {
-        "null" => col(c).is_not_null(),
-        _ => col(c).cast(DataType::Utf8).neq(lit::<&str>(v)),
+        None => col(c).is_not_null(),
+        Some(v) => col(c).cast(DataType::Utf8).neq(lit::<&str>(v)),
     }
 }
 
 pub fn fltr_chain(chain: &AndOrFltrChain) -> Option<Expr> {
     let mut res: Option<Expr> = None;
 
     // Loop from outer vec to inner
```

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/helpers/searches.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/helpers/searches.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/measure.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/measure.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/src/overrides.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/src/overrides.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/tests/add_row.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/tests/add_row.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/tests/agg_request.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/tests/agg_request.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/tests/aggregations.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/tests/common/mod.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/tests/data/bad_config2.toml` & `ultibi-0.3.3/local_dependencies/ultibi_core/tests/data/bad_config2.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/tests/datasource.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/tests/datasource.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/tests/dependants.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/tests/dependants.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/local_dependencies/ultibi_core/tests/filters.rs` & `ultibi-0.3.3/local_dependencies/ultibi_core/tests/filters.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/Cargo.toml` & `ultibi-0.3.3/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 name = "pyultima"
-version= "0.3.2"
+version= "0.3.3"
 edition = "2021"
 publish = false
 repository= "https://github.com/ultima-ib/ultima/"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "ultibi"
 crate-type = ["cdylib"]
 
 [package.metadata.maturin]
-name = "ultibi.rust_module.ultima_pyengine"
+name = "ultibi.rust_module.ultibi_engine"
 
 [dependencies]
-pyo3 = { version = "0.18.1", features = ["extension-module", "abi3-py37"] }
+pyo3 = { version = "0.19.0", features = ["extension-module", "abi3-py37"] }
 polars = { version = "0.28.0", features = [
     "performant",
     "strings",
     "ndarray",
     "lazy",
     "is_in",
     "dtype-categorical",
@@ -29,9 +29,10 @@
 ] }
 polars-arrow = "0.28.0"
 ultibi = { path = "local_dependencies/ultibi", features=["ui"] }
 frtb_engine = { path = "local_dependencies/frtb_engine", features=["CRR2"] }
 serde_json = "1.0"
 thiserror = "1.0.38"
 once_cell = "1.17.1"
+ciborium = "0.2"
 
 [features]
```

### Comparing `ultibi-0.3.2/.gitignore` & `ultibi-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/LICENSE` & `ultibi-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/Makefile` & `ultibi-0.3.3/Makefile`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/README.md` & `ultibi-0.3.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,36 @@
 # Examples
 
 Our userguide is under development.
 In the mean time refer to FRTB [userguide](https://ultimabi.uk/ultibi-frtb-book/).
 
 ## Python
 
+### Quickstart
+```python
+import ultibi as ul
+import polars as pl
+import os
+os.environ["RUST_LOG"] = "info" # enable logs
+os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address
+
+# Read Data
+# for more details: https://pola-rs.github.io/polars/py-polars/html/reference/api/polars.read_csv.html
+df = pl.read_csv("titanic.csv")
+
+# Convert it into an Ultibi DataSet
+ds = ul.DataSet.from_frame(df, bespoke_measures=measures)
+
+# By default (might change in the future)
+# Fields are Utf8 (non numerics) and integers
+# Measures are numeric columns.
+ds.ui() 
+```
+
+### More flexible - custom measures
 ```python
 import ultibi as ul
 import polars as pl
 import os
 os.environ["RUST_LOG"] = "info" # enable logs
 os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address
```

#### html2text {}

```diff
@@ -10,50 +10,58 @@
 to write any code to analyse the data.
                                  [Ultima_Logo]
 
 Ultibi leverages on the giants: [Actix](https://github.com/actix/actix-web),
 [Polars](https://github.com/pola-rs/polars) and Rust which make this possible.
 We use TypeScript for the frontend. # Examples Our userguide is under
 development. In the mean time refer to FRTB [userguide](https://ultimabi.uk/
-ultibi-frtb-book/). ## Python ```python import ultibi as ul import polars as pl
-import os os.environ["RUST_LOG"] = "info" # enable logs os.environ["ADDRESS"] =
-"0.0.0.0:8000" # host on this address # Read Data # for more details: https://
-pola-rs.github.io/polars/py-polars/html/reference/api/polars.read_csv.html df =
-pl.read_csv("titanic.csv") # Let's add some Custom/Bespoke Calculations to our
-UI # Standard Calculator def survival_mean_age(kwargs: dict[str, str]) -
-> pl.Expr: """Mean Age of Survivals pl.col("survived") is 0 or 1 pl.col("age")
-* pl.col("survived") - age of survived person, otherwise 0 pl.col
-("survived").sum() - number of survived """ return pl.col("age") * pl.col
-("survived") / pl.col("survived").sum() # Also a Standard Calculator def
-example_dep_calc(kwargs: dict[str, str]) -> pl.Expr: return pl.col
-("SurvivalMeanAge_sum") + pl.col("SouthamptonFareDivAge_sum") # When we need
-more involved calculations we go for a Custom Calculator def custom_calculator
-( srs: list[pl.Series], kwargs: dict[str, str] ) -> pl.Series: """ Southampton
-Fare/Age*multiplier """ df = pl.DataFrame({"age": srs[0], "fare": srs[1], "e":
-srs[2]}) # Add Indicator Column for Southampton df = df.with_columns(pl.when
-(pl.col("e")=="S").then(1).otherwise(0).alias("S")) multiplier = float
-(kwargs.get("multiplier", 1)) res = df["S"] * df["fare"] / df["age"] *
-multiplier return res # inputs for the custom_calculator srs param inputs =
-["age", "fare", "embarked"] # We return Floats res_type = pl.Float64 # We
-return a Series, not a scalar (which otherwise would be auto exploded)
-returns_scalar = False measures = [ ul.BaseMeasure( "SouthamptonFareDivAge",
-ul.CustomCalculator( custom_calculator, res_type, inputs, returns_scalar ), #
-(Optional) - we are only interested in Southampton, so # unless other measures
-requested we might as well filter for Southampton only # However, if if
-multiple measures requested, their precompute_filters will be joined as OR. [
-[ul.EqFilter("embarked", "S")]], # PARAMS tab of the UI calc_params=
-[ul.CalcParam("mltplr", "1", "float")] ), ul.BaseMeasure( "SurvivalMeanAge",
-ul.StandardCalculator(survival_mean_age), aggregation_restriction="sum", ),
-ul.DependantMeasure( "A_Dependant_Measure", ul.StandardCalculator
-(example_dep_calc), [("SurvivalMeanAge", "sum"), ("SouthamptonFareDivAge",
-"sum")], ), ] # Convert it into an Ultibi DataSet ds = ul.DataSet.from_frame
-(df, bespoke_measures=measures) # By default (might change in the future) #
-Fields are Utf8 (non numerics) and integers # Measures are numeric columns.
-ds.ui() ``` Then navigate to `http://localhost:8000` or checkout `http://
-localhost:8000/swagger-ui` for the OpenAPI documentation. ### FRTB SA [FRTB SA]
-(https://en.wikipedia.org/wiki/Fundamental_Review_of_the_Trading_Book) is a
-great usecase for `ultibi`. FRTB SA is a set of standardised, computationally
+ultibi-frtb-book/). ## Python ### Quickstart ```python import ultibi as ul
+import polars as pl import os os.environ["RUST_LOG"] = "info" # enable logs
+os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address # Read Data # for
+more details: https://pola-rs.github.io/polars/py-polars/html/reference/api/
+polars.read_csv.html df = pl.read_csv("titanic.csv") # Convert it into an
+Ultibi DataSet ds = ul.DataSet.from_frame(df, bespoke_measures=measures) # By
+default (might change in the future) # Fields are Utf8 (non numerics) and
+integers # Measures are numeric columns. ds.ui() ``` ### More flexible - custom
+measures ```python import ultibi as ul import polars as pl import os os.environ
+["RUST_LOG"] = "info" # enable logs os.environ["ADDRESS"] = "0.0.0.0:8000" #
+host on this address # Read Data # for more details: https://pola-rs.github.io/
+polars/py-polars/html/reference/api/polars.read_csv.html df = pl.read_csv
+("titanic.csv") # Let's add some Custom/Bespoke Calculations to our UI #
+Standard Calculator def survival_mean_age(kwargs: dict[str, str]) -> pl.Expr:
+"""Mean Age of Survivals pl.col("survived") is 0 or 1 pl.col("age") * pl.col
+("survived") - age of survived person, otherwise 0 pl.col("survived").sum() -
+number of survived """ return pl.col("age") * pl.col("survived") / pl.col
+("survived").sum() # Also a Standard Calculator def example_dep_calc(kwargs:
+dict[str, str]) -> pl.Expr: return pl.col("SurvivalMeanAge_sum") + pl.col
+("SouthamptonFareDivAge_sum") # When we need more involved calculations we go
+for a Custom Calculator def custom_calculator( srs: list[pl.Series], kwargs:
+dict[str, str] ) -> pl.Series: """ Southampton Fare/Age*multiplier """ df =
+pl.DataFrame({"age": srs[0], "fare": srs[1], "e": srs[2]}) # Add Indicator
+Column for Southampton df = df.with_columns(pl.when(pl.col("e")=="S").then
+(1).otherwise(0).alias("S")) multiplier = float(kwargs.get("multiplier", 1))
+res = df["S"] * df["fare"] / df["age"] * multiplier return res # inputs for the
+custom_calculator srs param inputs = ["age", "fare", "embarked"] # We return
+Floats res_type = pl.Float64 # We return a Series, not a scalar (which
+otherwise would be auto exploded) returns_scalar = False measures =
+[ ul.BaseMeasure( "SouthamptonFareDivAge", ul.CustomCalculator
+( custom_calculator, res_type, inputs, returns_scalar ), # (Optional) - we are
+only interested in Southampton, so # unless other measures requested we might
+as well filter for Southampton only # However, if if multiple measures
+requested, their precompute_filters will be joined as OR. [[ul.EqFilter
+("embarked", "S")]], # PARAMS tab of the UI calc_params=[ul.CalcParam("mltplr",
+"1", "float")] ), ul.BaseMeasure( "SurvivalMeanAge", ul.StandardCalculator
+(survival_mean_age), aggregation_restriction="sum", ), ul.DependantMeasure
+( "A_Dependant_Measure", ul.StandardCalculator(example_dep_calc), [
+("SurvivalMeanAge", "sum"), ("SouthamptonFareDivAge", "sum")], ), ] # Convert
+it into an Ultibi DataSet ds = ul.DataSet.from_frame(df,
+bespoke_measures=measures) # By default (might change in the future) # Fields
+are Utf8 (non numerics) and integers # Measures are numeric columns. ds.ui()
+``` Then navigate to `http://localhost:8000` or checkout `http://localhost:
+8000/swagger-ui` for the OpenAPI documentation. ### FRTB SA [FRTB SA](https://
+en.wikipedia.org/wiki/Fundamental_Review_of_the_Trading_Book) is a great
+usecase for `ultibi`. FRTB SA is a set of standardised, computationally
 intensive rules established by the regulator. High business impact of these
 rules manifests in need for **analysis** and **visibility** thoroughout an
 organisation. Note: Ultima is not a certified aggregator. Always benchmark the
 results against your own interpretation of the rules. See python frtb
 [userguide](https://ultimabi.uk/ultibi-frtb-book/).
```

### Comparing `ultibi-0.3.2/example.py` & `ultibi-0.3.3/example.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/pyproject.toml` & `ultibi-0.3.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.0,<1.1"]
 build-backend = "maturin"
 
 [project]
 name = "ultibi"
 description = "Flexible DataFrame Operations via UI"
 readme = "README.md"
 authors = [
@@ -55,22 +55,25 @@
 disable_error_code = [
   "empty-body",
 ]
 
 [[tool.mypy.overrides]]
 module = [
   "pyarrow.*",
-  "ultibi.rust_module.ultima_pyengine",
+  "ultibi.rust_module.ultibi_engine",
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = ["ultibi.*"]
 # We exclude the ultima module from warn_return_any, because the PyO3 api does not have Python
 # type annotations. See https://github.com/PyO3/pyo3/issues/1112 for a discussion on adding
-# this capability. We could add a stub file for ultima.rust_module.ultima_pyengine (the PyO3 api), but that
+# this capability. We could add a stub file for ultima.rust_module.ultibi_engine (the PyO3 api), but that
 # amounts to duplicating almost all type annotations on our api, as the Python api itself is a
 # thin wrapper around the PyO3 api to start with.
 warn_return_any = false
 
+[tool.maturin]
+module-name = "ultibi.rust_module.ultibi_engine"
+
```

### Comparing `ultibi-0.3.2/src/calculator.rs` & `ultibi-0.3.3/src/calculator.rs`

 * *Files 3% similar despite different names*

```diff
@@ -25,27 +25,30 @@
 pub struct CalculatorWrapper {
     #[allow(dead_code)]
     pub inner: Calculator,
 }
 #[pymethods]
 impl CalculatorWrapper {
     #[classmethod]
-    /// Converts str into AggregationRequest
     pub fn standard(_: &PyType, lambda: PyObject) -> PyResult<Self> {
         let calculator = move |op: &CPM| {
             let lambda = lambda.clone();
+
             Python::with_gil(move |py| {
                 // this is a python Series
                 let out = lambda
                     .call(py, (op.into_py_dict(py),), None)
                     .map_err(|e| PolarsError::ComputeError(e.value(py).to_string().into()))?;
                 let b = out.call_method(py, "__getstate__", (), None).unwrap(); // should never fail
                 let as_pybytes = b.downcast::<PyBytes>(py).unwrap(); // should never fail
                 let rustbytes = as_pybytes.as_bytes();
-                let e = serde_json::from_slice::<Expr>(rustbytes).unwrap(); // should never fail
+                //let e = serde_json::from_slice::<Expr>(rustbytes).unwrap(); // should never fail
+                let e: Expr = ciborium::de::from_reader(rustbytes).map_err(|e| {
+                    PolarsError::ComputeError(format!("{}. Try using Custom calculator", e).into())
+                })?;
                 Ok(e)
             })
         };
         let calculator = Arc::new(calculator);
         Ok(Self { inner: calculator })
     }
```

### Comparing `ultibi-0.3.2/src/conversions/series.rs` & `ultibi-0.3.3/src/conversions/series.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/src/conversions/wrappers.rs` & `ultibi-0.3.3/src/conversions/wrappers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/src/dataset.rs` & `ultibi-0.3.3/src/dataset.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/src/errors.rs` & `ultibi-0.3.3/src/errors.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/src/filter.rs` & `ultibi-0.3.3/src/filter.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/src/lib.rs` & `ultibi-0.3.3/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #![allow(clippy::unnecessary_lazy_evaluations)]
+extern crate ultibi as ultibi_rs;
 
 use errors::{
     ArrowErrorException, ComputeError, DuplicateError, InvalidOperationError, NoDataError,
     NotFoundError, OtherError, SchemaError, SerdeJsonError, ShapeError,
 };
 use pyo3::{pyfunction, pymodule, types::PyModule, wrap_pyfunction, PyResult, Python};
 
@@ -12,24 +13,24 @@
 mod errors;
 mod filter;
 mod measure;
 mod requests;
 
 #[pyfunction]
 fn agg_ops() -> Vec<&'static str> {
-    ultibi::aggregations::BASE_CALCS
+    ultibi_rs::aggregations::BASE_CALCS
         .keys()
         .filter(|el| **el != "scalar")
         .copied()
         .collect::<Vec<&str>>()
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
-fn ultima_pyengine(_py: Python, m: &PyModule) -> PyResult<()> {
+fn ultibi_engine(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(agg_ops, m)?)?;
     //m.add_function(wrap_pyfunction!(exec_agg, m)?)?;
     m.add_class::<requests::AggregationRequestWrapper>()?;
     m.add_class::<requests::ComputeRequestWrapper>()?;
     m.add_class::<dataset::DataSetWrapper>()?;
     m.add_class::<measure::MeasureWrapper>()?;
     m.add_class::<filter::FilterWrapper>()?;
```

### Comparing `ultibi-0.3.2/src/measure.rs` & `ultibi-0.3.3/src/measure.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/src/requests.rs` & `ultibi-0.3.3/src/requests.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/tests/data/datasource_config.toml` & `ultibi-0.3.3/tests/data/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/tests/docs/run_doc_examples.py` & `ultibi-0.3.3/tests/docs/run_doc_examples.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/tests/unit/test_compute.py` & `ultibi-0.3.3/tests/unit/test_compute.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/tests/unit/test_ds.py` & `ultibi-0.3.3/tests/unit/test_ds.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/tests/unit/test_measure.py` & `ultibi-0.3.3/tests/unit/test_measure.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/ultibi/__init__.py` & `ultibi-0.3.3/ultibi/__init__.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.2/ultibi/internals/__init__.py` & `ultibi-0.3.3/ultibi/internals/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Core Ultima functionality.
 
 The modules within `ultima.internals` are interdependent. To prevent cyclical imports,
 they all import from each other via this __init__ file using
 `import ultibi.internals as uli`. The imports below are being shared across this module.
 """
 
-from ..rust_module.ultima_pyengine import NoDataError, OtherError
+from ..rust_module.ultibi_engine import NoDataError, OtherError
 from .dataset import DS, DataSet, FRTBDataSet
 from .filters import EqFilter, Filter, InFilter, NeqFilter, NotInFilter
 from .measure import (
     BaseMeasure,
     CalcParam,
     Calculator,
     CustomCalculator,
```

### Comparing `ultibi-0.3.2/ultibi/internals/dataset.py` & `ultibi-0.3.3/ultibi/internals/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Type, TypeVar
 
 import polars as pl
 
 import ultibi.internals as uli
 from ultibi.internals.measure import Measure
 
-from ..rust_module.ultima_pyengine import DataSetWrapper
+from ..rust_module.ultibi_engine import DataSetWrapper
 
 TMeasure = TypeVar("TMeasure", bound=Measure)
 
 
 # Create a generic variable that can be 'Parent', or any subclass.
 DS = TypeVar("DS", bound="DataSet")
```

### Comparing `ultibi-0.3.2/ultibi/internals/filters.py` & `ultibi-0.3.3/ultibi/internals/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import json
 from typing import Any
 
-from ..rust_module.ultima_pyengine import FilterWrapper
+from ..rust_module.ultibi_engine import FilterWrapper
 
 
 class Filter:
     """
     This is Filter to be applied on the data with your request
 
     Examples
```

### Comparing `ultibi-0.3.2/ultibi/internals/measure.py` & `ultibi-0.3.3/ultibi/internals/measure.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from typing import Protocol, Type, TypeVar
 
 from polars import DataType, Expr, Series
 
 from ultibi.internals.filters import Filter
 
-from ..rust_module.ultima_pyengine import (
+from ..rust_module.ultibi_engine import (
     CalcParamWrapper,
     CalculatorWrapper,
     MeasureWrapper,
 )
 
 
 class CalcParam:
```

### Comparing `ultibi-0.3.2/ultibi/internals/requests.py` & `ultibi-0.3.3/ultibi/internals/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import json
 from typing import Any
 
-from ..rust_module.ultima_pyengine import (
+from ..rust_module.ultibi_engine import (
     AggregationRequestWrapper,
     ComputeRequestWrapper,
     agg_ops,
 )
 
 
 def aggregation_ops() -> list[str]:
```

### Comparing `ultibi-0.3.2/Cargo.lock` & `ultibi-0.3.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "actix-codec"
-version = "0.5.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57a7559404a7f3573127aab53c08ce37a6c6a315c374a31070f3c91cd1b4a7fe"
+checksum = "617a8268e3537fe1d8c9ead925fca49ef6400927ee7bc26750e90ecee14ce4b8"
 dependencies = [
  "bitflags",
  "bytes",
  "futures-core",
  "futures-sink",
- "log",
  "memchr",
  "pin-project-lite",
  "tokio",
  "tokio-util",
+ "tracing",
 ]
 
 [[package]]
 name = "actix-files"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d832782fac6ca7369a70c9ee9a20554623c5e51c76e190ad151780ebea1cf689"
@@ -49,15 +49,15 @@
 checksum = "c2079246596c18b4a33e274ae10c0e50613f4d32a4198e09c7b93771013fed74"
 dependencies = [
  "actix-codec",
  "actix-rt",
  "actix-service",
  "actix-utils",
  "ahash 0.8.3",
- "base64 0.21.0",
+ "base64 0.21.2",
  "bitflags",
  "brotli",
  "bytes",
  "bytestring",
  "derive_more",
  "encoding_rs",
  "flate2",
@@ -186,15 +186,15 @@
  "pin-project-lite",
  "regex",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "smallvec",
  "socket2",
- "time 0.3.20",
+ "time 0.3.22",
  "url",
 ]
 
 [[package]]
 name = "actix-web-codegen"
 version = "4.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -260,17 +260,17 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.1"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "alloc-no-stdlib"
 version = "2.0.4"
@@ -283,27 +283,33 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
 dependencies = [
  "alloc-no-stdlib",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6342bd4f5a1205d7f41e94a41a901f5647c938cdfa96036338e8533c9d6c2450"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "is-terminal",
@@ -342,17 +348,17 @@
 dependencies = [
  "anstyle",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.70"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "array-init-cursor"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf7d0a018de4f6aa429b9d33d69edf69072b1c5b1cb8d3e4a5f7ef898fc3eb76"
 
@@ -364,17 +370,17 @@
 dependencies = [
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "arrow2"
-version = "0.17.0"
+version = "0.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3c63cf31f1416ed2fab8f91e8488e10129f47bd89c553ec354a06751d5697f3"
+checksum = "15ae0428d69ab31d7b2adad22a752d6f11fef2e901d2262d0cad4f5cb08b7093"
 dependencies = [
  "ahash 0.8.3",
  "arrow-format",
  "bytemuck",
  "chrono",
  "dyn-clone",
  "either",
@@ -403,15 +409,15 @@
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "atoi"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
@@ -453,15 +459,15 @@
  "aws-smithy-types",
  "aws-types",
  "bytes",
  "hex",
  "http",
  "hyper",
  "ring",
- "time 0.3.20",
+ "time 0.3.22",
  "tokio",
  "tower",
  "tracing",
  "zeroize",
 ]
 
 [[package]]
@@ -594,15 +600,15 @@
  "form_urlencoded",
  "hex",
  "http",
  "once_cell",
  "percent-encoding",
  "regex",
  "ring",
- "time 0.3.20",
+ "time 0.3.22",
  "tracing",
 ]
 
 [[package]]
 name = "aws-smithy-async"
 version = "0.49.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -730,15 +736,15 @@
 version = "0.49.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e93b0c93a3b963da946a0b8ef3853a7252298eb75cdbfb21dad60f5ed0ded861"
 dependencies = [
  "itoa",
  "num-integer",
  "ryu",
- "time 0.3.20",
+ "time 0.3.22",
 ]
 
 [[package]]
 name = "aws-smithy-xml"
 version = "0.49.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "36b9efb4855b4acb29961a776d45680f3cbdd7c4783cbbae078da54c342575dd"
@@ -766,17 +772,17 @@
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
-version = "0.21.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -808,17 +814,17 @@
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.1"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "bytemuck"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 dependencies = [
@@ -829,15 +835,15 @@
 name = "bytemuck_derive"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fdde5c9cd29ebd706ce1b35600920a33550e402fc998a2e53ad3b42c3c47a192"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
@@ -890,91 +896,108 @@
 dependencies = [
  "path-matchers",
  "path-slash",
 ]
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
  "js-sys",
- "num-integer",
  "num-traits",
  "serde",
  "time 0.1.45",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
+name = "ciborium"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
+dependencies = [
+ "ciborium-io",
+ "ciborium-ll",
+ "serde",
+]
+
+[[package]]
+name = "ciborium-io"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
+
+[[package]]
+name = "ciborium-ll"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
+dependencies = [
+ "ciborium-io",
+ "half",
+]
+
+[[package]]
 name = "clap"
-version = "4.2.4"
+version = "4.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "956ac1f6381d8d82ab4684768f89c0ea3afe66925ceadb4eeb3fc452ffc55d62"
+checksum = "ca8f255e4b8027970e78db75e78831229c9815fdbfa67eb1a1b777a62e24b4a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.4"
+version = "4.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84080e799e54cff944f4b4a4b0e71630b0e0443b25b985175c7dddc1a859b749"
+checksum = "acd4f3c17c83b0ba34ffbc4f8bbd74f079413f747f84a6f89292f138057e36ab"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.2.0"
+version = "4.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f9644cd56d6b87dbe899ef8b053e331c0637664e9e21a33dfcdc36093f5c5c4"
+checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
-
-[[package]]
-name = "codespan-reporting"
-version = "0.11.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
 name = "comfy-table"
-version = "6.1.4"
+version = "6.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6e7b787b0dc42e8111badfdbe4c3059158ccb2db8780352fa1b01e8ccf45cc4d"
+checksum = "7e959d788268e3bf9d35ace83e81b124190378e4c91c9067524675e33394b8ba"
 dependencies = [
  "crossterm",
  "strum",
  "strum_macros",
  "unicode-width",
 ]
 
@@ -987,15 +1010,15 @@
 [[package]]
 name = "cookie"
 version = "0.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e859cd57d0710d9e06c381b550c06e76992472a8c6d527aecd2fc673dcc231fb"
 dependencies = [
  "percent-encoding",
- "time 0.3.20",
+ "time 0.3.22",
  "version_check",
 ]
 
 [[package]]
 name = "core-foundation"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1064,32 +1087,32 @@
 version = "0.9.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset",
+ "memoffset 0.8.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
 version = "0.8.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossterm"
-version = "0.25.0"
+version = "0.26.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e64e6c0fbe2c17357405f7c758c1ef960fce08bdfb2c03d88d2a18d7e09c4b67"
+checksum = "a84cda67535339806297f1b331d6dd6320470d2a0fe65381e79ee9e156dd3d13"
 dependencies = [
  "bitflags",
  "crossterm_winapi",
  "libc",
  "mio",
  "parking_lot 0.12.1",
  "signal-hook",
@@ -1122,68 +1145,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1a816186fa68d9e426e3cb4ae4dff1fcd8e4a2c34b781bf7a822574a0d0aac8"
 dependencies = [
  "sct",
 ]
 
 [[package]]
-name = "cxx"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12cee708e8962df2aeb38f594aae5d827c022b6460ac71a7a3e2c3c2aae5a07b"
-dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
- "proc-macro2",
- "quote",
- "scratch",
- "syn 2.0.15",
-]
-
-[[package]]
-name = "cxxbridge-flags"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
-
-[[package]]
-name = "cxxbridge-macro"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.15",
-]
-
-[[package]]
 name = "dashmap"
 version = "5.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
 dependencies = [
  "cfg-if",
  "hashbrown 0.12.3",
  "lock_api",
  "once_cell",
- "parking_lot_core 0.9.7",
+ "parking_lot_core 0.9.8",
 ]
 
 [[package]]
 name = "derivative"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcc3dd5e9e9c0b295d6e1e4d811fb6f157d5ffd784b8d202fc62eac8035a770b"
@@ -1204,17 +1183,17 @@
  "quote",
  "rustc_version",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "dirs"
@@ -1328,17 +1307,17 @@
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -1365,24 +1344,24 @@
 name = "foreign_vec"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "frtb_engine"
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
  "log",
  "ndarray",
  "once_cell",
  "polars",
  "rayon",
  "serde",
@@ -1445,15 +1424,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -1490,17 +1469,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
@@ -1509,17 +1488,17 @@
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "h2"
-version = "0.3.18"
+version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f8a914c2987b688368b5138aa05321db91f4090cf26118185672ad588bce21"
+checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -1527,14 +1506,20 @@
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
+name = "half"
+version = "1.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
+
+[[package]]
 name = "hash_hasher"
 version = "2.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "74721d007512d0cb3338cd20f0654ac913920061a4c4d0d8708edb3f2a698c0c"
 
 [[package]]
 name = "hashbrown"
@@ -1689,41 +1674,40 @@
  "native-tls",
  "tokio",
  "tokio-native-tls",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.56"
+version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "idna"
-version = "0.3.0"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
@@ -1749,17 +1733,17 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
@@ -1813,17 +1797,17 @@
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "language-tags"
 version = "0.3.2"
@@ -1907,48 +1891,39 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "libm"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "libmimalloc-sys"
-version = "0.1.32"
+version = "0.1.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43a558e3d911bc3c7bfc8c78bc580b404d6e51c1cefbf656e176a94b49b0df40"
+checksum = "f4ac0e912c8ef1b735e92369695618dc5b1819f5a7bf3f167301a3ba1cea515e"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
-name = "link-cplusplus"
-version = "1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
-dependencies = [
- "cc",
-]
-
-[[package]]
 name = "linux-raw-sys"
-version = "0.3.4"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36eb31c1778188ae1e64398743890d0877fef36d11521ac60406b42016e8c2cf"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "local-channel"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f303ec0e94c6c54447f84f3b0ef7af769858a9c4ef56ef2a986d3dcd4c3fc9c"
 dependencies = [
@@ -1962,30 +1937,27 @@
 name = "local-waker"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e34f76eb3611940e0e7d53a9aaa4e6a3151f69541a282fd0dad5571420c53ff1"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "lz4"
 version = "1.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e9e2dd86df36ce760a60f6ff6ad526f7ba1f14ba0356f8254fb6905e6494df1"
 dependencies = [
@@ -2001,18 +1973,19 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.3"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb99c395ae250e1bf9133673f03ca9f97b7e71b705436bf8f089453445d1e9fe"
+checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
+ "autocfg",
  "num_cpus",
  "once_cell",
  "rawpointer",
  "thread-tree",
 ]
 
 [[package]]
@@ -2045,18 +2018,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "mimalloc"
-version = "0.1.36"
+version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d88dad3f985ec267a3fcb7a1726f5cb1a7e8cad8b646e70a84f967210df23da"
+checksum = "4e2894987a3459f3ffb755608bd82188f8ed00d0ae077f1edea29c068d639d98"
 dependencies = [
  "libmimalloc-sys",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
@@ -2071,48 +2053,48 @@
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.6.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.6"
+version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
  "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "multiversion"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6a87eede2251ca235e5573086d01d2ab6b59dfaea54c2be10f9320980f7e8f7"
+checksum = "8cda45dade5144c2c929bf2ed6c24bebbba784e9198df049ec87d722b9462bd1"
 dependencies = [
  "multiversion-macros",
  "target-features",
 ]
 
 [[package]]
 name = "multiversion-macros"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1af1abf82261d780d114014eff4b555e47d823f3b84f893c4388572b40e089fb"
+checksum = "04bffdccbd4798b61dce08c97ce8c66a68976f95541aaf284a6e90c1d1c306e1"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
  "target-features",
 ]
 
@@ -2204,23 +2186,23 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "openssl"
-version = "0.10.52"
+version = "0.10.54"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01b8574602df80f7b85fdfc5392fa884a4e3b3f4f35402c070ab34c3d3f78d56"
+checksum = "69b3f656a17a6cbc115b5c7a40c616947d213ba182135b014d6051b73ab6f019"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
@@ -2231,28 +2213,28 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.87"
+version = "0.9.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e17f59264b2809d77ae94f0e1ebabc434773f370d6ca667bd223ea10e06cc7e"
+checksum = "c2ce0f250f34a308dcfdbb351f511359857d4ed2134ba715a4eadd46e1ffd617"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -2270,15 +2252,15 @@
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
- "parking_lot_core 0.9.7",
+ "parking_lot_core 0.9.8",
 ]
 
 [[package]]
 name = "parking_lot_core"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
@@ -2289,23 +2271,23 @@
  "redox_syscall 0.2.16",
  "smallvec",
  "winapi",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall 0.2.16",
+ "redox_syscall 0.3.5",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
@@ -2323,36 +2305,36 @@
 name = "path-slash"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "498a099351efa4becc6a19c72aa9270598e8fd274ca47052e37455241c88b696"
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pin-project"
-version = "1.0.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad29a609b6bcd67fee905812e544992d216af9d755757c05ed2d0e15a74c6ecc"
+checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.0.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "069bdb1e05adc7a8990dce9cc75370895fbe4e3d58b9b73bf1aee56359344a55"
+checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
@@ -2361,17 +2343,17 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "planus"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
@@ -2642,85 +2624,86 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
+ "memoffset 0.9.0",
  "parking_lot 0.12.1",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyultima"
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
+ "ciborium",
  "frtb_engine",
  "once_cell",
  "polars",
  "polars-arrow",
  "pyo3",
  "serde_json",
  "thiserror",
@@ -2731,17 +2714,17 @@
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -2837,36 +2820,36 @@
  "getrandom",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.1"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "reqwest"
-version = "0.11.16"
+version = "0.11.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "27b71749df584b7f4cac2c426c127a7c785a5106cc98f7a8feb044115f0fa254"
+checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
 dependencies = [
- "base64 0.21.0",
+ "base64 0.21.2",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -2906,34 +2889,34 @@
  "untrusted",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "rust-embed"
-version = "6.6.1"
+version = "6.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b68543d5527e158213414a92832d2aab11a84d2571a5eb021ebe22c43aab066"
+checksum = "b73e721f488c353141288f223b599b4ae9303ecf3e62923f40a492f0634a4dc3"
 dependencies = [
  "rust-embed-impl",
  "rust-embed-utils",
  "walkdir",
 ]
 
 [[package]]
 name = "rust-embed-impl"
-version = "6.5.0"
+version = "6.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d4e0f0ced47ded9a68374ac145edd65a6c1fa13a96447b873660b2a568a0fd7"
+checksum = "e22ce362f5561923889196595504317a4372b84210e6e335da529a65ea5452b5"
 dependencies = [
  "proc-macro2",
  "quote",
  "rust-embed-utils",
  "shellexpand",
- "syn 1.0.109",
+ "syn 2.0.18",
  "walkdir",
 ]
 
 [[package]]
 name = "rust-embed-utils"
 version = "7.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2950,17 +2933,17 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.14"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b864d3c18a5785a05953adeed93e2dca37ed30f18e69bba9f30079d51f363f"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -3024,76 +3007,70 @@
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
-name = "scratch"
-version = "1.0.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
-
-[[package]]
 name = "sct"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b362b83898e0e69f38515b82ee15aa80636befe47c3b6d3d89a911e78fc228ce"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.8.2"
+version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a332be01508d814fed64bf28f798a146d73792121129962fdf335bb3c49a4254"
+checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
 dependencies = [
  "bitflags",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.8.0"
+version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31c9bb296072e961fcbd8853511dd39c2d8be2deb1e17c6860b1d30732b323b4"
+checksum = "f51d0c0d83bec45f16480d0ce0058397a69e48fcdc52d1dc8855fb68acbd31a7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.160"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.160"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
@@ -3101,17 +3078,17 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0efd8caf556a6cebd3b285caf480045fcc1ac04f6bd786b09a6f11af30c4fcf4"
+checksum = "93107647184f6027e3b7dcb2e11034cf95ffa1e3a682c67951963ac69c1c007d"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
@@ -3294,17 +3271,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3319,40 +3296,41 @@
  "ntapi",
  "once_cell",
  "winapi",
 ]
 
 [[package]]
 name = "target-features"
-version = "0.1.3"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24840de800c1707d75c800893dbd727a5e1501ce921944e602f0698167491e36"
+checksum = "06f6b473c37f9add4cf1df5b4d66a8ef58ab6c895f1a3b3f949cf3e21230140e"
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
-version = "3.5.0"
+version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
+checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
+ "autocfg",
  "cfg-if",
  "fastrand",
  "redox_syscall 0.3.5",
  "rustix",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "template_drivers"
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
  "actix-files",
  "actix-web",
  "actix-web-httpauth",
  "actix-web-static-files",
  "anyhow",
  "clap",
@@ -3396,15 +3374,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "thread-tree"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ffbd370cb847953a25954d9f63e14824a36113f8c72eecf6eccef5dc4b45d630"
@@ -3421,35 +3399,35 @@
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.20"
+version = "0.3.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
 dependencies = [
  "itoa",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
@@ -3463,40 +3441,40 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.27.0"
+version = "1.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0de47a4eecbe11f498978a9b29d792f0d2692d1dd003650c24c76510e3bc001"
+checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot 0.12.1",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61a573bdc87985e9d6ddeed1b3d864e8a302c847e40d647746df2f1de209d1ce"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -3514,63 +3492,63 @@
  "rustls",
  "tokio",
  "webpki",
 ]
 
 [[package]]
 name = "tokio-stream"
-version = "0.1.12"
+version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8fb52b74f05dbf495a8fba459fdc331812b96aa086d9eb78101fa0d4569c3313"
+checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.7"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5427d89453009325de0d8f342c9490009f76e999cb7672d77e46267448f7e6b2"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "toml"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b403acf6f2bb0859c93c7f0d967cb4a75a7ac552100f9322faf64dc047669b21"
+checksum = "d6135d499e69981f9ff0ef2167955a5333c35e36f6937d382974566b3d5b94ec"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ab8ed2edee10b50132aed5f331333428b011c99402b5a534154ed15746f9622"
+checksum = "5a76a9312f5ba4c2dec6b9161fdf25d87ad8a09256ccea5a556fef03c706a10f"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.19.8"
+version = "0.19.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "239410c8609e8125456927e6707163a3b1fdb40561e4b803bc041f466ccfdc13"
+checksum = "2380d56e8670370eee6566b0bfd4265f65b3f432e8c6d85623f728d4fa31f739"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
@@ -3620,22 +3598,22 @@
 name = "tracing-attributes"
 version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "try-lock"
 version = "0.2.4"
@@ -3646,23 +3624,23 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "ultibi"
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
  "ultibi_core",
  "ultibi_server",
 ]
 
 [[package]]
 name = "ultibi_core"
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
  "aws-config",
  "aws-sdk-s3",
  "dashmap",
  "derivative",
  "futures",
  "once_cell",
@@ -3674,15 +3652,15 @@
  "tokio",
  "toml",
  "utoipa",
 ]
 
 [[package]]
 name = "ultibi_server"
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
  "actix-web",
  "actix-web-static-files",
  "anyhow",
  "dotenv",
  "log",
  "mime",
@@ -3710,17 +3688,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -3743,17 +3721,17 @@
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
@@ -3767,55 +3745,55 @@
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "utoipa"
 version = "3.3.0"
-source = "git+https://github.com/juhaku/utoipa#489ddd663051a578e9285f5f4b5d87c0f626d6c0"
+source = "git+https://github.com/juhaku/utoipa#f8c6d07ef699d4fd6d3eeddfb55d6955d89af0f6"
 dependencies = [
  "indexmap",
  "serde",
  "serde_json",
  "utoipa-gen",
 ]
 
 [[package]]
 name = "utoipa-gen"
 version = "3.3.0"
-source = "git+https://github.com/juhaku/utoipa#489ddd663051a578e9285f5f4b5d87c0f626d6c0"
+source = "git+https://github.com/juhaku/utoipa#f8c6d07ef699d4fd6d3eeddfb55d6955d89af0f6"
 dependencies = [
  "lazy_static",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "regex",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "utoipa-swagger-ui"
 version = "3.1.3"
-source = "git+https://github.com/juhaku/utoipa#489ddd663051a578e9285f5f4b5d87c0f626d6c0"
+source = "git+https://github.com/juhaku/utoipa#f8c6d07ef699d4fd6d3eeddfb55d6955d89af0f6"
 dependencies = [
  "actix-web",
  "mime_guess",
  "regex",
  "rust-embed",
  "serde",
  "serde_json",
  "utoipa",
  "zip",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.1"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b55a3fef2a1e3b3a00ce878640918820d3c51081576ac657d23af9fc7928fdb"
+checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
@@ -3858,77 +3836,77 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.34"
+version = "0.4.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f219e0d211ba40266969f6dbdd90636da12f75bee4fc9d6c23d1260dadb51454"
+checksum = "2d1985d03709c53167ce907ff394f5316aa22cb4e12761295c5dc57dacb6297e"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
 
 [[package]]
 name = "wasm-timer"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be0ecb0db480561e9a7642b5d3e4187c128914e58aa84330b9493e3eb68c5e7f"
 dependencies = [
@@ -3939,17 +3917,17 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
 ]
 
 [[package]]
 name = "web-sys"
-version = "0.3.61"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki"
@@ -3994,15 +3972,15 @@
 
 [[package]]
 name = "windows"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets 0.48.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
@@ -4014,43 +3992,19 @@
  "windows_x86_64_gnu 0.42.2",
  "windows_x86_64_gnullvm 0.42.2",
  "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.0",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
@@ -4146,17 +4100,17 @@
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winnow"
-version = "0.4.1"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
+checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.10.1"
@@ -4176,34 +4130,33 @@
 name = "xxhash-rust"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "735a71d46c4d68d71d4b24d03fdc2b98e38cea81730595801db779c04fe80d70"
 
 [[package]]
 name = "yearfrac"
-version = "0.1.6"
+version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73ba657166ee46d227598eb47c3c7d121eceea28aa43a03fbf76657ac8b4fea7"
+checksum = "e9d98f5fc90def6755a07c239d1852ed9f34535cfbf85ee9f62d87e62aebbbc3"
 dependencies = [
  "chrono",
- "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
 
 [[package]]
 name = "zip"
-version = "0.6.4"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0445d0fbc924bb93539b4316c11afb121ea39296f99a3c4c9edad09e3658cdef"
+checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
 dependencies = [
  "byteorder",
  "crc32fast",
  "crossbeam-utils",
  "flate2",
 ]
```

### Comparing `ultibi-0.3.2/PKG-INFO` & `ultibi-0.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultibi
-Version: 0.3.2
+Version: 0.3.3
 Classifier: Programming Language :: Rust
 Classifier: License :: Free for non-commercial use
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,17 +12,17 @@
 Requires-Dist: pyarrow
 License-File: LICENSE
 Summary: Flexible DataFrame Operations via UI
 Keywords: dataframe,visualization,aggregation,calculation,chart,data,dataviz,pivot-table,frtb,risk
 Author-email: Anatoly Bugakov <anatoly@ultimabi.uk>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Repository, https://github.com/ultima-ib/ultibi-frtb-book
 Project-URL: Documentation, https://ultimabi.uk/ultibi-frtb-book/
 Project-URL: Homepage, https://ultimabi.uk/
-Project-URL: Repository, https://github.com/ultima-ib/ultibi-frtb-book
 
 <br>
 
 <p align="center">
     <a href="https://ultimabi.uk/" target="_blank">
     <img width="900" src="https://ultima-bi.s3.eu-west-2.amazonaws.com/imgs/logo.png" alt="Ultima Logo">
     </a>
@@ -51,14 +51,36 @@
 # Examples
 
 Our userguide is under development.
 In the mean time refer to FRTB [userguide](https://ultimabi.uk/ultibi-frtb-book/).
 
 ## Python
 
+### Quickstart
+```python
+import ultibi as ul
+import polars as pl
+import os
+os.environ["RUST_LOG"] = "info" # enable logs
+os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address
+
+# Read Data
+# for more details: https://pola-rs.github.io/polars/py-polars/html/reference/api/polars.read_csv.html
+df = pl.read_csv("titanic.csv")
+
+# Convert it into an Ultibi DataSet
+ds = ul.DataSet.from_frame(df, bespoke_measures=measures)
+
+# By default (might change in the future)
+# Fields are Utf8 (non numerics) and integers
+# Measures are numeric columns.
+ds.ui() 
+```
+
+### More flexible - custom measures
 ```python
 import ultibi as ul
 import polars as pl
 import os
 os.environ["RUST_LOG"] = "info" # enable logs
 os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: ultibi Version: 0.3.2 Classifier: Programming
+Metadata-Version: 2.1 Name: ultibi Version: 0.3.3 Classifier: Programming
 Language :: Rust Classifier: License :: Free for non-commercial use Classifier:
 Topic :: Scientific/Engineering Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: polars Requires-Dist: pyarrow License-File: LICENSE Summary:
 Flexible DataFrame Operations via UI Keywords:
 dataframe,visualization,aggregation,calculation,chart,data,dataviz,pivot-
 table,frtb,risk Author-email: Anatoly Bugakov
 ultimabi.uk> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: Documentation, https://ultimabi.uk/
-ultibi-frtb-book/ Project-URL: Homepage, https://ultimabi.uk/ Project-URL:
-Repository, https://github.com/ultima-ib/ultibi-frtb-book
+charset=UTF-8; variant=GFM Project-URL: Repository, https://github.com/ultima-
+ib/ultibi-frtb-book Project-URL: Documentation, https://ultimabi.uk/ultibi-
+frtb-book/ Project-URL: Homepage, https://ultimabi.uk/
                                  [Ultima_Logo]
 
                     **** the ultimate data analytics tool
          for no code visualisation and collaborative exploration. ****
          **** Present easier.   Dig deeper.   Review together.   ****
 # The Ultimate BI tool With `Ultibi` you can turn your `DataFrame` into a pivot
 table with a UI and share it across organisation. You can also define measures
@@ -22,50 +22,58 @@
 to write any code to analyse the data.
                                  [Ultima_Logo]
 
 Ultibi leverages on the giants: [Actix](https://github.com/actix/actix-web),
 [Polars](https://github.com/pola-rs/polars) and Rust which make this possible.
 We use TypeScript for the frontend. # Examples Our userguide is under
 development. In the mean time refer to FRTB [userguide](https://ultimabi.uk/
-ultibi-frtb-book/). ## Python ```python import ultibi as ul import polars as pl
-import os os.environ["RUST_LOG"] = "info" # enable logs os.environ["ADDRESS"] =
-"0.0.0.0:8000" # host on this address # Read Data # for more details: https://
-pola-rs.github.io/polars/py-polars/html/reference/api/polars.read_csv.html df =
-pl.read_csv("titanic.csv") # Let's add some Custom/Bespoke Calculations to our
-UI # Standard Calculator def survival_mean_age(kwargs: dict[str, str]) -
-> pl.Expr: """Mean Age of Survivals pl.col("survived") is 0 or 1 pl.col("age")
-* pl.col("survived") - age of survived person, otherwise 0 pl.col
-("survived").sum() - number of survived """ return pl.col("age") * pl.col
-("survived") / pl.col("survived").sum() # Also a Standard Calculator def
-example_dep_calc(kwargs: dict[str, str]) -> pl.Expr: return pl.col
-("SurvivalMeanAge_sum") + pl.col("SouthamptonFareDivAge_sum") # When we need
-more involved calculations we go for a Custom Calculator def custom_calculator
-( srs: list[pl.Series], kwargs: dict[str, str] ) -> pl.Series: """ Southampton
-Fare/Age*multiplier """ df = pl.DataFrame({"age": srs[0], "fare": srs[1], "e":
-srs[2]}) # Add Indicator Column for Southampton df = df.with_columns(pl.when
-(pl.col("e")=="S").then(1).otherwise(0).alias("S")) multiplier = float
-(kwargs.get("multiplier", 1)) res = df["S"] * df["fare"] / df["age"] *
-multiplier return res # inputs for the custom_calculator srs param inputs =
-["age", "fare", "embarked"] # We return Floats res_type = pl.Float64 # We
-return a Series, not a scalar (which otherwise would be auto exploded)
-returns_scalar = False measures = [ ul.BaseMeasure( "SouthamptonFareDivAge",
-ul.CustomCalculator( custom_calculator, res_type, inputs, returns_scalar ), #
-(Optional) - we are only interested in Southampton, so # unless other measures
-requested we might as well filter for Southampton only # However, if if
-multiple measures requested, their precompute_filters will be joined as OR. [
-[ul.EqFilter("embarked", "S")]], # PARAMS tab of the UI calc_params=
-[ul.CalcParam("mltplr", "1", "float")] ), ul.BaseMeasure( "SurvivalMeanAge",
-ul.StandardCalculator(survival_mean_age), aggregation_restriction="sum", ),
-ul.DependantMeasure( "A_Dependant_Measure", ul.StandardCalculator
-(example_dep_calc), [("SurvivalMeanAge", "sum"), ("SouthamptonFareDivAge",
-"sum")], ), ] # Convert it into an Ultibi DataSet ds = ul.DataSet.from_frame
-(df, bespoke_measures=measures) # By default (might change in the future) #
-Fields are Utf8 (non numerics) and integers # Measures are numeric columns.
-ds.ui() ``` Then navigate to `http://localhost:8000` or checkout `http://
-localhost:8000/swagger-ui` for the OpenAPI documentation. ### FRTB SA [FRTB SA]
-(https://en.wikipedia.org/wiki/Fundamental_Review_of_the_Trading_Book) is a
-great usecase for `ultibi`. FRTB SA is a set of standardised, computationally
+ultibi-frtb-book/). ## Python ### Quickstart ```python import ultibi as ul
+import polars as pl import os os.environ["RUST_LOG"] = "info" # enable logs
+os.environ["ADDRESS"] = "0.0.0.0:8000" # host on this address # Read Data # for
+more details: https://pola-rs.github.io/polars/py-polars/html/reference/api/
+polars.read_csv.html df = pl.read_csv("titanic.csv") # Convert it into an
+Ultibi DataSet ds = ul.DataSet.from_frame(df, bespoke_measures=measures) # By
+default (might change in the future) # Fields are Utf8 (non numerics) and
+integers # Measures are numeric columns. ds.ui() ``` ### More flexible - custom
+measures ```python import ultibi as ul import polars as pl import os os.environ
+["RUST_LOG"] = "info" # enable logs os.environ["ADDRESS"] = "0.0.0.0:8000" #
+host on this address # Read Data # for more details: https://pola-rs.github.io/
+polars/py-polars/html/reference/api/polars.read_csv.html df = pl.read_csv
+("titanic.csv") # Let's add some Custom/Bespoke Calculations to our UI #
+Standard Calculator def survival_mean_age(kwargs: dict[str, str]) -> pl.Expr:
+"""Mean Age of Survivals pl.col("survived") is 0 or 1 pl.col("age") * pl.col
+("survived") - age of survived person, otherwise 0 pl.col("survived").sum() -
+number of survived """ return pl.col("age") * pl.col("survived") / pl.col
+("survived").sum() # Also a Standard Calculator def example_dep_calc(kwargs:
+dict[str, str]) -> pl.Expr: return pl.col("SurvivalMeanAge_sum") + pl.col
+("SouthamptonFareDivAge_sum") # When we need more involved calculations we go
+for a Custom Calculator def custom_calculator( srs: list[pl.Series], kwargs:
+dict[str, str] ) -> pl.Series: """ Southampton Fare/Age*multiplier """ df =
+pl.DataFrame({"age": srs[0], "fare": srs[1], "e": srs[2]}) # Add Indicator
+Column for Southampton df = df.with_columns(pl.when(pl.col("e")=="S").then
+(1).otherwise(0).alias("S")) multiplier = float(kwargs.get("multiplier", 1))
+res = df["S"] * df["fare"] / df["age"] * multiplier return res # inputs for the
+custom_calculator srs param inputs = ["age", "fare", "embarked"] # We return
+Floats res_type = pl.Float64 # We return a Series, not a scalar (which
+otherwise would be auto exploded) returns_scalar = False measures =
+[ ul.BaseMeasure( "SouthamptonFareDivAge", ul.CustomCalculator
+( custom_calculator, res_type, inputs, returns_scalar ), # (Optional) - we are
+only interested in Southampton, so # unless other measures requested we might
+as well filter for Southampton only # However, if if multiple measures
+requested, their precompute_filters will be joined as OR. [[ul.EqFilter
+("embarked", "S")]], # PARAMS tab of the UI calc_params=[ul.CalcParam("mltplr",
+"1", "float")] ), ul.BaseMeasure( "SurvivalMeanAge", ul.StandardCalculator
+(survival_mean_age), aggregation_restriction="sum", ), ul.DependantMeasure
+( "A_Dependant_Measure", ul.StandardCalculator(example_dep_calc), [
+("SurvivalMeanAge", "sum"), ("SouthamptonFareDivAge", "sum")], ), ] # Convert
+it into an Ultibi DataSet ds = ul.DataSet.from_frame(df,
+bespoke_measures=measures) # By default (might change in the future) # Fields
+are Utf8 (non numerics) and integers # Measures are numeric columns. ds.ui()
+``` Then navigate to `http://localhost:8000` or checkout `http://localhost:
+8000/swagger-ui` for the OpenAPI documentation. ### FRTB SA [FRTB SA](https://
+en.wikipedia.org/wiki/Fundamental_Review_of_the_Trading_Book) is a great
+usecase for `ultibi`. FRTB SA is a set of standardised, computationally
 intensive rules established by the regulator. High business impact of these
 rules manifests in need for **analysis** and **visibility** thoroughout an
 organisation. Note: Ultima is not a certified aggregator. Always benchmark the
 results against your own interpretation of the rules. See python frtb
 [userguide](https://ultimabi.uk/ultibi-frtb-book/).
```


# Comparing `tmp/highcharts_maps-1.0.0rc6.tar.gz` & `tmp/highcharts_maps-1.0.1.tar.gz`

## Comparing `highcharts_maps-1.0.0rc6.tar` & `highcharts_maps-1.0.1.tar`

### file list

```diff
@@ -1,1485 +1,1485 @@
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/.readthedocs.yaml
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/.travis.yml
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/CHANGES.rst
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/requirements.dev.txt
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/requirements.travis.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/requirements.txt
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/setup.cfg
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tox.ini
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/.github/workflows/pypi-test-publish.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/Makefile
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_contributors.rst
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_dependencies.rst
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_installation.rst
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_support.rst
--rw-r--r--   0        0        0     9776 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_versus_alternatives.rst
--rw-r--r--   0        0        0    56205 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api.rst
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/conf.py
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/contributing.rst
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/demos.rst
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/errors.rst
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/faq.rst
--rw-r--r--   0        0        0    34457 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/glossary.rst
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/history.rst
--rw-r--r--   0        0        0    16243 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/index.rst
--rw-r--r--   0        0        0    24959 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/license.rst
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/links.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/make.bat
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/quickstart.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/support.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/testing.rst
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/toolkit.rst
--rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using.rst
--rw-r--r--   0        0        0    41670 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/visualizations.rst
--rw-r--r--   0        0        0    54859 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/abands-example.png
--rw-r--r--   0        0        0    34552 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/ad-example.png
--rw-r--r--   0        0        0    43218 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/apo-example.png
--rw-r--r--   0        0        0    87899 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/arcdiagram-example.png
--rw-r--r--   0        0        0    72487 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/area-example.png
--rw-r--r--   0        0        0   124371 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/arearange-example.png
--rw-r--r--   0        0        0    55288 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/areaspline-example.png
--rw-r--r--   0        0        0    54998 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/aroon-example.png
--rw-r--r--   0        0        0    46438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/aroon-oscillator-example.png
--rw-r--r--   0        0        0    47100 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/atr-example.png
--rw-r--r--   0        0        0    20359 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/awesome-oscillator-example.png
--rw-r--r--   0        0        0   485952 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/axis-property-mapping.xlsx
--rw-r--r--   0        0        0    59173 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/bar-example.png
--rw-r--r--   0        0        0    48934 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/bellcurve-example.png
--rw-r--r--   0        0        0    43491 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/bollinger-bands-example.png
--rw-r--r--   0        0        0    37690 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/boxplot-example.png
--rw-r--r--   0        0        0    92954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/bubble-example.png
--rw-r--r--   0        0        0    26870 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/bullet-example.png
--rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/candlestick-example.png
--rw-r--r--   0        0        0    52121 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/cci-example.png
--rw-r--r--   0        0        0    49536 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/chaikin-example.png
--rw-r--r--   0        0        0    46772 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/cmf-example.png
--rw-r--r--   0        0        0    47632 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/cmo-example.png
--rw-r--r--   0        0        0    41242 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/column-example.png
--rw-r--r--   0        0        0    41567 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/columnpyramid-example-stacked-horizontal.png
--rw-r--r--   0        0        0    31515 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/columnpyramid-example-stacked.png
--rw-r--r--   0        0        0    51790 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/columnpyramid-example.png
--rw-r--r--   0        0        0    63741 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/columnrange-example-horizontal.png
--rw-r--r--   0        0        0    68246 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/columnrange-example.png
--rw-r--r--   0        0        0    67368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/cylinder-example.png
--rw-r--r--   0        0        0    54030 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/dema-example.png
--rw-r--r--   0        0        0   252801 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/dependencywheel-example.png
--rw-r--r--   0        0        0    49737 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/disparity-index-example.png
--rw-r--r--   0        0        0    45925 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/dmi-example.png
--rw-r--r--   0        0        0    37726 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/dpo-example.png
--rw-r--r--   0        0        0    66693 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/dumbbell-example.png
--rw-r--r--   0        0        0    38446 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/ema-example.png
--rw-r--r--   0        0        0    59876 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/errorbar-example.png
--rw-r--r--   0        0        0    27702 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/flags-example.png
--rw-r--r--   0        0        0    43626 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/funnel-example.png
--rw-r--r--   0        0        0    60815 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/funnel_3d-example.png
--rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/gantt-example.png
--rw-r--r--   0        0        0   129516 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/gauge-example.png
--rw-r--r--   0        0        0    87393 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/heatmap-example.png
--rw-r--r--   0        0        0    29731 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/heikin-ashi-example.png
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/highcharts-for-python-dark-32x32.png
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/highcharts-for-python-light-150x149.png
--rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/highcharts-logo.svg
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/highcharts-python-logo.png
--rw-r--r--   0        0        0    38747 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/histogram-example.png
--rw-r--r--   0        0        0    25456 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/hlc-example.png
--rw-r--r--   0        0        0    34397 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/hollow-candlestick-example.png
--rw-r--r--   0        0        0    73793 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/ikh-example.png
--rw-r--r--   0        0        0   208287 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/item-example-circular.png
--rw-r--r--   0        0        0   151954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/item-example-rectangular.png
--rw-r--r--   0        0        0    15447 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/item-example-symbols.png
--rw-r--r--   0        0        0    47093 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/keltner-channels-example.png
--rw-r--r--   0        0        0    40750 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/klinger-example.png
--rw-r--r--   0        0        0    81283 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/line-example.png
--rw-r--r--   0        0        0    59025 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/linear-regression-angle-example.png
--rw-r--r--   0        0        0    58305 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/linear-regression-example.png
--rw-r--r--   0        0        0    54179 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/linear-regression-intercept-example.png
--rw-r--r--   0        0        0    53628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/linear-regression-slope-example.png
--rw-r--r--   0        0        0    47835 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/lollipop-example.png
--rw-r--r--   0        0        0    41461 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/macd-example.png
--rw-r--r--   0        0        0   104539 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/map-example.png
--rw-r--r--   0        0        0   201616 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/mapbubble-example.png
--rw-r--r--   0        0        0   112234 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/mapline-example.png
--rw-r--r--   0        0        0   112234 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/mappoint-example.png
--rw-r--r--   0        0        0    44732 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/mfi-example.png
--rw-r--r--   0        0        0    51251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/momentum-example.png
--rw-r--r--   0        0        0    49554 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/natr-example.png
--rw-r--r--   0        0        0    53945 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/navigator-example.png
--rw-r--r--   0        0        0   269275 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/networkgraph-example.png
--rw-r--r--   0        0        0    34625 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/obv-example.png
--rw-r--r--   0        0        0    34656 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/ohlc-example.png
--rw-r--r--   0        0        0    48433 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/organization-example-horizontal.png
--rw-r--r--   0        0        0   106952 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/organization-example.png
--rw-r--r--   0        0        0   265002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/packedbubble-example-split.png
--rw-r--r--   0        0        0   298951 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/packedbubble-example.png
--rw-r--r--   0        0        0    58765 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/pareto-example.png
--rw-r--r--   0        0        0    90797 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/pie-example-donut.png
--rw-r--r--   0        0        0    97511 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/pie-example.png
--rw-r--r--   0        0        0    47842 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/pivot-points-example.png
--rw-r--r--   0        0        0    56333 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/polygon-example.png
--rw-r--r--   0        0        0    44413 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/ppo-example.png
--rw-r--r--   0        0        0    55355 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/price-channel-example.png
--rw-r--r--   0        0        0    43588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/price-envelopes-example.png
--rw-r--r--   0        0        0    47048 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/psar-example.png
--rw-r--r--   0        0        0    49049 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/pyramid-example.png
--rw-r--r--   0        0        0    53531 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/pyramid_3d-example.png
--rw-r--r--   0        0        0    44302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/range-selector-example.png
--rw-r--r--   0        0        0    49944 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/roc-example.png
--rw-r--r--   0        0        0    45958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/rsi-example.png
--rw-r--r--   0        0        0   197682 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/sankey-example-inverted.png
--rw-r--r--   0        0        0    79510 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/sankey-example-outgoing.png
--rw-r--r--   0        0        0   227684 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/sankey-example.png
--rw-r--r--   0        0        0   109494 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/scatter-example.png
--rw-r--r--   0        0        0    29303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/scatter_3d-example.png
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/shared_options.js
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/shared_options_output.js
--rw-r--r--   0        0        0    53177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/slow-stochastic-example.png
--rw-r--r--   0        0        0    50549 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/sma-example.png
--rw-r--r--   0        0        0    28628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/solidgauge-example.png
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/sphinx_rtd_theme_ext_color_contrast.css
--rw-r--r--   0        0        0    81626 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/spline-example.png
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/square-check-solid.svg
--rw-r--r--   0        0        0    41933 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/stochastic-example.png
--rw-r--r--   0        0        0    71303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/stock-tools-example.png
--rw-r--r--   0        0        0   278653 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/streamgraph-example.png
--rw-r--r--   0        0        0   397432 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/sunburst-example.png
--rw-r--r--   0        0        0    34040 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/supertrend-example.png
--rw-r--r--   0        0        0    55620 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/tema-example.png
--rw-r--r--   0        0        0   199024 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/tilemap-example-circle.png
--rw-r--r--   0        0        0    95113 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/tilemap-example-diamond.png
--rw-r--r--   0        0        0    81668 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/tilemap-example.png
--rw-r--r--   0        0        0    33235 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/timeline-example-datetime.png
--rw-r--r--   0        0        0    14778 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/timeline-example-inverted.png
--rw-r--r--   0        0        0    13386 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/timeline-example.png
--rw-r--r--   0        0        0    59391 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/treemap-example.png
--rw-r--r--   0        0        0    44325 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/trendline-example.png
--rw-r--r--   0        0        0    36104 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/trix-example.png
--rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/variablepie-example.png
--rw-r--r--   0        0        0    10175 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/variwide-example-datetime.png
--rw-r--r--   0        0        0    28517 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/variwide-example-inverted.png
--rw-r--r--   0        0        0    74616 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/variwide-example.png
--rw-r--r--   0        0        0    93945 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/vbp-example.png
--rw-r--r--   0        0        0   173850 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/vector-example.png
--rw-r--r--   0        0        0    58194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/venn-example-euler.png
--rw-r--r--   0        0        0    94796 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/venn-example.png
--rw-r--r--   0        0        0    41570 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/vwap-example.png
--rw-r--r--   0        0        0    59407 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/waterfall-example-inverted.png
--rw-r--r--   0        0        0    12628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/waterfall-example-stacked.png
--rw-r--r--   0        0        0    59664 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/waterfall-example.png
--rw-r--r--   0        0        0    36821 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/williamsr-example.png
--rw-r--r--   0        0        0    67964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/windbarb-example.png
--rw-r--r--   0        0        0    52744 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/wma-example.png
--rw-r--r--   0        0        0   177320 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/wordcloud-example.png
--rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/xrange-example-inverted.png
--rw-r--r--   0        0        0    30421 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/xrange-example.png
--rw-r--r--   0        0        0    64223 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/zigzag-example.png
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/_class_structures.rst
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/_deserialization_methods.rst
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/_handling_defaults.rst
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/_module_structure.rst
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/_other_convenience_methods.rst
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/_serialization_methods.rst
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/chart.rst
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/headless_export.rst
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/highcharts.rst
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/internals.rst
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/index.rst
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/shared_options.rst
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/export_data.rst
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/index.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/navigation.rst
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/announce_new_data.rst
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/axis.rst
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/chart_types.rst
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/exporting.rst
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/index.rst
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/legend.rst
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/range_selector.rst
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/screen_reader_section.rst
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/series.rst
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/sonification.rst
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/table.rst
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/zoom.rst
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/boost.rst
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/caption.rst
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/credits.rst
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/data.rst
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/defs.rst
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/drilldown.rst
--rw-r--r--   0        0        0    39926 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/index.rst
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/loading.rst
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/map_navigation.rst
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/responsive.rst
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/subtitle.rst
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/time.rst
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/title.rst
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/tooltips.rst
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/announce_new_data.rst
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/index.rst
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/point.rst
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/screen_reader_section.rst
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/series.rst
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/keyboard_navigation/focus_border.rst
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/keyboard_navigation/index.rst
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/keyboard_navigation/series_navigation.rst
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/animation.rst
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/control_point_options.rst
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/events.rst
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/index.rst
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/label_options.rst
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/points.rst
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/shape_options.rst
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/accessibility.rst
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/breaks.rst
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/color_axis.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/crosshair.rst
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/data_classes.rst
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/generic.rst
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/index.rst
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/labels.rst
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/markers.rst
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/numeric.rst
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/parallel_axes.rst
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/plot_bands.rst
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/title.rst
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/x_axis.rst
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/y_axis.rst
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/z_axis.rst
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/chart/index.rst
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/chart/options_3d.rst
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/chart/reset_zoom_button.rst
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/chart/scrollable_plot_area.rst
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/chart/zooming.rst
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/exporting/csv.rst
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/exporting/index.rst
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/exporting/pdf_font.rst
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/legend/accessibility.rst
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/legend/bubble_legend.rst
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/legend/index.rst
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/legend/navigation.rst
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/legend/title.rst
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/map_views/index.rst
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/map_views/insets.rst
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/navigation/bindings.rst
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/navigation/index.rst
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/accessibility.rst
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/arcdiagram.rst
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/area.rst
--rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bar.rst
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/base.rst
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bellcurve.rst
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/boxplot.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bubble.rst
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bullet.rst
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/data_sorting.rst
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/dependencywheel.rst
--rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/drag_drop.rst
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/dumbbell.rst
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/funnel.rst
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/gauge.rst
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/generic.rst
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/heatmap.rst
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/histogram.rst
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/index.rst
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/item.rst
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/levels.rst
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/link.rst
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/map.rst
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/mapbubble.rst
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/mapline.rst
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/mappoint.rst
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/networkgraph.rst
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/organization.rst
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/packedbubble.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/pareto.rst
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/pie.rst
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/points.rst
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/polygon.rst
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/pyramid.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/sankey.rst
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/scatter.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/series.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/spline.rst
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/sunburst.rst
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/timeline.rst
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/treemap.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/vector.rst
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/venn.rst
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/wordcloud.rst
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/arcdiagram.rst
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/area.rst
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/bar.rst
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/base.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/bellcurve.rst
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/boxplot.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/bubble.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/bullet.rst
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/dependencywheel.rst
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/dumbbell.rst
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/funnel.rst
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/gauge.rst
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/heatmap.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/histogram.rst
--rw-r--r--   0        0        0    13470 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/index.rst
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/item.rst
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/labels.rst
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/map.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/mapbubble.rst
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/mapline.rst
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/mappoint.rst
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/networkgraph.rst
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/organization.rst
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/packedbubble.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/pareto.rst
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/pie.rst
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/polygon.rst
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/pyramid.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/sankey.rst
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/scatter.rst
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/series_generator.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/spline.rst
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/sunburst.rst
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/timeline.rst
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/treemap.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/vector.rst
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/venn.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/wordcloud.rst
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/accessibility.rst
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/arcdiagram.rst
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/bar.rst
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/base.rst
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/boxplot.rst
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/bullet.rst
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/cartesian.rst
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/connections.rst
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/geometric.rst
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/index.rst
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/map_data.rst
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/pie.rst
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/range.rst
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/single_point.rst
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/sunburst.rst
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/treemap.rst
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/vector.rst
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/venn.rst
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/wordcloud.rst
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/animation.rst
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/ast.rst
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/breadcrumbs.rst
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/buttons.rst
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/clusters.rst
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/data_grouping.rst
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/data_labels.rst
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/date_time_label_formats.rst
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/events.rst
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/fetch_configuration.rst
--rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/geojson.rst
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/gradients.rst
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/index.rst
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/javascript_functions.rst
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/jitter.rst
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/markers.rst
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/menus.rst
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/nodes.rst
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/partial_fill.rst
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/patterns.rst
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/position.rst
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/projections.rst
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/shadows.rst
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/states.rst
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/topojson.rst
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/zones.rst
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/_code_style_naming_conventions.rst
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/_importing.rst
--rw-r--r--   0        0        0     7632 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/_working_with_maps_features.rst
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_add_series.rst
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_from_geopandas.rst
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_from_series.rst
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_series_property.rst
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_using_async_map_data.rst
--rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_using_synchronous_map_data.rst
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_with_chart_map.rst
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_with_series_map_data.rst
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/download_visualizations/_using_custom.rst
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/download_visualizations/_using_highsoft.rst
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_csv.rst
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_geopandas.rst
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_pandas.rst
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_pyspark.rst
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_csv.rst
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_geopandas.rst
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_pandas.rst
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_pyspark.rst
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_with_data_property.rst
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_with_from_array.rst
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/rendering_your_visualizations/_as_jupyter.rst
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/rendering_your_visualizations/_as_web_content.rst
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/shared_options/_with_dict.rst
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/shared_options/_with_js_literal.rst
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/shared_options/_with_json.rst
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/templates/_with_copy.rst
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/templates/_with_dict.rst
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/templates/_with_js_literal.rst
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/templates/_with_json.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/__init__.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/__version__.py
--rw-r--r--   0        0        0    51211 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/chart.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/constants.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/decorators.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/errors.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/headless_export.py
--rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/highcharts.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/js_literal_functions.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/metaclasses.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/__init__.py
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/shared_options.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/export_data.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/navigation.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/announce_new_data.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/axis.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/chart_types.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/exporting.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/legend.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/range_selector.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/screen_reader_section.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/series.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/sonification.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/table.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/zoom.py
--rw-r--r--   0        0        0     8744 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/boost.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/caption.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/credits.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/data.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/defs.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/drilldown.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/loading.py
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/map_navigation.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/responsive.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/subtitle.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/time.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/title.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/tooltips.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/announce_new_data.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/high_contrast_theme.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/point.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/screen_reader_section.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/series.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/keyboard_navigation/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/keyboard_navigation/focus_border.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/keyboard_navigation/series_navigation.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/__init__.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/animation.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/control_point_options.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/events.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/label_options.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/points.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/shape_options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/accessibility.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/breaks.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/color_axis.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/crosshair.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/data_classes.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/generic.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/labels.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/markers.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/numeric.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/parallel_axes.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/plot_bands.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/title.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/x_axis.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/y_axis.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/z_axis.py
--rw-r--r--   0        0        0    11458 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/chart/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/chart/options_3d.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/chart/reset_zoom_button.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/chart/scrollable_plot_area.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/chart/zooming.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/exporting/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/exporting/csv.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/exporting/pdf_font.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/legend/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/legend/accessibility.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/legend/bubble_legend.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/legend/navigation.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/legend/title.py
--rw-r--r--   0        0        0     7665 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/map_views/__init__.py
--rw-r--r--   0        0        0    11283 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/map_views/insets.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/navigation/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/navigation/bindings.py
--rw-r--r--   0        0        0    53247 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/accessibility.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/arcdiagram.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/area.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/bar.py
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/base.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/bellcurve.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/boxplot.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/bubble.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/bullet.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/data_sorting.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/dependencywheel.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/drag_drop.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/dumbbell.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/funnel.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/gauge.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/generic.py
--rw-r--r--   0        0        0    15221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/heatmap.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/histogram.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/item.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/levels.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/link.py
--rw-r--r--   0        0        0    17236 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/map.py
--rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/mapbubble.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/mapline.py
--rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/mappoint.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/networkgraph.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/organization.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/packedbubble.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/pareto.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/pie.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/points.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/polygon.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/pyramid.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/sankey.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/scatter.py
--rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/series.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/spline.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/sunburst.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/timeline.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/treemap.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/vector.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/venn.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/arcdiagram.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/area.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/bar.py
--rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/base.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/bellcurve.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/boxplot.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/bubble.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/bullet.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/dependencywheel.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/dumbbell.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/funnel.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/gauge.py
--rw-r--r--   0        0        0    14416 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/heatmap.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/histogram.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/item.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/labels.py
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/map.py
--rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/mapbubble.py
--rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/mapline.py
--rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/mappoint.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/networkgraph.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/organization.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/packedbubble.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/pareto.py
--rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/pie.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/polygon.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/pyramid.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/sankey.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/scatter.py
--rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/series_generator.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/spline.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/sunburst.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/timeline.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/treemap.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/vector.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/venn.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/accessibility.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/arcdiagram.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/bar.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/base.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/boxplot.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/bullet.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/cartesian.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/connections.py
--rw-r--r--   0        0        0    25787 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/geometric.py
--rw-r--r--   0        0        0    26792 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/map_data.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/pie.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/range.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/single_point.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/sunburst.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/treemap.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/vector.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/venn.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/animation.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/ast.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/breadcrumbs.py
--rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/buttons.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/clusters.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/data_grouping.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/data_labels.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/date_time_label_formats.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/events.py
--rw-r--r--   0        0        0    14873 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/fetch_configuration.py
--rw-r--r--   0        0        0    20197 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/geojson.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/gradients.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/javascript_functions.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/jitter.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/markers.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/menus.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/nodes.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/partial_fill.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/patterns.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/position.py
--rw-r--r--   0        0        0    13187 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/projections.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/shadows.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/states.py
--rw-r--r--   0        0        0    23958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/topojson.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/zones.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/__init__.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/conftest.py
--rw-r--r--   0        0        0    37707 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/fixtures.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_chart.py
--rw-r--r--   0        0        0     7569 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_decorators.py
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_headless_export.py
--rw-r--r--   0        0        0     7798 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_js_literal_functions.py
--rw-r--r--   0        0        0    10008 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_metaclasses.py
--rw-r--r--   0        0        0    14064 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_mro.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_utility_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/__init__.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/test_shared_options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/__init__.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/test_export_data.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/test_language.py
--rw-r--r--   0        0        0    10946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/test_navigation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/accessibility/__init__.py
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/accessibility/test_accessibility.py
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/accessibility/test_series.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/accessibility/accessibility/01.js
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/accessibility/accessibility/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/accessibility/accessibility/error-02.js
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/annotation/01.js
--rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/annotation/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/annotation/error-02.js
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/01.js
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/02.js
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/03.js
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/04.js
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/05.js
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/06.js
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/07.js
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/08.js
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/09.js
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/10.js
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-01.js
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-02.js
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-03.js
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-04.js
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-05.js
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-06.js
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-07.js
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-08.js
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-09.js
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-10.js
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/01.js
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/02.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/error-01.js
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/error-02.js
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/01.js
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/02.js
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/error-01.js
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/error-02.js
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/01.js
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/02.js
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/error-01.js
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/error-02.js
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/01.js
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/02.js
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/error-01.js
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/error-02.js
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/resize/01.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/resize/error-01.js
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/x_axis/01.js
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/x_axis/02.js
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/x_axis/error-01.js
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/x_axis/error-02.js
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/01.js
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/02.js
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/error-01.js
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/error-02.js
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/01.js
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/02.js
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/error-01.js
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/error-02.js
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/boost/01.js
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/boost/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/boost/error-02.js
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/caption/01.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/caption/02.js
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/caption/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/caption/error-02.js
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/chart/01.js
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/chart/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/chart/error-02.js
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/options_3d/01.js
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/options_3d/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/options_3d/error-02.js
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/zooming/01.js
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/zooming/error-01.js
--rw-r--r--   0        0        0   461024 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart_obj/01-expected.js
--rw-r--r--   0        0        0   496450 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart_obj/01-input.js
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/credits/01.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/credits/02.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/credits/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/credits/error-02.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/data/01.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/data/02.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/data/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/data/error-02.js
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/drilldown/01.js
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/drilldown/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/drilldown/error-02.js
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/exporting/csv/01.js
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/exporting/csv/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/exporting/csv/error-02.js
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/exporting/exporting/01.js
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/exporting/exporting/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/exporting/exporting/error-02.js
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/accessibility/01.js
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/accessibility/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/accessibility/error-02.js
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/01.js
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/02.js
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/error-02.js
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/error-03.js
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/export_data/01.js
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/export_data/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/export_data/error-02.js
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/language/01.js
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/language/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/language/error-02.js
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/01.js
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/02.js
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/error-02.js
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/error-03.js
--rw-r--r--   0        0        0   461353 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/shared_options/01-expected.js
--rw-r--r--   0        0        0   461329 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/shared_options/01-input.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/basic.json
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/with-chart-type.js
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/with-series-types.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/output/placeholder.txt
--rw-r--r--   0        0        0    20068 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/output/test-basic.png
--rw-r--r--   0        0        0    10527 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/output/test-with-chart-type.png
--rw-r--r--   0        0        0    10527 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/output/test-with-series-types.png
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/bubble_legend/01.js
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/bubble_legend/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/bubble_legend/error-02.js
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/legend/01.js
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/legend/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/legend/error-02.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/navigation/01.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/navigation/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/navigation/error-02.js
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/loading/01.js
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/loading/02.js
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/loading/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/loading/error-02.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/01.js
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/02.js
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/error-02.js
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/error-03.js
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/navigation/01.js
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/navigation/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/navigation/error-02.js
--rw-r--r--   0        0        0   461329 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/options/01.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/01.js
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/error-00.js
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/error-01.js
--rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/error-02.js
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/01.js
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/error-00.js
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/error-01.js
--rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/error-02.js
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/01.js
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/02.js
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/03.js
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/04.js
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/05.js
--rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/06.js
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/07.js
--rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/08.js
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/09.js
--rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/10.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/error-00.js
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/error-01.js
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/error-02.js
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/01.js
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/error-00.js
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/error-01.js
--rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/error-02.js
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/01.js
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/error-00.js
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/error-01.js
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/error-02.js
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/01.js
--rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/error-00.js
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/error-01.js
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/error-02.js
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/01.js
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/error-00.js
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/error-01.js
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/error-02.js
--rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/01.js
--rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/error-00.js
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/error-01.js
--rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/error-02.js
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/01.js
--rw-r--r--   0        0        0     7490 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/error-00.js
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/error-01.js
--rw-r--r--   0        0        0     7503 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/error-02.js
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/01.js
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/02.js
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/03.js
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/04.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-00.js
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-01.js
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-02.js
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-03.js
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-04.js
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/01.js
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/02.js
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/03.js
--rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/04.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-00.js
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-01.js
--rw-r--r--   0        0        0     5865 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-02.js
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-03.js
--rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-04.js
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/generic/01.js
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/generic/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/generic/error-02.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/01.js
--rw-r--r--   0        0        0     7338 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/02.js
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/03.js
--rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/04.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-00.js
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-01.js
--rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-02.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-03.js
--rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-04.js
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/01.js
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/02.js
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/03.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/error-00.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/error-01.js
--rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/error-02.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/01.js
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/error-00.js
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/error-01.js
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/error-02.js
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/map/01.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/map/error-01.js
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/mapbubble/01.js
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/mapbubble/error-01.js
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/mapline/01.js
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/mapline/error-01.js
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/mappoint/01.js
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/mappoint/error-01.js
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/01.js
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/error-00.js
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/error-01.js
--rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/error-02.js
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/01.js
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/error-00.js
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/error-01.js
--rw-r--r--   0        0        0    12187 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/error-02.js
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/01.js
--rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/error-00.js
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/error-01.js
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/error-02.js
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/01.js
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/02.js
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/03.js
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/04.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-00.js
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-01.js
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-02.js
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-03.js
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-04.js
--rw-r--r--   0        0        0   396839 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/plot_options/01.js
--rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/01.js
--rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/error-00.js
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/error-01.js
--rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/error-02.js
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/01.js
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/error-00.js
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/error-01.js
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/error-02.js
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/01.js
--rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/error-00.js
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/error-01.js
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/error-02.js
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/01.js
--rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/error-00.js
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/error-01.js
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/error-02.js
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/01.js
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/error-00.js
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/error-01.js
--rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/error-02.js
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/01.js
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/error-00.js
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/error-01.js
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/error-02.js
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/01.js
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/error-00.js
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/error-01.js
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/error-02.js
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/01.js
--rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/error-00.js
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/error-01.js
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/error-02.js
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/01.js
--rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/error-00.js
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/error-01.js
--rw-r--r--   0        0        0     8908 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/error-02.js
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/01.js
--rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/error-00.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/error-01.js
--rw-r--r--   0        0        0     5767 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/error-02.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/responsive/01.js
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/responsive/02.js
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/responsive/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/responsive/error-02.js
--rw-r--r--   0        0        0    14433 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/arcdiagram/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/arcdiagram/error-00.js
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/arcdiagram/error-01.js
--rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/01.js
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/02.js
--rw-r--r--   0        0        0    15908 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/03.js
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/04.js
--rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/05.js
--rw-r--r--   0        0        0    13465 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/06.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-00.js
--rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-01.js
--rw-r--r--   0        0        0     9285 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-02.js
--rw-r--r--   0        0        0    16547 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-03.js
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-04.js
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/01.js
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/02.js
--rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/03.js
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/04.js
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/05.js
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/06.js
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/07.js
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/08.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/error-00.js
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/error-01.js
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/base/01.js
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/base/02.js
--rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/base/03.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/base/error-00.js
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/base/error-01.js
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/base/error-02.js
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bellcurve/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bellcurve/error-00.js
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bellcurve/error-01.js
--rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/01.js
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/error-00.js
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/error-01.js
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/error-02.js
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bubble/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bubble/error-00.js
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bubble/error-01.js
--rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bullet/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bullet/error-00.js
--rw-r--r--   0        0        0    12938 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bullet/error-01.js
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/01.js
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/02.js
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/03.js
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/04.js
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/05.js
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/06.js
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-01.js
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-02.js
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-03.js
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-04.js
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/base/01.js
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/base/error-01.js
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/boxplot/01.js
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/boxplot/error-01.js
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bullet/01.js
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bullet/error-01.js
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/01.js
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/02.js
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/03.js
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/04.js
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/05.js
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/06.js
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/07.js
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/08.js
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/error-01.js
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/error-02.js
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/error-05.js
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/error-07.js
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/01.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/02.js
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/03.js
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/04.js
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/error-01.js
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/error-02.js
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/error-03.js
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/01.js
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/02.js
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/03.js
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/error-01.js
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/error-03.js
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/async_map_data/01-expected.js
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/async_map_data/01-input.js
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/01.js
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/02.js
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/03.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/error-01.js
--rw-r--r--   0        0        0   433034 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/world.geo.json
--rw-r--r--   0        0        0   153391 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/world.topo.json
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/01.js
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/02.js
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/error-01.js
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/error-02.js
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/01.js
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/02.js
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/03.js
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/04.js
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/error-01.js
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/error-02.js
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/error-03.js
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/01.js
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/02.js
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/03.js
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/04.js
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/05.js
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/06.js
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-01.js
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-02.js
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-03.js
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-04.js
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-05.js
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-06.js
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/01.js
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/02.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/error-01.js
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/error-02.js
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/vector/01.js
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/vector/error-01.js
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/venn/01.js
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/venn/error-01.js
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/wordcloud/01.js
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/wordcloud/error-01.js
--rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/dependencywheel/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/dependencywheel/error-00.js
--rw-r--r--   0        0        0    15237 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/dependencywheel/error-01.js
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/dumbbell/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/dumbbell/error-00.js
--rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/dumbbell/error-01.js
--rw-r--r--   0        0        0     9240 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/01.js
--rw-r--r--   0        0        0     9266 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/error-00.js
--rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/error-01.js
--rw-r--r--   0        0        0     9284 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/error-02.js
--rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/01.js
--rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/error-00.js
--rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/error-01.js
--rw-r--r--   0        0        0    10236 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/error-02.js
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/generic/01.js
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/generic/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/generic/error-02.js
--rw-r--r--   0        0        0     9920 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/01.js
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/error-00.js
--rw-r--r--   0        0        0     9954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/error-01.js
--rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/error-02.js
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/histogram/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/histogram/error-00.js
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/histogram/error-01.js
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/item/01.js
--rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/item/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/item/error-00.js
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/item/error-01.js
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/item/error-02.js
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/map/01.js
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/map/error-01.js
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/mapbubble/01.js
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/mapbubble/error-01.js
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/mapline/01.js
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/mapline/error-01.js
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/mappoint/01.js
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/mappoint/error-01.js
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/01.js
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/error-00.js
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/error-01.js
--rw-r--r--   0        0        0     9403 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/error-02.js
--rw-r--r--   0        0        0     9388 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/organization/01.js
--rw-r--r--   0        0        0    15633 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/organization/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/organization/error-00.js
--rw-r--r--   0        0        0     9422 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/organization/error-01.js
--rw-r--r--   0        0        0    15667 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/organization/error-02.js
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/01.js
--rw-r--r--   0        0        0     9528 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/error-00.js
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/error-01.js
--rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/error-02.js
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pareto/01.js
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pareto/02.js
--rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pareto/error-01.js
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pie/01.js
--rw-r--r--   0        0        0     9268 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pie/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pie/error-00.js
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pie/error-01.js
--rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pie/error-02.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/01.js
--rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/02.js
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/error-01.js
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/error-02.js
--rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/01.js
--rw-r--r--   0        0        0    15255 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/error-00.js
--rw-r--r--   0        0        0     9961 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/error-01.js
--rw-r--r--   0        0        0    15258 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/error-02.js
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/01.js
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/error-00.js
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/error-01.js
--rw-r--r--   0        0        0     9848 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/error-02.js
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/spline/01.js
--rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/spline/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/spline/error-00.js
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/spline/error-01.js
--rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/spline/error-02.js
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/01.js
--rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/error-00.js
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/error-01.js
--rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/error-02.js
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/01.js
--rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/error-00.js
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/error-01.js
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/error-02.js
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/01.js
--rw-r--r--   0        0        0    10307 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/error-00.js
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/error-01.js
--rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/error-02.js
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/vector/01.js
--rw-r--r--   0        0        0    10768 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/vector/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/vector/error-00.js
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/vector/error-01.js
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/vector/error-02.js
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/venn/01.js
--rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/venn/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/venn/error-00.js
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/venn/error-01.js
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/venn/error-02.js
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/01.js
--rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/error-00.js
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/error-01.js
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/error-02.js
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/subtitle/01.js
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/subtitle/02.js
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/subtitle/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/subtitle/error-02.js
--rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/test-data-files/nst-est2019-01-transposed.csv
--rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/test-data-files/nst-est2019-01.csv
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/time/01.js
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/time/02.js
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/time/error-01.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/time/error-02.js
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/title/01.js
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/title/02.js
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/title/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/title/error-02.js
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/tooltips/01.js
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/tooltips/02.js
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/tooltips/error-01.js
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/tooltips/error-02.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/animation/01.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/animation/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/animation/error-02.js
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/breadcrumbs/01.js
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/breadcrumbs/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/breadcrumbs/error-02.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/buttons/01.js
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/buttons/02.js
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/buttons/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/buttons/error-02.js
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/buttons/error-03.js
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/clusters/01.js
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/clusters/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/clusters/error-02.js
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_grouping/01.js
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_grouping/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_grouping/error-02.js
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/01.js
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/02.js
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/error-02.js
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/error-03.js
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/date_time_label_formats/01.js
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/date_time_label_formats/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/date_time_label_formats/error-02.js
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/01.js
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/02.js
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/03.js
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/04.js
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/05.js
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/06.js
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/07.js
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/08.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/09.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-00.js
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-01.js
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-02.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-03.js
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-04.js
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-05.js
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-06.js
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-07.js
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-08.js
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-09.js
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/gradients/01.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/gradients/02.js
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/gradients/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/gradients/error-02.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/gradients/error-03.js
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/jitter/01.js
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/jitter/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/jitter/error-02.js
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/markers/01.js
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/markers/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/markers/error-02.js
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/menus/01.js
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/menus/02.js
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/menus/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/menus/error-02.js
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/menus/error-03.js
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/01.js
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/02.js
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/03.js
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/error-02.js
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/error-03.js
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/error-04.js
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/partial_fill/01.js
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/partial_fill/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/partial_fill/error-02.js
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/patterns/01.js
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/patterns/02.js
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/patterns/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/patterns/error-02.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/patterns/error-03.js
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/position/01.js
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/position/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/position/error-02.js
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/shadows/01.js
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/shadows/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/shadows/error-02.js
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/states/01.js
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/states/02.js
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/states/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/states/error-02.js
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/zones/01.js
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/zones/02.js
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/zones/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/zones/error-02.js
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/zones/error-03.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/__init__.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_boost.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_caption.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_credits.py
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_data.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_defs.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_drilldown.py
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_loading.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_options.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_responsive.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_subtitle.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_time.py
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_title.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_tooltips.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/accessibility/__init__.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/accessibility/test_accessibility.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/annotations/__init__.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/annotations/test_annotation.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/__init__.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_color_axis.py
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_numeric.py
--rw-r--r--   0        0        0    12026 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_parallel_axes.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_plot_bands.py
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_x_axis.py
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_y_axis.py
--rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_z_axis.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/chart/__init__.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/chart/test_chart.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/chart/test_options_3d.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/chart/test_zooming.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/exporting/__init__.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/exporting/test_csv.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/exporting/test_exporting.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/legend/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/legend/test_bubble_legend.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/legend/test_legend.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/legend/test_navigation.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/navigation/__init__.py
--rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/navigation/test_bindings.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/navigation/test_navigation.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/__init__.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_PlotOptions.py
--rw-r--r--   0        0        0    25301 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_arcdiagram.py
--rw-r--r--   0        0        0    21498 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_area.py
--rw-r--r--   0        0        0   141328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bar.py
--rw-r--r--   0        0        0    12455 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bellcurve.py
--rw-r--r--   0        0        0    37409 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_boxplot.py
--rw-r--r--   0        0        0    14722 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bubble.py
--rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bullet.py
--rw-r--r--   0        0        0    25444 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_dependencywheel.py
--rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_dumbbell.py
--rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_funnel.py
--rw-r--r--   0        0        0    24453 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_gauge.py
--rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_generic.py
--rw-r--r--   0        0        0    23344 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_heatmap.py
--rw-r--r--   0        0        0    13615 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_histogram.py
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_item.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_map.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_mapbubble.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_mapline.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_mappoint.py
--rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_networkgraph.py
--rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_organization.py
--rw-r--r--   0        0        0    12697 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_packedbubble.py
--rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_pareto.py
--rw-r--r--   0        0        0    23106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_pie.py
--rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_polygon.py
--rw-r--r--   0        0        0    23521 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_pyramid.py
--rw-r--r--   0        0        0    25426 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_sankey.py
--rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_scatter.py
--rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_series.py
--rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_spline.py
--rw-r--r--   0        0        0    11946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_sunburst.py
--rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_timeline.py
--rw-r--r--   0        0        0    14286 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_treemap.py
--rw-r--r--   0        0        0    27094 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_vector.py
--rw-r--r--   0        0        0    18068 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_venn.py
--rw-r--r--   0        0        0    10190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/__init__.py
--rw-r--r--   0        0        0    37684 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_arcdiagram.py
--rw-r--r--   0        0        0    86365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_area.py
--rw-r--r--   0        0        0   184797 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_bar.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_base.py
--rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_bellcurve.py
--rw-r--r--   0        0        0    38600 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_boxplot.py
--rw-r--r--   0        0        0    27700 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_bubble.py
--rw-r--r--   0        0        0    19900 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_bullet.py
--rw-r--r--   0        0        0    38082 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_dependencywheel.py
--rw-r--r--   0        0        0    25823 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_dumbbell.py
--rw-r--r--   0        0        0    45949 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_funnel.py
--rw-r--r--   0        0        0    43973 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_gauge.py
--rw-r--r--   0        0        0    52024 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_heatmap.py
--rw-r--r--   0        0        0    13338 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_histogram.py
--rw-r--r--   0        0        0    23439 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_item.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_map.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_mapbubble.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_mapline.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_mappoint.py
--rw-r--r--   0        0        0    20751 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_networkgraph.py
--rw-r--r--   0        0        0    53769 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_organization.py
--rw-r--r--   0        0        0    27719 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_packedbubble.py
--rw-r--r--   0        0        0    13693 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_pareto.py
--rw-r--r--   0        0        0    42404 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_pie.py
--rw-r--r--   0        0        0    26395 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_polygon.py
--rw-r--r--   0        0        0    45967 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_pyramid.py
--rw-r--r--   0        0        0    38538 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_sankey.py
--rw-r--r--   0        0        0    29328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_scatter.py
--rw-r--r--   0        0        0    23877 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_spline.py
--rw-r--r--   0        0        0    20920 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_sunburst.py
--rw-r--r--   0        0        0    20357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_timeline.py
--rw-r--r--   0        0        0    23259 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_treemap.py
--rw-r--r--   0        0        0    27497 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_vector.py
--rw-r--r--   0        0        0    27155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_venn.py
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/__init__.py
--rw-r--r--   0        0        0    31572 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_bar.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_base.py
--rw-r--r--   0        0        0    22036 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_boxplot.py
--rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_bullet.py
--rw-r--r--   0        0        0    36534 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_cartesian.py
--rw-r--r--   0        0        0    30915 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_connections.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_geometric.py
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_map_data.py
--rw-r--r--   0        0        0    14300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_pie.py
--rw-r--r--   0        0        0    16010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_range.py
--rw-r--r--   0        0        0    42349 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_single_point.py
--rw-r--r--   0        0        0    15434 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_sunburst.py
--rw-r--r--   0        0        0    20702 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_vector.py
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_venn.py
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/__init__.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_animation.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_ast.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_breadcrumbs.py
--rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_buttons.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_clusters.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_data_grouping.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_data_labels.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_date_time_label_formats.py
--rw-r--r--   0        0        0    21674 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_events.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_gradients.py
--rw-r--r--   0        0        0    17810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_javascript_functions.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_jitter.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_markers.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_menus.py
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_nodes.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_partial_fill.py
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_patterns.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_position.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_shadows.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_states.py
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_zones.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/.gitignore
--rw-r--r--   0        0        0    24468 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/LICENSE
--rw-r--r--   0        0        0    17509 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/README.rst
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/pyproject.toml
--rw-r--r--   0        0        0    20818 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/PKG-INFO
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/.travis.yml
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/CHANGES.rst
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/requirements.dev.txt
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/requirements.travis.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/requirements.txt
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/setup.cfg
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tox.ini
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/.github/workflows/pypi-test-publish.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_contributors.rst
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_dependencies.rst
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_installation.rst
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_support.rst
+-rw-r--r--   0        0        0     9776 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_versus_alternatives.rst
+-rw-r--r--   0        0        0    56205 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api.rst
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/contributing.rst
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/demos.rst
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/errors.rst
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/faq.rst
+-rw-r--r--   0        0        0    34457 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/glossary.rst
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/history.rst
+-rw-r--r--   0        0        0    16243 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/index.rst
+-rw-r--r--   0        0        0    24959 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/license.rst
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/links.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/quickstart.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/support.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/testing.rst
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/toolkit.rst
+-rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using.rst
+-rw-r--r--   0        0        0    41670 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/visualizations.rst
+-rw-r--r--   0        0        0    54859 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/abands-example.png
+-rw-r--r--   0        0        0    34552 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/ad-example.png
+-rw-r--r--   0        0        0    43218 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/apo-example.png
+-rw-r--r--   0        0        0    87899 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/arcdiagram-example.png
+-rw-r--r--   0        0        0    72487 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/area-example.png
+-rw-r--r--   0        0        0   124371 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/arearange-example.png
+-rw-r--r--   0        0        0    55288 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/areaspline-example.png
+-rw-r--r--   0        0        0    54998 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/aroon-example.png
+-rw-r--r--   0        0        0    46438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/aroon-oscillator-example.png
+-rw-r--r--   0        0        0    47100 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/atr-example.png
+-rw-r--r--   0        0        0    20359 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/awesome-oscillator-example.png
+-rw-r--r--   0        0        0   485952 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/axis-property-mapping.xlsx
+-rw-r--r--   0        0        0    59173 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/bar-example.png
+-rw-r--r--   0        0        0    48934 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/bellcurve-example.png
+-rw-r--r--   0        0        0    43491 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/bollinger-bands-example.png
+-rw-r--r--   0        0        0    37690 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/boxplot-example.png
+-rw-r--r--   0        0        0    92954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/bubble-example.png
+-rw-r--r--   0        0        0    26870 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/bullet-example.png
+-rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/candlestick-example.png
+-rw-r--r--   0        0        0    52121 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/cci-example.png
+-rw-r--r--   0        0        0    49536 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/chaikin-example.png
+-rw-r--r--   0        0        0    46772 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/cmf-example.png
+-rw-r--r--   0        0        0    47632 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/cmo-example.png
+-rw-r--r--   0        0        0    41242 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/column-example.png
+-rw-r--r--   0        0        0    41567 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/columnpyramid-example-stacked-horizontal.png
+-rw-r--r--   0        0        0    31515 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/columnpyramid-example-stacked.png
+-rw-r--r--   0        0        0    51790 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/columnpyramid-example.png
+-rw-r--r--   0        0        0    63741 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/columnrange-example-horizontal.png
+-rw-r--r--   0        0        0    68246 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/columnrange-example.png
+-rw-r--r--   0        0        0    67368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/cylinder-example.png
+-rw-r--r--   0        0        0    54030 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/dema-example.png
+-rw-r--r--   0        0        0   252801 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/dependencywheel-example.png
+-rw-r--r--   0        0        0    49737 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/disparity-index-example.png
+-rw-r--r--   0        0        0    45925 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/dmi-example.png
+-rw-r--r--   0        0        0    37726 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/dpo-example.png
+-rw-r--r--   0        0        0    66693 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/dumbbell-example.png
+-rw-r--r--   0        0        0    38446 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/ema-example.png
+-rw-r--r--   0        0        0    59876 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/errorbar-example.png
+-rw-r--r--   0        0        0    27702 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/flags-example.png
+-rw-r--r--   0        0        0    43626 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/funnel-example.png
+-rw-r--r--   0        0        0    60815 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/funnel_3d-example.png
+-rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/gantt-example.png
+-rw-r--r--   0        0        0   129516 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/gauge-example.png
+-rw-r--r--   0        0        0    87393 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/heatmap-example.png
+-rw-r--r--   0        0        0    29731 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/heikin-ashi-example.png
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/highcharts-for-python-dark-32x32.png
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/highcharts-for-python-light-150x149.png
+-rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/highcharts-logo.svg
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/highcharts-python-logo.png
+-rw-r--r--   0        0        0    38747 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/histogram-example.png
+-rw-r--r--   0        0        0    25456 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/hlc-example.png
+-rw-r--r--   0        0        0    34397 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/hollow-candlestick-example.png
+-rw-r--r--   0        0        0    73793 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/ikh-example.png
+-rw-r--r--   0        0        0   208287 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/item-example-circular.png
+-rw-r--r--   0        0        0   151954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/item-example-rectangular.png
+-rw-r--r--   0        0        0    15447 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/item-example-symbols.png
+-rw-r--r--   0        0        0    47093 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/keltner-channels-example.png
+-rw-r--r--   0        0        0    40750 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/klinger-example.png
+-rw-r--r--   0        0        0    81283 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/line-example.png
+-rw-r--r--   0        0        0    59025 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/linear-regression-angle-example.png
+-rw-r--r--   0        0        0    58305 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/linear-regression-example.png
+-rw-r--r--   0        0        0    54179 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/linear-regression-intercept-example.png
+-rw-r--r--   0        0        0    53628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/linear-regression-slope-example.png
+-rw-r--r--   0        0        0    47835 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/lollipop-example.png
+-rw-r--r--   0        0        0    41461 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/macd-example.png
+-rw-r--r--   0        0        0   104539 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/map-example.png
+-rw-r--r--   0        0        0   201616 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/mapbubble-example.png
+-rw-r--r--   0        0        0   112234 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/mapline-example.png
+-rw-r--r--   0        0        0   112234 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/mappoint-example.png
+-rw-r--r--   0        0        0    44732 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/mfi-example.png
+-rw-r--r--   0        0        0    51251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/momentum-example.png
+-rw-r--r--   0        0        0    49554 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/natr-example.png
+-rw-r--r--   0        0        0    53945 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/navigator-example.png
+-rw-r--r--   0        0        0   269275 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/networkgraph-example.png
+-rw-r--r--   0        0        0    34625 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/obv-example.png
+-rw-r--r--   0        0        0    34656 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/ohlc-example.png
+-rw-r--r--   0        0        0    48433 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/organization-example-horizontal.png
+-rw-r--r--   0        0        0   106952 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/organization-example.png
+-rw-r--r--   0        0        0   265002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/packedbubble-example-split.png
+-rw-r--r--   0        0        0   298951 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/packedbubble-example.png
+-rw-r--r--   0        0        0    58765 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/pareto-example.png
+-rw-r--r--   0        0        0    90797 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/pie-example-donut.png
+-rw-r--r--   0        0        0    97511 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/pie-example.png
+-rw-r--r--   0        0        0    47842 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/pivot-points-example.png
+-rw-r--r--   0        0        0    56333 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/polygon-example.png
+-rw-r--r--   0        0        0    44413 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/ppo-example.png
+-rw-r--r--   0        0        0    55355 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/price-channel-example.png
+-rw-r--r--   0        0        0    43588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/price-envelopes-example.png
+-rw-r--r--   0        0        0    47048 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/psar-example.png
+-rw-r--r--   0        0        0    49049 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/pyramid-example.png
+-rw-r--r--   0        0        0    53531 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/pyramid_3d-example.png
+-rw-r--r--   0        0        0    44302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/range-selector-example.png
+-rw-r--r--   0        0        0    49944 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/roc-example.png
+-rw-r--r--   0        0        0    45958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/rsi-example.png
+-rw-r--r--   0        0        0   197682 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/sankey-example-inverted.png
+-rw-r--r--   0        0        0    79510 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/sankey-example-outgoing.png
+-rw-r--r--   0        0        0   227684 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/sankey-example.png
+-rw-r--r--   0        0        0   109494 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/scatter-example.png
+-rw-r--r--   0        0        0    29303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/scatter_3d-example.png
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/shared_options.js
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/shared_options_output.js
+-rw-r--r--   0        0        0    53177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/slow-stochastic-example.png
+-rw-r--r--   0        0        0    50549 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/sma-example.png
+-rw-r--r--   0        0        0    28628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/solidgauge-example.png
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/sphinx_rtd_theme_ext_color_contrast.css
+-rw-r--r--   0        0        0    81626 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/spline-example.png
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/square-check-solid.svg
+-rw-r--r--   0        0        0    41933 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/stochastic-example.png
+-rw-r--r--   0        0        0    71303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/stock-tools-example.png
+-rw-r--r--   0        0        0   278653 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/streamgraph-example.png
+-rw-r--r--   0        0        0   397432 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/sunburst-example.png
+-rw-r--r--   0        0        0    34040 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/supertrend-example.png
+-rw-r--r--   0        0        0    55620 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/tema-example.png
+-rw-r--r--   0        0        0   199024 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/tilemap-example-circle.png
+-rw-r--r--   0        0        0    95113 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/tilemap-example-diamond.png
+-rw-r--r--   0        0        0    81668 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/tilemap-example.png
+-rw-r--r--   0        0        0    33235 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/timeline-example-datetime.png
+-rw-r--r--   0        0        0    14778 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/timeline-example-inverted.png
+-rw-r--r--   0        0        0    13386 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/timeline-example.png
+-rw-r--r--   0        0        0    59391 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/treemap-example.png
+-rw-r--r--   0        0        0    44325 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/trendline-example.png
+-rw-r--r--   0        0        0    36104 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/trix-example.png
+-rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/variablepie-example.png
+-rw-r--r--   0        0        0    10175 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/variwide-example-datetime.png
+-rw-r--r--   0        0        0    28517 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/variwide-example-inverted.png
+-rw-r--r--   0        0        0    74616 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/variwide-example.png
+-rw-r--r--   0        0        0    93945 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/vbp-example.png
+-rw-r--r--   0        0        0   173850 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/vector-example.png
+-rw-r--r--   0        0        0    58194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/venn-example-euler.png
+-rw-r--r--   0        0        0    94796 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/venn-example.png
+-rw-r--r--   0        0        0    41570 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/vwap-example.png
+-rw-r--r--   0        0        0    59407 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/waterfall-example-inverted.png
+-rw-r--r--   0        0        0    12628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/waterfall-example-stacked.png
+-rw-r--r--   0        0        0    59664 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/waterfall-example.png
+-rw-r--r--   0        0        0    36821 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/williamsr-example.png
+-rw-r--r--   0        0        0    67964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/windbarb-example.png
+-rw-r--r--   0        0        0    52744 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/wma-example.png
+-rw-r--r--   0        0        0   177320 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/wordcloud-example.png
+-rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/xrange-example-inverted.png
+-rw-r--r--   0        0        0    30421 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/xrange-example.png
+-rw-r--r--   0        0        0    64223 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/_static/zigzag-example.png
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/_class_structures.rst
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/_deserialization_methods.rst
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/_handling_defaults.rst
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/_module_structure.rst
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/_other_convenience_methods.rst
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/_serialization_methods.rst
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/chart.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/headless_export.rst
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/highcharts.rst
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/internals.rst
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/index.rst
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/shared_options.rst
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/export_data.rst
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/index.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/navigation.rst
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/announce_new_data.rst
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/axis.rst
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/chart_types.rst
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/exporting.rst
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/index.rst
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/legend.rst
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/range_selector.rst
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/screen_reader_section.rst
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/series.rst
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/sonification.rst
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/table.rst
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/zoom.rst
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/boost.rst
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/caption.rst
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/credits.rst
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/data.rst
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/defs.rst
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/drilldown.rst
+-rw-r--r--   0        0        0    39926 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/index.rst
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/loading.rst
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/map_navigation.rst
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/responsive.rst
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/subtitle.rst
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/time.rst
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/title.rst
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/tooltips.rst
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/accessibility/announce_new_data.rst
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/accessibility/index.rst
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/accessibility/point.rst
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/accessibility/screen_reader_section.rst
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/accessibility/series.rst
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/accessibility/keyboard_navigation/focus_border.rst
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/accessibility/keyboard_navigation/index.rst
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/accessibility/keyboard_navigation/series_navigation.rst
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/annotations/animation.rst
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/annotations/control_point_options.rst
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/annotations/events.rst
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/annotations/index.rst
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/annotations/label_options.rst
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/annotations/points.rst
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/annotations/shape_options.rst
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/accessibility.rst
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/breaks.rst
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/color_axis.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/crosshair.rst
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/data_classes.rst
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/generic.rst
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/index.rst
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/labels.rst
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/markers.rst
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/numeric.rst
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/parallel_axes.rst
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/plot_bands.rst
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/title.rst
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/x_axis.rst
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/y_axis.rst
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/axes/z_axis.rst
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/chart/index.rst
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/chart/options_3d.rst
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/chart/reset_zoom_button.rst
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/chart/scrollable_plot_area.rst
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/chart/zooming.rst
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/exporting/csv.rst
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/exporting/index.rst
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/exporting/pdf_font.rst
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/legend/accessibility.rst
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/legend/bubble_legend.rst
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/legend/index.rst
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/legend/navigation.rst
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/legend/title.rst
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/map_views/index.rst
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/map_views/insets.rst
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/navigation/bindings.rst
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/navigation/index.rst
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/accessibility.rst
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/arcdiagram.rst
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/area.rst
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/bar.rst
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/base.rst
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/bellcurve.rst
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/boxplot.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/bubble.rst
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/bullet.rst
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/data_sorting.rst
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/dependencywheel.rst
+-rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/drag_drop.rst
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/dumbbell.rst
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/funnel.rst
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/gauge.rst
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/generic.rst
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/heatmap.rst
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/histogram.rst
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/index.rst
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/item.rst
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/levels.rst
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/link.rst
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/map.rst
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/mapbubble.rst
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/mapline.rst
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/mappoint.rst
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/networkgraph.rst
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/organization.rst
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/packedbubble.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/pareto.rst
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/pie.rst
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/points.rst
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/polygon.rst
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/pyramid.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/sankey.rst
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/scatter.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/series.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/spline.rst
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/sunburst.rst
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/timeline.rst
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/treemap.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/vector.rst
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/venn.rst
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/plot_options/wordcloud.rst
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/arcdiagram.rst
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/area.rst
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/bar.rst
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/base.rst
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/bellcurve.rst
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/boxplot.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/bubble.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/bullet.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/dependencywheel.rst
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/dumbbell.rst
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/funnel.rst
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/gauge.rst
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/heatmap.rst
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/histogram.rst
+-rw-r--r--   0        0        0    13470 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/index.rst
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/item.rst
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/labels.rst
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/map.rst
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/mapbubble.rst
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/mapline.rst
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/mappoint.rst
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/networkgraph.rst
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/organization.rst
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/packedbubble.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/pareto.rst
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/pie.rst
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/polygon.rst
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/pyramid.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/sankey.rst
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/scatter.rst
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/series_generator.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/spline.rst
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/sunburst.rst
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/timeline.rst
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/treemap.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/vector.rst
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/venn.rst
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/wordcloud.rst
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/accessibility.rst
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/arcdiagram.rst
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/bar.rst
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/base.rst
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/boxplot.rst
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/bullet.rst
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/cartesian.rst
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/connections.rst
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/geometric.rst
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/index.rst
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/map_data.rst
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/pie.rst
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/range.rst
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/single_point.rst
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/sunburst.rst
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/treemap.rst
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/vector.rst
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/venn.rst
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/options/series/data/wordcloud.rst
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/animation.rst
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/ast.rst
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/breadcrumbs.rst
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/buttons.rst
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/clusters.rst
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/data_grouping.rst
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/data_labels.rst
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/date_time_label_formats.rst
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/events.rst
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/fetch_configuration.rst
+-rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/geojson.rst
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/gradients.rst
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/index.rst
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/javascript_functions.rst
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/jitter.rst
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/markers.rst
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/menus.rst
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/nodes.rst
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/partial_fill.rst
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/patterns.rst
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/position.rst
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/projections.rst
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/shadows.rst
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/states.rst
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/topojson.rst
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/api/utility_classes/zones.rst
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/_code_style_naming_conventions.rst
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/_importing.rst
+-rw-r--r--   0        0        0     7632 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/_working_with_maps_features.rst
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/assembling_your_chart/_using_add_series.rst
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/assembling_your_chart/_using_from_geopandas.rst
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/assembling_your_chart/_using_from_series.rst
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/assembling_your_chart/_using_series_property.rst
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/configuring_map_data/_using_async_map_data.rst
+-rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/configuring_map_data/_using_synchronous_map_data.rst
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/configuring_map_data/_with_chart_map.rst
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/configuring_map_data/_with_series_map_data.rst
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/download_visualizations/_using_custom.rst
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/download_visualizations/_using_highsoft.rst
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/populating_series_data/_load_from_csv.rst
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/populating_series_data/_load_from_geopandas.rst
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/populating_series_data/_load_from_pandas.rst
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/populating_series_data/_load_from_pyspark.rst
+-rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/populating_series_data/_new_from_csv.rst
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/populating_series_data/_new_from_geopandas.rst
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/populating_series_data/_new_from_pandas.rst
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/populating_series_data/_new_from_pyspark.rst
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/populating_series_data/_with_data_property.rst
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/populating_series_data/_with_from_array.rst
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/rendering_your_visualizations/_as_jupyter.rst
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/rendering_your_visualizations/_as_web_content.rst
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/shared_options/_with_dict.rst
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/shared_options/_with_js_literal.rst
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/shared_options/_with_json.rst
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/templates/_with_copy.rst
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/templates/_with_dict.rst
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/templates/_with_js_literal.rst
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/docs/using/templates/_with_json.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/__version__.py
+-rw-r--r--   0        0        0    51211 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/chart.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/constants.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/decorators.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/errors.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/headless_export.py
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/highcharts.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/js_literal_functions.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/metaclasses.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/__init__.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/shared_options.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/export_data.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/navigation.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/accessibility/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/accessibility/announce_new_data.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/accessibility/axis.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/accessibility/chart_types.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/accessibility/exporting.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/accessibility/legend.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/accessibility/range_selector.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/accessibility/screen_reader_section.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/accessibility/series.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/accessibility/sonification.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/accessibility/table.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/global_options/language/accessibility/zoom.py
+-rw-r--r--   0        0        0     8744 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/boost.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/caption.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/credits.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/data.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/defs.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/drilldown.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/loading.py
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/map_navigation.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/responsive.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/subtitle.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/time.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/title.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/tooltips.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/accessibility/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/accessibility/announce_new_data.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/accessibility/high_contrast_theme.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/accessibility/point.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/accessibility/screen_reader_section.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/accessibility/series.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/accessibility/keyboard_navigation/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/accessibility/keyboard_navigation/focus_border.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/accessibility/keyboard_navigation/series_navigation.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/annotations/__init__.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/annotations/animation.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/annotations/control_point_options.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/annotations/events.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/annotations/label_options.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/annotations/points.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/annotations/shape_options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/accessibility.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/breaks.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/color_axis.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/crosshair.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/data_classes.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/generic.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/labels.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/markers.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/numeric.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/parallel_axes.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/plot_bands.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/title.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/x_axis.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/y_axis.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/axes/z_axis.py
+-rw-r--r--   0        0        0    11458 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/chart/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/chart/options_3d.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/chart/reset_zoom_button.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/chart/scrollable_plot_area.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/chart/zooming.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/exporting/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/exporting/csv.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/exporting/pdf_font.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/legend/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/legend/accessibility.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/legend/bubble_legend.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/legend/navigation.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/legend/title.py
+-rw-r--r--   0        0        0     7665 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/map_views/__init__.py
+-rw-r--r--   0        0        0    11283 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/map_views/insets.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/navigation/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/navigation/bindings.py
+-rw-r--r--   0        0        0    53247 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/accessibility.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/arcdiagram.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/area.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/bar.py
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/base.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/bellcurve.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/boxplot.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/bubble.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/bullet.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/data_sorting.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/dependencywheel.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/drag_drop.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/dumbbell.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/funnel.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/gauge.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/generic.py
+-rw-r--r--   0        0        0    15221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/heatmap.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/histogram.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/item.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/levels.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/link.py
+-rw-r--r--   0        0        0    17236 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/map.py
+-rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/mapbubble.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/mapline.py
+-rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/mappoint.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/networkgraph.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/organization.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/packedbubble.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/pareto.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/pie.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/points.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/polygon.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/pyramid.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/sankey.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/scatter.py
+-rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/series.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/spline.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/sunburst.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/timeline.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/treemap.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/vector.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/venn.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/plot_options/wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/arcdiagram.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/area.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/bar.py
+-rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/base.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/bellcurve.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/boxplot.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/bubble.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/bullet.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/dependencywheel.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/dumbbell.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/funnel.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/gauge.py
+-rw-r--r--   0        0        0    14416 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/heatmap.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/histogram.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/item.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/labels.py
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/map.py
+-rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/mapbubble.py
+-rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/mapline.py
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/mappoint.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/networkgraph.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/organization.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/packedbubble.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/pareto.py
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/pie.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/polygon.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/pyramid.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/sankey.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/scatter.py
+-rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/series_generator.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/spline.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/sunburst.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/timeline.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/treemap.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/vector.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/venn.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/accessibility.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/arcdiagram.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/bar.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/base.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/boxplot.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/bullet.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/cartesian.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/connections.py
+-rw-r--r--   0        0        0    25787 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/geometric.py
+-rw-r--r--   0        0        0    26792 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/map_data.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/pie.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/range.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/single_point.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/sunburst.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/treemap.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/vector.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/venn.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/options/series/data/wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/animation.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/ast.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/breadcrumbs.py
+-rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/buttons.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/clusters.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/data_grouping.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/data_labels.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/date_time_label_formats.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/events.py
+-rw-r--r--   0        0        0    14873 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/fetch_configuration.py
+-rw-r--r--   0        0        0    20197 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/geojson.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/gradients.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/javascript_functions.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/jitter.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/markers.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/menus.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/nodes.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/partial_fill.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/patterns.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/position.py
+-rw-r--r--   0        0        0    13187 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/projections.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/shadows.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/states.py
+-rw-r--r--   0        0        0    23958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/topojson.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/highcharts_maps/utility_classes/zones.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0    37707 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/fixtures.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/test_chart.py
+-rw-r--r--   0        0        0     7569 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/test_decorators.py
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/test_headless_export.py
+-rw-r--r--   0        0        0     7798 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/test_js_literal_functions.py
+-rw-r--r--   0        0        0    10008 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/test_metaclasses.py
+-rw-r--r--   0        0        0    14064 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/test_mro.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/test_utility_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/global_options/__init__.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/global_options/test_shared_options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/global_options/language/__init__.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/global_options/language/test_export_data.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/global_options/language/test_language.py
+-rw-r--r--   0        0        0    10946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/global_options/language/test_navigation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/global_options/language/accessibility/__init__.py
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/global_options/language/accessibility/test_accessibility.py
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/global_options/language/accessibility/test_series.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/accessibility/accessibility/01.js
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/accessibility/accessibility/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/accessibility/accessibility/error-02.js
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/annotation/01.js
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/annotation/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/annotation/error-02.js
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/01.js
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/02.js
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/03.js
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/04.js
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/05.js
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/06.js
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/07.js
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/08.js
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/09.js
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/10.js
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-01.js
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-02.js
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-03.js
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-04.js
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-05.js
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-06.js
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-07.js
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-08.js
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-09.js
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-10.js
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/color_axis/01.js
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/color_axis/02.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/color_axis/error-01.js
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/color_axis/error-02.js
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/numeric/01.js
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/numeric/02.js
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/numeric/error-01.js
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/numeric/error-02.js
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/parallel_axes/01.js
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/parallel_axes/02.js
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/parallel_axes/error-01.js
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/parallel_axes/error-02.js
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/plot_bands/01.js
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/plot_bands/02.js
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/plot_bands/error-01.js
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/plot_bands/error-02.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/resize/01.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/resize/error-01.js
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/x_axis/01.js
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/x_axis/02.js
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/x_axis/error-01.js
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/x_axis/error-02.js
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/y_axis/01.js
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/y_axis/02.js
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/y_axis/error-01.js
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/y_axis/error-02.js
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/z_axis/01.js
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/z_axis/02.js
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/z_axis/error-01.js
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/axes/z_axis/error-02.js
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/boost/01.js
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/boost/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/boost/error-02.js
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/caption/01.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/caption/02.js
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/caption/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/caption/error-02.js
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/chart/chart/01.js
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/chart/chart/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/chart/chart/error-02.js
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/chart/options_3d/01.js
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/chart/options_3d/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/chart/options_3d/error-02.js
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/chart/zooming/01.js
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/chart/zooming/error-01.js
+-rw-r--r--   0        0        0   461024 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/chart_obj/01-expected.js
+-rw-r--r--   0        0        0   496450 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/chart_obj/01-input.js
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/credits/01.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/credits/02.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/credits/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/credits/error-02.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/data/01.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/data/02.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/data/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/data/error-02.js
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/drilldown/01.js
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/drilldown/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/drilldown/error-02.js
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/exporting/csv/01.js
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/exporting/csv/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/exporting/csv/error-02.js
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/exporting/exporting/01.js
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/exporting/exporting/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/exporting/exporting/error-02.js
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/accessibility/accessibility/01.js
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/accessibility/accessibility/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/accessibility/accessibility/error-02.js
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/accessibility/series/01.js
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/accessibility/series/02.js
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/accessibility/series/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/accessibility/series/error-02.js
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/accessibility/series/error-03.js
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/export_data/01.js
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/export_data/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/export_data/error-02.js
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/language/01.js
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/language/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/language/error-02.js
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/navigation/01.js
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/navigation/02.js
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/navigation/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/navigation/error-02.js
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/language/navigation/error-03.js
+-rw-r--r--   0        0        0   461353 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/shared_options/01-expected.js
+-rw-r--r--   0        0        0   461329 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/global_options/shared_options/01-input.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/headless_export/basic.json
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/headless_export/with-chart-type.js
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/headless_export/with-series-types.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/headless_export/output/placeholder.txt
+-rw-r--r--   0        0        0    20068 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/headless_export/output/test-basic.png
+-rw-r--r--   0        0        0    10527 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/headless_export/output/test-with-chart-type.png
+-rw-r--r--   0        0        0    10527 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/headless_export/output/test-with-series-types.png
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/legend/bubble_legend/01.js
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/legend/bubble_legend/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/legend/bubble_legend/error-02.js
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/legend/legend/01.js
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/legend/legend/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/legend/legend/error-02.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/legend/navigation/01.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/legend/navigation/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/legend/navigation/error-02.js
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/loading/01.js
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/loading/02.js
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/loading/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/loading/error-02.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/navigation/bindings/01.js
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/navigation/bindings/02.js
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/navigation/bindings/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/navigation/bindings/error-02.js
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/navigation/bindings/error-03.js
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/navigation/navigation/01.js
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/navigation/navigation/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/navigation/navigation/error-02.js
+-rw-r--r--   0        0        0   461329 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/options/01.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/arcdiagram/01.js
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/arcdiagram/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/arcdiagram/error-00.js
+-rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/arcdiagram/error-01.js
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/arcdiagram/error-02.js
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/area/01.js
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/area/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/area/error-00.js
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/area/error-01.js
+-rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/area/error-02.js
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/01.js
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/02.js
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/03.js
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/04.js
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/05.js
+-rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/06.js
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/07.js
+-rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/08.js
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/09.js
+-rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/10.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/error-00.js
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/error-01.js
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bar/error-02.js
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bellcurve/01.js
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bellcurve/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bellcurve/error-00.js
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bellcurve/error-01.js
+-rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bellcurve/error-02.js
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/boxplot/01.js
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/boxplot/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/boxplot/error-00.js
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/boxplot/error-01.js
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/boxplot/error-02.js
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bubble/01.js
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bubble/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bubble/error-00.js
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bubble/error-01.js
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bubble/error-02.js
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bullet/01.js
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bullet/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bullet/error-00.js
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bullet/error-01.js
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/bullet/error-02.js
+-rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/dependencywheel/01.js
+-rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/dependencywheel/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/dependencywheel/error-00.js
+-rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/dependencywheel/error-01.js
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/dependencywheel/error-02.js
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/dumbbell/01.js
+-rw-r--r--   0        0        0     7490 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/dumbbell/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/dumbbell/error-00.js
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/dumbbell/error-01.js
+-rw-r--r--   0        0        0     7503 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/dumbbell/error-02.js
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/01.js
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/02.js
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/03.js
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/04.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/error-00.js
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/error-01.js
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/error-02.js
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/error-03.js
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/error-04.js
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/01.js
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/02.js
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/03.js
+-rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/04.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/error-00.js
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/error-01.js
+-rw-r--r--   0        0        0     5865 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/error-02.js
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/error-03.js
+-rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/error-04.js
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/generic/01.js
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/generic/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/generic/error-02.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/01.js
+-rw-r--r--   0        0        0     7338 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/02.js
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/03.js
+-rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/04.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/error-00.js
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/error-01.js
+-rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/error-02.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/error-03.js
+-rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/error-04.js
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/histogram/01.js
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/histogram/02.js
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/histogram/03.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/histogram/error-00.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/histogram/error-01.js
+-rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/histogram/error-02.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/item/01.js
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/item/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/item/error-00.js
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/item/error-01.js
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/item/error-02.js
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/map/01.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/map/error-01.js
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/mapbubble/01.js
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/mapbubble/error-01.js
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/mapline/01.js
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/mapline/error-01.js
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/mappoint/01.js
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/mappoint/error-01.js
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/networkgraph/01.js
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/networkgraph/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/networkgraph/error-00.js
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/networkgraph/error-01.js
+-rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/networkgraph/error-02.js
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/organization/01.js
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/organization/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/organization/error-00.js
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/organization/error-01.js
+-rw-r--r--   0        0        0    12187 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/organization/error-02.js
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/packedbubble/01.js
+-rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/packedbubble/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/packedbubble/error-00.js
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/packedbubble/error-01.js
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/packedbubble/error-02.js
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/pie/01.js
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/pie/02.js
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/pie/03.js
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/pie/04.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/pie/error-00.js
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/pie/error-01.js
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/pie/error-02.js
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/pie/error-03.js
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/pie/error-04.js
+-rw-r--r--   0        0        0   396839 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/plot_options/01.js
+-rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/sankey/01.js
+-rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/sankey/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/sankey/error-00.js
+-rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/sankey/error-01.js
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/sankey/error-02.js
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/scatter/01.js
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/scatter/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/scatter/error-00.js
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/scatter/error-01.js
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/scatter/error-02.js
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/series/01.js
+-rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/series/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/series/error-00.js
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/series/error-01.js
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/series/error-02.js
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/spline/01.js
+-rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/spline/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/spline/error-00.js
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/spline/error-01.js
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/spline/error-02.js
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/sunburst/01.js
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/sunburst/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/sunburst/error-00.js
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/sunburst/error-01.js
+-rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/sunburst/error-02.js
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/timeline/01.js
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/timeline/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/timeline/error-00.js
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/timeline/error-01.js
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/timeline/error-02.js
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/treemap/01.js
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/treemap/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/treemap/error-00.js
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/treemap/error-01.js
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/treemap/error-02.js
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/vector/01.js
+-rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/vector/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/vector/error-00.js
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/vector/error-01.js
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/vector/error-02.js
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/venn/01.js
+-rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/venn/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/venn/error-00.js
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/venn/error-01.js
+-rw-r--r--   0        0        0     8908 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/venn/error-02.js
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/wordcloud/01.js
+-rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/wordcloud/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/wordcloud/error-00.js
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/wordcloud/error-01.js
+-rw-r--r--   0        0        0     5767 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/plot_options/wordcloud/error-02.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/responsive/01.js
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/responsive/02.js
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/responsive/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/responsive/error-02.js
+-rw-r--r--   0        0        0    14433 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/arcdiagram/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/arcdiagram/error-00.js
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/arcdiagram/error-01.js
+-rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/area/01.js
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/area/02.js
+-rw-r--r--   0        0        0    15908 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/area/03.js
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/area/04.js
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/area/05.js
+-rw-r--r--   0        0        0    13465 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/area/06.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/area/error-00.js
+-rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/area/error-01.js
+-rw-r--r--   0        0        0     9285 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/area/error-02.js
+-rw-r--r--   0        0        0    16547 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/area/error-03.js
+-rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/area/error-04.js
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bar/01.js
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bar/02.js
+-rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bar/03.js
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bar/04.js
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bar/05.js
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bar/06.js
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bar/07.js
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bar/08.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bar/error-00.js
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bar/error-01.js
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/base/01.js
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/base/02.js
+-rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/base/03.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/base/error-00.js
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/base/error-01.js
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/base/error-02.js
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bellcurve/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bellcurve/error-00.js
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bellcurve/error-01.js
+-rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/boxplot/01.js
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/boxplot/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/boxplot/error-00.js
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/boxplot/error-01.js
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/boxplot/error-02.js
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bubble/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bubble/error-00.js
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bubble/error-01.js
+-rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bullet/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bullet/error-00.js
+-rw-r--r--   0        0        0    12938 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/bullet/error-01.js
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/bar/01.js
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/bar/02.js
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/bar/03.js
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/bar/04.js
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/bar/05.js
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/bar/06.js
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/bar/error-01.js
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/bar/error-02.js
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/bar/error-03.js
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/bar/error-04.js
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/base/01.js
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/base/error-01.js
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/boxplot/01.js
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/boxplot/error-01.js
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/bullet/01.js
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/bullet/error-01.js
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/01.js
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/02.js
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/03.js
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/04.js
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/05.js
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/06.js
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/07.js
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/08.js
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/error-01.js
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/error-02.js
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/error-05.js
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/error-07.js
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/connections/01.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/connections/02.js
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/connections/03.js
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/connections/04.js
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/connections/error-01.js
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/connections/error-02.js
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/connections/error-03.js
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/geometric/01.js
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/geometric/02.js
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/geometric/03.js
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/geometric/error-01.js
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/geometric/error-03.js
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/map_data/async_map_data/01-expected.js
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/map_data/async_map_data/01-input.js
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/map_data/map_data/01.js
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/map_data/map_data/02.js
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/map_data/map_data/03.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/map_data/map_data/error-01.js
+-rw-r--r--   0        0        0   433034 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/map_data/map_data/world.geo.json
+-rw-r--r--   0        0        0   153391 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/map_data/map_data/world.topo.json
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/pie/01.js
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/pie/02.js
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/pie/error-01.js
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/pie/error-02.js
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/range/01.js
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/range/02.js
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/range/03.js
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/range/04.js
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/range/error-01.js
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/range/error-02.js
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/range/error-03.js
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/single_point/01.js
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/single_point/02.js
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/single_point/03.js
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/single_point/04.js
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/single_point/05.js
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/single_point/06.js
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/single_point/error-01.js
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/single_point/error-02.js
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/single_point/error-03.js
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/single_point/error-04.js
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/single_point/error-05.js
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/single_point/error-06.js
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/sunburst/01.js
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/sunburst/02.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/sunburst/error-01.js
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/sunburst/error-02.js
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/vector/01.js
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/vector/error-01.js
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/venn/01.js
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/venn/error-01.js
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/wordcloud/01.js
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/data/wordcloud/error-01.js
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/dependencywheel/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/dependencywheel/error-00.js
+-rw-r--r--   0        0        0    15237 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/dependencywheel/error-01.js
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/dumbbell/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/dumbbell/error-00.js
+-rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/dumbbell/error-01.js
+-rw-r--r--   0        0        0     9240 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/funnel/01.js
+-rw-r--r--   0        0        0     9266 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/funnel/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/funnel/error-00.js
+-rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/funnel/error-01.js
+-rw-r--r--   0        0        0     9284 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/funnel/error-02.js
+-rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/gauge/01.js
+-rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/gauge/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/gauge/error-00.js
+-rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/gauge/error-01.js
+-rw-r--r--   0        0        0    10236 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/gauge/error-02.js
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/generic/01.js
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/generic/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/generic/error-02.js
+-rw-r--r--   0        0        0     9920 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/heatmap/01.js
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/heatmap/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/heatmap/error-00.js
+-rw-r--r--   0        0        0     9954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/heatmap/error-01.js
+-rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/heatmap/error-02.js
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/histogram/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/histogram/error-00.js
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/histogram/error-01.js
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/item/01.js
+-rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/item/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/item/error-00.js
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/item/error-01.js
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/item/error-02.js
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/map/01.js
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/map/error-01.js
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/mapbubble/01.js
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/mapbubble/error-01.js
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/mapline/01.js
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/mapline/error-01.js
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/mappoint/01.js
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/mappoint/error-01.js
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/networkgraph/01.js
+-rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/networkgraph/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/networkgraph/error-00.js
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/networkgraph/error-01.js
+-rw-r--r--   0        0        0     9403 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/networkgraph/error-02.js
+-rw-r--r--   0        0        0     9388 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/organization/01.js
+-rw-r--r--   0        0        0    15633 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/organization/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/organization/error-00.js
+-rw-r--r--   0        0        0     9422 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/organization/error-01.js
+-rw-r--r--   0        0        0    15667 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/organization/error-02.js
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/packedbubble/01.js
+-rw-r--r--   0        0        0     9528 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/packedbubble/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/packedbubble/error-00.js
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/packedbubble/error-01.js
+-rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/packedbubble/error-02.js
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/pareto/01.js
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/pareto/02.js
+-rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/pareto/error-01.js
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/pie/01.js
+-rw-r--r--   0        0        0     9268 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/pie/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/pie/error-00.js
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/pie/error-01.js
+-rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/pie/error-02.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/polygon/01.js
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/polygon/02.js
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/polygon/error-01.js
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/polygon/error-02.js
+-rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/sankey/01.js
+-rw-r--r--   0        0        0    15255 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/sankey/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/sankey/error-00.js
+-rw-r--r--   0        0        0     9961 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/sankey/error-01.js
+-rw-r--r--   0        0        0    15258 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/sankey/error-02.js
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/scatter/01.js
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/scatter/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/scatter/error-00.js
+-rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/scatter/error-01.js
+-rw-r--r--   0        0        0     9848 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/scatter/error-02.js
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/spline/01.js
+-rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/spline/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/spline/error-00.js
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/spline/error-01.js
+-rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/spline/error-02.js
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/sunburst/01.js
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/sunburst/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/sunburst/error-00.js
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/sunburst/error-01.js
+-rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/sunburst/error-02.js
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/timeline/01.js
+-rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/timeline/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/timeline/error-00.js
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/timeline/error-01.js
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/timeline/error-02.js
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/treemap/01.js
+-rw-r--r--   0        0        0    10307 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/treemap/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/treemap/error-00.js
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/treemap/error-01.js
+-rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/treemap/error-02.js
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/vector/01.js
+-rw-r--r--   0        0        0    10768 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/vector/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/vector/error-00.js
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/vector/error-01.js
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/vector/error-02.js
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/venn/01.js
+-rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/venn/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/venn/error-00.js
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/venn/error-01.js
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/venn/error-02.js
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/wordcloud/01.js
+-rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/wordcloud/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/wordcloud/error-00.js
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/wordcloud/error-01.js
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/series/wordcloud/error-02.js
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/subtitle/01.js
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/subtitle/02.js
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/subtitle/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/subtitle/error-02.js
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/test-data-files/nst-est2019-01-transposed.csv
+-rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/test-data-files/nst-est2019-01.csv
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/time/01.js
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/time/02.js
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/time/error-01.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/time/error-02.js
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/title/01.js
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/title/02.js
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/title/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/title/error-02.js
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/tooltips/01.js
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/tooltips/02.js
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/tooltips/error-01.js
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/tooltips/error-02.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/animation/01.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/animation/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/animation/error-02.js
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/breadcrumbs/01.js
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/breadcrumbs/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/breadcrumbs/error-02.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/buttons/01.js
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/buttons/02.js
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/buttons/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/buttons/error-02.js
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/buttons/error-03.js
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/clusters/01.js
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/clusters/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/clusters/error-02.js
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/data_grouping/01.js
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/data_grouping/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/data_grouping/error-02.js
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/data_labels/01.js
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/data_labels/02.js
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/data_labels/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/data_labels/error-02.js
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/data_labels/error-03.js
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/date_time_label_formats/01.js
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/date_time_label_formats/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/date_time_label_formats/error-02.js
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/01.js
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/02.js
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/03.js
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/04.js
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/05.js
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/06.js
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/07.js
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/08.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/09.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/error-00.js
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/error-01.js
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/error-02.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/error-03.js
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/error-04.js
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/error-05.js
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/error-06.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/error-07.js
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/error-08.js
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/events/error-09.js
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/gradients/01.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/gradients/02.js
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/gradients/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/gradients/error-02.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/gradients/error-03.js
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/jitter/01.js
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/jitter/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/jitter/error-02.js
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/markers/01.js
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/markers/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/markers/error-02.js
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/menus/01.js
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/menus/02.js
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/menus/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/menus/error-02.js
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/menus/error-03.js
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/nodes/01.js
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/nodes/02.js
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/nodes/03.js
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/nodes/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/nodes/error-02.js
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/nodes/error-03.js
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/nodes/error-04.js
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/partial_fill/01.js
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/partial_fill/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/partial_fill/error-02.js
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/patterns/01.js
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/patterns/02.js
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/patterns/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/patterns/error-02.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/patterns/error-03.js
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/position/01.js
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/position/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/position/error-02.js
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/shadows/01.js
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/shadows/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/shadows/error-02.js
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/states/01.js
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/states/02.js
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/states/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/states/error-02.js
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/zones/01.js
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/zones/02.js
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/zones/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/zones/error-02.js
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/input_files/utility_classes/zones/error-03.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/__init__.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_boost.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_caption.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_credits.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_data.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_defs.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_drilldown.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_loading.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_options.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_responsive.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_subtitle.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_time.py
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_title.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/test_tooltips.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/accessibility/__init__.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/accessibility/test_accessibility.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/annotations/__init__.py
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/annotations/test_annotation.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/axes/__init__.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/axes/test_color_axis.py
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/axes/test_numeric.py
+-rw-r--r--   0        0        0    12026 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/axes/test_parallel_axes.py
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/axes/test_plot_bands.py
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/axes/test_x_axis.py
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/axes/test_y_axis.py
+-rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/axes/test_z_axis.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/chart/__init__.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/chart/test_chart.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/chart/test_options_3d.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/chart/test_zooming.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/exporting/__init__.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/exporting/test_csv.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/exporting/test_exporting.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/legend/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/legend/test_bubble_legend.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/legend/test_legend.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/legend/test_navigation.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/navigation/__init__.py
+-rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/navigation/test_bindings.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/navigation/test_navigation.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/__init__.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_PlotOptions.py
+-rw-r--r--   0        0        0    25301 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_arcdiagram.py
+-rw-r--r--   0        0        0    21498 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_area.py
+-rw-r--r--   0        0        0   141328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_bar.py
+-rw-r--r--   0        0        0    12455 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_bellcurve.py
+-rw-r--r--   0        0        0    37409 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_boxplot.py
+-rw-r--r--   0        0        0    14722 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_bubble.py
+-rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_bullet.py
+-rw-r--r--   0        0        0    25444 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_dependencywheel.py
+-rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_dumbbell.py
+-rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_funnel.py
+-rw-r--r--   0        0        0    24453 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_gauge.py
+-rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_generic.py
+-rw-r--r--   0        0        0    23344 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_heatmap.py
+-rw-r--r--   0        0        0    13615 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_histogram.py
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_item.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_map.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_mapbubble.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_mapline.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_mappoint.py
+-rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_networkgraph.py
+-rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_organization.py
+-rw-r--r--   0        0        0    12697 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_packedbubble.py
+-rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_pareto.py
+-rw-r--r--   0        0        0    23106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_pie.py
+-rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_polygon.py
+-rw-r--r--   0        0        0    23521 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_pyramid.py
+-rw-r--r--   0        0        0    25426 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_sankey.py
+-rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_scatter.py
+-rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_series.py
+-rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_spline.py
+-rw-r--r--   0        0        0    11946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_sunburst.py
+-rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_timeline.py
+-rw-r--r--   0        0        0    14286 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_treemap.py
+-rw-r--r--   0        0        0    27094 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_vector.py
+-rw-r--r--   0        0        0    18068 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_venn.py
+-rw-r--r--   0        0        0    10190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/plot_options/test_wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/__init__.py
+-rw-r--r--   0        0        0    37684 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_arcdiagram.py
+-rw-r--r--   0        0        0    86365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_area.py
+-rw-r--r--   0        0        0   184797 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_bar.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_base.py
+-rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_bellcurve.py
+-rw-r--r--   0        0        0    38600 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_boxplot.py
+-rw-r--r--   0        0        0    27700 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_bubble.py
+-rw-r--r--   0        0        0    19900 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_bullet.py
+-rw-r--r--   0        0        0    38082 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_dependencywheel.py
+-rw-r--r--   0        0        0    25823 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_dumbbell.py
+-rw-r--r--   0        0        0    45949 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_funnel.py
+-rw-r--r--   0        0        0    43973 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_gauge.py
+-rw-r--r--   0        0        0    52024 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_heatmap.py
+-rw-r--r--   0        0        0    13338 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_histogram.py
+-rw-r--r--   0        0        0    23439 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_item.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_map.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_mapbubble.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_mapline.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_mappoint.py
+-rw-r--r--   0        0        0    20751 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_networkgraph.py
+-rw-r--r--   0        0        0    53769 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_organization.py
+-rw-r--r--   0        0        0    27719 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_packedbubble.py
+-rw-r--r--   0        0        0    13693 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_pareto.py
+-rw-r--r--   0        0        0    42404 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_pie.py
+-rw-r--r--   0        0        0    26395 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_polygon.py
+-rw-r--r--   0        0        0    45967 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_pyramid.py
+-rw-r--r--   0        0        0    38538 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_sankey.py
+-rw-r--r--   0        0        0    29328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_scatter.py
+-rw-r--r--   0        0        0    23877 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_spline.py
+-rw-r--r--   0        0        0    20920 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_sunburst.py
+-rw-r--r--   0        0        0    20357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_timeline.py
+-rw-r--r--   0        0        0    23259 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_treemap.py
+-rw-r--r--   0        0        0    27497 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_vector.py
+-rw-r--r--   0        0        0    27155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_venn.py
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/test_wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/__init__.py
+-rw-r--r--   0        0        0    31572 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_bar.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_base.py
+-rw-r--r--   0        0        0    22036 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_boxplot.py
+-rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_bullet.py
+-rw-r--r--   0        0        0    36534 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_cartesian.py
+-rw-r--r--   0        0        0    30915 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_connections.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_geometric.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_map_data.py
+-rw-r--r--   0        0        0    14300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_pie.py
+-rw-r--r--   0        0        0    16010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_range.py
+-rw-r--r--   0        0        0    42349 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_single_point.py
+-rw-r--r--   0        0        0    15434 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_sunburst.py
+-rw-r--r--   0        0        0    20702 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_vector.py
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_venn.py
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/options/series/data/test_wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/__init__.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_animation.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_ast.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_breadcrumbs.py
+-rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_buttons.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_clusters.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_data_grouping.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_data_labels.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_date_time_label_formats.py
+-rw-r--r--   0        0        0    21674 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_events.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_gradients.py
+-rw-r--r--   0        0        0    17810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_javascript_functions.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_jitter.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_markers.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_menus.py
+-rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_nodes.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_partial_fill.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_patterns.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_position.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_shadows.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_states.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/tests/utility_classes/test_zones.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/.gitignore
+-rw-r--r--   0        0        0    24468 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/LICENSE
+-rw-r--r--   0        0        0    18435 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/README.rst
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    21842 2020-02-02 00:00:00.000000 highcharts_maps-1.0.1/PKG-INFO
```

### Comparing `highcharts_maps-1.0.0rc6/.readthedocs.yaml` & `highcharts_maps-1.0.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/.travis.yml` & `highcharts_maps-1.0.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/CHANGES.rst` & `highcharts_maps-1.0.1/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Release 1.0.1
+=========================================
+
+* Added documentation of "hard" dependencies to the README.
+* Fixed broken links in documentation to ``options.plot_options.heatmap.HeatmapOptions`` 
+  and ``options.plot_options.heatmap.TilemapOptions``.
+
+---------------
+
+Release 1.0.0
+=========================================
+
+* **First official release!**
+
+---------------
+
 Release 1.0.0-rc6
 =========================================
 
 * Fixed bug in deserialization of ``options.plot_options.base.MapBaseOptions.join_by``.
 * Fixed Heatmap and Highcharts Maps JavaScript import conflict.
 * Fixed bug in utility_classes.projections.ProjectionOptions.custom property.
 * Fixed serialization bugs in options.series.data.map_data.MapData.
```

### Comparing `highcharts_maps-1.0.0rc6/CODE_OF_CONDUCT.md` & `highcharts_maps-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tox.ini` & `highcharts_maps-1.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.md` & `highcharts_maps-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/.github/workflows/pypi-publish.yml` & `highcharts_maps-1.0.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/.github/workflows/pypi-test-publish.yml` & `highcharts_maps-1.0.1/.github/workflows/pypi-test-publish.yml`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/Makefile` & `highcharts_maps-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_dependencies.rst` & `highcharts_maps-1.0.1/docs/_dependencies.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_support.rst` & `highcharts_maps-1.0.1/docs/_support.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_versus_alternatives.rst` & `highcharts_maps-1.0.1/docs/_versus_alternatives.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api.rst` & `highcharts_maps-1.0.1/docs/api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -344,17 +344,17 @@
     - :class:`FunnelOptions <highcharts_maps.options.plot_options.funnel.FunnelOptions>`
       :class:`Funnel3DOptions <highcharts_maps.options.plot_options.funnel.Funnel3DOptions>`
   * - :mod:`.options.plot_options.gauge <highcharts_maps.options.plot_options.gauge>`
     - :class:`GaugeOptions <highcharts_maps.options.plot_options.gauge.GaugeOptions>`
       :class:`SolidGaugeOptions <highcharts_maps.options.plot_options.gauge.SolidGaugeOptions>`
   * - :mod:`.options.plot_options.generic <highcharts_maps.options.plot_options.generic>`
     - :class:`GenericTypeOptions <highcharts_maps.options.plot_options.generic.GenericTypeOptions>`
-  * - :mod:`.options.plot_options.Heatmap <highcharts_maps.options.plot_options.Heatmap>`
-    - :class:`HeatmapOptions <highcharts_maps.options.plot_options.Heatmap.HeatmapOptions>`
-      :class:`TilemapOptions <highcharts_maps.options.plot_options.Tilemap.TilemapOptions>`
+  * - :mod:`.options.plot_options.heatmap <highcharts_maps.options.plot_options.heatmap>`
+    - :class:`HeatmapOptions <highcharts_maps.options.plot_options.heatmap.HeatmapOptions>`
+      :class:`TilemapOptions <highcharts_maps.options.plot_options.heatmap.TilemapOptions>`
   * - :mod:`.options.plot_options.histogram <highcharts_maps.options.plot_options.histogram>`
     - :class:`HistogramOptions <highcharts_maps.options.plot_options.histogram.HistogramOptions>`
   * - :mod:`.options.plot_options.item <highcharts_maps.options.plot_options.item>`
     - :class:`ItemOptions <highcharts_maps.options.plot_options.item.ItemOptions>`
   * - :mod:`.options.plot_options.levels <highcharts_maps.options.plot_options.levels>`
     - :class:`LevelOptions <highcharts_maps.options.plot_options.levels.LevelOptions>`
       :class:`SunburstLevelOptions <highcharts_maps.options.plot_options.levels.SunburstLevelOptions>`
```

### Comparing `highcharts_maps-1.0.0rc6/docs/conf.py` & `highcharts_maps-1.0.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     'topojson': ('https://mattijn.github.io/topojson/', None),
     'highcharts_core': ('https://core-docs.highchartspython.com/en/latest/', None),
 }
 
 # -- Options for todo extension ----------------------------------------------
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = True
+todo_include_todos = False
 
 # Inheritance Diagram configuration
 inheritance_graph_attrs = {
     'rankdir': 'TB'
 }
 
 suppress_warnings = [
```

### Comparing `highcharts_maps-1.0.0rc6/docs/contributing.rst` & `highcharts_maps-1.0.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/demos.rst` & `highcharts_maps-1.0.1/docs/demos.rst`

 * *Files 2% similar despite different names*

```diff
@@ -115,11 +115,11 @@
 
 ------------------
 
 *******************************
 Running Demos Locally
 *******************************
 
-.. info::
+.. note::
   
   You can run the demos locally by following instructions in the 
   `Highcharts for Python Demos <https://github.com/highcharts-for-python-demos>`__ Github repo's README.
```

### Comparing `highcharts_maps-1.0.0rc6/docs/errors.rst` & `highcharts_maps-1.0.1/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/faq.rst` & `highcharts_maps-1.0.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/glossary.rst` & `highcharts_maps-1.0.1/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/index.rst` & `highcharts_maps-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/license.rst` & `highcharts_maps-1.0.1/docs/license.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/make.bat` & `highcharts_maps-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/quickstart.rst` & `highcharts_maps-1.0.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/toolkit.rst` & `highcharts_maps-1.0.1/docs/toolkit.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using.rst` & `highcharts_maps-1.0.1/docs/using.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/visualizations.rst` & `highcharts_maps-1.0.1/docs/visualizations.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/abands-example.png` & `highcharts_maps-1.0.1/docs/_static/abands-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/ad-example.png` & `highcharts_maps-1.0.1/docs/_static/ad-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/apo-example.png` & `highcharts_maps-1.0.1/docs/_static/apo-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/arcdiagram-example.png` & `highcharts_maps-1.0.1/docs/_static/arcdiagram-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/area-example.png` & `highcharts_maps-1.0.1/docs/_static/area-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/arearange-example.png` & `highcharts_maps-1.0.1/docs/_static/arearange-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/areaspline-example.png` & `highcharts_maps-1.0.1/docs/_static/areaspline-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/aroon-example.png` & `highcharts_maps-1.0.1/docs/_static/aroon-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/aroon-oscillator-example.png` & `highcharts_maps-1.0.1/docs/_static/aroon-oscillator-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/atr-example.png` & `highcharts_maps-1.0.1/docs/_static/atr-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/awesome-oscillator-example.png` & `highcharts_maps-1.0.1/docs/_static/awesome-oscillator-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/axis-property-mapping.xlsx` & `highcharts_maps-1.0.1/docs/_static/axis-property-mapping.xlsx`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/bar-example.png` & `highcharts_maps-1.0.1/docs/_static/bar-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/bellcurve-example.png` & `highcharts_maps-1.0.1/docs/_static/bellcurve-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/bollinger-bands-example.png` & `highcharts_maps-1.0.1/docs/_static/bollinger-bands-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/boxplot-example.png` & `highcharts_maps-1.0.1/docs/_static/boxplot-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/bubble-example.png` & `highcharts_maps-1.0.1/docs/_static/bubble-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/bullet-example.png` & `highcharts_maps-1.0.1/docs/_static/bullet-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/candlestick-example.png` & `highcharts_maps-1.0.1/docs/_static/candlestick-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/cci-example.png` & `highcharts_maps-1.0.1/docs/_static/cci-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/chaikin-example.png` & `highcharts_maps-1.0.1/docs/_static/chaikin-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/cmf-example.png` & `highcharts_maps-1.0.1/docs/_static/cmf-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/cmo-example.png` & `highcharts_maps-1.0.1/docs/_static/cmo-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/column-example.png` & `highcharts_maps-1.0.1/docs/_static/column-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/columnpyramid-example-stacked-horizontal.png` & `highcharts_maps-1.0.1/docs/_static/columnpyramid-example-stacked-horizontal.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/columnpyramid-example-stacked.png` & `highcharts_maps-1.0.1/docs/_static/columnpyramid-example-stacked.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/columnpyramid-example.png` & `highcharts_maps-1.0.1/docs/_static/columnpyramid-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/columnrange-example-horizontal.png` & `highcharts_maps-1.0.1/docs/_static/columnrange-example-horizontal.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/columnrange-example.png` & `highcharts_maps-1.0.1/docs/_static/columnrange-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/cylinder-example.png` & `highcharts_maps-1.0.1/docs/_static/cylinder-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/dema-example.png` & `highcharts_maps-1.0.1/docs/_static/dema-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/dependencywheel-example.png` & `highcharts_maps-1.0.1/docs/_static/dependencywheel-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/disparity-index-example.png` & `highcharts_maps-1.0.1/docs/_static/disparity-index-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/dmi-example.png` & `highcharts_maps-1.0.1/docs/_static/dmi-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/dpo-example.png` & `highcharts_maps-1.0.1/docs/_static/dpo-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/dumbbell-example.png` & `highcharts_maps-1.0.1/docs/_static/dumbbell-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/ema-example.png` & `highcharts_maps-1.0.1/docs/_static/ema-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/errorbar-example.png` & `highcharts_maps-1.0.1/docs/_static/errorbar-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/flags-example.png` & `highcharts_maps-1.0.1/docs/_static/flags-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/funnel-example.png` & `highcharts_maps-1.0.1/docs/_static/funnel-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/funnel_3d-example.png` & `highcharts_maps-1.0.1/docs/_static/funnel_3d-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/gantt-example.png` & `highcharts_maps-1.0.1/docs/_static/gantt-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/gauge-example.png` & `highcharts_maps-1.0.1/docs/_static/gauge-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/heatmap-example.png` & `highcharts_maps-1.0.1/docs/_static/heatmap-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/heikin-ashi-example.png` & `highcharts_maps-1.0.1/docs/_static/heikin-ashi-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/highcharts-for-python-dark-32x32.png` & `highcharts_maps-1.0.1/docs/_static/highcharts-for-python-dark-32x32.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/highcharts-for-python-light-150x149.png` & `highcharts_maps-1.0.1/docs/_static/highcharts-for-python-light-150x149.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/highcharts-logo.svg` & `highcharts_maps-1.0.1/docs/_static/highcharts-logo.svg`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/highcharts-python-logo.png` & `highcharts_maps-1.0.1/docs/_static/highcharts-python-logo.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/histogram-example.png` & `highcharts_maps-1.0.1/docs/_static/histogram-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/hlc-example.png` & `highcharts_maps-1.0.1/docs/_static/hlc-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/hollow-candlestick-example.png` & `highcharts_maps-1.0.1/docs/_static/hollow-candlestick-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/ikh-example.png` & `highcharts_maps-1.0.1/docs/_static/ikh-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/item-example-circular.png` & `highcharts_maps-1.0.1/docs/_static/item-example-circular.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/item-example-rectangular.png` & `highcharts_maps-1.0.1/docs/_static/item-example-rectangular.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/item-example-symbols.png` & `highcharts_maps-1.0.1/docs/_static/item-example-symbols.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/keltner-channels-example.png` & `highcharts_maps-1.0.1/docs/_static/keltner-channels-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/klinger-example.png` & `highcharts_maps-1.0.1/docs/_static/klinger-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/line-example.png` & `highcharts_maps-1.0.1/docs/_static/line-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/linear-regression-angle-example.png` & `highcharts_maps-1.0.1/docs/_static/linear-regression-angle-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/linear-regression-example.png` & `highcharts_maps-1.0.1/docs/_static/linear-regression-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/linear-regression-intercept-example.png` & `highcharts_maps-1.0.1/docs/_static/linear-regression-intercept-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/linear-regression-slope-example.png` & `highcharts_maps-1.0.1/docs/_static/linear-regression-slope-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/lollipop-example.png` & `highcharts_maps-1.0.1/docs/_static/lollipop-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/macd-example.png` & `highcharts_maps-1.0.1/docs/_static/macd-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/map-example.png` & `highcharts_maps-1.0.1/docs/_static/map-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/mapbubble-example.png` & `highcharts_maps-1.0.1/docs/_static/mapbubble-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/mapline-example.png` & `highcharts_maps-1.0.1/docs/_static/mapline-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/mappoint-example.png` & `highcharts_maps-1.0.1/docs/_static/mappoint-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/mfi-example.png` & `highcharts_maps-1.0.1/docs/_static/mfi-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/momentum-example.png` & `highcharts_maps-1.0.1/docs/_static/momentum-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/natr-example.png` & `highcharts_maps-1.0.1/docs/_static/natr-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/navigator-example.png` & `highcharts_maps-1.0.1/docs/_static/navigator-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/networkgraph-example.png` & `highcharts_maps-1.0.1/docs/_static/networkgraph-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/obv-example.png` & `highcharts_maps-1.0.1/docs/_static/obv-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/ohlc-example.png` & `highcharts_maps-1.0.1/docs/_static/ohlc-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/organization-example-horizontal.png` & `highcharts_maps-1.0.1/docs/_static/organization-example-horizontal.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/organization-example.png` & `highcharts_maps-1.0.1/docs/_static/organization-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/packedbubble-example-split.png` & `highcharts_maps-1.0.1/docs/_static/packedbubble-example-split.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/packedbubble-example.png` & `highcharts_maps-1.0.1/docs/_static/packedbubble-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/pareto-example.png` & `highcharts_maps-1.0.1/docs/_static/pareto-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/pie-example-donut.png` & `highcharts_maps-1.0.1/docs/_static/pie-example-donut.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/pie-example.png` & `highcharts_maps-1.0.1/docs/_static/pie-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/pivot-points-example.png` & `highcharts_maps-1.0.1/docs/_static/pivot-points-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/polygon-example.png` & `highcharts_maps-1.0.1/docs/_static/polygon-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/ppo-example.png` & `highcharts_maps-1.0.1/docs/_static/ppo-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/price-channel-example.png` & `highcharts_maps-1.0.1/docs/_static/price-channel-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/price-envelopes-example.png` & `highcharts_maps-1.0.1/docs/_static/price-envelopes-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/psar-example.png` & `highcharts_maps-1.0.1/docs/_static/psar-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/pyramid-example.png` & `highcharts_maps-1.0.1/docs/_static/pyramid-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/pyramid_3d-example.png` & `highcharts_maps-1.0.1/docs/_static/pyramid_3d-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/range-selector-example.png` & `highcharts_maps-1.0.1/docs/_static/range-selector-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/roc-example.png` & `highcharts_maps-1.0.1/docs/_static/roc-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/rsi-example.png` & `highcharts_maps-1.0.1/docs/_static/rsi-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/sankey-example-inverted.png` & `highcharts_maps-1.0.1/docs/_static/sankey-example-inverted.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/sankey-example-outgoing.png` & `highcharts_maps-1.0.1/docs/_static/sankey-example-outgoing.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/sankey-example.png` & `highcharts_maps-1.0.1/docs/_static/sankey-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/scatter-example.png` & `highcharts_maps-1.0.1/docs/_static/scatter-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/scatter_3d-example.png` & `highcharts_maps-1.0.1/docs/_static/scatter_3d-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/shared_options.js` & `highcharts_maps-1.0.1/docs/_static/shared_options.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/shared_options_output.js` & `highcharts_maps-1.0.1/docs/_static/shared_options_output.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/slow-stochastic-example.png` & `highcharts_maps-1.0.1/docs/_static/slow-stochastic-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/sma-example.png` & `highcharts_maps-1.0.1/docs/_static/sma-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/solidgauge-example.png` & `highcharts_maps-1.0.1/docs/_static/solidgauge-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/sphinx_rtd_theme_ext_color_contrast.css` & `highcharts_maps-1.0.1/docs/_static/sphinx_rtd_theme_ext_color_contrast.css`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/spline-example.png` & `highcharts_maps-1.0.1/docs/_static/spline-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/stochastic-example.png` & `highcharts_maps-1.0.1/docs/_static/stochastic-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/stock-tools-example.png` & `highcharts_maps-1.0.1/docs/_static/stock-tools-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/streamgraph-example.png` & `highcharts_maps-1.0.1/docs/_static/streamgraph-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/sunburst-example.png` & `highcharts_maps-1.0.1/docs/_static/sunburst-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/supertrend-example.png` & `highcharts_maps-1.0.1/docs/_static/supertrend-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/tema-example.png` & `highcharts_maps-1.0.1/docs/_static/tema-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/tilemap-example-circle.png` & `highcharts_maps-1.0.1/docs/_static/tilemap-example-circle.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/tilemap-example-diamond.png` & `highcharts_maps-1.0.1/docs/_static/tilemap-example-diamond.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/tilemap-example.png` & `highcharts_maps-1.0.1/docs/_static/tilemap-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/timeline-example-datetime.png` & `highcharts_maps-1.0.1/docs/_static/timeline-example-datetime.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/timeline-example-inverted.png` & `highcharts_maps-1.0.1/docs/_static/timeline-example-inverted.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/timeline-example.png` & `highcharts_maps-1.0.1/docs/_static/timeline-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/treemap-example.png` & `highcharts_maps-1.0.1/docs/_static/treemap-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/trendline-example.png` & `highcharts_maps-1.0.1/docs/_static/trendline-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/trix-example.png` & `highcharts_maps-1.0.1/docs/_static/trix-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/variablepie-example.png` & `highcharts_maps-1.0.1/docs/_static/variablepie-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/variwide-example-datetime.png` & `highcharts_maps-1.0.1/docs/_static/variwide-example-datetime.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/variwide-example-inverted.png` & `highcharts_maps-1.0.1/docs/_static/variwide-example-inverted.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/variwide-example.png` & `highcharts_maps-1.0.1/docs/_static/variwide-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/vbp-example.png` & `highcharts_maps-1.0.1/docs/_static/vbp-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/vector-example.png` & `highcharts_maps-1.0.1/docs/_static/vector-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/venn-example-euler.png` & `highcharts_maps-1.0.1/docs/_static/venn-example-euler.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/venn-example.png` & `highcharts_maps-1.0.1/docs/_static/venn-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/vwap-example.png` & `highcharts_maps-1.0.1/docs/_static/vwap-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/waterfall-example-inverted.png` & `highcharts_maps-1.0.1/docs/_static/waterfall-example-inverted.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/waterfall-example-stacked.png` & `highcharts_maps-1.0.1/docs/_static/waterfall-example-stacked.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/waterfall-example.png` & `highcharts_maps-1.0.1/docs/_static/waterfall-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/williamsr-example.png` & `highcharts_maps-1.0.1/docs/_static/williamsr-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/windbarb-example.png` & `highcharts_maps-1.0.1/docs/_static/windbarb-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/wma-example.png` & `highcharts_maps-1.0.1/docs/_static/wma-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/wordcloud-example.png` & `highcharts_maps-1.0.1/docs/_static/wordcloud-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/xrange-example-inverted.png` & `highcharts_maps-1.0.1/docs/_static/xrange-example-inverted.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/xrange-example.png` & `highcharts_maps-1.0.1/docs/_static/xrange-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/_static/zigzag-example.png` & `highcharts_maps-1.0.1/docs/_static/zigzag-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/_class_structures.rst` & `highcharts_maps-1.0.1/docs/api/_class_structures.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/_deserialization_methods.rst` & `highcharts_maps-1.0.1/docs/api/_deserialization_methods.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/_handling_defaults.rst` & `highcharts_maps-1.0.1/docs/api/_handling_defaults.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/_module_structure.rst` & `highcharts_maps-1.0.1/docs/api/_module_structure.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/_other_convenience_methods.rst` & `highcharts_maps-1.0.1/docs/api/_other_convenience_methods.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/_serialization_methods.rst` & `highcharts_maps-1.0.1/docs/api/_serialization_methods.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/chart.rst` & `highcharts_maps-1.0.1/docs/api/chart.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/headless_export.rst` & `highcharts_maps-1.0.1/docs/api/headless_export.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/highcharts.rst` & `highcharts_maps-1.0.1/docs/api/highcharts.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/internals.rst` & `highcharts_maps-1.0.1/docs/api/internals.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/index.rst` & `highcharts_maps-1.0.1/docs/api/global_options/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/shared_options.rst` & `highcharts_maps-1.0.1/docs/api/global_options/shared_options.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/export_data.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/export_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/index.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/navigation.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/navigation.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/announce_new_data.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/announce_new_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/axis.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/axis.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/chart_types.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/chart_types.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/exporting.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/exporting.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/index.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/legend.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/legend.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/range_selector.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/range_selector.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/screen_reader_section.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/screen_reader_section.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/series.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/series.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/sonification.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/sonification.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/table.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/table.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/zoom.rst` & `highcharts_maps-1.0.1/docs/api/global_options/language/accessibility/zoom.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/boost.rst` & `highcharts_maps-1.0.1/docs/api/options/boost.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/caption.rst` & `highcharts_maps-1.0.1/docs/api/options/caption.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/credits.rst` & `highcharts_maps-1.0.1/docs/api/options/credits.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/data.rst` & `highcharts_maps-1.0.1/docs/api/options/data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/defs.rst` & `highcharts_maps-1.0.1/docs/api/options/defs.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/drilldown.rst` & `highcharts_maps-1.0.1/docs/api/options/drilldown.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/index.rst` & `highcharts_maps-1.0.1/docs/api/options/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -296,17 +296,17 @@
     - :class:`FunnelOptions <highcharts_maps.options.plot_options.funnel.FunnelOptions>`
       :class:`Funnel3DOptions <highcharts_maps.options.plot_options.funnel.Funnel3DOptions>`
   * - :mod:`.options.plot_options.gauge <highcharts_maps.options.plot_options.gauge>`
     - :class:`GaugeOptions <highcharts_maps.options.plot_options.gauge.GaugeOptions>`
       :class:`SolidGaugeOptions <highcharts_maps.options.plot_options.gauge.SolidGaugeOptions>`
   * - :mod:`.options.plot_options.generic <highcharts_maps.options.plot_options.generic>`
     - :class:`GenericTypeOptions <highcharts_maps.options.plot_options.generic.GenericTypeOptions>`
-  * - :mod:`.options.plot_options.Heatmap <highcharts_maps.options.plot_options.Heatmap>`
-    - :class:`HeatmapOptions <highcharts_maps.options.plot_options.Heatmap.HeatmapOptions>`
-      :class:`TilemapOptions <highcharts_maps.options.plot_options.Tilemap.TilemapOptions>`
+  * - :mod:`.options.plot_options.heatmap <highcharts_maps.options.plot_options.heatmap>`
+    - :class:`HeatmapOptions <highcharts_maps.options.plot_options.heatmap.HeatmapOptions>`
+      :class:`TilemapOptions <highcharts_maps.options.plot_options.heatmap.TilemapOptions>`
   * - :mod:`.options.plot_options.histogram <highcharts_maps.options.plot_options.histogram>`
     - :class:`HistogramOptions <highcharts_maps.options.plot_options.histogram.HistogramOptions>`
   * - :mod:`.options.plot_options.item <highcharts_maps.options.plot_options.item>`
     - :class:`ItemOptions <highcharts_maps.options.plot_options.item.ItemOptions>`
   * - :mod:`.options.plot_options.levels <highcharts_maps.options.plot_options.levels>`
     - :class:`LevelOptions <highcharts_maps.options.plot_options.levels.LevelOptions>`
       :class:`SunburstLevelOptions <highcharts_maps.options.plot_options.levels.SunburstLevelOptions>`
```

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/loading.rst` & `highcharts_maps-1.0.1/docs/api/options/loading.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/map_navigation.rst` & `highcharts_maps-1.0.1/docs/api/options/map_navigation.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/responsive.rst` & `highcharts_maps-1.0.1/docs/api/options/responsive.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/subtitle.rst` & `highcharts_maps-1.0.1/docs/api/options/subtitle.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/time.rst` & `highcharts_maps-1.0.1/docs/api/options/time.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/title.rst` & `highcharts_maps-1.0.1/docs/api/options/title.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/tooltips.rst` & `highcharts_maps-1.0.1/docs/api/options/tooltips.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/announce_new_data.rst` & `highcharts_maps-1.0.1/docs/api/options/accessibility/announce_new_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/index.rst` & `highcharts_maps-1.0.1/docs/api/options/accessibility/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/point.rst` & `highcharts_maps-1.0.1/docs/api/options/accessibility/point.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/screen_reader_section.rst` & `highcharts_maps-1.0.1/docs/api/options/accessibility/screen_reader_section.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/series.rst` & `highcharts_maps-1.0.1/docs/api/options/accessibility/series.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/keyboard_navigation/focus_border.rst` & `highcharts_maps-1.0.1/docs/api/options/accessibility/keyboard_navigation/focus_border.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/keyboard_navigation/index.rst` & `highcharts_maps-1.0.1/docs/api/options/accessibility/keyboard_navigation/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/keyboard_navigation/series_navigation.rst` & `highcharts_maps-1.0.1/docs/api/options/accessibility/keyboard_navigation/series_navigation.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/annotations/animation.rst` & `highcharts_maps-1.0.1/docs/api/options/annotations/animation.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/annotations/control_point_options.rst` & `highcharts_maps-1.0.1/docs/api/options/annotations/control_point_options.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/annotations/events.rst` & `highcharts_maps-1.0.1/docs/api/options/annotations/events.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/annotations/index.rst` & `highcharts_maps-1.0.1/docs/api/options/annotations/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/annotations/label_options.rst` & `highcharts_maps-1.0.1/docs/api/options/annotations/label_options.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/annotations/points.rst` & `highcharts_maps-1.0.1/docs/api/options/annotations/points.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/annotations/shape_options.rst` & `highcharts_maps-1.0.1/docs/api/options/annotations/shape_options.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/accessibility.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/accessibility.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/breaks.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/breaks.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/color_axis.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/color_axis.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/crosshair.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/crosshair.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/data_classes.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/data_classes.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/generic.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/generic.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/index.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/labels.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/labels.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/markers.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/markers.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/numeric.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/numeric.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/parallel_axes.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/parallel_axes.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/plot_bands.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/plot_bands.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/title.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/title.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/x_axis.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/x_axis.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/y_axis.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/y_axis.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/axes/z_axis.rst` & `highcharts_maps-1.0.1/docs/api/options/axes/z_axis.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/chart/index.rst` & `highcharts_maps-1.0.1/docs/api/options/chart/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/chart/options_3d.rst` & `highcharts_maps-1.0.1/docs/api/options/chart/options_3d.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/chart/reset_zoom_button.rst` & `highcharts_maps-1.0.1/docs/api/options/chart/reset_zoom_button.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/chart/scrollable_plot_area.rst` & `highcharts_maps-1.0.1/docs/api/options/chart/scrollable_plot_area.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/chart/zooming.rst` & `highcharts_maps-1.0.1/docs/api/options/chart/zooming.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/exporting/csv.rst` & `highcharts_maps-1.0.1/docs/api/options/exporting/csv.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/exporting/index.rst` & `highcharts_maps-1.0.1/docs/api/options/exporting/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/exporting/pdf_font.rst` & `highcharts_maps-1.0.1/docs/api/options/exporting/pdf_font.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/legend/accessibility.rst` & `highcharts_maps-1.0.1/docs/api/options/legend/accessibility.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/legend/bubble_legend.rst` & `highcharts_maps-1.0.1/docs/api/options/legend/bubble_legend.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/legend/index.rst` & `highcharts_maps-1.0.1/docs/api/options/legend/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/legend/navigation.rst` & `highcharts_maps-1.0.1/docs/api/options/legend/navigation.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/legend/title.rst` & `highcharts_maps-1.0.1/docs/api/options/legend/title.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/map_views/index.rst` & `highcharts_maps-1.0.1/docs/api/options/map_views/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/map_views/insets.rst` & `highcharts_maps-1.0.1/docs/api/options/map_views/insets.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/navigation/bindings.rst` & `highcharts_maps-1.0.1/docs/api/options/navigation/bindings.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/navigation/index.rst` & `highcharts_maps-1.0.1/docs/api/options/navigation/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/accessibility.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/accessibility.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/arcdiagram.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/arcdiagram.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/area.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/area.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bar.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/bar.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/base.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/base.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bellcurve.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/bellcurve.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/boxplot.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/boxplot.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bubble.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/bubble.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bullet.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/bullet.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/data_sorting.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/data_sorting.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/dependencywheel.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/dependencywheel.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/drag_drop.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/drag_drop.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/dumbbell.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/dumbbell.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/funnel.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/funnel.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/gauge.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/gauge.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/generic.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/generic.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/heatmap.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/heatmap.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/histogram.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/histogram.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/index.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -142,17 +142,17 @@
     - :class:`FunnelOptions <highcharts_maps.options.plot_options.funnel.FunnelOptions>`
       :class:`Funnel3DOptions <highcharts_maps.options.plot_options.funnel.Funnel3DOptions>`
   * - :mod:`.options.plot_options.gauge <highcharts_maps.options.plot_options.gauge>`
     - :class:`GaugeOptions <highcharts_maps.options.plot_options.gauge.GaugeOptions>`
       :class:`SolidGaugeOptions <highcharts_maps.options.plot_options.gauge.SolidGaugeOptions>`
   * - :mod:`.options.plot_options.generic <highcharts_maps.options.plot_options.generic>`
     - :class:`GenericTypeOptions <highcharts_maps.options.plot_options.generic.GenericTypeOptions>`
-  * - :mod:`.options.plot_options.Heatmap <highcharts_maps.options.plot_options.Heatmap>`
-    - :class:`HeatmapOptions <highcharts_maps.options.plot_options.Heatmap.HeatmapOptions>`
-      :class:`TilemapOptions <highcharts_maps.options.plot_options.Tilemap.TilemapOptions>`
+  * - :mod:`.options.plot_options.heatmap <highcharts_maps.options.plot_options.heatmap>`
+    - :class:`HeatmapOptions <highcharts_maps.options.plot_options.heatmap.HeatmapOptions>`
+      :class:`TilemapOptions <highcharts_maps.options.plot_options.heatmap.TilemapOptions>`
   * - :mod:`.options.plot_options.histogram <highcharts_maps.options.plot_options.histogram>`
     - :class:`HistogramOptions <highcharts_maps.options.plot_options.histogram.HistogramOptions>`
   * - :mod:`.options.plot_options.item <highcharts_maps.options.plot_options.item>`
     - :class:`ItemOptions <highcharts_maps.options.plot_options.item.ItemOptions>`
   * - :mod:`.options.plot_options.levels <highcharts_maps.options.plot_options.levels>`
     - :class:`LevelOptions <highcharts_maps.options.plot_options.levels.LevelOptions>`
       :class:`SunburstLevelOptions <highcharts_maps.options.plot_options.levels.SunburstLevelOptions>`
```

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/item.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/item.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/levels.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/levels.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/link.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/link.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/map.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/map.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/mapbubble.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/mapbubble.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/mapline.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/mapline.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/mappoint.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/mappoint.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/networkgraph.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/networkgraph.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/organization.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/organization.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/packedbubble.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/packedbubble.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/pareto.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/pareto.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/pie.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/pie.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/points.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/points.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/polygon.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/polygon.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/pyramid.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/pyramid.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/sankey.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/sankey.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/scatter.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/scatter.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/series.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/series.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/spline.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/spline.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/sunburst.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/sunburst.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/timeline.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/timeline.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/treemap.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/treemap.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/vector.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/vector.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/venn.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/venn.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/wordcloud.rst` & `highcharts_maps-1.0.1/docs/api/options/plot_options/wordcloud.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/arcdiagram.rst` & `highcharts_maps-1.0.1/docs/api/options/series/arcdiagram.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/area.rst` & `highcharts_maps-1.0.1/docs/api/options/series/area.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/bar.rst` & `highcharts_maps-1.0.1/docs/api/options/series/bar.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/base.rst` & `highcharts_maps-1.0.1/docs/api/options/series/base.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/bellcurve.rst` & `highcharts_maps-1.0.1/docs/api/options/series/bellcurve.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/boxplot.rst` & `highcharts_maps-1.0.1/docs/api/options/series/boxplot.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/bubble.rst` & `highcharts_maps-1.0.1/docs/api/options/series/bubble.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/bullet.rst` & `highcharts_maps-1.0.1/docs/api/options/series/bullet.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/dependencywheel.rst` & `highcharts_maps-1.0.1/docs/api/options/series/dependencywheel.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/dumbbell.rst` & `highcharts_maps-1.0.1/docs/api/options/series/dumbbell.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/funnel.rst` & `highcharts_maps-1.0.1/docs/api/options/series/funnel.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/gauge.rst` & `highcharts_maps-1.0.1/docs/api/options/series/gauge.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/heatmap.rst` & `highcharts_maps-1.0.1/docs/api/options/series/heatmap.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/histogram.rst` & `highcharts_maps-1.0.1/docs/api/options/series/histogram.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/index.rst` & `highcharts_maps-1.0.1/docs/api/options/series/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/item.rst` & `highcharts_maps-1.0.1/docs/api/options/series/item.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/labels.rst` & `highcharts_maps-1.0.1/docs/api/options/series/labels.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/map.rst` & `highcharts_maps-1.0.1/docs/api/options/series/map.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/mapbubble.rst` & `highcharts_maps-1.0.1/docs/api/options/series/mapbubble.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/mapline.rst` & `highcharts_maps-1.0.1/docs/api/options/series/mapline.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/mappoint.rst` & `highcharts_maps-1.0.1/docs/api/options/series/mappoint.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/networkgraph.rst` & `highcharts_maps-1.0.1/docs/api/options/series/networkgraph.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/organization.rst` & `highcharts_maps-1.0.1/docs/api/options/series/organization.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/packedbubble.rst` & `highcharts_maps-1.0.1/docs/api/options/series/packedbubble.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/pareto.rst` & `highcharts_maps-1.0.1/docs/api/options/series/pareto.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/pie.rst` & `highcharts_maps-1.0.1/docs/api/options/series/pie.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/polygon.rst` & `highcharts_maps-1.0.1/docs/api/options/series/polygon.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/pyramid.rst` & `highcharts_maps-1.0.1/docs/api/options/series/pyramid.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/sankey.rst` & `highcharts_maps-1.0.1/docs/api/options/series/sankey.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/scatter.rst` & `highcharts_maps-1.0.1/docs/api/options/series/scatter.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/series_generator.rst` & `highcharts_maps-1.0.1/docs/api/options/series/series_generator.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/spline.rst` & `highcharts_maps-1.0.1/docs/api/options/series/spline.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/sunburst.rst` & `highcharts_maps-1.0.1/docs/api/options/series/sunburst.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/timeline.rst` & `highcharts_maps-1.0.1/docs/api/options/series/timeline.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/treemap.rst` & `highcharts_maps-1.0.1/docs/api/options/series/treemap.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/vector.rst` & `highcharts_maps-1.0.1/docs/api/options/series/vector.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/venn.rst` & `highcharts_maps-1.0.1/docs/api/options/series/venn.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/wordcloud.rst` & `highcharts_maps-1.0.1/docs/api/options/series/wordcloud.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/accessibility.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/accessibility.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/arcdiagram.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/arcdiagram.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/bar.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/bar.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/base.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/base.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/boxplot.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/boxplot.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/bullet.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/bullet.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/cartesian.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/cartesian.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/connections.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/connections.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/geometric.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/geometric.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/index.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/map_data.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/map_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/pie.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/pie.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/range.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/range.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/single_point.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/single_point.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/sunburst.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/sunburst.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/treemap.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/treemap.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/vector.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/vector.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/venn.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/venn.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/options/series/data/wordcloud.rst` & `highcharts_maps-1.0.1/docs/api/options/series/data/wordcloud.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/animation.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/animation.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/ast.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/ast.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/breadcrumbs.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/breadcrumbs.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/buttons.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/buttons.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/clusters.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/clusters.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/data_grouping.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/data_grouping.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/data_labels.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/data_labels.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/date_time_label_formats.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/date_time_label_formats.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/events.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/events.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/fetch_configuration.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/fetch_configuration.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/geojson.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/geojson.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/gradients.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/gradients.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/index.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/javascript_functions.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/javascript_functions.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/jitter.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/jitter.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/markers.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/markers.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/menus.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/menus.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/nodes.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/nodes.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/partial_fill.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/partial_fill.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/patterns.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/patterns.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/position.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/position.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/projections.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/projections.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/shadows.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/shadows.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/states.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/states.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/topojson.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/topojson.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/api/utility_classes/zones.rst` & `highcharts_maps-1.0.1/docs/api/utility_classes/zones.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/_code_style_naming_conventions.rst` & `highcharts_maps-1.0.1/docs/using/_code_style_naming_conventions.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/_importing.rst` & `highcharts_maps-1.0.1/docs/using/_importing.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/_working_with_maps_features.rst` & `highcharts_maps-1.0.1/docs/using/_working_with_maps_features.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_add_series.rst` & `highcharts_maps-1.0.1/docs/using/assembling_your_chart/_using_add_series.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_from_geopandas.rst` & `highcharts_maps-1.0.1/docs/using/assembling_your_chart/_using_from_geopandas.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_from_series.rst` & `highcharts_maps-1.0.1/docs/using/assembling_your_chart/_using_from_series.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_series_property.rst` & `highcharts_maps-1.0.1/docs/using/assembling_your_chart/_using_series_property.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_using_async_map_data.rst` & `highcharts_maps-1.0.1/docs/using/configuring_map_data/_using_async_map_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_using_synchronous_map_data.rst` & `highcharts_maps-1.0.1/docs/using/configuring_map_data/_using_synchronous_map_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_with_chart_map.rst` & `highcharts_maps-1.0.1/docs/using/configuring_map_data/_with_chart_map.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_with_series_map_data.rst` & `highcharts_maps-1.0.1/docs/using/configuring_map_data/_with_series_map_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/download_visualizations/_using_custom.rst` & `highcharts_maps-1.0.1/docs/using/download_visualizations/_using_custom.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/download_visualizations/_using_highsoft.rst` & `highcharts_maps-1.0.1/docs/using/download_visualizations/_using_highsoft.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_csv.rst` & `highcharts_maps-1.0.1/docs/using/populating_series_data/_load_from_csv.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_geopandas.rst` & `highcharts_maps-1.0.1/docs/using/populating_series_data/_load_from_geopandas.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_pandas.rst` & `highcharts_maps-1.0.1/docs/using/populating_series_data/_load_from_pandas.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_pyspark.rst` & `highcharts_maps-1.0.1/docs/using/populating_series_data/_load_from_pyspark.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_csv.rst` & `highcharts_maps-1.0.1/docs/using/populating_series_data/_new_from_csv.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_geopandas.rst` & `highcharts_maps-1.0.1/docs/using/populating_series_data/_new_from_geopandas.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_pandas.rst` & `highcharts_maps-1.0.1/docs/using/populating_series_data/_new_from_pandas.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_pyspark.rst` & `highcharts_maps-1.0.1/docs/using/populating_series_data/_new_from_pyspark.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_with_data_property.rst` & `highcharts_maps-1.0.1/docs/using/populating_series_data/_with_data_property.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_with_from_array.rst` & `highcharts_maps-1.0.1/docs/using/populating_series_data/_with_from_array.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/rendering_your_visualizations/_as_jupyter.rst` & `highcharts_maps-1.0.1/docs/using/rendering_your_visualizations/_as_jupyter.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/rendering_your_visualizations/_as_web_content.rst` & `highcharts_maps-1.0.1/docs/using/rendering_your_visualizations/_as_web_content.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/shared_options/_with_dict.rst` & `highcharts_maps-1.0.1/docs/using/shared_options/_with_dict.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/shared_options/_with_js_literal.rst` & `highcharts_maps-1.0.1/docs/using/shared_options/_with_js_literal.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/shared_options/_with_json.rst` & `highcharts_maps-1.0.1/docs/using/shared_options/_with_json.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/templates/_with_copy.rst` & `highcharts_maps-1.0.1/docs/using/templates/_with_copy.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/templates/_with_js_literal.rst` & `highcharts_maps-1.0.1/docs/using/templates/_with_js_literal.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/docs/using/templates/_with_json.rst` & `highcharts_maps-1.0.1/docs/using/templates/_with_json.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/chart.py` & `highcharts_maps-1.0.1/highcharts_maps/chart.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/headless_export.py` & `highcharts_maps-1.0.1/highcharts_maps/headless_export.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/highcharts.py` & `highcharts_maps-1.0.1/highcharts_maps/highcharts.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/utility_functions.py` & `highcharts_maps-1.0.1/highcharts_maps/utility_functions.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/global_options/shared_options.py` & `highcharts_maps-1.0.1/highcharts_maps/global_options/shared_options.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/__init__.py` & `highcharts_maps-1.0.1/highcharts_maps/global_options/language/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/__init__.py` & `highcharts_maps-1.0.1/highcharts_maps/options/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/map_navigation.py` & `highcharts_maps-1.0.1/highcharts_maps/options/map_navigation.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/chart/__init__.py` & `highcharts_maps-1.0.1/highcharts_maps/options/chart/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/map_views/__init__.py` & `highcharts_maps-1.0.1/highcharts_maps/options/map_views/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/map_views/insets.py` & `highcharts_maps-1.0.1/highcharts_maps/options/map_views/insets.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/navigation/__init__.py` & `highcharts_maps-1.0.1/highcharts_maps/options/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/__init__.py` & `highcharts_maps-1.0.1/highcharts_maps/options/plot_options/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/base.py` & `highcharts_maps-1.0.1/highcharts_maps/options/plot_options/base.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/heatmap.py` & `highcharts_maps-1.0.1/highcharts_maps/options/plot_options/heatmap.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/map.py` & `highcharts_maps-1.0.1/highcharts_maps/options/plot_options/map.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/mapbubble.py` & `highcharts_maps-1.0.1/highcharts_maps/options/plot_options/mapbubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/mapline.py` & `highcharts_maps-1.0.1/highcharts_maps/options/plot_options/mapline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/mappoint.py` & `highcharts_maps-1.0.1/highcharts_maps/options/plot_options/mappoint.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/pie.py` & `highcharts_maps-1.0.1/highcharts_maps/options/plot_options/pie.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/series.py` & `highcharts_maps-1.0.1/highcharts_maps/options/plot_options/series.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/base.py` & `highcharts_maps-1.0.1/highcharts_maps/options/series/base.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/heatmap.py` & `highcharts_maps-1.0.1/highcharts_maps/options/series/heatmap.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/map.py` & `highcharts_maps-1.0.1/highcharts_maps/options/series/map.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/mapbubble.py` & `highcharts_maps-1.0.1/highcharts_maps/options/series/mapbubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/mapline.py` & `highcharts_maps-1.0.1/highcharts_maps/options/series/mapline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/mappoint.py` & `highcharts_maps-1.0.1/highcharts_maps/options/series/mappoint.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/pie.py` & `highcharts_maps-1.0.1/highcharts_maps/options/series/pie.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/series_generator.py` & `highcharts_maps-1.0.1/highcharts_maps/options/series/series_generator.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/geometric.py` & `highcharts_maps-1.0.1/highcharts_maps/options/series/data/geometric.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/map_data.py` & `highcharts_maps-1.0.1/highcharts_maps/options/series/data/map_data.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/buttons.py` & `highcharts_maps-1.0.1/highcharts_maps/utility_classes/buttons.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/fetch_configuration.py` & `highcharts_maps-1.0.1/highcharts_maps/utility_classes/fetch_configuration.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/geojson.py` & `highcharts_maps-1.0.1/highcharts_maps/utility_classes/geojson.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/projections.py` & `highcharts_maps-1.0.1/highcharts_maps/utility_classes/projections.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/topojson.py` & `highcharts_maps-1.0.1/highcharts_maps/utility_classes/topojson.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/__init__.py` & `highcharts_maps-1.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/conftest.py` & `highcharts_maps-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/fixtures.py` & `highcharts_maps-1.0.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/test_chart.py` & `highcharts_maps-1.0.1/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/test_decorators.py` & `highcharts_maps-1.0.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/test_headless_export.py` & `highcharts_maps-1.0.1/tests/test_headless_export.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/test_js_literal_functions.py` & `highcharts_maps-1.0.1/tests/test_js_literal_functions.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/test_metaclasses.py` & `highcharts_maps-1.0.1/tests/test_metaclasses.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/test_mro.py` & `highcharts_maps-1.0.1/tests/test_mro.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/global_options/test_shared_options.py` & `highcharts_maps-1.0.1/tests/global_options/test_shared_options.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/global_options/language/test_export_data.py` & `highcharts_maps-1.0.1/tests/global_options/language/test_export_data.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/global_options/language/test_language.py` & `highcharts_maps-1.0.1/tests/global_options/language/test_language.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/global_options/language/test_navigation.py` & `highcharts_maps-1.0.1/tests/global_options/language/test_navigation.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/global_options/language/accessibility/test_accessibility.py` & `highcharts_maps-1.0.1/tests/global_options/language/accessibility/test_accessibility.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/global_options/language/accessibility/test_series.py` & `highcharts_maps-1.0.1/tests/global_options/language/accessibility/test_series.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/accessibility/accessibility/01.js` & `highcharts_maps-1.0.1/tests/input_files/accessibility/accessibility/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/accessibility/accessibility/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/accessibility/accessibility/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/annotation/01.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/annotation/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/annotation/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/annotation/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/01.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/02.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/03.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/04.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/05.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/05.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/06.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/07.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/07.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/08.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/08.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/09.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/09.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/10.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/10.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-03.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-04.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-05.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-05.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-06.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-07.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-07.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-08.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-08.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-09.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-09.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-10.js` & `highcharts_maps-1.0.1/tests/input_files/annotations/stock_tools/error-10.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/01.js` & `highcharts_maps-1.0.1/tests/input_files/axes/color_axis/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/color_axis/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/axes/color_axis/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/color_axis/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/01.js` & `highcharts_maps-1.0.1/tests/input_files/axes/numeric/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/numeric/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/axes/numeric/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/numeric/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/01.js` & `highcharts_maps-1.0.1/tests/input_files/axes/parallel_axes/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/parallel_axes/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/axes/parallel_axes/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/parallel_axes/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/01.js` & `highcharts_maps-1.0.1/tests/input_files/axes/plot_bands/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/plot_bands/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/axes/plot_bands/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/plot_bands/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/x_axis/02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/x_axis/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/x_axis/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/x_axis/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/01.js` & `highcharts_maps-1.0.1/tests/input_files/axes/y_axis/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/y_axis/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/axes/y_axis/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/y_axis/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/01.js` & `highcharts_maps-1.0.1/tests/input_files/axes/z_axis/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/z_axis/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/axes/z_axis/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/axes/z_axis/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/chart/chart/01.js` & `highcharts_maps-1.0.1/tests/input_files/chart/chart/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/chart/chart/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/chart/chart/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/chart/options_3d/01.js` & `highcharts_maps-1.0.1/tests/input_files/chart/options_3d/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/chart/options_3d/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/chart/options_3d/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/chart_obj/01-expected.js` & `highcharts_maps-1.0.1/tests/input_files/chart_obj/01-expected.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/chart_obj/01-input.js` & `highcharts_maps-1.0.1/tests/input_files/chart_obj/01-input.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/drilldown/01.js` & `highcharts_maps-1.0.1/tests/input_files/drilldown/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/drilldown/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/drilldown/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/exporting/exporting/01.js` & `highcharts_maps-1.0.1/tests/input_files/exporting/exporting/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/exporting/exporting/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/exporting/exporting/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/accessibility/01.js` & `highcharts_maps-1.0.1/tests/input_files/global_options/language/accessibility/accessibility/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/accessibility/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/global_options/language/accessibility/accessibility/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/02.js` & `highcharts_maps-1.0.1/tests/input_files/global_options/language/accessibility/series/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/error-03.js` & `highcharts_maps-1.0.1/tests/input_files/global_options/language/accessibility/series/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/language/01.js` & `highcharts_maps-1.0.1/tests/input_files/global_options/language/language/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/language/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/global_options/language/language/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/01.js` & `highcharts_maps-1.0.1/tests/input_files/global_options/language/navigation/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/02.js` & `highcharts_maps-1.0.1/tests/input_files/global_options/language/navigation/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/global_options/language/navigation/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/error-03.js` & `highcharts_maps-1.0.1/tests/input_files/global_options/language/navigation/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/global_options/shared_options/01-expected.js` & `highcharts_maps-1.0.1/tests/input_files/global_options/shared_options/01-expected.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/global_options/shared_options/01-input.js` & `highcharts_maps-1.0.1/tests/input_files/global_options/shared_options/01-input.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/headless_export/output/test-basic.png` & `highcharts_maps-1.0.1/tests/input_files/headless_export/output/test-basic.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/headless_export/output/test-with-chart-type.png` & `highcharts_maps-1.0.1/tests/input_files/headless_export/output/test-with-chart-type.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/headless_export/output/test-with-series-types.png` & `highcharts_maps-1.0.1/tests/input_files/headless_export/output/test-with-series-types.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/legend/bubble_legend/01.js` & `highcharts_maps-1.0.1/tests/input_files/legend/bubble_legend/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/legend/bubble_legend/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/legend/bubble_legend/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/legend/legend/01.js` & `highcharts_maps-1.0.1/tests/input_files/legend/legend/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/legend/legend/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/legend/legend/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/02.js` & `highcharts_maps-1.0.1/tests/input_files/navigation/bindings/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/error-03.js` & `highcharts_maps-1.0.1/tests/input_files/navigation/bindings/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/navigation/navigation/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/navigation/navigation/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/options/01.js` & `highcharts_maps-1.0.1/tests/input_files/options/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/arcdiagram/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/arcdiagram/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/arcdiagram/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/arcdiagram/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/area/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/area/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bar/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bar/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/04.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bar/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/06.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bar/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/07.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bar/07.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/08.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bar/08.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/09.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bar/09.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/10.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bar/10.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bar/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bar/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bellcurve/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bellcurve/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/boxplot/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/boxplot/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/boxplot/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/boxplot/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bubble/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bubble/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bubble/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bullet/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bullet/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bullet/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/bullet/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/dependencywheel/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/dependencywheel/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/dependencywheel/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/dependencywheel/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/dumbbell/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/dumbbell/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/dumbbell/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/dumbbell/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/03.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/04.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-03.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-04.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/funnel/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/04.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-04.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/gauge/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/generic/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/generic/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/generic/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/generic/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/04.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-04.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/heatmap/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/histogram/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/histogram/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/item/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/item/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/networkgraph/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/networkgraph/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/networkgraph/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/networkgraph/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/organization/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/organization/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/organization/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/organization/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/packedbubble/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/packedbubble/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/pie/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/pie/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/03.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/pie/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/04.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/pie/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/pie/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/pie/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-03.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/pie/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-04.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/pie/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/plot_options/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/plot_options/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/sankey/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/sankey/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/sankey/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/sankey/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/scatter/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/scatter/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/scatter/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/scatter/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/series/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/series/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/series/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/series/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/spline/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/spline/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/spline/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/spline/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/sunburst/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/sunburst/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/sunburst/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/sunburst/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/timeline/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/timeline/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/timeline/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/timeline/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/treemap/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/treemap/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/treemap/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/treemap/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/vector/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/vector/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/vector/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/vector/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/venn/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/venn/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/venn/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/venn/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/wordcloud/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/plot_options/wordcloud/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/arcdiagram/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/arcdiagram/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/arcdiagram/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/arcdiagram/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/area/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/area/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/area/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/area/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/area/03.js` & `highcharts_maps-1.0.1/tests/input_files/series/area/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/area/04.js` & `highcharts_maps-1.0.1/tests/input_files/series/area/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/area/05.js` & `highcharts_maps-1.0.1/tests/input_files/series/area/05.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/area/06.js` & `highcharts_maps-1.0.1/tests/input_files/series/area/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/area/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/area/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-03.js` & `highcharts_maps-1.0.1/tests/input_files/series/area/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-04.js` & `highcharts_maps-1.0.1/tests/input_files/series/area/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/bar/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/bar/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/03.js` & `highcharts_maps-1.0.1/tests/input_files/series/bar/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/04.js` & `highcharts_maps-1.0.1/tests/input_files/series/bar/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/06.js` & `highcharts_maps-1.0.1/tests/input_files/series/bar/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/07.js` & `highcharts_maps-1.0.1/tests/input_files/series/bar/07.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/08.js` & `highcharts_maps-1.0.1/tests/input_files/series/bar/08.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/bar/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/base/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/base/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/base/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/base/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/base/03.js` & `highcharts_maps-1.0.1/tests/input_files/series/base/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/base/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/base/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/base/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/base/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bellcurve/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/bellcurve/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bellcurve/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/bellcurve/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/boxplot/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/boxplot/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/boxplot/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/boxplot/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bubble/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/bubble/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bubble/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/bubble/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bullet/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/bullet/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/bullet/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/bullet/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/bar/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/bar/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/03.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/bar/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/04.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/bar/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/05.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/bar/05.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/06.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/bar/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/bar/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/bar/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-03.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/bar/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-04.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/bar/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/base/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/base/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/base/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/base/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/boxplot/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/boxplot/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/boxplot/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/boxplot/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bullet/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/bullet/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bullet/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/bullet/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/03.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/04.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/06.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/08.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/08.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/cartesian/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/connections/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/connections/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/03.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/connections/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/04.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/connections/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/connections/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/connections/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/error-03.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/connections/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/geometric/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/geometric/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/03.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/geometric/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/geometric/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/error-03.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/geometric/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/world.geo.json` & `highcharts_maps-1.0.1/tests/input_files/series/data/map_data/map_data/world.geo.json`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/world.topo.json` & `highcharts_maps-1.0.1/tests/input_files/series/data/map_data/map_data/world.topo.json`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/pie/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/pie/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/pie/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/pie/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/range/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/range/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/04.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/range/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/range/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/range/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/single_point/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/single_point/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/03.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/single_point/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/04.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/single_point/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/05.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/single_point/05.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/06.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/single_point/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/single_point/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/single_point/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-03.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/single_point/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-04.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/single_point/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-05.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/single_point/error-05.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-06.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/single_point/error-06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/sunburst/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/sunburst/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/sunburst/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/sunburst/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/vector/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/vector/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/vector/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/vector/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/venn/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/venn/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/venn/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/venn/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/wordcloud/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/wordcloud/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/data/wordcloud/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/data/wordcloud/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/dependencywheel/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/dependencywheel/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/dependencywheel/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/dependencywheel/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/dumbbell/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/dumbbell/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/dumbbell/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/dumbbell/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/funnel/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/funnel/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/funnel/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/funnel/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/gauge/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/gauge/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/gauge/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/gauge/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/generic/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/generic/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/generic/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/generic/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/heatmap/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/heatmap/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/heatmap/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/heatmap/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/histogram/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/histogram/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/histogram/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/histogram/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/item/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/item/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/item/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/item/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/item/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/item/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/item/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/item/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/map/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/map/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/mapbubble/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/mapbubble/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/mapbubble/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/mapbubble/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/mapline/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/mapline/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/mapline/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/mapline/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/mappoint/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/mappoint/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/mappoint/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/mappoint/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/networkgraph/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/networkgraph/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/networkgraph/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/networkgraph/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/organization/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/organization/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/organization/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/organization/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/organization/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/organization/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/organization/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/organization/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/packedbubble/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/packedbubble/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/packedbubble/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/packedbubble/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/pareto/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/pareto/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/pareto/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/pareto/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/pareto/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/pareto/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/pie/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/pie/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/pie/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/pie/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/pie/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/pie/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/pie/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/pie/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/polygon/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/polygon/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/polygon/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/polygon/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/sankey/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/sankey/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/sankey/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/sankey/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/scatter/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/scatter/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/scatter/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/scatter/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/spline/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/spline/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/spline/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/spline/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/spline/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/spline/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/spline/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/spline/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/sunburst/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/sunburst/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/sunburst/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/sunburst/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/timeline/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/timeline/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/timeline/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/timeline/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/treemap/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/treemap/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/treemap/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/treemap/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/vector/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/vector/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/vector/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/vector/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/vector/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/vector/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/vector/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/vector/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/venn/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/venn/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/venn/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/venn/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/venn/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/venn/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/venn/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/venn/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/01.js` & `highcharts_maps-1.0.1/tests/input_files/series/wordcloud/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/02.js` & `highcharts_maps-1.0.1/tests/input_files/series/wordcloud/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/series/wordcloud/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/error-02.js` & `highcharts_maps-1.0.1/tests/input_files/series/wordcloud/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/test-data-files/nst-est2019-01-transposed.csv` & `highcharts_maps-1.0.1/tests/input_files/test-data-files/nst-est2019-01-transposed.csv`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/test-data-files/nst-est2019-01.csv` & `highcharts_maps-1.0.1/tests/input_files/test-data-files/nst-est2019-01.csv`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/clusters/01.js` & `highcharts_maps-1.0.1/tests/input_files/utility_classes/clusters/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/clusters/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/utility_classes/clusters/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_grouping/01.js` & `highcharts_maps-1.0.1/tests/input_files/utility_classes/data_grouping/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_grouping/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/utility_classes/data_grouping/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/01.js` & `highcharts_maps-1.0.1/tests/input_files/utility_classes/data_labels/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/02.js` & `highcharts_maps-1.0.1/tests/input_files/utility_classes/data_labels/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/error-01.js` & `highcharts_maps-1.0.1/tests/input_files/utility_classes/data_labels/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/error-03.js` & `highcharts_maps-1.0.1/tests/input_files/utility_classes/data_labels/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_boost.py` & `highcharts_maps-1.0.1/tests/options/test_boost.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_caption.py` & `highcharts_maps-1.0.1/tests/options/test_caption.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_credits.py` & `highcharts_maps-1.0.1/tests/options/test_credits.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_data.py` & `highcharts_maps-1.0.1/tests/options/test_data.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_defs.py` & `highcharts_maps-1.0.1/tests/options/test_defs.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_drilldown.py` & `highcharts_maps-1.0.1/tests/options/test_drilldown.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_loading.py` & `highcharts_maps-1.0.1/tests/options/test_loading.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_options.py` & `highcharts_maps-1.0.1/tests/options/test_options.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_responsive.py` & `highcharts_maps-1.0.1/tests/options/test_responsive.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_subtitle.py` & `highcharts_maps-1.0.1/tests/options/test_subtitle.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_time.py` & `highcharts_maps-1.0.1/tests/options/test_time.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_title.py` & `highcharts_maps-1.0.1/tests/options/test_title.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/test_tooltips.py` & `highcharts_maps-1.0.1/tests/options/test_tooltips.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/accessibility/test_accessibility.py` & `highcharts_maps-1.0.1/tests/options/accessibility/test_accessibility.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/annotations/test_annotation.py` & `highcharts_maps-1.0.1/tests/options/annotations/test_annotation.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/axes/test_color_axis.py` & `highcharts_maps-1.0.1/tests/options/axes/test_color_axis.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/axes/test_numeric.py` & `highcharts_maps-1.0.1/tests/options/axes/test_numeric.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/axes/test_parallel_axes.py` & `highcharts_maps-1.0.1/tests/options/axes/test_parallel_axes.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/axes/test_plot_bands.py` & `highcharts_maps-1.0.1/tests/options/axes/test_plot_bands.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/axes/test_x_axis.py` & `highcharts_maps-1.0.1/tests/options/axes/test_x_axis.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/axes/test_y_axis.py` & `highcharts_maps-1.0.1/tests/options/axes/test_y_axis.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/axes/test_z_axis.py` & `highcharts_maps-1.0.1/tests/options/axes/test_z_axis.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/chart/test_chart.py` & `highcharts_maps-1.0.1/tests/options/chart/test_chart.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/chart/test_options_3d.py` & `highcharts_maps-1.0.1/tests/options/chart/test_options_3d.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/chart/test_zooming.py` & `highcharts_maps-1.0.1/tests/options/chart/test_zooming.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/exporting/test_csv.py` & `highcharts_maps-1.0.1/tests/options/exporting/test_csv.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/exporting/test_exporting.py` & `highcharts_maps-1.0.1/tests/options/exporting/test_exporting.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/legend/test_bubble_legend.py` & `highcharts_maps-1.0.1/tests/options/legend/test_bubble_legend.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/legend/test_legend.py` & `highcharts_maps-1.0.1/tests/options/legend/test_legend.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/legend/test_navigation.py` & `highcharts_maps-1.0.1/tests/options/legend/test_navigation.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/navigation/test_bindings.py` & `highcharts_maps-1.0.1/tests/options/navigation/test_bindings.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/navigation/test_navigation.py` & `highcharts_maps-1.0.1/tests/options/navigation/test_navigation.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_PlotOptions.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_PlotOptions.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_arcdiagram.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_arcdiagram.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_area.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_area.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bar.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_bar.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bellcurve.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_bellcurve.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_boxplot.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_boxplot.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bubble.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_bubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bullet.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_bullet.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_dependencywheel.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_dependencywheel.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_dumbbell.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_dumbbell.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_funnel.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_funnel.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_gauge.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_gauge.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_generic.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_generic.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_heatmap.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_heatmap.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_histogram.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_histogram.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_item.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_item.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_map.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_map.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_mapbubble.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_mapbubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_mapline.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_mapline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_mappoint.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_mappoint.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_networkgraph.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_networkgraph.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_organization.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_organization.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_packedbubble.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_packedbubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_pareto.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_pareto.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_pie.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_pie.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_polygon.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_polygon.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_pyramid.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_pyramid.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_sankey.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_sankey.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_scatter.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_scatter.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_series.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_series.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_spline.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_spline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_sunburst.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_sunburst.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_timeline.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_timeline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_treemap.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_treemap.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_vector.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_vector.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_venn.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_venn.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_wordcloud.py` & `highcharts_maps-1.0.1/tests/options/plot_options/test_wordcloud.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_arcdiagram.py` & `highcharts_maps-1.0.1/tests/options/series/test_arcdiagram.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_area.py` & `highcharts_maps-1.0.1/tests/options/series/test_area.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_bar.py` & `highcharts_maps-1.0.1/tests/options/series/test_bar.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_base.py` & `highcharts_maps-1.0.1/tests/options/series/test_base.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_bellcurve.py` & `highcharts_maps-1.0.1/tests/options/series/test_bellcurve.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_boxplot.py` & `highcharts_maps-1.0.1/tests/options/series/test_boxplot.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_bubble.py` & `highcharts_maps-1.0.1/tests/options/series/test_bubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_bullet.py` & `highcharts_maps-1.0.1/tests/options/series/test_bullet.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_dependencywheel.py` & `highcharts_maps-1.0.1/tests/options/series/test_dependencywheel.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_dumbbell.py` & `highcharts_maps-1.0.1/tests/options/series/test_dumbbell.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_funnel.py` & `highcharts_maps-1.0.1/tests/options/series/test_funnel.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_gauge.py` & `highcharts_maps-1.0.1/tests/options/series/test_gauge.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_heatmap.py` & `highcharts_maps-1.0.1/tests/options/series/test_heatmap.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_histogram.py` & `highcharts_maps-1.0.1/tests/options/series/test_histogram.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_item.py` & `highcharts_maps-1.0.1/tests/options/series/test_item.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_map.py` & `highcharts_maps-1.0.1/tests/options/series/test_map.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_mapbubble.py` & `highcharts_maps-1.0.1/tests/options/series/test_mapbubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_mapline.py` & `highcharts_maps-1.0.1/tests/options/series/test_mapline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_mappoint.py` & `highcharts_maps-1.0.1/tests/options/series/test_mappoint.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_networkgraph.py` & `highcharts_maps-1.0.1/tests/options/series/test_networkgraph.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_organization.py` & `highcharts_maps-1.0.1/tests/options/series/test_organization.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_packedbubble.py` & `highcharts_maps-1.0.1/tests/options/series/test_packedbubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_pareto.py` & `highcharts_maps-1.0.1/tests/options/series/test_pareto.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_pie.py` & `highcharts_maps-1.0.1/tests/options/series/test_pie.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_polygon.py` & `highcharts_maps-1.0.1/tests/options/series/test_polygon.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_pyramid.py` & `highcharts_maps-1.0.1/tests/options/series/test_pyramid.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_sankey.py` & `highcharts_maps-1.0.1/tests/options/series/test_sankey.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_scatter.py` & `highcharts_maps-1.0.1/tests/options/series/test_scatter.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_spline.py` & `highcharts_maps-1.0.1/tests/options/series/test_spline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_sunburst.py` & `highcharts_maps-1.0.1/tests/options/series/test_sunburst.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_timeline.py` & `highcharts_maps-1.0.1/tests/options/series/test_timeline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_treemap.py` & `highcharts_maps-1.0.1/tests/options/series/test_treemap.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_vector.py` & `highcharts_maps-1.0.1/tests/options/series/test_vector.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_venn.py` & `highcharts_maps-1.0.1/tests/options/series/test_venn.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/test_wordcloud.py` & `highcharts_maps-1.0.1/tests/options/series/test_wordcloud.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_bar.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_bar.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_base.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_base.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_boxplot.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_boxplot.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_bullet.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_bullet.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_cartesian.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_cartesian.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_connections.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_connections.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_geometric.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_geometric.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_map_data.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_map_data.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_pie.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_pie.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_range.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_range.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_single_point.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_single_point.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_sunburst.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_sunburst.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_vector.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_vector.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_venn.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_venn.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/options/series/data/test_wordcloud.py` & `highcharts_maps-1.0.1/tests/options/series/data/test_wordcloud.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_animation.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_animation.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_ast.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_ast.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_breadcrumbs.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_buttons.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_buttons.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_clusters.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_clusters.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_data_grouping.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_data_grouping.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_data_labels.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_data_labels.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_date_time_label_formats.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_date_time_label_formats.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_events.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_events.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_gradients.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_gradients.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_javascript_functions.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_javascript_functions.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_jitter.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_jitter.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_markers.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_markers.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_menus.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_menus.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_nodes.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_nodes.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_partial_fill.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_partial_fill.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_patterns.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_patterns.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_position.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_position.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_shadows.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_shadows.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_states.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_states.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/tests/utility_classes/test_zones.py` & `highcharts_maps-1.0.1/tests/utility_classes/test_zones.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/.gitignore` & `highcharts_maps-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/LICENSE` & `highcharts_maps-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc6/README.rst` & `highcharts_maps-1.0.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,31 @@
 
 To install **Highcharts Maps for Python**, just execute:
 
   .. code-block:: bash
 
     $ pip install highcharts-maps
 
+Before you install, please be aware of the following "hard" dependencies:
+
+  * Python 3.10 or higher
+  * Highcharts Maps (JS) v.10.2 or higher (not technically a Python dependency, but 
+    it won't work with earlier versions of Highcharts)
+  * `Highcharts Core for Python <https://core-docs.highchartspython.com/en/latest/>`__ v.1.0 or higher
+  * `esprima-python <https://github.com/Kronuz/esprima-python>`__ v.4.0 or higher
+  * `requests <https://requests.readthedocs.io/en/latest/>`__ v.2.28 or higher
+  * `validator-collection <https://validator-collection.readthedocs.io/en/latest/>`__
+    v.1.5 or higher
+  * `topojson <https://mattijn.github.io/topojson/>`__ v.1.5 or higher
+  * `geojson <https://github.com/jazzband/geojson/>`__ v.3.0 or higher
+
+You can find more information about soft and development dependencies in the
+`complete documentation <https://maps-docs.highchartspython.com/en/latest/#dependencies>`__.
+
+
 -------------
 
 *********************************
 Why Highcharts for Python?
 *********************************
 
 `Highcharts <https://www.highcharts.com>`__ is the world's most popular, most powerful,
```

### Comparing `highcharts_maps-1.0.0rc6/pyproject.toml` & `highcharts_maps-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "plotting",
     "gis",
     "maps",
     "geospatial"
 ]
 
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Manufacturing",
@@ -72,16 +72,16 @@
 [project.urls]
 "Homepage" = "https://www.highchartspython.com"
 "Documentation" = "https://maps-docs.highchartspython.com/en/latest/"
 "Support" = "https://www.highchartspython.com/get-help"
 "Source Code" = "https://github.com/highcharts-for-python/highcharts-maps"
 "History" = "https://github.com/highcharts-for-python/highcharts-maps/blob/master/CHANGES.rst"
 "Bug Tracker" = "https://github.com/highcharts-for-python/highcharts-maps/issues"
-# TODO: Add a Sponsor section
-# "Sponsor" = "https://github.com/sponsors/highcharts-for-python"
+"Demo" = "https://github.com/highcharts-for-python/highcharts-for-python-demos"
+#"Sponsor" = "https://github.com/sponsors/highcharts-for-python"
 
 [project.optional-dependencies]
 dev = [
     "pytest>=7.0.2",
     "pytest-cov>=3.0.0",
     "pytest-xdist>=2.5.0",
     "python-dotenv>=1.0.0",
```

### Comparing `highcharts_maps-1.0.0rc6/PKG-INFO` & `highcharts_maps-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: highcharts-maps
-Version: 1.0.0rc6
+Version: 1.0.1
 Summary: High-end Map Data Visualization for the Python Ecosystem
 Project-URL: Homepage, https://www.highchartspython.com
 Project-URL: Documentation, https://maps-docs.highchartspython.com/en/latest/
 Project-URL: Support, https://www.highchartspython.com/get-help
 Project-URL: Source Code, https://github.com/highcharts-for-python/highcharts-maps
 Project-URL: History, https://github.com/highcharts-for-python/highcharts-maps/blob/master/CHANGES.rst
 Project-URL: Bug Tracker, https://github.com/highcharts-for-python/highcharts-maps/issues
+Project-URL: Demo, https://github.com/highcharts-for-python/highcharts-for-python-demos
 Author-email: HCP LLC <support@highchartspython.com>
 License-File: LICENSE
 Keywords: charts,data visualization,data viz,geospatial,gis,graphing,highcharts,highcharts maps,maps,plotting
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Manufacturing
@@ -144,14 +145,31 @@
 
 To install **Highcharts Maps for Python**, just execute:
 
   .. code-block:: bash
 
     $ pip install highcharts-maps
 
+Before you install, please be aware of the following "hard" dependencies:
+
+  * Python 3.10 or higher
+  * Highcharts Maps (JS) v.10.2 or higher (not technically a Python dependency, but 
+    it won't work with earlier versions of Highcharts)
+  * `Highcharts Core for Python <https://core-docs.highchartspython.com/en/latest/>`__ v.1.0 or higher
+  * `esprima-python <https://github.com/Kronuz/esprima-python>`__ v.4.0 or higher
+  * `requests <https://requests.readthedocs.io/en/latest/>`__ v.2.28 or higher
+  * `validator-collection <https://validator-collection.readthedocs.io/en/latest/>`__
+    v.1.5 or higher
+  * `topojson <https://mattijn.github.io/topojson/>`__ v.1.5 or higher
+  * `geojson <https://github.com/jazzband/geojson/>`__ v.3.0 or higher
+
+You can find more information about soft and development dependencies in the
+`complete documentation <https://maps-docs.highchartspython.com/en/latest/#dependencies>`__.
+
+
 -------------
 
 *********************************
 Why Highcharts for Python?
 *********************************
 
 `Highcharts <https://www.highcharts.com>`__ is the world's most popular, most powerful,
```


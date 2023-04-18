# Comparing `tmp/voici-0.3.3.tar.gz` & `tmp/voici-0.4.0.tar.gz`

## Comparing `voici-0.3.3.tar` & `voici-0.4.0.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 voici-0.3.3/.eslintignore
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 voici-0.3.3/.eslintrc.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 voici-0.3.3/.prettierignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 voici-0.3.3/.prettierrc
--rw-r--r--   0        0        0    10857 2020-02-02 00:00:00.000000 voici-0.3.3/CHANGELOG.md
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 voici-0.3.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 voici-0.3.3/RELEASE.md
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 voici-0.3.3/environment.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 voici-0.3.3/lerna.json
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 voici-0.3.3/lint-staged.config.js
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 voici-0.3.3/package.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 voici-0.3.3/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 voici-0.3.3/setup.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.3.3/tsconfig.eslint.json
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 voici-0.3.3/tsconfigbase.json
--rw-r--r--   0        0        0   537654 2020-02-02 00:00:00.000000 voici-0.3.3/yarn.lock
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.3.3/demo/environment.yml
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 voici-0.3.3/demo/notebooks/iris.csv
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 voici-0.3.3/demo/notebooks/voici.ipynb
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 voici-0.3.3/demo/notebooks/widgets/bqplot.ipynb
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 voici-0.3.3/demo/notebooks/widgets/ipycanvas.ipynb
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 voici-0.3.3/docs/changelog.md
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 voici-0.3.3/docs/conf.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 voici-0.3.3/docs/configuration.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 voici-0.3.3/docs/contributing.md
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 voici-0.3.3/docs/deploy.md
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 voici-0.3.3/docs/environment.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 voici-0.3.3/docs/index.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 voici-0.3.3/docs/install.md
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 voici-0.3.3/docs/voila-logo.svg
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 voici-0.3.3/scripts/bump-version.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/package.json
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/playwright.config.js
--rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/yarn.lock
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/tests/voici.test.ts
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png
--rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png
--rw-r--r--   0        0        0   186883 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png
--rw-r--r--   0        0        0    46536 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png
--rw-r--r--   0        0        0    53032 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png
--rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png
--rw-r--r--   0        0        0    13752 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png
--rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png
--rw-r--r--   0        0        0    12468 2020-02-02 00:00:00.000000 voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 voici-0.3.3/voici/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 voici-0.3.3/voici/__main__.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 voici-0.3.3/voici/_version.py
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 voici-0.3.3/voici/addon.py
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 voici-0.3.3/voici/app.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 voici-0.3.3/voici/exporter.py
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 voici-0.3.3/voici/tree_exporter.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/index.html
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1023.js
--rw-r--r--   0        0        0   599879 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1024.js
--rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/103.js
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1053.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1058.js
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1100.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1105.js
--rw-r--r--   0        0        0    23883 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1432.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1497.js
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1553.js
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1581.js
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1667.js
--rw-r--r--   0        0        0    53409 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1672.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1672.js.LICENSE.txt
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1732.js
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1770.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1890.js
--rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/1980.js
--rw-r--r--   0        0        0    24245 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2075.js
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2106.js
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2230.js
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2266.js
--rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2322.js
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2359.js
--rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2361.js
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2488.js
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2516.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2630.js
--rw-r--r--   0        0        0    11565 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2687.js
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/275.js
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2784.js
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2784.js.LICENSE.txt
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/286.js
--rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/2950.js
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3008.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3086.js
--rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3251.js
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3256.js
--rw-r--r--   0        0        0   432937 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/330.js
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3305.js
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3312.js
--rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3316.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3316.js.LICENSE.txt
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3349.js
--rw-r--r--   0        0        0   198935 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/339.js
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3504.js
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3655.js
--rw-r--r--   0        0        0    13521 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3693.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3811.js
--rw-r--r--   0        0        0   152146 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3851.js
--rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/3922.js
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/4259.js
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/4359.js
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/4382.js
--rw-r--r--   0        0        0   173449 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/450.js
--rw-r--r--   0        0        0    44048 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/4530.js
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/4530.js.LICENSE.txt
--rw-r--r--   0        0        0    33749 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/4875.js
--rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/4896.js
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/4939.js
--rw-r--r--   0        0        0   901507 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/4963.js
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/4963.js.LICENSE.txt
--rw-r--r--   0        0        0   130996 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/4977.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/5188.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/5291.js
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/53.js
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/5403.js
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/5445.js
--rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/5474.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/5826.js
--rw-r--r--   0        0        0   103087 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/5950.js
--rw-r--r--   0        0        0   306356 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/5952.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/5952.js.LICENSE.txt
--rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/596.js
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/5985.js
--rw-r--r--   0        0        0    31585 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6111.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6178.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6196.js
--rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6219.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6219.js.LICENSE.txt
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6417.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6527.js
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6587.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6614.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6616.js
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6757.js
--rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6770.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6790.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6839.js
--rw-r--r--   0        0        0    10288 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6852.js
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6856.js
--rw-r--r--   0        0        0    88422 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6914.js
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/6976.js
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/7003.js
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/7015.js
--rw-r--r--   0        0        0    31429 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/7066.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/709.js
--rw-r--r--   0        0        0    89502 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/74.js
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/7469.js
--rw-r--r--   0        0        0    82106 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/7560.js
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/7623.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/7695.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/7795.js
--rw-r--r--   0        0        0    37531 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/8085.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/8164.js
--rw-r--r--   0        0        0    89999 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/8291.js
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/8291.js.LICENSE.txt
--rw-r--r--   0        0        0   123750 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/8316.js
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/8316.js.LICENSE.txt
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/846.js
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/86.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/8679.js
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/8809.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/8874.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9060.js
--rw-r--r--   0        0        0   528943 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9112.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9320.js
--rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9339.js
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9406.js
--rw-r--r--   0        0        0   135493 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9513.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9513.js.LICENSE.txt
--rw-r--r--   0        0        0   248014 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9727.js
--rw-r--r--   0        0        0    53651 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9757.js
--rw-r--r--   0        0        0    37027 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9780.js
--rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9807.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9817.js
--rw-r--r--   0        0        0    84485 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9900.js
--rw-r--r--   0        0        0    22979 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/9988.js
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/service-worker-b2fb40a.js
--rw-r--r--   0        0        0    23293 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/treepage.js
--rw-r--r--   0        0        0    24001 2020-02-02 00:00:00.000000 voici-0.3.3/voici/static/build/voici.js
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 voici-0.3.3/.gitignore
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 voici-0.3.3/LICENSE
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 voici-0.3.3/README.md
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 voici-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 voici-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 voici-0.4.0/.eslintignore
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 voici-0.4.0/.eslintrc.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 voici-0.4.0/.prettierignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 voici-0.4.0/.prettierrc
+-rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 voici-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 voici-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 voici-0.4.0/RELEASE.md
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 voici-0.4.0/environment.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 voici-0.4.0/lerna.json
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 voici-0.4.0/lint-staged.config.js
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 voici-0.4.0/package.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 voici-0.4.0/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 voici-0.4.0/setup.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.0/tsconfig.eslint.json
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 voici-0.4.0/tsconfigbase.json
+-rw-r--r--   0        0        0   537654 2020-02-02 00:00:00.000000 voici-0.4.0/yarn.lock
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.0/demo/environment.yml
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 voici-0.4.0/demo/notebooks/iris.csv
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 voici-0.4.0/demo/notebooks/voici.ipynb
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 voici-0.4.0/demo/notebooks/widgets/bqplot.ipynb
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 voici-0.4.0/demo/notebooks/widgets/ipycanvas.ipynb
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 voici-0.4.0/docs/changelog.md
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 voici-0.4.0/docs/conf.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 voici-0.4.0/docs/configuration.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 voici-0.4.0/docs/contributing.md
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 voici-0.4.0/docs/deploy.md
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 voici-0.4.0/docs/environment.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 voici-0.4.0/docs/index.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 voici-0.4.0/docs/install.md
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 voici-0.4.0/docs/voila-logo.svg
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 voici-0.4.0/scripts/bump-version.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/package.json
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png
+-rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png
+-rw-r--r--   0        0        0   186883 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png
+-rw-r--r--   0        0        0    46536 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png
+-rw-r--r--   0        0        0    53032 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png
+-rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png
+-rw-r--r--   0        0        0    13752 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png
+-rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png
+-rw-r--r--   0        0        0    12468 2020-02-02 00:00:00.000000 voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 voici-0.4.0/voici/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 voici-0.4.0/voici/__main__.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 voici-0.4.0/voici/_version.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 voici-0.4.0/voici/addon.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 voici-0.4.0/voici/app.py
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 voici-0.4.0/voici/exporter.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 voici-0.4.0/voici/tree_exporter.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/index.html
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1023.js
+-rw-r--r--   0        0        0   599879 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1024.js
+-rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/103.js
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1053.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1058.js
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1100.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1105.js
+-rw-r--r--   0        0        0    23883 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1432.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1497.js
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1553.js
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1581.js
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1667.js
+-rw-r--r--   0        0        0    53409 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1672.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1672.js.LICENSE.txt
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1732.js
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1770.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1890.js
+-rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/1980.js
+-rw-r--r--   0        0        0    24245 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2075.js
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2106.js
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2230.js
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2266.js
+-rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2322.js
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2359.js
+-rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2361.js
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2488.js
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2516.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2630.js
+-rw-r--r--   0        0        0    11565 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2687.js
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/275.js
+-rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2784.js
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2784.js.LICENSE.txt
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/286.js
+-rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/2950.js
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3008.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3086.js
+-rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3251.js
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3256.js
+-rw-r--r--   0        0        0   432937 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/330.js
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3305.js
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3312.js
+-rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3316.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3316.js.LICENSE.txt
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3349.js
+-rw-r--r--   0        0        0   198935 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/339.js
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3504.js
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3655.js
+-rw-r--r--   0        0        0    13521 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3693.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3811.js
+-rw-r--r--   0        0        0   152146 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3851.js
+-rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/3922.js
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4259.js
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4359.js
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4382.js
+-rw-r--r--   0        0        0   173449 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/450.js
+-rw-r--r--   0        0        0    44048 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4530.js
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4530.js.LICENSE.txt
+-rw-r--r--   0        0        0    33749 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4875.js
+-rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4896.js
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4939.js
+-rw-r--r--   0        0        0   901507 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4963.js
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4963.js.LICENSE.txt
+-rw-r--r--   0        0        0   130996 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/4977.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5188.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5291.js
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/53.js
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5403.js
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5445.js
+-rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5474.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5826.js
+-rw-r--r--   0        0        0   103087 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5950.js
+-rw-r--r--   0        0        0   306356 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5952.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5952.js.LICENSE.txt
+-rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/596.js
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/5985.js
+-rw-r--r--   0        0        0    31585 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6111.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6178.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6196.js
+-rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6219.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6219.js.LICENSE.txt
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6417.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6527.js
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6587.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6614.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6616.js
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6757.js
+-rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6770.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6790.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6839.js
+-rw-r--r--   0        0        0    10288 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6852.js
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6856.js
+-rw-r--r--   0        0        0    88422 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6914.js
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/6976.js
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7003.js
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7015.js
+-rw-r--r--   0        0        0    31429 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7066.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/709.js
+-rw-r--r--   0        0        0    89502 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/74.js
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7469.js
+-rw-r--r--   0        0        0    82106 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7560.js
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7623.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7695.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/7795.js
+-rw-r--r--   0        0        0    37531 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8085.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8164.js
+-rw-r--r--   0        0        0    89999 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8291.js
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8291.js.LICENSE.txt
+-rw-r--r--   0        0        0   123750 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8316.js
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8316.js.LICENSE.txt
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/846.js
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/86.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8679.js
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8809.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/8874.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9060.js
+-rw-r--r--   0        0        0   528943 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9112.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9320.js
+-rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9339.js
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9406.js
+-rw-r--r--   0        0        0   135493 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9513.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9513.js.LICENSE.txt
+-rw-r--r--   0        0        0   248014 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9727.js
+-rw-r--r--   0        0        0    53651 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9757.js
+-rw-r--r--   0        0        0    37027 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9780.js
+-rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9807.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9817.js
+-rw-r--r--   0        0        0    84485 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9900.js
+-rw-r--r--   0        0        0    22979 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/9988.js
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/service-worker-b2fb40a.js
+-rw-r--r--   0        0        0    23293 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/treepage.js
+-rw-r--r--   0        0        0    24001 2020-02-02 00:00:00.000000 voici-0.4.0/voici/static/build/voici.js
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 voici-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 voici-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 voici-0.4.0/README.md
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 voici-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8455 2020-02-02 00:00:00.000000 voici-0.4.0/PKG-INFO
```

### Comparing `voici-0.3.3/.eslintrc.js` & `voici-0.4.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/CHANGELOG.md` & `voici-0.4.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.4.0
+
+([Full Changelog](https://github.com/voila-dashboards/voici/compare/v0.3.3...3fb43ef1d143a3e78939e7e35d293cda01d58867))
+
+### Enhancements made
+
+- Update CLI [#65](https://github.com/voila-dashboards/voici/pull/65) ([@trungleduc](https://github.com/trungleduc))
+
+### Documentation improvements
+
+- Update readme [#66](https://github.com/voila-dashboards/voici/pull/66) ([@trungleduc](https://github.com/trungleduc))
+- Add badges to the README [#64](https://github.com/voila-dashboards/voici/pull/64) ([@jtpio](https://github.com/jtpio))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/voila-dashboards/voici/graphs/contributors?from=2023-04-13&to=2023-04-18&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Agithub-actions+updated%3A2023-04-13..2023-04-18&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Ajtpio+updated%3A2023-04-13..2023-04-18&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3AmartinRenou+updated%3A2023-04-13..2023-04-18&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Atrungleduc+updated%3A2023-04-13..2023-04-18&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.3.3
 
 ([Full Changelog](https://github.com/voila-dashboards/voici/compare/@voila-dashboards/voici@0.3.2...1e5b08a398d89d69bcdd746ec47fb09be5b8f0df))
 
 ### Enhancements made
 
 - Fix handling of the base url to enable the Service Worker [#59](https://github.com/voila-dashboards/voici/pull/59) ([@jtpio](https://github.com/jtpio))
@@ -26,16 +47,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/voila-dashboards/voici/graphs/contributors?from=2023-04-12&to=2023-04-13&type=c))
 
 [@jtpio](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Ajtpio+updated%3A2023-04-12..2023-04-13&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.3.2
 
 ([Full Changelog](https://github.com/voila-dashboards/voici/compare/@voila-dashboards/voici@0.3.1...db3b22a3d267337ee8dbded091948ac574588c66))
 
 ### Enhancements made
 
 - Create `__main__.py` [#56](https://github.com/voila-dashboards/voici/pull/56) ([@jtpio](https://github.com/jtpio))
```

### Comparing `voici-0.3.3/CONTRIBUTING.md` & `voici-0.4.0/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Note: You will need NodeJS to build the extension package.
 
 **Note**: we recommend using `mamba` to speed the creating of the environment.
 
 ```bash
 # create a new environment
-mamba create -f environment.yml
+mamba env create -f environment.yml
 
 # activate the environment
 mamba activate voici-dev
 
 # Install package in development mode
 pip install -e ".[dev,docs]"
 ```
```

### Comparing `voici-0.3.3/RELEASE.md` & `voici-0.4.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/lint-staged.config.js` & `voici-0.4.0/lint-staged.config.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/package.json` & `voici-0.4.0/package.json`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/tsconfigbase.json` & `voici-0.4.0/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/yarn.lock` & `voici-0.4.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/demo/notebooks/iris.csv` & `voici-0.4.0/demo/notebooks/iris.csv`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/demo/notebooks/voici.ipynb` & `voici-0.4.0/demo/notebooks/voici.ipynb`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/demo/notebooks/widgets/bqplot.ipynb` & `voici-0.4.0/demo/notebooks/widgets/bqplot.ipynb`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/demo/notebooks/widgets/ipycanvas.ipynb` & `voici-0.4.0/demo/notebooks/widgets/ipycanvas.ipynb`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/docs/conf.py` & `voici-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/docs/configuration.md` & `voici-0.4.0/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/docs/deploy.md` & `voici-0.4.0/docs/deploy.md`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/docs/index.md` & `voici-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/docs/install.md` & `voici-0.4.0/docs/install.md`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/docs/voila-logo.svg` & `voici-0.4.0/docs/voila-logo.svg`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/scripts/bump-version.py` & `voici-0.4.0/scripts/bump-version.py`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/ui-tests/package.json` & `voici-0.4.0/ui-tests/package.json`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/ui-tests/yarn.lock` & `voici-0.4.0/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/ui-tests/tests/voici.test.ts` & `voici-0.4.0/ui-tests/tests/voici.test.ts`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png` & `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png` & `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png` & `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png` & `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png` & `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png` & `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png` & `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png` & `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png` & `voici-0.4.0/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/_version.py` & `voici-0.4.0/voici/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Distributed under the terms of the Modified BSD License.
 
 import re
 
 from collections import namedtuple
 
 # Use "hatch version xx.yy.zz" to handle version changes
-__version__ = "0.3.3"
+__version__ = "0.4.0"
 
 # PEP440 version parser
 _version_regex = re.compile(
     r"""
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `voici-0.3.3/voici/addon.py` & `voici-0.4.0/voici/addon.py`

 * *Files 12% similar despite different names*

```diff
@@ -126,14 +126,40 @@
                     (
                         self.create_dashboard_or_tree,
                         [generate_file, self.manager.output_dir / "voici" / file_path],
                     )
                 ],
             )
 
+        # Update index page
+        yield dict(
+            name=f"voici:update_index:{self.manager.output_dir}",
+            actions=[
+                (
+                    self.update_index,
+                    [self.manager.output_dir / "voici"],
+                )
+            ],
+        )
+
+    def update_index(self, desc: Path):
+        """Update the redirect URL"""
+
+        if len(self.manager.contents) == 1 and self.manager.contents[0].is_file():
+            file_name = self.manager.contents[0].stem
+            new_url = f"/voici/render/{file_name}.html"
+        else:
+            new_url = "/voici/tree/index.html"
+        index_file = desc / "index.html"
+        with open(index_file, "r+") as f:
+            content = f.read()
+            new_content = content.replace(r"{{voici_index_url}}", new_url)
+            f.seek(0)
+            f.write(new_content)
+
     def create_dashboard_or_tree(
         self, generate_file: Callable[[Dict], io.StringIO], dest: Path
     ):
         """generate a voici dashboard or tree view in the lite output"""
         # Get page_config
         jupyterlite_json = self.manager.output_dir / JUPYTERLITE_JSON
         config = json.loads(jupyterlite_json.read_text(**UTF8))
@@ -173,15 +199,15 @@
             return
 
         jupyterlite_json = self.manager.output_dir / JUPYTERLITE_JSON
         config = json.loads(jupyterlite_json.read_text(**UTF8))
         page_config = config.get(JUPYTER_CONFIG_DATA, {})
 
         # Patch appUrl
-        page_config["appUrl"] = "./voici/tree"
+        page_config["appUrl"] = "./voici"
 
         # Path favicon
         page_config["faviconUrl"] = "./voici/favicon.ico"
 
         config[JUPYTER_CONFIG_DATA] = page_config
 
         jupyterlite_json.write_text(json.dumps(config, **JSON_FMT), **UTF8)
```

### Comparing `voici-0.3.3/voici/exporter.py` & `voici-0.4.0/voici/exporter.py`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/tree_exporter.py` & `voici-0.4.0/voici/tree_exporter.py`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1023.js` & `voici-0.4.0/voici/static/build/1023.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1024.js` & `voici-0.4.0/voici/static/build/1024.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/103.js` & `voici-0.4.0/voici/static/build/103.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1053.js` & `voici-0.4.0/voici/static/build/1053.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1058.js` & `voici-0.4.0/voici/static/build/1058.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1100.js` & `voici-0.4.0/voici/static/build/1100.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1105.js` & `voici-0.4.0/voici/static/build/1105.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1432.js` & `voici-0.4.0/voici/static/build/1432.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1553.js` & `voici-0.4.0/voici/static/build/1553.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1581.js` & `voici-0.4.0/voici/static/build/1581.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1667.js` & `voici-0.4.0/voici/static/build/1667.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1672.js` & `voici-0.4.0/voici/static/build/1672.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1770.js` & `voici-0.4.0/voici/static/build/1770.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1890.js` & `voici-0.4.0/voici/static/build/1890.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/1980.js` & `voici-0.4.0/voici/static/build/1980.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/2075.js` & `voici-0.4.0/voici/static/build/2075.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/2106.js` & `voici-0.4.0/voici/static/build/2106.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/2230.js` & `voici-0.4.0/voici/static/build/2230.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/2322.js` & `voici-0.4.0/voici/static/build/2322.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/2359.js` & `voici-0.4.0/voici/static/build/2359.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/2361.js` & `voici-0.4.0/voici/static/build/2361.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/2488.js` & `voici-0.4.0/voici/static/build/2488.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/2630.js` & `voici-0.4.0/voici/static/build/2630.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/2687.js` & `voici-0.4.0/voici/static/build/2687.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/275.js` & `voici-0.4.0/voici/static/build/275.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/2784.js` & `voici-0.4.0/voici/static/build/2784.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/286.js` & `voici-0.4.0/voici/static/build/286.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/2950.js` & `voici-0.4.0/voici/static/build/2950.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3008.js` & `voici-0.4.0/voici/static/build/3008.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3086.js` & `voici-0.4.0/voici/static/build/3086.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3251.js` & `voici-0.4.0/voici/static/build/3251.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3256.js` & `voici-0.4.0/voici/static/build/3256.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/330.js` & `voici-0.4.0/voici/static/build/330.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3305.js` & `voici-0.4.0/voici/static/build/3305.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3312.js` & `voici-0.4.0/voici/static/build/3312.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3316.js` & `voici-0.4.0/voici/static/build/3316.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3316.js.LICENSE.txt` & `voici-0.4.0/voici/static/build/3316.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3349.js` & `voici-0.4.0/voici/static/build/3349.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/339.js` & `voici-0.4.0/voici/static/build/339.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3504.js` & `voici-0.4.0/voici/static/build/3504.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3655.js` & `voici-0.4.0/voici/static/build/3655.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3693.js` & `voici-0.4.0/voici/static/build/3693.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3811.js` & `voici-0.4.0/voici/static/build/3811.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3851.js` & `voici-0.4.0/voici/static/build/3851.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/3922.js` & `voici-0.4.0/voici/static/build/3922.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/4259.js` & `voici-0.4.0/voici/static/build/4259.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/4359.js` & `voici-0.4.0/voici/static/build/4359.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/4382.js` & `voici-0.4.0/voici/static/build/4382.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/450.js` & `voici-0.4.0/voici/static/build/450.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/4530.js` & `voici-0.4.0/voici/static/build/4530.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/4875.js` & `voici-0.4.0/voici/static/build/4875.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/4896.js` & `voici-0.4.0/voici/static/build/4896.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/4939.js` & `voici-0.4.0/voici/static/build/4939.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/4963.js` & `voici-0.4.0/voici/static/build/4963.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/4963.js.LICENSE.txt` & `voici-0.4.0/voici/static/build/4963.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/4977.js` & `voici-0.4.0/voici/static/build/4977.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/5188.js` & `voici-0.4.0/voici/static/build/5188.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/5291.js` & `voici-0.4.0/voici/static/build/5291.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/53.js` & `voici-0.4.0/voici/static/build/53.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/5403.js` & `voici-0.4.0/voici/static/build/5403.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/5445.js` & `voici-0.4.0/voici/static/build/5445.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/5474.js` & `voici-0.4.0/voici/static/build/5474.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [5474], {
         27693: e => {
             e.exports = {
                 name: "@voila-dashboards/voici",
-                version: "0.3.3",
+                version: "0.4.0",
                 description: "The Voici Frontend",
                 author: "Voilà contributors",
                 license: "BSD-3-Clause",
                 main: "lib/index.js",
                 browserslist: ">0.8%, not ie 11, not op_mini all, not dead",
                 dependencies: {
                     "@jupyter-widgets/base": "^6.0.1",
```

### Comparing `voici-0.3.3/voici/static/build/5826.js` & `voici-0.4.0/voici/static/build/5826.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/5950.js` & `voici-0.4.0/voici/static/build/5950.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/5952.js` & `voici-0.4.0/voici/static/build/5952.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/596.js` & `voici-0.4.0/voici/static/build/596.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/5985.js` & `voici-0.4.0/voici/static/build/5985.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6111.js` & `voici-0.4.0/voici/static/build/6111.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6178.js` & `voici-0.4.0/voici/static/build/6178.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6196.js` & `voici-0.4.0/voici/static/build/6196.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6219.js` & `voici-0.4.0/voici/static/build/6219.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6219.js.LICENSE.txt` & `voici-0.4.0/voici/static/build/6219.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6527.js` & `voici-0.4.0/voici/static/build/6527.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6614.js` & `voici-0.4.0/voici/static/build/6614.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6616.js` & `voici-0.4.0/voici/static/build/6616.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6757.js` & `voici-0.4.0/voici/static/build/6757.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6770.js` & `voici-0.4.0/voici/static/build/6770.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6790.js` & `voici-0.4.0/voici/static/build/6790.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6839.js` & `voici-0.4.0/voici/static/build/6839.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6852.js` & `voici-0.4.0/voici/static/build/6852.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6852], {
         27693: e => {
             e.exports = {
                 name: "@voila-dashboards/voici",
-                version: "0.3.3",
+                version: "0.4.0",
                 description: "The Voici Frontend",
                 author: "Voilà contributors",
                 license: "BSD-3-Clause",
                 main: "lib/index.js",
                 browserslist: ">0.8%, not ie 11, not op_mini all, not dead",
                 dependencies: {
                     "@jupyter-widgets/base": "^6.0.1",
```

### Comparing `voici-0.3.3/voici/static/build/6856.js` & `voici-0.4.0/voici/static/build/6856.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6914.js` & `voici-0.4.0/voici/static/build/6914.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/6976.js` & `voici-0.4.0/voici/static/build/6976.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/7003.js` & `voici-0.4.0/voici/static/build/7003.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/7015.js` & `voici-0.4.0/voici/static/build/7015.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/7066.js` & `voici-0.4.0/voici/static/build/7066.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/709.js` & `voici-0.4.0/voici/static/build/709.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/74.js` & `voici-0.4.0/voici/static/build/74.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/7469.js` & `voici-0.4.0/voici/static/build/7469.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/7560.js` & `voici-0.4.0/voici/static/build/7560.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/7623.js` & `voici-0.4.0/voici/static/build/7623.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/7695.js` & `voici-0.4.0/voici/static/build/7695.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/7795.js` & `voici-0.4.0/voici/static/build/7795.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/8085.js` & `voici-0.4.0/voici/static/build/8085.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/8164.js` & `voici-0.4.0/voici/static/build/8164.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/8291.js` & `voici-0.4.0/voici/static/build/8291.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/8316.js` & `voici-0.4.0/voici/static/build/8316.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/8316.js.LICENSE.txt` & `voici-0.4.0/voici/static/build/8316.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/846.js` & `voici-0.4.0/voici/static/build/846.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/86.js` & `voici-0.4.0/voici/static/build/86.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/8809.js` & `voici-0.4.0/voici/static/build/8809.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/8874.js` & `voici-0.4.0/voici/static/build/8874.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/9060.js` & `voici-0.4.0/voici/static/build/9060.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/9112.js` & `voici-0.4.0/voici/static/build/9112.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/9339.js` & `voici-0.4.0/voici/static/build/9339.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/9406.js` & `voici-0.4.0/voici/static/build/9406.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/9513.js` & `voici-0.4.0/voici/static/build/9513.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/9727.js` & `voici-0.4.0/voici/static/build/9727.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/9757.js` & `voici-0.4.0/voici/static/build/9757.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/9780.js` & `voici-0.4.0/voici/static/build/9780.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/9807.js` & `voici-0.4.0/voici/static/build/9807.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/9900.js` & `voici-0.4.0/voici/static/build/9900.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/9988.js` & `voici-0.4.0/voici/static/build/9988.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/service-worker-b2fb40a.js` & `voici-0.4.0/voici/static/build/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/treepage.js` & `voici-0.4.0/voici/static/build/treepage.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/voici/static/build/voici.js` & `voici-0.4.0/voici/static/build/voici.js`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/LICENSE` & `voici-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/README.md` & `voici-0.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Voici
 
+![Github Actions Status](https://github.com/voila-dashboards/voici/actions/workflows/main.yml/badge.svg)
+[![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge-launch.svg)](https://voici.readthedocs.io/en/latest/_static/lite)
+[![Documentation Status](https://readthedocs.org/projects/voici/badge/?version=latest)](https://voici.readthedocs.io/en/latest/?badge=latest)
+
 🚧 **WARNING: Voici is still a work in progress and should not be used for production workloads.** 🚧
 
-Voici is a tool for generating static dashboards from Jupyter Notebooks. Unlike [Voilà](https://github.com/voila-dashboards/voila), which renders interactive dashboards using server-side execution, Voici uses [WebAssembly](https://developer.mozilla.org/en-US/docs/WebAssembly) (Wasm) kernels to render notebooks in the browser, making the resulting dashboard entirely self-contained and distributable.
+Voici is a tool for generating static dashboards from Jupyter Notebooks. It can be used as a drop-in replacement for [Voilà](https://github.com/voila-dashboards/voila) and it has the same commands and supports most of Voila's configuration options.
+
+Unlike Voila, which renders interactive dashboards using server-side execution, Voici uses [WebAssembly](https://developer.mozilla.org/en-US/docs/WebAssembly) (Wasm) kernels to render notebooks in the browser, making the resulting dashboard entirely self-contained and distributable.
 
 This is made possible thanks to the amazing work done in the [JupyterLite project](https://github.com/jupyterlite/jupyterlite).
 
 https://user-images.githubusercontent.com/591645/222892327-2a5b1341-640d-49c2-9e95-1f2d3ec122be.mp4
 
 ## Features 🚀
 
@@ -19,43 +25,58 @@
 
 To use Voici, you'll need to install it first:
 
 ```bash
 pip install voici
 ```
 
-Then, you can generate static dashboards from a directory of Notebooks like this:
+Then, you can generate static dashboards from a notebook or a directory of Notebooks like this:
 
 ```bash
-voici build --contents notebooks/
+# Build a single dashboard
+voici my-notebook.ipynb
+# Build a directory of notebooks
+voici notebooks/
 ```
 
-Once your dashboards built, you can simply serve them with a simple static server, _e.g._:
+Once your dashboards are built, you can simply serve them with a simple static server, _e.g._:
 
 ```bash
 cd _output
 python -m http.server
 ```
 
-The `voici` command line interface is the same as the `jupyter lite` one. The only difference is that the `voici build` command will only generate Voici dashboards, excluding the full JupyterLab interface from the output. Running `voici build .` is equivalent to running `jupyter lite build . --apps voici`
+## Advanced usage
+
+The `voici` command line interface is a mix between `voila` and `jupyter lite`. For most cases, users can rely on the `voici` command by using the `voila` CLI syntax.
+
+Voici runs the `build` sub-command by default, the `voici my-notebook.ipynb` command is a shortcut for `voici build --contents my-notebook.ipynb`
+For advanced usage, users can invoke `voici` with the `jupyter lite` CLI syntax, _e.g._:
+
+```bash
+voici build --contents my-notebook.ipynb
+```
+
+The difference between `voici build` and `jupyter lite build` commands is that the voici one will only generate Voici dashboards, excluding the full JupyterLab interface from the output. Running `voici build --contents .` is equivalent to running `jupyter lite build --contents . --apps voici`.
+
 You can generate the classic `jupyter lite` output alongside your dashboards by specifying the additional apps you want:
 
 ```bash
-voici build --apps lab --apps retro
+voici build --contents . --apps lab --apps retro
 ```
 
 In order to get some help on how to use the `voici` command, you can run:
 
 ```bash
 voici --help
 ```
 
 We'd also suggest looking into the [JupyterLite documentation](https://jupyterlite.readthedocs.io/en/latest/howto/index.html) for more insights on how to configure your `voici` deployment.
 
-### Build the demo site yourself
+## Build the demo site yourself
 
 Before you can build the demo site from this repository, you will need to install [jupyterlite-xeus-python](https://github.com/jupyterlite/xeus-python-kernel):
 
 ```bash
 pip install jupyterlite-xeus-python
 ```
```

### Comparing `voici-0.3.3/pyproject.toml` & `voici-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `voici-0.3.3/PKG-INFO` & `voici-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voici
-Version: 0.3.3
+Version: 0.4.0
 Summary: Voici turns Jupyter notebooks into static web applications
 Project-URL: Homepage, https://github.com/voila-dashboards/voici
 Author: Voila Development Team
 License: BSD License
         
         Copyright (c) 2018 Voilà contributors.
         All rights reserved.
@@ -59,17 +59,23 @@
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Requires-Dist: sphinxcontrib-video; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # Voici
 
+![Github Actions Status](https://github.com/voila-dashboards/voici/actions/workflows/main.yml/badge.svg)
+[![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge-launch.svg)](https://voici.readthedocs.io/en/latest/_static/lite)
+[![Documentation Status](https://readthedocs.org/projects/voici/badge/?version=latest)](https://voici.readthedocs.io/en/latest/?badge=latest)
+
 🚧 **WARNING: Voici is still a work in progress and should not be used for production workloads.** 🚧
 
-Voici is a tool for generating static dashboards from Jupyter Notebooks. Unlike [Voilà](https://github.com/voila-dashboards/voila), which renders interactive dashboards using server-side execution, Voici uses [WebAssembly](https://developer.mozilla.org/en-US/docs/WebAssembly) (Wasm) kernels to render notebooks in the browser, making the resulting dashboard entirely self-contained and distributable.
+Voici is a tool for generating static dashboards from Jupyter Notebooks. It can be used as a drop-in replacement for [Voilà](https://github.com/voila-dashboards/voila) and it has the same commands and supports most of Voila's configuration options.
+
+Unlike Voila, which renders interactive dashboards using server-side execution, Voici uses [WebAssembly](https://developer.mozilla.org/en-US/docs/WebAssembly) (Wasm) kernels to render notebooks in the browser, making the resulting dashboard entirely self-contained and distributable.
 
 This is made possible thanks to the amazing work done in the [JupyterLite project](https://github.com/jupyterlite/jupyterlite).
 
 https://user-images.githubusercontent.com/591645/222892327-2a5b1341-640d-49c2-9e95-1f2d3ec122be.mp4
 
 ## Features 🚀
 
@@ -82,43 +88,58 @@
 
 To use Voici, you'll need to install it first:
 
 ```bash
 pip install voici
 ```
 
-Then, you can generate static dashboards from a directory of Notebooks like this:
+Then, you can generate static dashboards from a notebook or a directory of Notebooks like this:
 
 ```bash
-voici build --contents notebooks/
+# Build a single dashboard
+voici my-notebook.ipynb
+# Build a directory of notebooks
+voici notebooks/
 ```
 
-Once your dashboards built, you can simply serve them with a simple static server, _e.g._:
+Once your dashboards are built, you can simply serve them with a simple static server, _e.g._:
 
 ```bash
 cd _output
 python -m http.server
 ```
 
-The `voici` command line interface is the same as the `jupyter lite` one. The only difference is that the `voici build` command will only generate Voici dashboards, excluding the full JupyterLab interface from the output. Running `voici build .` is equivalent to running `jupyter lite build . --apps voici`
+## Advanced usage
+
+The `voici` command line interface is a mix between `voila` and `jupyter lite`. For most cases, users can rely on the `voici` command by using the `voila` CLI syntax.
+
+Voici runs the `build` sub-command by default, the `voici my-notebook.ipynb` command is a shortcut for `voici build --contents my-notebook.ipynb`
+For advanced usage, users can invoke `voici` with the `jupyter lite` CLI syntax, _e.g._:
+
+```bash
+voici build --contents my-notebook.ipynb
+```
+
+The difference between `voici build` and `jupyter lite build` commands is that the voici one will only generate Voici dashboards, excluding the full JupyterLab interface from the output. Running `voici build --contents .` is equivalent to running `jupyter lite build --contents . --apps voici`.
+
 You can generate the classic `jupyter lite` output alongside your dashboards by specifying the additional apps you want:
 
 ```bash
-voici build --apps lab --apps retro
+voici build --contents . --apps lab --apps retro
 ```
 
 In order to get some help on how to use the `voici` command, you can run:
 
 ```bash
 voici --help
 ```
 
 We'd also suggest looking into the [JupyterLite documentation](https://jupyterlite.readthedocs.io/en/latest/howto/index.html) for more insights on how to configure your `voici` deployment.
 
-### Build the demo site yourself
+## Build the demo site yourself
 
 Before you can build the demo site from this repository, you will need to install [jupyterlite-xeus-python](https://github.com/jupyterlite/xeus-python-kernel):
 
 ```bash
 pip install jupyterlite-xeus-python
 ```
```


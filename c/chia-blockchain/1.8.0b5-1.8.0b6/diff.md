# Comparing `tmp/chia-blockchain-1.8.0b5.tar.gz` & `tmp/chia-blockchain-1.8.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chia-blockchain-1.8.0b5.tar", last modified: Fri Apr  7 22:42:50 2023, max compression
+gzip compressed data, was "chia-blockchain-1.8.0b6.tar", last modified: Mon Apr 17 22:35:09 2023, max compression
```

## Comparing `chia-blockchain-1.8.0b5.tar` & `chia-blockchain-1.8.0b6.tar`

### file list

```diff
@@ -1,1102 +1,1105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.707946 chia-blockchain-1.8.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.587937 chia-blockchain-1.8.0b5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.587937 chia-blockchain-1.8.0b5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.575937 chia-blockchain-1.8.0b5/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.587937 chia-blockchain-1.8.0b5/.github/actions/install/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/actions/install/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.591938 chia-blockchain-1.8.0b5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/build-linux-arm64-installer.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/build-linux-installer-deb.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/build-linux-installer-rpm.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/build-macos-installers.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/build-windows-installer.yml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/check-commit-signing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/check_wheel_availability.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/conflict-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/mozilla-ca-cert.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/require-labels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/snyk-python-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/stale-issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/start-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/start-sync-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/super-linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/test-install-scripts.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/test-single.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/trigger-docker-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/trigger-docker-main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.github/workflows/upload-pypi-source.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.markdown-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/BUILD_TIMELORD.md
--rw-r--r--   0 runner    (1001) docker     (123)   207286 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/Install-gui.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/Install-plotter.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/Install.ps1
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-07 22:42:50.707946 chia-blockchain-1.8.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33099 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/PRETTY_GOOD_PRACTICES.md
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/activated.ps1
--rwxr-xr-x   0 runner    (1001) docker     (123)      630 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/activated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      155 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/activated.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.595938 chia-blockchain-1.8.0b5/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/benchmarks/block_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/benchmarks/block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)   121543 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/benchmarks/clvm_generator.bin
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/benchmarks/coin_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/benchmarks/jsonify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/benchmarks/mempool-long-lived.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/benchmarks/mempool.py
--rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/benchmarks/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)   439288 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/benchmarks/transaction_height_delta
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.595938 chia-blockchain-1.8.0b5/build_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.595938 chia-blockchain-1.8.0b5/build_scripts/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.595938 chia-blockchain-1.8.0b5/build_scripts/assets/deb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/assets/deb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/assets/deb/control.j2
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/assets/deb/postinst.sh
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/assets/deb/prerm.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.595938 chia-blockchain-1.8.0b5/build_scripts/assets/dmg/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/assets/dmg/README
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/assets/dmg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   507222 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/assets/dmg/background.tiff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.595938 chia-blockchain-1.8.0b5/build_scripts/assets/rpm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/assets/rpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/assets/rpm/postinst.sh
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/assets/rpm/prerm.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/build_linux_deb-1-gui.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/build_linux_deb-2-installer.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/build_linux_rpm-1-gui.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/build_linux_rpm-2-installer.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/build_macos-1-gui.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/build_macos-2-installer.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/build_windows-1-gui.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/build_windows-2-installer.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/check_dependency_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/clean-runner.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/installer-version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.595938 chia-blockchain-1.8.0b5/build_scripts/npm_global/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/npm_global/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/npm_global/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/npm_global/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.599938 chia-blockchain-1.8.0b5/build_scripts/npm_linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/npm_linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   539731 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/npm_linux/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/npm_linux/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.599938 chia-blockchain-1.8.0b5/build_scripts/npm_macos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/npm_macos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   572329 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/npm_macos/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/npm_macos/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.599938 chia-blockchain-1.8.0b5/build_scripts/npm_windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/npm_windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   553007 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/npm_windows/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/build_scripts/npm_windows/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.599938 chia-blockchain-1.8.0b5/chia/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.599938 chia-blockchain-1.8.0b5/chia/clvm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/clvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/clvm/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    18468 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/clvm/spend_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.603938 chia-blockchain-1.8.0b5/chia/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/beta_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16346 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/check_wallet_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/chia.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/cmds_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/coin_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/coins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/data_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/db_backup_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    17725 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/db_upgrade_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/db_validate_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/farm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/farm_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/init_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    26855 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/keys_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/netspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/netspace_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/passphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/passphrase_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/peer_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/plotnft.py
--rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/plotnft_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/show_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/start_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    38959 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)    49571 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/cmds/wallet_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.607939 chia-blockchain-1.8.0b5/chia/consensus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/block_body_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21437 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/block_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)    51022 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/block_header_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/block_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/block_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/block_root_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    42752 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/blockchain_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/coinbase.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/condition_costs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/cost_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/default_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18266 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/difficulty_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/find_fork_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/full_block_to_block_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/get_block_challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/make_sub_epoch_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    18835 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/multiprocess_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/pos_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/pot_iterations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/consensus/vdf_info_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.607939 chia-blockchain-1.8.0b5/chia/daemon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/daemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/daemon/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/daemon/keychain_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/daemon/keychain_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    56085 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/daemon/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/daemon/windows_signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.611939 chia-blockchain-1.8.0b5/chia/data_layer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/data_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35381 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/data_layer/data_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/data_layer/data_layer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/data_layer/data_layer_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/data_layer/data_layer_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/data_layer/data_layer_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    62659 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/data_layer/data_layer_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)    62999 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/data_layer/data_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/data_layer/dl_wallet_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/data_layer/download_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.611939 chia-blockchain-1.8.0b5/chia/data_layer/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/data_layer/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/data_layer/util/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.611939 chia-blockchain-1.8.0b5/chia/farmer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/farmer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36458 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/farmer/farmer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28233 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/farmer/farmer_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.615939 chia-blockchain-1.8.0b5/chia/full_node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/bitcoin_fee_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/block_height_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    32512 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/bundle_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    24796 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/coin_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/fee_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/fee_estimate_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/fee_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/fee_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/fee_estimator_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/fee_estimator_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/fee_estimator_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/fee_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    22559 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/fee_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)   130034 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/full_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    79149 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/full_node_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36689 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/full_node_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/hint_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/hint_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/lock_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/mempool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/mempool_check_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33407 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/mempool_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/pending_tx_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/signage_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/sync_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/tx_processing_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    72530 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/full_node/weight_proof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.615939 chia-blockchain-1.8.0b5/chia/harvester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/harvester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/harvester/harvester.py
--rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/harvester/harvester_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.615939 chia-blockchain-1.8.0b5/chia/introducer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/introducer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/introducer/introducer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/introducer/introducer_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.615939 chia-blockchain-1.8.0b5/chia/plot_sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plot_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plot_sync/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plot_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plot_sync/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plot_sync/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plot_sync/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.615939 chia-blockchain-1.8.0b5/chia/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plotters/bladebit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plotters/chiapos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plotters/madmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plotters/plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plotters/plotters_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.615939 chia-blockchain-1.8.0b5/chia/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plotting/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plotting/check_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10542 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plotting/create_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plotting/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/plotting/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.619940 chia-blockchain-1.8.0b5/chia/pools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/pools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/pools/pool_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17113 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/pools/pool_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)    44516 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/pools/pool_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/pools/pool_wallet_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.619940 chia-blockchain-1.8.0b5/chia/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/protocols/farmer_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/protocols/full_node_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/protocols/harvester_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/protocols/introducer_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/protocols/pool_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/protocols/protocol_message_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/protocols/protocol_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/protocols/protocol_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/protocols/shared_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/protocols/timelord_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/protocols/wallet_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/pyinstaller.spec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.623940 chia-blockchain-1.8.0b5/chia/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/crawler_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18161 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/data_layer_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/data_layer_rpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/data_layer_rpc_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13582 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/farmer_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/farmer_rpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41276 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/full_node_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/full_node_rpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/harvester_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/harvester_rpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/rpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/timelord_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/util.py
--rw-r--r--   0 runner    (1001) docker     (123)   160896 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/wallet_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    44813 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/rpc/wallet_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.623940 chia-blockchain-1.8.0b5/chia/seeder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/seeder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/seeder/crawl_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/seeder/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/seeder/crawler_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/seeder/dns_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/seeder/peer_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/seeder/start_crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.627940 chia-blockchain-1.8.0b5/chia/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27079 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/address_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/address_manager_sqlite_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/address_manager_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/chia_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/introducer_peers.py
--rw-r--r--   0 runner    (1001) docker     (123)    33197 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/node_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/outbound_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/peer_store_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/rate_limit_numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/rate_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/reconnect_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    30238 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/ssl_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/start_data_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/start_farmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/start_full_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/start_harvester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/start_introducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/start_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/start_timelord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/start_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/upnp.py
--rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/server/ws_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.627940 chia-blockchain-1.8.0b5/chia/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95653 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/block_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    28844 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/full_node_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)    17163 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/setup_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15060 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/setup_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/simulator_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/simulator_full_node_rpc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/simulator_full_node_rpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/simulator_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/simulator_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/ssl_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    39473 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_10.py
--rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    39471 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_3.py
--rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_4.py
--rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_5.py
--rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_6.py
--rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_7.py
--rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_8.py
--rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_9.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/start_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/time_out_assert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/simulator/wallet_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.631940 chia-blockchain-1.8.0b5/chia/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/ssl/chia_ca.crt
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/ssl/chia_ca.key
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/ssl/create_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/ssl/dst_root_ca.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.631940 chia-blockchain-1.8.0b5/chia/timelord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/timelord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/timelord/iters_from_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    58703 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/timelord/timelord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/timelord/timelord_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/timelord/timelord_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/timelord/timelord_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/timelord/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.635941 chia-blockchain-1.8.0b5/chia/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/block_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.635941 chia-blockchain-1.8.0b5/chia/types/blockchain_format/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/classgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/foliage.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/pool_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/proof_of_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/reward_chain_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/serialized_program.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/sized_bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/slots.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/sub_epoch_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/tree_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/blockchain_format/vdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/clvm_cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/coin_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/coin_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/coin_spend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/condition_opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/condition_with_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/end_of_slot_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/fee_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/full_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/generator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/header_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/mempool_inclusion_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/mempool_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/mempool_submission_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/mojos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/peer_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/signing_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/spend_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/spend_bundle_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/transaction_queue_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/unfinished_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/unfinished_header_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/types/weight_proof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.643941 chia-blockchain-1.8.0b5/chia/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/api_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/bech32m.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/beta_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/block_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/byte_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/cached_bls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/check_fork_next_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/chia_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/condition_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/create_alert_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/db_synchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/db_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/db_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/default_root.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2866 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/dump_keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/english.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/file_keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/full_block_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/generator_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    24217 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/initial-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/inline_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/ints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    22165 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/keyring_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/limited_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/log_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/make_test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/merkle_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/partial_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/prev_transaction_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/recursive_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/safe_cancel_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/setproctitle.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/significant_bits.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/ssl_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/struct_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/task_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/validate_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/vdf_prover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/util/ws_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.647942 chia-blockchain-1.8.0b5/chia/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/block_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.647942 chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/cat_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/cat_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/cat_outer_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/cat_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    43047 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/cat_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/lineage_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/chialisp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/coin_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.647942 chia-blockchain-1.8.0b5/chia/wallet/dao_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/dao_wallet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.647942 chia-blockchain-1.8.0b5/chia/wallet/db_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/db_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/db_wallet/db_wallet_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/derivation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/derive_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.647942 chia-blockchain-1.8.0b5/chia/wallet/did_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/did_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/did_wallet/did_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    63627 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/did_wallet/did_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/did_wallet/did_wallet_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/driver_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/key_val_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/lineage_proof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.651942 chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/metadata_outer_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/nft_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/nft_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)    85099 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/nft_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/ownership_outer_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/singleton_outer_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/transfer_program_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/uncurry_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/notification_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/notification_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/outer_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzle_drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.667943 chia-blockchain-1.8.0b5/chia/wallet/puzzles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/block_program_zero.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/block_program_zero.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/block_program_zero.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/calculate_synthetic_public_key.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/calculate_synthetic_public_key.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/calculate_synthetic_public_key.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/cat_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/cat_truths.clib
--rw-r--r--   0 runner    (1001) docker     (123)    17221 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/cat_v2.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/cat_v2.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/cat_v2.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/chialisp_deserialisation.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/chialisp_deserialisation.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/chialisp_deserialisation.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/condition_codes.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/create-lock-puzzlehash.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/create_nft_launcher_from_did.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/create_nft_launcher_from_did.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/create_nft_launcher_from_did.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/curry-and-treehash.clinc
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/curry.clib
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/decompress_coin_spend_entry.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/decompress_coin_spend_entry.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/decompress_coin_spend_entry.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/decompress_puzzle.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/decompress_puzzle.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/decompress_puzzle.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/delegated_tail.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/delegated_tail.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/delegated_tail.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/did_innerpuz.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/did_innerpuz.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/did_innerpuz.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/everything_with_signature.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/everything_with_signature.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/everything_with_signature.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/genesis_by_coin_id.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/genesis_by_coin_id.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/genesis_by_coin_id.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/genesis_by_puzzle_hash.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/genesis_by_puzzle_hash.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/genesis_by_puzzle_hash.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/graftroot_dl_offers.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/graftroot_dl_offers.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/graftroot_dl_offers.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/json.clib
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/load_clvm.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/lock.inner.puzzle.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/lock.inner.puzzle.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/lock.inner.puzzle.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/merkle_utils.clib
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_intermediate_launcher.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_intermediate_launcher.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_intermediate_launcher.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_metadata_updater_default.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_metadata_updater_default.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_metadata_updater_default.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_metadata_updater_updateable.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_metadata_updater_updateable.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_metadata_updater_updateable.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_ownership_layer.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_ownership_layer.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_ownership_layer.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_state_layer.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_state_layer.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_state_layer.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/notification.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/notification.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/notification.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_conditions.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_conditions.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_conditions.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_conditions.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_conditions.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_conditions.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_puzzle.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_puzzle.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_puzzle.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_m_of_n_delegate_direct.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_parent.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_parent.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_parent.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_puzzle_hash.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_puzzle_hash.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_puzzle_hash.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_puzzle_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_singleton.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_singleton.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_singleton.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/pool_member_innerpuz.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/pool_member_innerpuz.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/pool_member_innerpuz.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm.hex.sha256tree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.667943 chia-blockchain-1.8.0b5/chia/wallet/puzzles/prefarm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/prefarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/prefarm/make_prefarm_ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/prefarm/spend_prefarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/puzzle_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/recompile-all.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/rom_bootstrap_generator.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/rom_bootstrap_generator.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/rom_bootstrap_generator.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/rom_bootstrap_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/settlement_payments.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/settlement_payments.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/settlement_payments.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/settlement_payments_old.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/settlement_payments_old.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/settlement_payments_old.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/sha256tree.clib
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/sha256tree_module.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/sha256tree_module.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/sha256tree_module.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_launcher.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_launcher.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_launcher.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_truths.clib
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/tails.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/test_generator_deserialize.clvm
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/test_generator_deserialize.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/test_generator_deserialize.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm.hex
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm.hex.sha256tree
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/puzzles/utility_macros.clib
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/secret_key_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/sign_coin_spends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    43023 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/trade_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/trade_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.667943 chia-blockchain-1.8.0b5/chia/wallet/trading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/trading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32738 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/trading/offer.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/trading/trade_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/trading/trade_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/transaction_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/transaction_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/uncurried_puzzle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.671943 chia-blockchain-1.8.0b5/chia/wallet/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/address_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/compute_hints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/compute_memos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/curry_and_treehash.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/debug_spend_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/json_clvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/merkle_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/merkle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/new_peak_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/peer_request_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/puzzle_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/transaction_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    16079 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/wallet_sync_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/util/wallet_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    29129 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_coin_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_coin_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_interested_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_nft_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    81101 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_node_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_pool_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    13735 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_puzzle_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_retry_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    86490 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_state_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_transaction_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_user_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/chia/wallet/wallet_weight_proof_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.671943 chia-blockchain-1.8.0b5/chia_blockchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-07 22:42:50.000000 chia-blockchain-1.8.0b5/chia_blockchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34783 2023-04-07 22:42:50.000000 chia-blockchain-1.8.0b5/chia_blockchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:42:50.000000 chia-blockchain-1.8.0b5/chia_blockchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-07 22:42:50.000000 chia-blockchain-1.8.0b5/chia_blockchain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:38:11.000000 chia-blockchain-1.8.0b5/chia_blockchain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-07 22:42:50.000000 chia-blockchain-1.8.0b5/chia_blockchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-07 22:42:50.000000 chia-blockchain-1.8.0b5/chia_blockchain.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     6676 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/install-gui.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4910 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/install-plotter.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/install-timelord.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)    12552 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/install.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/installhelper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.671943 chia-blockchain-1.8.0b5/mozilla-ca/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:51.000000 chia-blockchain-1.8.0b5/mozilla-ca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   216583 2023-04-07 22:37:51.000000 chia-blockchain-1.8.0b5/mozilla-ca/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/pytest.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/run-py-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 22:42:50.707946 chia-blockchain-1.8.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/start-gui.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.671943 chia-blockchain-1.8.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.671943 chia-blockchain-1.8.0b5/tests/blockchain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/blockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/blockchain/blockchain_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/blockchain/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   166834 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/blockchain/test_blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    37640 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/blockchain/test_blockchain_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2431 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/build-init-files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/build-job-matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/check_pytest_monitor_output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2398 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/check_sql_statements.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1750 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/chia-start-sim
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.675943 chia-blockchain-1.8.0b5/tests/clvm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/benchmark_costs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/coin_store.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/test_chialisp_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/test_clvm_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/test_curry_and_treehash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/test_puzzle_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/test_puzzle_drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/test_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/test_serialized_program.py
--rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/test_singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/clvm/test_spend_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.675943 chia-blockchain-1.8.0b5/tests/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/cmds/test_wallet_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    28614 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/connection_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.675943 chia-blockchain-1.8.0b5/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.679944 chia-blockchain-1.8.0b5/tests/core/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/cmds/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13587 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/cmds/test_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)    38994 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/cmds/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/cmds/test_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.679944 chia-blockchain-1.8.0b5/tests/core/consensus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/consensus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/consensus/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/consensus/test_pot_iterations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.679944 chia-blockchain-1.8.0b5/tests/core/custom_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/custom_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/custom_types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/custom_types/test_coin.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/custom_types/test_proof_of_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/custom_types/test_spend_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.679944 chia-blockchain-1.8.0b5/tests/core/daemon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/daemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/daemon/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/daemon/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/daemon/test_daemon_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/daemon/test_keychain_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.679944 chia-blockchain-1.8.0b5/tests/core/data_layer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/data_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/data_layer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/data_layer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/data_layer/test_data_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/data_layer/test_data_layer_util.py
--rw-r--r--   0 runner    (1001) docker     (123)   245320 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/data_layer/test_data_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    47306 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/data_layer/test_data_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/data_layer/test_data_store_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/data_layer/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.683944 chia-blockchain-1.8.0b5/tests/core/full_node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.683944 chia-blockchain-1.8.0b5/tests/core/full_node/dos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/dos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/dos/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.683944 chia-blockchain-1.8.0b5/tests/core/full_node/full_sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/full_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/full_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19025 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/full_sync/test_full_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/ram_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.683944 chia-blockchain-1.8.0b5/tests/core/full_node/stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/stores/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/stores/test_block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21322 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/stores/test_coin_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    34130 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/stores/test_full_node_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/stores/test_hint_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/stores/test_sync_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    23835 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/test_address_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16506 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/test_block_height_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    13828 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/test_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    87563 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/test_full_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/test_generator_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/test_hint_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/test_node_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/test_peer_store_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/test_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/full_node/test_tx_processing_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)   187863 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/large_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/make_block_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.683944 chia-blockchain-1.8.0b5/tests/core/mempool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/mempool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/mempool/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   121724 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/mempool/test_mempool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/mempool/test_mempool_fee_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/mempool/test_mempool_fee_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    51432 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/mempool/test_mempool_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/mempool/test_mempool_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/node_height.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.687944 chia-blockchain-1.8.0b5/tests/core/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/server/flood.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/server/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/server/test_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/server/test_dos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/server/test_event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/server/test_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/server/test_rate_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/server/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/server/test_upnp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.687944 chia-blockchain-1.8.0b5/tests/core/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/ssl/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/ssl/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/test_coins.py
--rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/test_cost_calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/test_crawler_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/test_daemon_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/test_db_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/test_db_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23550 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/test_farmer_harvester_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/test_full_node_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/test_merkle_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/test_setproctitle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.687944 chia-blockchain-1.8.0b5/tests/core/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/test_cached_bls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/test_file_keyring_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/test_jsonify.py
--rw-r--r--   0 runner    (1001) docker     (123)    20681 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/test_keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)    22952 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/test_keyring_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/test_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/test_significant_bits.py
--rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/core/util/test_streamable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.687944 chia-blockchain-1.8.0b5/tests/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/db/test_db_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.687944 chia-blockchain-1.8.0b5/tests/farmer_harvester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/farmer_harvester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/farmer_harvester/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/farmer_harvester/test_farmer_harvester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.687944 chia-blockchain-1.8.0b5/tests/fee_estimation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/fee_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/fee_estimation/cmdline_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/fee_estimation/test_fee_estimation_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/fee_estimation/test_fee_estimation_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/fee_estimation/test_fee_estimation_unit_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/fee_estimation/test_mempoolitem_height_added.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.691945 chia-blockchain-1.8.0b5/tests/generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/generator/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/generator/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/generator/test_generator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/generator/test_list_to_batches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/generator/test_rom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/generator/test_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.691945 chia-blockchain-1.8.0b5/tests/plot_sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/plot_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/plot_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/plot_sync/test_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)    29318 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/plot_sync/test_plot_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    17895 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/plot_sync/test_receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/plot_sync/test_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)    18095 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/plot_sync/test_sync_simulated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/plot_sync/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.691945 chia-blockchain-1.8.0b5/tests/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/plotting/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    32802 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/plotting/test_plot_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/plotting/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.691945 chia-blockchain-1.8.0b5/tests/pools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/pools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/pools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/pools/test_pool_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/pools/test_pool_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/pools/test_pool_puzzles_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    47263 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/pools/test_pool_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/pools/test_pool_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/pools/test_wallet_pool_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.691945 chia-blockchain-1.8.0b5/tests/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/simulation/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/simulation/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10038 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/simulation/test_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/simulation/test_start_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/testconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.695945 chia-blockchain-1.8.0b5/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/tools/1315537.json
--rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/tools/1315544.json
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/tools/1315630.json
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/tools/300000.json
--rw-r--r--   0 runner    (1001) docker     (123)    17387 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/tools/442734.json
--rw-r--r--   0 runner    (1001) docker     (123)   233251 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/tools/466212.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   405504 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/tools/test-blockchain-db.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/tools/test_full_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/tools/test_legacy_keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/tools/test_run_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.699945 chia-blockchain-1.8.0b5/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/alert_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/benchmark_cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/bip39_test_vectors.json
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/build_network_protocol_files.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/db_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/gen_ssl_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/generator_tools_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/key_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31159 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/network_protocol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    46740 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/protocol_messages_bytes-v1.0
--rw-r--r--   0 runner    (1001) docker     (123)   170660 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/protocol_messages_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/temp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_full_block_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_limited_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_lock_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    22379 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_network_protocol_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_network_protocol_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_network_protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/util/test_struct_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.703945 chia-blockchain-1.8.0b5/tests/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.703945 chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25164 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/test_cat_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/test_cat_outer_puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39540 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/test_cat_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/test_offer_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)   162923 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/test_trades.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.703945 chia-blockchain-1.8.0b5/tests/wallet/dao_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/dao_wallet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.703945 chia-blockchain-1.8.0b5/tests/wallet/db_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/db_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/db_wallet/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/db_wallet/test_db_graftroot.py
--rw-r--r--   0 runner    (1001) docker     (123)   135852 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/db_wallet/test_dl_offers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26485 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/db_wallet/test_dl_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.703945 chia-blockchain-1.8.0b5/tests/wallet/did_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/did_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/did_wallet/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    65879 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/did_wallet/test_did.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.703945 chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   374078 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_nft_1_offers.py
--rw-r--r--   0 runner    (1001) docker     (123)    43345 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_nft_bulk_mint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_nft_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    66774 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_nft_offers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_nft_puzzles.py
--rw-r--r--   0 runner    (1001) docker     (123)    76327 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_nft_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_ownership_outer_puzzle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.707946 chia-blockchain-1.8.0b5/tests/wallet/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/rpc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/rpc/test_dl_wallet_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    74646 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/rpc/test_wallet_rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.707946 chia-blockchain-1.8.0b5/tests/wallet/simple_sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/simple_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/simple_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/simple_sync/test_simple_sync_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.707946 chia-blockchain-1.8.0b5/tests/wallet/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    65523 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/sync/test_wallet_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_address_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_bech32m.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_chialisp.py
--rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_coin_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_nft_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_offer_parsing_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_puzzle_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_singleton_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_singleton_lifecycle_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_taproot.py
--rw-r--r--   0 runner    (1001) docker     (123)    27395 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_transaction_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    43806 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_wallet_blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_wallet_coin_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_wallet_interested_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_wallet_key_val_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_wallet_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_wallet_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_wallet_state_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_wallet_trade_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/wallet/test_wallet_user_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.707946 chia-blockchain-1.8.0b5/tests/weight_proof/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/weight_proof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/weight_proof/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tests/weight_proof/test_weight_proof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:42:50.707946 chia-blockchain-1.8.0b5/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tools/analyze-chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tools/analyze_memory_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tools/cpu_utilization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tools/generate_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tools/legacy_keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tools/manage_clvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tools/plot-log.gnuplot
--rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tools/run_benchmark.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tools/run_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tools/test_constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13441 2023-04-07 22:37:43.000000 chia-blockchain-1.8.0b5/tools/test_full_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.356978 chia-blockchain-1.8.0b6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.356978 chia-blockchain-1.8.0b6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.344978 chia-blockchain-1.8.0b6/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.356978 chia-blockchain-1.8.0b6/.github/actions/install/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/actions/install/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.360978 chia-blockchain-1.8.0b6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/build-linux-arm64-installer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/build-linux-installer-deb.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/build-linux-installer-rpm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/build-macos-installers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/build-windows-installer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/check-commit-signing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/check_wheel_availability.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/conflict-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/mozilla-ca-cert.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/require-labels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/snyk-python-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/stale-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/start-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/start-sync-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/super-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/test-install-scripts.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/test-single.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/trigger-docker-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/trigger-docker-main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.github/workflows/upload-pypi-source.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.markdown-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/BUILD_TIMELORD.md
+-rw-r--r--   0 runner    (1001) docker     (123)   207286 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/Install-gui.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/Install-plotter.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/Install.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33099 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/PRETTY_GOOD_PRACTICES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/activated.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (123)      630 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/activated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      155 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/activated.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.360978 chia-blockchain-1.8.0b6/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/block_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121543 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/clvm_generator.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/coin_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/jsonify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/mempool-long-lived.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/mempool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)   439288 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/transaction_height_delta
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.360978 chia-blockchain-1.8.0b6/build_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.360978 chia-blockchain-1.8.0b6/build_scripts/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.360978 chia-blockchain-1.8.0b6/build_scripts/assets/deb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/deb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/deb/control.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/deb/postinst.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/deb/prerm.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.364978 chia-blockchain-1.8.0b6/build_scripts/assets/dmg/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/dmg/README
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/dmg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   507222 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/dmg/background.tiff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.364978 chia-blockchain-1.8.0b6/build_scripts/assets/rpm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/rpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/rpm/postinst.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/assets/rpm/prerm.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_linux_deb-1-gui.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_linux_deb-2-installer.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_linux_rpm-1-gui.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_linux_rpm-2-installer.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_macos-1-gui.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_macos-2-installer.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_windows-1-gui.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/build_windows-2-installer.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/check_dependency_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/clean-runner.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/installer-version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.364978 chia-blockchain-1.8.0b6/build_scripts/npm_global/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_global/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_global/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_global/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.364978 chia-blockchain-1.8.0b6/build_scripts/npm_linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539731 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_linux/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_linux/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.364978 chia-blockchain-1.8.0b6/build_scripts/npm_macos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_macos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   572329 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_macos/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_macos/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.364978 chia-blockchain-1.8.0b6/build_scripts/npm_windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   553007 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_windows/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/build_scripts/npm_windows/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.368978 chia-blockchain-1.8.0b6/chia/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.368978 chia-blockchain-1.8.0b6/chia/clvm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/clvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/clvm/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/clvm/spend_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.372978 chia-blockchain-1.8.0b6/chia/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/beta_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16346 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/check_wallet_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/chia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/cmds_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/coin_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/coins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/data_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/db_backup_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17725 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/db_upgrade_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/db_validate_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/farm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/farm_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/init_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26855 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/keys_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/netspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/netspace_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/passphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/passphrase_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/peer_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/plotnft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/plotnft_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/show_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/start_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38959 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49571 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/cmds/wallet_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.376978 chia-blockchain-1.8.0b6/chia/consensus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/block_body_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21437 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/block_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51022 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/block_header_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/block_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/block_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/block_root_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42752 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/blockchain_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/condition_costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/cost_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/default_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18266 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/difficulty_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/find_fork_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/full_block_to_block_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/get_block_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/make_sub_epoch_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18835 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/multiprocess_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/pos_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/pot_iterations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/consensus/vdf_info_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.376978 chia-blockchain-1.8.0b6/chia/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/daemon/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/daemon/keychain_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/daemon/keychain_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56085 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/daemon/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/daemon/windows_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.376978 chia-blockchain-1.8.0b6/chia/data_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38872 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_layer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_layer_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_layer_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_layer_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62659 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_layer_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62999 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/dl_wallet_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/s3_plugin_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/s3_plugin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.376978 chia-blockchain-1.8.0b6/chia/data_layer/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/data_layer/util/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.376978 chia-blockchain-1.8.0b6/chia/farmer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/farmer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36468 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/farmer/farmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28233 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/farmer/farmer_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.380978 chia-blockchain-1.8.0b6/chia/full_node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/bitcoin_fee_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/block_height_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32512 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/bundle_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24796 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/coin_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimate_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimator_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimator_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_estimator_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22559 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/fee_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130083 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/full_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79298 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/full_node_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36689 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/full_node_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/hint_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/hint_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/lock_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/mempool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/mempool_check_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33485 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/mempool_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/pending_tx_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/signage_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/sync_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/tx_processing_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72530 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/full_node/weight_proof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.380978 chia-blockchain-1.8.0b6/chia/harvester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/harvester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/harvester/harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/harvester/harvester_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.380978 chia-blockchain-1.8.0b6/chia/introducer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/introducer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/introducer/introducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/introducer/introducer_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.384978 chia-blockchain-1.8.0b6/chia/plot_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plot_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plot_sync/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plot_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plot_sync/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plot_sync/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plot_sync/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.384978 chia-blockchain-1.8.0b6/chia/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotters/bladebit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotters/chiapos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotters/madmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotters/plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotters/plotters_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.384978 chia-blockchain-1.8.0b6/chia/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotting/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotting/check_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10542 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotting/create_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotting/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/plotting/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.384978 chia-blockchain-1.8.0b6/chia/pools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/pools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/pools/pool_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17113 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/pools/pool_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44516 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/pools/pool_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/pools/pool_wallet_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.384978 chia-blockchain-1.8.0b6/chia/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/farmer_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/full_node_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/harvester_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/introducer_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/pool_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/protocol_message_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/protocol_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/protocol_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/shared_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/timelord_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/protocols/wallet_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/pyinstaller.spec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.388978 chia-blockchain-1.8.0b6/chia/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/crawler_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18161 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/data_layer_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/data_layer_rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/data_layer_rpc_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13582 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/farmer_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/farmer_rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41327 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/full_node_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/full_node_rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/harvester_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/harvester_rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/timelord_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160950 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/wallet_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44813 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/rpc/wallet_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.388978 chia-blockchain-1.8.0b6/chia/seeder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/crawl_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/crawler_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/dns_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/peer_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/seeder/start_crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.392978 chia-blockchain-1.8.0b6/chia/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27079 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/address_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/address_manager_sqlite_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/address_manager_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/chia_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/introducer_peers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33202 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/node_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/outbound_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/peer_store_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/rate_limit_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/rate_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30966 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/ssl_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_data_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_farmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_full_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_introducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_timelord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/start_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/upnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30397 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/server/ws_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.396978 chia-blockchain-1.8.0b6/chia/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95653 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/block_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28844 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/full_node_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/setup_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/setup_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/simulator_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/simulator_full_node_rpc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/simulator_full_node_rpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/simulator_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/simulator_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39473 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39471 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39479 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/start_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/time_out_assert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/simulator/wallet_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.396978 chia-blockchain-1.8.0b6/chia/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/ssl/chia_ca.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/ssl/chia_ca.key
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/ssl/create_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/ssl/dst_root_ca.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.396978 chia-blockchain-1.8.0b6/chia/timelord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/iters_from_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58402 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/timelord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/timelord_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/timelord_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/timelord_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/timelord/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.400978 chia-blockchain-1.8.0b6/chia/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/block_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.400978 chia-blockchain-1.8.0b6/chia/types/blockchain_format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/classgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/foliage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/pool_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/proof_of_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/reward_chain_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/serialized_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/sized_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/sub_epoch_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/tree_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/blockchain_format/vdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/clvm_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/coin_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/coin_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/coin_spend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/condition_opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/condition_with_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/end_of_slot_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/fee_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/full_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/generator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/header_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/mempool_inclusion_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/mempool_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/mempool_submission_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/mojos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/peer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/signing_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/spend_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/spend_bundle_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/transaction_queue_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/unfinished_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/unfinished_header_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/types/weight_proof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.408978 chia-blockchain-1.8.0b6/chia/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/api_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/bech32m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/beta_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/block_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/byte_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/cached_bls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/check_fork_next_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/chia_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/condition_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/create_alert_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/db_synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/db_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/db_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/default_root.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2866 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/dump_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/english.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/file_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/full_block_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/generator_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24198 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/initial-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/inline_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/ints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/keyring_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/limited_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/log_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/make_test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/merkle_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/partial_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/prev_transaction_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/recursive_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/safe_cancel_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/setproctitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/significant_bits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/ssl_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/struct_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/task_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/validate_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/vdf_prover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/util/ws_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.412978 chia-blockchain-1.8.0b6/chia/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/block_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.412978 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_outer_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42955 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/lineage_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/chialisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/coin_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.412978 chia-blockchain-1.8.0b6/chia/wallet/dao_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/dao_wallet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.412978 chia-blockchain-1.8.0b6/chia/wallet/db_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/db_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/db_wallet/db_wallet_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/derivation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/derive_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.416978 chia-blockchain-1.8.0b6/chia/wallet/did_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/did_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/did_wallet/did_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62287 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/did_wallet/did_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/did_wallet/did_wallet_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/driver_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/key_val_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/lineage_proof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.416978 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/metadata_outer_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/nft_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/nft_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83964 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/nft_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/ownership_outer_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/singleton_outer_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/transfer_program_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/uncurry_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/notification_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/notification_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/outer_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzle_drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.432978 chia-blockchain-1.8.0b6/chia/wallet/puzzles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/block_program_zero.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/block_program_zero.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/block_program_zero.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/calculate_synthetic_public_key.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/calculate_synthetic_public_key.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/calculate_synthetic_public_key.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_truths.clib
+-rw-r--r--   0 runner    (1001) docker     (123)    17221 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_v2.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_v2.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_v2.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/chialisp_deserialisation.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/chialisp_deserialisation.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/chialisp_deserialisation.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/condition_codes.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/create-lock-puzzlehash.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/create_nft_launcher_from_did.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/create_nft_launcher_from_did.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/create_nft_launcher_from_did.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/curry-and-treehash.clinc
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/curry.clib
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_coin_spend_entry.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_coin_spend_entry.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_coin_spend_entry.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_coin_spend_entry_with_prefix.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_puzzle.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_puzzle.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/decompress_puzzle.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/delegated_tail.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/delegated_tail.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/delegated_tail.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/did_innerpuz.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/did_innerpuz.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/did_innerpuz.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/everything_with_signature.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/everything_with_signature.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/everything_with_signature.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_coin_id.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_coin_id.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_coin_id.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_puzzle_hash.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_puzzle_hash.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_puzzle_hash.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/graftroot_dl_offers.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/graftroot_dl_offers.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/graftroot_dl_offers.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/json.clib
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/load_clvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/lock.inner.puzzle.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/lock.inner.puzzle.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/lock.inner.puzzle.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/merkle_utils.clib
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_intermediate_launcher.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_intermediate_launcher.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_intermediate_launcher.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_default.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_default.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_default.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_updateable.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_updateable.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_updateable.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_layer.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_layer.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_layer.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_state_layer.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_state_layer.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_state_layer.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/notification.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/notification.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/notification.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_conditions.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_conditions.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_conditions.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_conditions.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_conditions.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_conditions.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_parent.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_parent.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_parent.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_puzzle_hash.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_puzzle_hash.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_puzzle_hash.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_puzzle_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_member_innerpuz.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_member_innerpuz.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_member_innerpuz.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm.hex.sha256tree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.432978 chia-blockchain-1.8.0b6/chia/wallet/puzzles/prefarm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/prefarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/prefarm/make_prefarm_ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/prefarm/spend_prefarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/puzzle_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/recompile-all.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/rom_bootstrap_generator.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/rom_bootstrap_generator.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/rom_bootstrap_generator.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/rom_bootstrap_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments_old.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments_old.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments_old.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/sha256tree.clib
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/sha256tree_module.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/sha256tree_module.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/sha256tree_module.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_launcher.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_launcher.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_launcher.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_truths.clib
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/tails.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_generator_deserialize.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_generator_deserialize.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_generator_deserialize.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm.hex
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm.hex.sha256tree
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/puzzles/utility_macros.clib
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/secret_key_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/sign_coin_spends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43570 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/trade_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/trade_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.432978 chia-blockchain-1.8.0b6/chia/wallet/trading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/trading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32738 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/trading/offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/trading/trade_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/trading/trade_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/transaction_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/transaction_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/uncurried_puzzle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.436977 chia-blockchain-1.8.0b6/chia/wallet/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/address_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/compute_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/compute_memos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/curry_and_treehash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/debug_spend_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/json_clvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/merkle_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/merkle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/new_peak_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/peer_request_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/puzzle_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/transaction_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/wallet_sync_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/util/wallet_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27732 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_coin_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_coin_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_interested_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_nft_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80370 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_node_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_pool_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13735 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_puzzle_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_retry_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86139 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_transaction_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_user_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/chia/wallet/wallet_weight_proof_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.436977 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-17 22:35:09.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34876 2023-04-17 22:35:09.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:35:09.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-17 22:35:09.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:30:52.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-17 22:35:09.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-17 22:35:09.000000 chia-blockchain-1.8.0b6/chia_blockchain.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6676 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/install-gui.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4910 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/install-plotter.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/install-timelord.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12552 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/installhelper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.436977 chia-blockchain-1.8.0b6/mozilla-ca/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:31.000000 chia-blockchain-1.8.0b6/mozilla-ca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   216583 2023-04-17 22:30:31.000000 chia-blockchain-1.8.0b6/mozilla-ca/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/pytest.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/run-py-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/start-gui.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.436977 chia-blockchain-1.8.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.440977 chia-blockchain-1.8.0b6/tests/blockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/blockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/blockchain/blockchain_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/blockchain/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166834 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/blockchain/test_blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37614 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/blockchain/test_blockchain_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2431 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/build-init-files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/build-job-matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/check_pytest_monitor_output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2398 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/check_sql_statements.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1750 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/chia-start-sim
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.440977 chia-blockchain-1.8.0b6/tests/clvm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/benchmark_costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/coin_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_chialisp_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_clvm_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_curry_and_treehash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_puzzle_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_puzzle_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_serialized_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/clvm/test_spend_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.440977 chia-blockchain-1.8.0b6/tests/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/cmds/test_wallet_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28614 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/connection_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.444977 chia-blockchain-1.8.0b6/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.444977 chia-blockchain-1.8.0b6/tests/core/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/cmds/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13587 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/cmds/test_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38994 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/cmds/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/cmds/test_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.444977 chia-blockchain-1.8.0b6/tests/core/consensus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/consensus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/consensus/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/consensus/test_pot_iterations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.444977 chia-blockchain-1.8.0b6/tests/core/custom_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/custom_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/custom_types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/custom_types/test_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/custom_types/test_proof_of_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/custom_types/test_spend_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.444977 chia-blockchain-1.8.0b6/tests/core/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/daemon/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/daemon/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/daemon/test_daemon_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/daemon/test_keychain_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.444977 chia-blockchain-1.8.0b6/tests/core/data_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_layer_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245364 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47306 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_store_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/data_layer/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.448977 chia-blockchain-1.8.0b6/tests/core/full_node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.448977 chia-blockchain-1.8.0b6/tests/core/full_node/dos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/dos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/dos/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.448977 chia-blockchain-1.8.0b6/tests/core/full_node/full_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/full_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/full_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19025 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/full_sync/test_full_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/ram_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.448977 chia-blockchain-1.8.0b6/tests/core/full_node/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21322 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_coin_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34130 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_full_node_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_hint_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_sync_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23835 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_address_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16506 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_block_height_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13828 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87563 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_full_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_generator_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_hint_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_node_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_peer_store_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/full_node/test_tx_processing_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187863 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/large_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/make_block_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.448977 chia-blockchain-1.8.0b6/tests/core/mempool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123916 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_fee_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_fee_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51540 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/node_height.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.452978 chia-blockchain-1.8.0b6/tests/core/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/flood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_rate_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/server/test_upnp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.452978 chia-blockchain-1.8.0b6/tests/core/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/ssl/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/ssl/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_coins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_cost_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_crawler_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_daemon_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_db_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_db_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23550 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_farmer_harvester_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_full_node_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_merkle_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/test_setproctitle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.452978 chia-blockchain-1.8.0b6/tests/core/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_cached_bls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_file_keyring_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_jsonify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20681 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22952 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_keyring_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_significant_bits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/core/util/test_streamable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.452978 chia-blockchain-1.8.0b6/tests/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/db/test_db_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.452978 chia-blockchain-1.8.0b6/tests/farmer_harvester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/farmer_harvester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/farmer_harvester/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/farmer_harvester/test_farmer_harvester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.452978 chia-blockchain-1.8.0b6/tests/fee_estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/fee_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/fee_estimation/cmdline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/fee_estimation/test_fee_estimation_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/fee_estimation/test_fee_estimation_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/fee_estimation/test_fee_estimation_unit_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/fee_estimation/test_mempoolitem_height_added.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.456977 chia-blockchain-1.8.0b6/tests/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/test_generator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/test_list_to_batches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/test_rom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/generator/test_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.456977 chia-blockchain-1.8.0b6/tests/plot_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/test_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29365 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/test_plot_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/test_receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/test_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18095 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/test_sync_simulated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plot_sync/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.456977 chia-blockchain-1.8.0b6/tests/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plotting/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32802 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plotting/test_plot_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/plotting/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.456977 chia-blockchain-1.8.0b6/tests/pools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/test_pool_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/test_pool_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/test_pool_puzzles_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47263 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/test_pool_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/test_pool_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/pools/test_wallet_pool_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.456977 chia-blockchain-1.8.0b6/tests/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/simulation/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/simulation/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10038 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/simulation/test_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/simulation/test_start_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/testconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.460977 chia-blockchain-1.8.0b6/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/1315537.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/1315544.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/1315630.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/300000.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17387 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/442734.json
+-rw-r--r--   0 runner    (1001) docker     (123)   233251 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/466212.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   405504 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/test-blockchain-db.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/test_full_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/test_legacy_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/tools/test_run_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.464977 chia-blockchain-1.8.0b6/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/alert_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/benchmark_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/bip39_test_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/build_network_protocol_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/gen_ssl_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/generator_tools_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/key_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31159 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/network_protocol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46740 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/protocol_messages_bytes-v1.0
+-rw-r--r--   0 runner    (1001) docker     (123)   170660 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/protocol_messages_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/temp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_full_block_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_limited_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_lock_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22379 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_network_protocol_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_network_protocol_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_network_protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_struct_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/util/test_trusted_peer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.468977 chia-blockchain-1.8.0b6/tests/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.468977 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25164 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_cat_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_cat_outer_puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39540 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_cat_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_offer_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162923 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.468977 chia-blockchain-1.8.0b6/tests/wallet/dao_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/dao_wallet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.468977 chia-blockchain-1.8.0b6/tests/wallet/db_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/db_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/db_wallet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/db_wallet/test_db_graftroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135852 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/db_wallet/test_dl_offers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26485 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/db_wallet/test_dl_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.468977 chia-blockchain-1.8.0b6/tests/wallet/did_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/did_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/did_wallet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65884 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/did_wallet/test_did.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.468977 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   374078 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_1_offers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43345 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_bulk_mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66774 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_offers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_puzzles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76327 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_ownership_outer_puzzle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/tests/wallet/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/rpc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/rpc/test_dl_wallet_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74646 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/rpc/test_wallet_rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/tests/wallet/simple_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/simple_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/simple_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/simple_sync/test_simple_sync_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/tests/wallet/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65523 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/sync/test_wallet_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_address_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_bech32m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_chialisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_coin_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_nft_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_offer_parsing_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_puzzle_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_singleton_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_singleton_lifecycle_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_taproot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27395 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_transaction_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43806 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16405 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_coin_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_interested_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_key_val_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_trade_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/wallet/test_wallet_user_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/tests/weight_proof/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/weight_proof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/weight_proof/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tests/weight_proof/test_weight_proof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:35:09.472977 chia-blockchain-1.8.0b6/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/analyze-chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/analyze_memory_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/cpu_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/generate_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/legacy_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/manage_clvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/plot-log.gnuplot
+-rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/run_benchmark.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/run_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/test_constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13441 2023-04-17 22:30:23.000000 chia-blockchain-1.8.0b6/tools/test_full_sync.py
```

### Comparing `chia-blockchain-1.8.0b5/.github/ISSUE_TEMPLATE/bug_report.yaml` & `chia-blockchain-1.8.0b6/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/ISSUE_TEMPLATE/config.yml` & `chia-blockchain-1.8.0b6/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/PULL_REQUEST_TEMPLATE.md` & `chia-blockchain-1.8.0b6/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/actions/install/action.yml` & `chia-blockchain-1.8.0b6/.github/actions/install/action.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/dependabot.yml` & `chia-blockchain-1.8.0b6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/benchmarks.yml` & `chia-blockchain-1.8.0b6/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/build-linux-arm64-installer.yml` & `chia-blockchain-1.8.0b6/.github/workflows/build-linux-arm64-installer.yml`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
       uses: actions/upload-artifact@v3
       with:
         name: chia-installers-linux-deb-arm64
         path: ${{ github.workspace }}/build_scripts/final_installer/
 
     - name: Configure AWS Credentials
       if: steps.check_secrets.outputs.HAS_AWS_SECRET
-      uses: aws-actions/configure-aws-credentials@v1
+      uses: aws-actions/configure-aws-credentials@v2
       with:
         aws-access-key-id: ${{ secrets.INSTALLER_UPLOAD_KEY }}
         aws-secret-access-key: ${{ secrets.INSTALLER_UPLOAD_SECRET }}
         aws-region: us-west-2
 
     - name: Upload to s3
       if: steps.check_secrets.outputs.HAS_AWS_SECRET
```

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/build-linux-installer-deb.yml` & `chia-blockchain-1.8.0b6/.github/workflows/build-linux-installer-deb.yml`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
       uses: actions/upload-artifact@v3
       with:
         name: chia-installers-linux-deb-intel
         path: ${{ github.workspace }}/build_scripts/final_installer/
 
     - name: Configure AWS Credentials
       if: steps.check_secrets.outputs.HAS_AWS_SECRET
-      uses: aws-actions/configure-aws-credentials@v1
+      uses: aws-actions/configure-aws-credentials@v2
       with:
         aws-access-key-id: ${{ secrets.INSTALLER_UPLOAD_KEY }}
         aws-secret-access-key: ${{ secrets.INSTALLER_UPLOAD_SECRET }}
         aws-region: us-west-2
 
     - name: Upload to s3
       if: steps.check_secrets.outputs.HAS_AWS_SECRET
```

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/build-linux-installer-rpm.yml` & `chia-blockchain-1.8.0b6/.github/workflows/build-linux-installer-rpm.yml`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
       uses: actions/upload-artifact@v3
       with:
         name: chia-installers-linux-rpm-intel
         path: ${{ github.workspace }}/build_scripts/final_installer/
 
     - name: Configure AWS Credentials
       if: steps.check_secrets.outputs.HAS_AWS_SECRET
-      uses: aws-actions/configure-aws-credentials@v1
+      uses: aws-actions/configure-aws-credentials@v2
       with:
         aws-access-key-id: ${{ secrets.INSTALLER_UPLOAD_KEY }}
         aws-secret-access-key: ${{ secrets.INSTALLER_UPLOAD_SECRET }}
         aws-region: us-west-2
 
     - name: Upload to s3
       if: steps.check_secrets.outputs.HAS_AWS_SECRET
```

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/build-macos-installers.yml` & `chia-blockchain-1.8.0b6/.github/workflows/build-macos-installers.yml`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
       # Done now and at the end of the workflow in case the last workflow fails, and this is still around
       - name: Delete keychain if it already exists
         run:
           security delete-keychain signing_temp.keychain || true
 
       - name: Import Apple app signing certificate
         if: steps.check_secrets.outputs.HAS_APPLE_SECRET
-        uses: Apple-Actions/import-codesign-certs@v1
+        uses: Apple-Actions/import-codesign-certs@v2
         with:
           p12-file-base64: ${{ secrets.APPLE_DEV_ID_APP }}
           p12-password: ${{ secrets.APPLE_DEV_ID_APP_PASS }}
 
       - name: Get latest madmax plotter
         env:
           GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/build-windows-installer.yml` & `chia-blockchain-1.8.0b6/.github/workflows/build-windows-installer.yml`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
     - name: Install AWS CLI
       if: steps.check_secrets.outputs.HAS_AWS_SECRET
       run: |
           msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi
 
     - name: Configure AWS Credentials
       if: steps.check_secrets.outputs.HAS_AWS_SECRET
-      uses: aws-actions/configure-aws-credentials@v1
+      uses: aws-actions/configure-aws-credentials@v2
       with:
         aws-access-key-id: ${{ secrets.INSTALLER_UPLOAD_KEY }}
         aws-secret-access-key: ${{ secrets.INSTALLER_UPLOAD_SECRET }}
         aws-region: us-west-2
 
     - name: Upload to s3
       if: steps.check_secrets.outputs.HAS_AWS_SECRET
```

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/check-commit-signing.yml` & `chia-blockchain-1.8.0b6/.github/workflows/check-commit-signing.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/check_wheel_availability.yaml` & `chia-blockchain-1.8.0b6/.github/workflows/check_wheel_availability.yaml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/codeql-analysis.yml` & `chia-blockchain-1.8.0b6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/conflict-check.yml` & `chia-blockchain-1.8.0b6/.github/workflows/conflict-check.yml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 on:
   # So that PRs touching the same files as the push are updated
   push:
   # So that the `dirtyLabel` is removed if conflicts are resolve
   # We recommend `pull_request_target` so that github secrets are available.
   # In `pull_request` we wouldn't be able to change labels of fork PRs
   pull_request_target:
-    types: [synchronize]
+    types: [opened, synchronize, reopened]
 
 jobs:
   main:
     runs-on: ubuntu-latest
     steps:
       - name: check if prs are behind main
         uses: Chia-Network/actions/label-conflict@main
```

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/dependency-review.yml` & `chia-blockchain-1.8.0b6/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/mozilla-ca-cert.yml` & `chia-blockchain-1.8.0b6/.github/workflows/mozilla-ca-cert.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/pre-commit.yml` & `chia-blockchain-1.8.0b6/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/require-labels.yml` & `chia-blockchain-1.8.0b6/.github/workflows/require-labels.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/snyk-python-scan.yml` & `chia-blockchain-1.8.0b6/.github/workflows/snyk-python-scan.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/stale-issue.yml` & `chia-blockchain-1.8.0b6/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/start-release.yml` & `chia-blockchain-1.8.0b6/.github/workflows/start-release.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/start-sync-test.yml` & `chia-blockchain-1.8.0b6/.github/workflows/start-sync-test.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/super-linter.yml` & `chia-blockchain-1.8.0b6/.github/workflows/super-linter.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/test-single.yml` & `chia-blockchain-1.8.0b6/.github/workflows/test-single.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/test.yml` & `chia-blockchain-1.8.0b6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/trigger-docker-dev.yml` & `chia-blockchain-1.8.0b6/.github/workflows/trigger-docker-dev.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/trigger-docker-main.yml` & `chia-blockchain-1.8.0b6/.github/workflows/trigger-docker-main.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.github/workflows/upload-pypi-source.yml` & `chia-blockchain-1.8.0b6/.github/workflows/upload-pypi-source.yml`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
     - name: Lint source with flake8
       run: |
         flake8 benchmarks build_scripts chia tests tools *.py
 
     - name: Lint source with mypy
       run: |
+        echo "MYPY VERSION IS: $(mypy --version)"
         mypy
 
     - name: Lint source with pylint
       run: |
         pylint benchmarks build_scripts chia tests tools *.py
 
     - name: Build source distribution
```

### Comparing `chia-blockchain-1.8.0b5/.gitignore` & `chia-blockchain-1.8.0b6/.gitignore`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.markdown-lint.yml` & `chia-blockchain-1.8.0b6/.markdown-lint.yml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/.pre-commit-config.yaml` & `chia-blockchain-1.8.0b6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/BUILD_TIMELORD.md` & `chia-blockchain-1.8.0b6/BUILD_TIMELORD.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/CHANGELOG.md` & `chia-blockchain-1.8.0b6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/CODE_OF_CONDUCT.md` & `chia-blockchain-1.8.0b6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/CONTRIBUTING.md` & `chia-blockchain-1.8.0b6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/Install-gui.ps1` & `chia-blockchain-1.8.0b6/Install-gui.ps1`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/Install-plotter.ps1` & `chia-blockchain-1.8.0b6/Install-plotter.ps1`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/Install.ps1` & `chia-blockchain-1.8.0b6/Install.ps1`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/LICENSE` & `chia-blockchain-1.8.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/PKG-INFO` & `chia-blockchain-1.8.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chia-blockchain
-Version: 1.8.0b5
+Version: 1.8.0b6
 Summary: Chia blockchain full node, farmer, timelord, and wallet.
 Home-page: https://chia.net/
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
 Project-URL: Source, https://github.com/Chia-Network/chia-blockchain/
 Project-URL: Changelog, https://github.com/Chia-Network/chia-blockchain/blob/main/CHANGELOG.md
```

### Comparing `chia-blockchain-1.8.0b5/PRETTY_GOOD_PRACTICES.md` & `chia-blockchain-1.8.0b6/PRETTY_GOOD_PRACTICES.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/README.md` & `chia-blockchain-1.8.0b6/README.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/SECURITY.md` & `chia-blockchain-1.8.0b6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/activated.py` & `chia-blockchain-1.8.0b6/activated.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/benchmarks/block_ref.py` & `chia-blockchain-1.8.0b6/benchmarks/block_ref.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/benchmarks/block_store.py` & `chia-blockchain-1.8.0b6/benchmarks/block_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/benchmarks/clvm_generator.bin` & `chia-blockchain-1.8.0b6/benchmarks/clvm_generator.bin`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/benchmarks/coin_store.py` & `chia-blockchain-1.8.0b6/benchmarks/coin_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/benchmarks/jsonify.py` & `chia-blockchain-1.8.0b6/benchmarks/jsonify.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/benchmarks/mempool-long-lived.py` & `chia-blockchain-1.8.0b6/benchmarks/mempool-long-lived.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/benchmarks/mempool.py` & `chia-blockchain-1.8.0b6/benchmarks/mempool.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from chia.simulator.wallet_tools import WalletTool
 from chia.types.blockchain_format.coin import Coin
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.types.coin_record import CoinRecord
 from chia.types.mempool_inclusion_status import MempoolInclusionStatus
 from chia.types.spend_bundle import SpendBundle
 from chia.types.spend_bundle_conditions import Spend, SpendBundleConditions
+from chia.util.chunks import chunks
 from chia.util.ints import uint32, uint64
 
 NUM_ITERS = 200
 NUM_PEERS = 5
 
 
 @contextmanager
@@ -85,14 +86,18 @@
     wt = WalletTool(DEFAULT_CONSTANTS)
 
     spend_bundles: List[List[SpendBundle]] = []
 
     # these spend the same coins as spend_bundles but with a higher fee
     replacement_spend_bundles: List[List[SpendBundle]] = []
 
+    # these spend the same coins as spend_bundles, but they are organized in
+    # much larger bundles
+    large_spend_bundles: List[List[SpendBundle]] = []
+
     timestamp = uint64(1631794488)
 
     height = uint32(1)
 
     print("Building SpendBundles")
     for peer in range(NUM_PEERS):
         print(f"  peer {peer}")
@@ -129,14 +134,27 @@
         for coin in unspent:
             tx = wt.generate_signed_transaction(
                 uint64(coin.amount // 2), wt.get_new_puzzlehash(), coin, fee=peer + idx + 10000000
             )
             bundles.append(tx)
         replacement_spend_bundles.append(bundles)
 
+        bundles = []
+        print("     large spend bundles")
+        for coins in chunks(unspent, 200):
+            print(f"{len(coins)} coins")
+            tx = SpendBundle.aggregate(
+                [
+                    wt.generate_signed_transaction(uint64(c.amount // 2), wt.get_new_puzzlehash(), c, fee=peer + idx)
+                    for c in coins
+                ]
+            )
+            bundles.append(tx)
+        large_spend_bundles.append(bundles)
+
     start_height = height
     for single_threaded in [False, True]:
         if single_threaded:
             print("\n== Single-threaded")
         else:
             print("\n== Multi-threaded")
 
@@ -153,14 +171,33 @@
                 assert npc is not None
                 _, status, error = await mempool.add_spend_bundle(tx, npc, spend_bundle_id, height)
                 assert status == MempoolInclusionStatus.SUCCESS
                 assert error is None
 
         suffix = "st" if single_threaded else "mt"
 
+        print("\nProfiling add_spend_bundle() with large bundles")
+        total_bundles = 0
+        tasks = []
+        with enable_profiler(True, f"add-large-{suffix}"):
+            start = monotonic()
+            for peer in range(NUM_PEERS):
+                total_bundles += len(large_spend_bundles[peer])
+                tasks.append(asyncio.create_task(add_spend_bundles(large_spend_bundles[peer])))
+            await asyncio.gather(*tasks)
+            stop = monotonic()
+        print(f"  time: {stop - start:0.4f}s")
+        print(f"  per call: {(stop - start) / total_bundles * 1000:0.2f}ms")
+
+        mempool = MempoolManager(get_coin_record, DEFAULT_CONSTANTS, single_threaded=single_threaded)
+
+        height = start_height
+        rec = fake_block_record(height, timestamp)
+        await mempool.new_peak(rec, None)
+
         print("\nProfiling add_spend_bundle()")
         total_bundles = 0
         tasks = []
         with enable_profiler(True, f"add-{suffix}"):
             start = monotonic()
             for peer in range(NUM_PEERS):
                 total_bundles += len(spend_bundles[peer])
```

### Comparing `chia-blockchain-1.8.0b5/benchmarks/streamable.py` & `chia-blockchain-1.8.0b6/benchmarks/streamable.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/benchmarks/transaction_height_delta` & `chia-blockchain-1.8.0b6/benchmarks/transaction_height_delta`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/benchmarks/utils.py` & `chia-blockchain-1.8.0b6/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/assets/dmg/background.tiff` & `chia-blockchain-1.8.0b6/build_scripts/assets/dmg/background.tiff`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/build_linux_deb-1-gui.sh` & `chia-blockchain-1.8.0b6/build_scripts/build_linux_deb-1-gui.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/build_linux_deb-2-installer.sh` & `chia-blockchain-1.8.0b6/build_scripts/build_linux_deb-2-installer.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/build_linux_rpm-1-gui.sh` & `chia-blockchain-1.8.0b6/build_scripts/build_linux_rpm-1-gui.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/build_linux_rpm-2-installer.sh` & `chia-blockchain-1.8.0b6/build_scripts/build_linux_rpm-2-installer.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/build_macos-1-gui.sh` & `chia-blockchain-1.8.0b6/build_scripts/build_macos-1-gui.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/build_macos-2-installer.sh` & `chia-blockchain-1.8.0b6/build_scripts/build_macos-2-installer.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/build_windows-1-gui.ps1` & `chia-blockchain-1.8.0b6/build_scripts/build_windows-1-gui.ps1`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/build_windows-2-installer.ps1` & `chia-blockchain-1.8.0b6/build_scripts/build_windows-2-installer.ps1`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/check_dependency_artifacts.py` & `chia-blockchain-1.8.0b6/build_scripts/check_dependency_artifacts.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/clean-runner.sh` & `chia-blockchain-1.8.0b6/build_scripts/clean-runner.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/installer-version.py` & `chia-blockchain-1.8.0b6/build_scripts/installer-version.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/npm_linux/package-lock.json` & `chia-blockchain-1.8.0b6/build_scripts/npm_linux/package-lock.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/npm_macos/package-lock.json` & `chia-blockchain-1.8.0b6/build_scripts/npm_macos/package-lock.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/build_scripts/npm_windows/package-lock.json` & `chia-blockchain-1.8.0b6/build_scripts/npm_windows/package-lock.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/clvm/spend_sim.py` & `chia-blockchain-1.8.0b6/chia/clvm/spend_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,21 +250,21 @@
         return_removals: List[Coin] = []
         if (len(self.block_records) > 0) and (self.mempool_manager.mempool.size() > 0):
             peak = self.mempool_manager.peak
             if peak is not None:
                 result = self.mempool_manager.create_bundle_from_mempool(peak.header_hash, item_inclusion_filter)
 
                 if result is not None:
-                    bundle, additions, removals = result
+                    bundle, additions = result
                     generator_bundle = bundle
                     return_additions = additions
-                    return_removals = removals
+                    return_removals = bundle.removals()
 
                     await self.coin_store._add_coin_records([self.new_coin_record(addition) for addition in additions])
-                    await self.coin_store._set_spent([r.name() for r in removals], uint32(self.block_height + 1))
+                    await self.coin_store._set_spent([r.name() for r in return_removals], uint32(self.block_height + 1))
 
         # SimBlockRecord is created
         generator: Optional[BlockGenerator] = await self.generate_transaction_generator(generator_bundle)
         self.block_records.append(
             SimBlockRecord.create(
                 [pool_coin, farmer_coin],
                 next_block_height,
```

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/beta.py` & `chia-blockchain-1.8.0b6/chia/cmds/beta.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/beta_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/beta_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/check_wallet_db.py` & `chia-blockchain-1.8.0b6/chia/cmds/check_wallet_db.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/chia.py` & `chia-blockchain-1.8.0b6/chia/cmds/chia.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/cmds_util.py` & `chia-blockchain-1.8.0b6/chia/cmds/cmds_util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/coin_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/coin_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/coins.py` & `chia-blockchain-1.8.0b6/chia/cmds/coins.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/completion.py` & `chia-blockchain-1.8.0b6/chia/cmds/completion.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/configure.py` & `chia-blockchain-1.8.0b6/chia/cmds/configure.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/data.py` & `chia-blockchain-1.8.0b6/chia/cmds/data.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/data_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/data_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/db.py` & `chia-blockchain-1.8.0b6/chia/cmds/db.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/db_backup_func.py` & `chia-blockchain-1.8.0b6/chia/cmds/db_backup_func.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/db_upgrade_func.py` & `chia-blockchain-1.8.0b6/chia/cmds/db_upgrade_func.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/db_validate_func.py` & `chia-blockchain-1.8.0b6/chia/cmds/db_validate_func.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/farm.py` & `chia-blockchain-1.8.0b6/chia/cmds/farm.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/farm_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/farm_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/init.py` & `chia-blockchain-1.8.0b6/chia/cmds/init.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/init_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/init_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/keys.py` & `chia-blockchain-1.8.0b6/chia/cmds/keys.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/keys_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/keys_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/netspace.py` & `chia-blockchain-1.8.0b6/chia/cmds/netspace.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/netspace_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/netspace_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/passphrase.py` & `chia-blockchain-1.8.0b6/chia/cmds/passphrase.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import click
 
 from chia.util.config import load_config
 
 
 @click.group("passphrase", short_help="Manage your keyring passphrase")
-def passphrase_cmd():
+def passphrase_cmd() -> None:
     pass
 
 
 @passphrase_cmd.command(
     "set",
     help="""Sets or updates the keyring passphrase. If --passphrase-file and/or --current-passphrase-file options are
             provided, the passphrases will be read from the specified files. Otherwise, a prompt will be provided to
@@ -105,26 +105,26 @@
 
 @passphrase_cmd.group("hint", short_help="Manage the optional keyring passphrase hint")
 def hint_cmd() -> None:
     pass
 
 
 @hint_cmd.command("display", short_help="Display the keyring passphrase hint")
-def display_hint():
+def display_hint() -> None:
     from .passphrase_funcs import display_passphrase_hint
 
     display_passphrase_hint()
 
 
 @hint_cmd.command("set", short_help="Set or update the keyring passphrase hint")
 @click.argument("hint", nargs=1)
-def set_hint(hint):
+def set_hint(hint: str) -> None:
     from .passphrase_funcs import set_passphrase_hint
 
     set_passphrase_hint(hint)
 
 
 @hint_cmd.command("remove", short_help="Remove the keyring passphrase hint")
-def remove_hint():
+def remove_hint() -> None:
     from .passphrase_funcs import remove_passphrase_hint
 
     remove_passphrase_hint()
```

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/passphrase_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/passphrase_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/peer.py` & `chia-blockchain-1.8.0b6/chia/cmds/peer.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/peer_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/peer_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,30 +49,30 @@
     print(result_txt)
 
 
 async def print_connections(rpc_client: RpcClient, trusted_peers: Dict[str, Any]) -> None:
     import time
 
     from chia.server.outbound_message import NodeType
-    from chia.util.network import is_trusted_inner
+    from chia.util.network import is_trusted_peer
 
     connections = await rpc_client.get_connections()
     print("Connections:")
     print("Type      IP                                      Ports       NodeID      Last Connect" + "      MiB Up|Dwn")
     for con in connections:
         last_connect_tuple = time.struct_time(time.localtime(con["last_message_time"]))
         last_connect = time.strftime("%b %d %T", last_connect_tuple)
         mb_down = con["bytes_read"] / (1024 * 1024)
         mb_up = con["bytes_written"] / (1024 * 1024)
 
         host = con["peer_host"]
         # Strip IPv6 brackets
         host = host.strip("[]")
 
-        trusted: bool = is_trusted_inner(host, con["node_id"], trusted_peers, False)
+        trusted: bool = is_trusted_peer(host, con["node_id"], trusted_peers, False)
         # Nodetype length is 9 because INTRODUCER will be deprecated
         if NodeType(con["type"]) is NodeType.FULL_NODE:
             peak_height = con.get("peak_height", None)
             connection_peak_hash = con.get("peak_hash", None)
             if connection_peak_hash is None:
                 connection_peak_hash = "No Info"
             else:
```

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/plotnft.py` & `chia-blockchain-1.8.0b6/chia/cmds/plotnft.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/plotnft_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/plotnft_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/plots.py` & `chia-blockchain-1.8.0b6/chia/cmds/plots.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/rpc.py` & `chia-blockchain-1.8.0b6/chia/cmds/rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/show.py` & `chia-blockchain-1.8.0b6/chia/cmds/show.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/show_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/show_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/start.py` & `chia-blockchain-1.8.0b6/chia/cmds/start.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/start_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/start_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         await asyncio.sleep(1)
         # it prints "daemon: listening"
         connection = await connect_to_daemon_and_validate(root_path, config)
     if connection:
         passphrase = None
         if await connection.is_keyring_locked():
             passphrase = Keychain.get_cached_master_passphrase()
-            if not Keychain.master_passphrase_is_valid(passphrase):
+            if passphrase is None or not Keychain.master_passphrase_is_valid(passphrase):
                 with ThreadPoolExecutor(max_workers=1, thread_name_prefix="get_current_passphrase") as executor:
                     passphrase = await asyncio.get_running_loop().run_in_executor(executor, get_current_passphrase)
 
         if passphrase:
             print("Unlocking daemon keyring")
             await connection.unlock_keyring(passphrase)
```

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/stop.py` & `chia-blockchain-1.8.0b6/chia/cmds/stop.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/wallet.py` & `chia-blockchain-1.8.0b6/chia/cmds/wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/cmds/wallet_funcs.py` & `chia-blockchain-1.8.0b6/chia/cmds/wallet_funcs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/block_body_validation.py` & `chia-blockchain-1.8.0b6/chia/consensus/block_body_validation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/block_creation.py` & `chia-blockchain-1.8.0b6/chia/consensus/block_creation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/block_header_validation.py` & `chia-blockchain-1.8.0b6/chia/consensus/block_header_validation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/block_record.py` & `chia-blockchain-1.8.0b6/chia/consensus/block_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/block_rewards.py` & `chia-blockchain-1.8.0b6/chia/consensus/block_rewards.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/block_root_validation.py` & `chia-blockchain-1.8.0b6/chia/consensus/block_root_validation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/blockchain.py` & `chia-blockchain-1.8.0b6/chia/consensus/blockchain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/blockchain_interface.py` & `chia-blockchain-1.8.0b6/chia/consensus/blockchain_interface.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/coinbase.py` & `chia-blockchain-1.8.0b6/chia/consensus/coinbase.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/constants.py` & `chia-blockchain-1.8.0b6/chia/consensus/constants.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/cost_calculator.py` & `chia-blockchain-1.8.0b6/chia/consensus/cost_calculator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/default_constants.py` & `chia-blockchain-1.8.0b6/chia/consensus/default_constants.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/deficit.py` & `chia-blockchain-1.8.0b6/chia/consensus/deficit.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/difficulty_adjustment.py` & `chia-blockchain-1.8.0b6/chia/consensus/difficulty_adjustment.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/find_fork_point.py` & `chia-blockchain-1.8.0b6/chia/consensus/find_fork_point.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/full_block_to_block_record.py` & `chia-blockchain-1.8.0b6/chia/consensus/full_block_to_block_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/get_block_challenge.py` & `chia-blockchain-1.8.0b6/chia/consensus/get_block_challenge.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/make_sub_epoch_summary.py` & `chia-blockchain-1.8.0b6/chia/consensus/make_sub_epoch_summary.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/multiprocess_validation.py` & `chia-blockchain-1.8.0b6/chia/consensus/multiprocess_validation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/pos_quality.py` & `chia-blockchain-1.8.0b6/chia/consensus/pos_quality.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/pot_iterations.py` & `chia-blockchain-1.8.0b6/chia/consensus/pot_iterations.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/consensus/vdf_info_computation.py` & `chia-blockchain-1.8.0b6/chia/consensus/vdf_info_computation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/daemon/client.py` & `chia-blockchain-1.8.0b6/chia/daemon/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,10 +211,10 @@
 
     daemon: Optional[DaemonProxy] = None
     try:
         daemon = await connect_to_daemon_and_validate(root_path, config, quiet=quiet)
         yield daemon  # <----
     except Exception as e:
         print(f"Exception occurred while communicating with the daemon: {e}")
-
-    if daemon is not None:
-        await daemon.close()
+    finally:
+        if daemon is not None:
+            await daemon.close()
```

### Comparing `chia-blockchain-1.8.0b5/chia/daemon/keychain_proxy.py` & `chia-blockchain-1.8.0b6/chia/daemon/keychain_proxy.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/daemon/keychain_server.py` & `chia-blockchain-1.8.0b6/chia/daemon/keychain_server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/daemon/server.py` & `chia-blockchain-1.8.0b6/chia/daemon/server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/daemon/windows_signal.py` & `chia-blockchain-1.8.0b6/chia/daemon/windows_signal.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/data_layer/data_layer.py` & `chia-blockchain-1.8.0b6/chia/data_layer/data_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import logging
+import os
 import random
 import time
 import traceback
 from pathlib import Path
 from typing import Any, Awaitable, Dict, List, Optional, Set, Tuple, Union
 
 import aiohttp
@@ -54,14 +55,16 @@
     wallet_rpc_init: Awaitable[WalletRpcClient]
     state_changed_callback: Optional[StateChangedProtocol] = None
     wallet_id: uint64
     initialized: bool
     none_bytes: bytes32
     lock: asyncio.Lock
     _server: Optional[ChiaServer]
+    downloaders: List[str]
+    uploaders: List[str]
 
     @property
     def server(self) -> ChiaServer:
         # This is a stop gap until the class usage is refactored such the values of
         # integral attributes are known at creation of the instance.
         if self._server is None:
             raise RuntimeError("server not assigned")
@@ -69,14 +72,16 @@
         return self._server
 
     def __init__(
         self,
         config: Dict[str, Any],
         root_path: Path,
         wallet_rpc_init: Awaitable[WalletRpcClient],
+        downloaders: List[str],
+        uploaders: List[str],  # dont add FilesystemUploader to this, it is the default uploader
         name: Optional[str] = None,
     ):
         if name == "":
             # TODO: If no code depends on "" counting as 'unspecified' then we do not
             #       need this.
             name = None
         self.initialized = False
@@ -92,14 +97,16 @@
             "server_files_location", "data_layer/db/server_files_location_CHALLENGE"
         ).replace("CHALLENGE", config["selected_network"])
         self.server_files_location = path_from_root(root_path, server_files_replaced)
         self.server_files_location.mkdir(parents=True, exist_ok=True)
         self.none_bytes = bytes32([0] * 32)
         self.lock = asyncio.Lock()
         self._server = None
+        self.downloaders = downloaders
+        self.uploaders = uploaders
 
     def _set_state_changed_callback(self, callback: StateChangedProtocol) -> None:
         self.state_changed_callback = callback
 
     async def on_connect(self, connection: WSChiaConnection) -> None:
         pass
 
@@ -348,14 +355,15 @@
 
         timestamp = int(time.time())
         servers_info = await self.data_store.get_available_servers_for_store(tree_id, timestamp)
         # TODO: maybe append a random object to the whole DataLayer class?
         random.shuffle(servers_info)
         for server_info in servers_info:
             url = server_info.url
+
             root = await self.data_store.get_tree_root(tree_id=tree_id)
             if root.generation > singleton_record.generation:
                 self.log.info(
                     "Fetch data: local DL store is ahead of chain generation. "
                     f"Local root: {root}. Singleton: {singleton_record}"
                 )
                 break
@@ -371,28 +379,28 @@
             )
 
             to_download = await self.wallet_rpc.dl_history(
                 launcher_id=tree_id,
                 min_generation=uint32(root.generation + 1),
                 max_generation=singleton_record.generation,
             )
-
             try:
                 timeout = self.config.get("client_timeout", 15)
                 proxy_url = self.config.get("proxy_url", None)
                 success = await insert_from_delta_file(
                     self.data_store,
                     tree_id,
                     root.generation,
                     [record.root for record in reversed(to_download)],
                     server_info,
                     self.server_files_location,
                     timeout,
                     self.log,
                     proxy_url,
+                    await self.get_downloader(tree_id, url),
                 )
                 if success:
                     self.log.info(
                         f"Finished downloading and validating {tree_id}. "
                         f"Wallet generation saved: {singleton_record.generation}. "
                         f"Root hash saved: {singleton_record.root}."
                     )
@@ -400,33 +408,73 @@
             except asyncio.CancelledError:
                 raise
             except aiohttp.client_exceptions.ClientConnectorError:
                 self.log.warning(f"Server {url} unavailable for {tree_id}.")
             except Exception as e:
                 self.log.warning(f"Exception while downloading files for {tree_id}: {e} {traceback.format_exc()}.")
 
+    async def get_downloader(self, tree_id: bytes32, url: str) -> Optional[str]:
+        request_json = {"store_id": tree_id.hex(), "url": url}
+        for d in self.downloaders:
+            async with aiohttp.ClientSession() as session:
+                try:
+                    async with session.post(d + "/handle_download", json=request_json) as response:
+                        res_json = await response.json()
+                        if res_json["handle_download"]:
+                            return d
+                except Exception as e:
+                    self.log.error(f"get_downloader could not get response: {type(e).__name__}: {e}")
+        return None
+
     async def upload_files(self, tree_id: bytes32) -> None:
+        uploaders = await self.get_uploaders(tree_id)
         singleton_record: Optional[SingletonRecord] = await self.wallet_rpc.dl_latest_singleton(tree_id, True)
         if singleton_record is None:
             self.log.info(f"Upload files: no on-chain record for {tree_id}.")
             return
         async with self.lock:
             await self._update_confirmation_status(tree_id=tree_id)
 
         root = await self.data_store.get_tree_root(tree_id=tree_id)
         publish_generation = min(singleton_record.generation, 0 if root is None else root.generation)
         # If we make some batch updates, which get confirmed to the chain, we need to create the files.
         # We iterate back and write the missing files, until we find the files already written.
         root = await self.data_store.get_tree_root(tree_id=tree_id, generation=publish_generation)
-        while publish_generation > 0 and await write_files_for_root(
-            self.data_store,
-            tree_id,
-            root,
-            self.server_files_location,
-        ):
+        while publish_generation > 0:
+            write_file_result = await write_files_for_root(self.data_store, tree_id, root, self.server_files_location)
+            if not write_file_result.result:
+                self.log.error("failed to write files")
+                break
+            try:
+                if uploaders is not None and len(uploaders) > 0:
+                    request_json = {
+                        "store_id": tree_id.hex(),
+                        "full_tree_path": str(write_file_result.full_tree),
+                        "diff_path": str(write_file_result.diff_tree),
+                    }
+                    for uploader in uploaders:
+                        self.log.info(f"Using uploader {uploader} for store {tree_id.hex()}")
+                        async with aiohttp.ClientSession() as session:
+                            async with session.post(uploader + "/upload", json=request_json) as response:
+                                res_json = await response.json()
+                                if res_json["uploaded"]:
+                                    self.log.info(
+                                        f"Uploaded files to {uploader} for store {tree_id.hex()} "
+                                        "generation {publish_generation}"
+                                    )
+                                else:
+                                    self.log.error(
+                                        f"Failed to upload files to, will retry later: {uploader} : {res_json}"
+                                    )
+                                    break  # todo this will retry all uploaders
+            except Exception as e:
+                self.log.error(f"Exception uploading files, will retry later: tree id {tree_id}")
+                self.log.debug(f"Failed to upload files, cleaning local files: {type(e).__name__}: {e}")
+                os.remove(write_file_result.full_tree)
+                os.remove(write_file_result.diff_tree)
             publish_generation -= 1
             root = await self.data_store.get_tree_root(tree_id=tree_id, generation=publish_generation)
 
     async def add_missing_files(self, store_id: bytes32, overwrite: bool, foldername: Optional[Path]) -> None:
         root = await self.data_store.get_tree_root(tree_id=store_id)
         singleton_record: Optional[SingletonRecord] = await self.wallet_rpc.dl_latest_singleton(store_id, True)
         if singleton_record is None:
@@ -798,7 +846,20 @@
 
         return SyncStatus(
             root_hash=self.none_bytes if root.node_hash is None else root.node_hash,
             generation=root.generation,
             target_root_hash=singleton_record.root,
             target_generation=singleton_record.generation,
         )
+
+    async def get_uploaders(self, tree_id: bytes32) -> List[str]:
+        uploaders = []
+        for uploader in self.uploaders:
+            async with aiohttp.ClientSession() as session:
+                try:
+                    async with session.post(uploader + "/handle_upload", json={"store_id": tree_id.hex()}) as response:
+                        res_json = await response.json()
+                        if res_json["handle_upload"]:
+                            uploaders.append(uploader)
+                except Exception as e:
+                    self.log.error(f"get_uploader could not get response {e}")
+        return uploaders
```

### Comparing `chia-blockchain-1.8.0b5/chia/data_layer/data_layer_api.py` & `chia-blockchain-1.8.0b6/chia/data_layer/data_layer_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/data_layer/data_layer_errors.py` & `chia-blockchain-1.8.0b6/chia/data_layer/data_layer_errors.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/data_layer/data_layer_server.py` & `chia-blockchain-1.8.0b6/chia/data_layer/data_layer_server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/data_layer/data_layer_util.py` & `chia-blockchain-1.8.0b6/chia/data_layer/data_layer_util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/data_layer/data_layer_wallet.py` & `chia-blockchain-1.8.0b6/chia/data_layer/data_layer_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/data_layer/data_store.py` & `chia-blockchain-1.8.0b6/chia/data_layer/data_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/data_layer/dl_wallet_store.py` & `chia-blockchain-1.8.0b6/chia/data_layer/dl_wallet_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/data_layer/download_data.py` & `chia-blockchain-1.8.0b6/chia/data_layer/download_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import os
 import time
+from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Optional
 
 import aiohttp
 from typing_extensions import Literal
 
 from chia.data_layer.data_layer_util import NodeType, Root, SerializedNode, ServerInfo, Status
@@ -82,21 +83,28 @@
 
             node_type = NodeType.TERMINAL if serialized_node.is_terminal else NodeType.INTERNAL
             await data_store.insert_node(node_type, serialized_node.value1, serialized_node.value2)
 
     await data_store.insert_root_with_ancestor_table(tree_id=tree_id, node_hash=root_hash, status=Status.COMMITTED)
 
 
+@dataclass
+class WriteFilesResult:
+    result: bool
+    full_tree: Path
+    diff_tree: Path
+
+
 async def write_files_for_root(
     data_store: DataStore,
     tree_id: bytes32,
     root: Root,
     foldername: Path,
     overwrite: bool = False,
-) -> bool:
+) -> WriteFilesResult:
     if root.node_hash is not None:
         node_hash = root.node_hash
     else:
         node_hash = bytes32([0] * 32)  # todo change
 
     filename_full_tree = foldername.joinpath(get_full_tree_filename(tree_id, node_hash, root.generation))
     filename_diff_tree = foldername.joinpath(get_delta_filename(tree_id, node_hash, root.generation))
@@ -120,58 +128,46 @@
                 await data_store.write_tree_to_file(root, node_hash, tree_id, True, writer)
         else:
             open(filename_diff_tree, mode).close()
         written = True
     except FileExistsError:
         pass
 
-    return written
+    return WriteFilesResult(written, filename_full_tree, filename_diff_tree)
 
 
 async def insert_from_delta_file(
     data_store: DataStore,
     tree_id: bytes32,
     existing_generation: int,
     root_hashes: List[bytes32],
     server_info: ServerInfo,
     client_foldername: Path,
     timeout: int,
     log: logging.Logger,
     proxy_url: str,
+    downloader: Optional[str],
 ) -> bool:
     for root_hash in root_hashes:
         timestamp = int(time.time())
         existing_generation += 1
         filename = get_delta_filename(tree_id, root_hash, existing_generation)
-
-        try:
+        request_json = {"url": server_info.url, "client_folder": str(client_foldername), "filename": filename}
+        if downloader is None:
+            # use http downloader
+            if not await http_download(client_foldername, filename, proxy_url, server_info, timeout, log):
+                break
+        else:
+            log.info(f"Using downloader {downloader} for store {tree_id.hex()}.")
             async with aiohttp.ClientSession() as session:
-                headers = {"accept-encoding": "gzip"}
-                async with session.get(
-                    server_info.url + "/" + filename, headers=headers, timeout=timeout, proxy=proxy_url
-                ) as resp:
-                    resp.raise_for_status()
-                    size = int(resp.headers.get("content-length", 0))
-                    log.debug(f"Downloading delta file {filename}. Size {size} bytes.")
-                    progress_byte = 0
-                    progress_percentage = "{:.0%}".format(0)
-                    target_filename = client_foldername.joinpath(filename)
-                    with target_filename.open(mode="wb") as f:
-                        async for chunk, _ in resp.content.iter_chunks():
-                            f.write(chunk)
-                            progress_byte += len(chunk)
-                            new_percentage = "{:.0%}".format(progress_byte / size)
-                            if new_percentage != progress_percentage:
-                                progress_percentage = new_percentage
-                                log.info(f"Downloading delta file {filename}. {progress_percentage} of {size} bytes.")
-        except Exception:
-            target_filename = client_foldername.joinpath(filename)
-            os.remove(target_filename)
-            await data_store.server_misses_file(tree_id, server_info, timestamp)
-            raise
+                async with session.post(downloader + "/download", json=request_json) as response:
+                    res_json = await response.json()
+                    if not res_json["downloaded"]:
+                        log.error(f"Failed to download delta file {filename} from {downloader}: {res_json}")
+                        break
 
         log.info(f"Successfully downloaded delta file {filename}.")
         try:
             await insert_into_data_store_from_file(
                 data_store,
                 tree_id,
                 None if root_hash == bytes32([0] * 32) else root_hash,
@@ -196,7 +192,38 @@
             target_filename = client_foldername.joinpath(filename)
             os.remove(target_filename)
             await data_store.received_incorrect_file(tree_id, server_info, timestamp)
             await data_store.rollback_to_generation(tree_id, existing_generation - 1)
             raise
 
     return True
+
+
+async def http_download(
+    client_folder: Path,
+    filename: str,
+    proxy_url: str,
+    server_info: ServerInfo,
+    timeout: int,
+    log: logging.Logger,
+) -> bool:
+    async with aiohttp.ClientSession() as session:
+        headers = {"accept-encoding": "gzip"}
+        async with session.get(
+            server_info.url + "/" + filename, headers=headers, timeout=timeout, proxy=proxy_url
+        ) as resp:
+            resp.raise_for_status()
+            size = int(resp.headers.get("content-length", 0))
+            log.debug(f"Downloading delta file {filename}. Size {size} bytes.")
+            progress_byte = 0
+            progress_percentage = "{:.0%}".format(0)
+            target_filename = client_folder.joinpath(filename)
+            with target_filename.open(mode="wb") as f:
+                async for chunk, _ in resp.content.iter_chunks():
+                    f.write(chunk)
+                    progress_byte += len(chunk)
+                    new_percentage = "{:.0%}".format(progress_byte / size)
+                    if new_percentage != progress_percentage:
+                        progress_percentage = new_percentage
+                        log.info(f"Downloading delta file {filename}. {progress_percentage} of {size} bytes.")
+
+    return True
```

### Comparing `chia-blockchain-1.8.0b5/chia/data_layer/util/benchmark.py` & `chia-blockchain-1.8.0b6/chia/data_layer/util/benchmark.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/farmer/farmer.py` & `chia-blockchain-1.8.0b6/chia/farmer/farmer.py`

 * *Files 1% similar despite different names*

```diff
@@ -649,21 +649,21 @@
                 )
 
         return None
 
     async def get_harvesters(self, counts_only: bool = False) -> Dict[str, Any]:
         harvesters: List[Dict[str, Any]] = []
         for connection in self.server.get_connections(NodeType.HARVESTER):
-            self.log.debug(f"get_harvesters host: {connection.peer_host}, node_id: {connection.peer_node_id}")
+            self.log.debug(f"get_harvesters host: {connection.peer_info.host}, node_id: {connection.peer_node_id}")
             receiver = self.plot_sync_receivers.get(connection.peer_node_id)
             if receiver is not None:
                 harvesters.append(receiver.to_dict(counts_only))
             else:
                 self.log.debug(
-                    f"get_harvesters invalid peer: {connection.peer_host}, node_id: {connection.peer_node_id}"
+                    f"get_harvesters invalid peer: {connection.peer_info.host}, node_id: {connection.peer_node_id}"
                 )
 
         return {"harvesters": harvesters}
 
     def get_receiver(self, node_id: bytes32) -> Receiver:
         receiver: Optional[Receiver] = self.plot_sync_receivers.get(node_id)
         if receiver is None:
```

### Comparing `chia-blockchain-1.8.0b5/chia/farmer/farmer_api.py` & `chia-blockchain-1.8.0b6/chia/farmer/farmer_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/bitcoin_fee_estimator.py` & `chia-blockchain-1.8.0b6/chia/full_node/bitcoin_fee_estimator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/block_height_map.py` & `chia-blockchain-1.8.0b6/chia/full_node/block_height_map.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/block_store.py` & `chia-blockchain-1.8.0b6/chia/full_node/block_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/bundle_tools.py` & `chia-blockchain-1.8.0b6/chia/full_node/bundle_tools.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/coin_store.py` & `chia-blockchain-1.8.0b6/chia/full_node/coin_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/fee_estimate.py` & `chia-blockchain-1.8.0b6/chia/full_node/fee_estimate.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/fee_estimate_store.py` & `chia-blockchain-1.8.0b6/chia/full_node/fee_estimate_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/fee_estimation.py` & `chia-blockchain-1.8.0b6/chia/full_node/fee_estimation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/fee_estimator.py` & `chia-blockchain-1.8.0b6/chia/full_node/fee_estimator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/fee_estimator_constants.py` & `chia-blockchain-1.8.0b6/chia/full_node/fee_estimator_constants.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/fee_estimator_example.py` & `chia-blockchain-1.8.0b6/chia/full_node/fee_estimator_example.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/fee_estimator_interface.py` & `chia-blockchain-1.8.0b6/chia/full_node/fee_estimator_interface.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/fee_history.py` & `chia-blockchain-1.8.0b6/chia/full_node/fee_history.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/fee_tracker.py` & `chia-blockchain-1.8.0b6/chia/full_node/fee_tracker.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/full_node.py` & `chia-blockchain-1.8.0b6/chia/full_node/full_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,16 +276,16 @@
             else:
                 peak_height = None
                 peak_hash = None
                 peak_weight = None
             con_dict: Dict[str, Any] = {
                 "type": con.connection_type,
                 "local_port": con.local_port,
-                "peer_host": con.peer_host,
-                "peer_port": con.peer_port,
+                "peer_host": con.peer_info.host,
+                "peer_port": con.peer_info.port,
                 "peer_server_port": con.peer_server_port,
                 "node_id": con.peer_node_id,
                 "creation_time": con.creation_time,
                 "bytes_read": con.bytes_read,
                 "bytes_written": con.bytes_written,
                 "last_message_time": con.last_message_time,
                 "peak_height": peak_height,
@@ -984,15 +984,16 @@
                 c for c in self.server.all_connections.values() if c.peer_node_id in peer_ids
             ]
 
             # Request weight proof from a random peer
             self.log.info(f"Total of {len(peers_with_peak)} peers with peak {target_peak.height}")
             weight_proof_peer: WSChiaConnection = random.choice(peers_with_peak)
             self.log.info(
-                f"Requesting weight proof from peer {weight_proof_peer.peer_host} up to height {target_peak.height}"
+                f"Requesting weight proof from peer {weight_proof_peer.peer_info.host} "
+                f"up to height {target_peak.height}"
             )
             cur_peak: Optional[BlockRecord] = self.blockchain.get_peak()
             if cur_peak is not None and target_peak.weight <= cur_peak.weight:
                 raise ValueError("Not performing sync, already caught up.")
 
             wp_timeout = 360
             if "weight_proof_timeout" in self.config:
@@ -1002,28 +1003,30 @@
             response = await weight_proof_peer.call_api(
                 FullNodeAPI.request_proof_of_weight, request, timeout=wp_timeout
             )
 
             # Disconnect from this peer, because they have not behaved properly
             if response is None or not isinstance(response, full_node_protocol.RespondProofOfWeight):
                 await weight_proof_peer.close(600)
-                raise RuntimeError(f"Weight proof did not arrive in time from peer: {weight_proof_peer.peer_host}")
+                raise RuntimeError(f"Weight proof did not arrive in time from peer: {weight_proof_peer.peer_info.host}")
             if response.wp.recent_chain_data[-1].reward_chain_block.height != target_peak.height:
                 await weight_proof_peer.close(600)
-                raise RuntimeError(f"Weight proof had the wrong height: {weight_proof_peer.peer_host}")
+                raise RuntimeError(f"Weight proof had the wrong height: {weight_proof_peer.peer_info.host}")
             if response.wp.recent_chain_data[-1].reward_chain_block.weight != target_peak.weight:
                 await weight_proof_peer.close(600)
-                raise RuntimeError(f"Weight proof had the wrong weight: {weight_proof_peer.peer_host}")
+                raise RuntimeError(f"Weight proof had the wrong weight: {weight_proof_peer.peer_info.host}")
 
             # dont sync to wp if local peak is heavier,
             # dont ban peer, we asked for this peak
             current_peak = self.blockchain.get_peak()
             if current_peak is not None:
                 if response.wp.recent_chain_data[-1].reward_chain_block.weight <= current_peak.weight:
-                    raise RuntimeError(f"current peak is heavier than Weight proof peek: {weight_proof_peer.peer_host}")
+                    raise RuntimeError(
+                        f"current peak is heavier than Weight proof peek: {weight_proof_peer.peer_info.host}"
+                    )
 
             try:
                 validated, fork_point, summaries = await self.weight_proof_handler.validate_weight_proof(response.wp)
             except Exception as e:
                 await weight_proof_peer.close(600)
                 raise ValueError(f"Weight proof validation threw an error {e}")
 
@@ -1083,15 +1086,14 @@
                             peers_with_peak.remove(peer)
                         elif isinstance(response, RespondBlocks):
                             await batch_queue.put((peer, response.blocks))
                             fetched = True
                             break
                     if fetched is False:
                         self.log.error(f"failed fetching {start_height} to {end_height} from peers")
-                        await batch_queue.put(None)
                         return
                     if self.sync_store.peers_changed.is_set():
                         new_peers_with_peak = self.get_peers_with_peak(peak_hash)
                         self.sync_store.peers_changed.clear()
             except Exception as e:
                 self.log.error(f"Exception fetching {start_height} to {end_height} from peer {e}")
             finally:
```

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/full_node_api.py` & `chia-blockchain-1.8.0b6/chia/full_node/full_node_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     @api_request(peer_required=True, reply_types=[ProtocolMessageTypes.respond_peers])
     async def request_peers(
         self, _request: full_node_protocol.RequestPeers, peer: WSChiaConnection
     ) -> Optional[Message]:
         if peer.peer_server_port is None:
             return None
-        peer_info = PeerInfo(peer.peer_host, peer.peer_server_port)
+        peer_info = PeerInfo(peer.peer_info.host, peer.peer_server_port)
         if self.full_node.full_node_peers is not None:
             msg = await self.full_node.full_node_peers.request_peers(peer_info)
             return msg
         return None
 
     @api_request(peer_required=True)
     async def respond_peers(
@@ -128,14 +128,15 @@
         """
         # this semaphore limits the number of tasks that can call new_peak() at
         # the same time, since it can be expensive
         try:
             async with self.full_node.new_peak_sem.acquire():
                 await self.full_node.new_peak(request, peer)
         except LimitedSemaphoreFullError:
+            self.log.debug("Ignoring NewPeak, limited semaphore full: %s %s", peer.get_peer_logging(), request)
             return None
 
         return None
 
     @api_request(peer_required=True)
     async def new_transaction(
         self, transaction: full_node_protocol.NewTransaction, peer: WSChiaConnection
@@ -750,17 +751,16 @@
                             curr_l_tb.header_hash
                         )
                     except Exception as e:
                         self.log.error(f"Traceback: {traceback.format_exc()}")
                         self.full_node.log.error(f"Error making spend bundle {e} peak: {peak}")
                         mempool_bundle = None
                     if mempool_bundle is not None:
-                        spend_bundle = mempool_bundle[0]
-                        additions = mempool_bundle[1]
-                        removals = mempool_bundle[2]
+                        spend_bundle, additions = mempool_bundle
+                        removals = spend_bundle.removals()
                         self.full_node.log.info(f"Add rem: {len(additions)} {len(removals)}")
                         aggregate_signature = spend_bundle.aggregated_signature
                         if self.full_node.full_node_store.previous_generator is not None:
                             self.log.info(
                                 f"Using previous generator for height "
                                 f"{self.full_node.full_node_store.previous_generator}"
                             )
@@ -1413,28 +1413,28 @@
         self, request: full_node_protocol.NewCompactVDF, peer: WSChiaConnection, request_bytes: bytes = b""
     ) -> None:
         if self.full_node.sync_store.get_sync_mode():
             return None
 
         name = std_hash(request_bytes)
         if name in self.full_node.compact_vdf_requests:
-            self.log.debug(f"Ignoring NewCompactVDF: {request}, already requested")
+            self.log.debug("Ignoring NewCompactVDF, already requested: %s %s", peer.get_peer_logging(), request)
             return None
         self.full_node.compact_vdf_requests.add(name)
 
         # this semaphore will only allow a limited number of tasks call
         # new_compact_vdf() at a time, since it can be expensive
         try:
             async with self.full_node.compact_vdf_sem.acquire():
                 try:
                     await self.full_node.new_compact_vdf(request, peer)
                 finally:
                     self.full_node.compact_vdf_requests.remove(name)
         except LimitedSemaphoreFullError:
-            self.log.debug(f"Ignoring NewCompactVDF: {request}, _waiters")
+            self.log.debug("Ignoring NewCompactVDF, limited semaphore full: %s %s", peer.get_peer_logging(), request)
             return None
 
         return None
 
     @api_request(peer_required=True, reply_types=[ProtocolMessageTypes.respond_compact_vdf])
     async def request_compact_vdf(self, request: full_node_protocol.RequestCompactVDF, peer: WSChiaConnection) -> None:
         if self.full_node.sync_store.get_sync_mode():
```

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/full_node_store.py` & `chia-blockchain-1.8.0b6/chia/full_node/full_node_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/generator.py` & `chia-blockchain-1.8.0b6/chia/full_node/generator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/hint_management.py` & `chia-blockchain-1.8.0b6/chia/full_node/hint_management.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/hint_store.py` & `chia-blockchain-1.8.0b6/chia/full_node/hint_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/lock_queue.py` & `chia-blockchain-1.8.0b6/chia/full_node/lock_queue.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/mempool.py` & `chia-blockchain-1.8.0b6/chia/full_node/mempool.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from chia.full_node.fee_estimator_interface import FeeEstimatorInterface
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.types.clvm_cost import CLVMCost
 from chia.types.mempool_item import MempoolItem
 from chia.types.spend_bundle import SpendBundle
 from chia.util.chunks import chunks
 from chia.util.db_wrapper import SQLITE_MAX_VARIABLE_NUMBER
+from chia.util.errors import Err
 from chia.util.ints import uint32, uint64
 
 log = logging.getLogger(__name__)
 
 # We impose a limit on the fee a single transaction can pay in order to have the
 # sum of all fees in the mempool be less than 2^63. That's the limit of sqlite's
 # integers, which we rely on for computing fee per cost as well as the fee sum
@@ -47,17 +48,23 @@
 
 class Mempool:
     _db_conn: sqlite3.Connection
     # it's expensive to serialize and deserialize G2Element, so we keep those in
     # this separate dictionary
     _items: Dict[bytes32, InternalMempoolItem]
 
+    # the most recent block height and timestamp that we know of
+    _block_height: uint32
+    _timestamp: uint64
+
     def __init__(self, mempool_info: MempoolInfo, fee_estimator: FeeEstimatorInterface):
         self._db_conn = sqlite3.connect(":memory:")
         self._items = {}
+        self._block_height = uint32(0)
+        self._timestamp = uint64(0)
 
         with self._db_conn:
             # name means SpendBundle hash
             # assert_height may be NIL
             generated = ""
             if not SQLITE_NO_GENERATED_COLUMNS:
                 generated = " GENERATED ALWAYS AS (CAST(fee AS REAL) / cost) VIRTUAL"
@@ -77,18 +84,16 @@
                 """
             )
             self._db_conn.execute("CREATE INDEX name_idx ON tx(name)")
             self._db_conn.execute("CREATE INDEX fee_sum ON tx(fee)")
             self._db_conn.execute("CREATE INDEX cost_sum ON tx(cost)")
             self._db_conn.execute("CREATE INDEX feerate ON tx(fee_per_cost)")
             self._db_conn.execute(
-                "CREATE INDEX assert_before_height ON tx(assert_before_height) WHERE assert_before_height != NULL"
-            )
-            self._db_conn.execute(
-                "CREATE INDEX assert_before_seconds ON tx(assert_before_seconds) WHERE assert_before_seconds != NULL"
+                "CREATE INDEX assert_before ON tx(assert_before_height, assert_before_seconds) "
+                "WHERE assert_before_height IS NOT NULL OR assert_before_seconds IS NOT NULL"
             )
 
             # This table maps coin IDs to spend bundles hashes
             self._db_conn.execute(
                 """CREATE TABLE spends(
                 coin_id BLOB NOT NULL,
                 tx BLOB NOT NULL,
@@ -212,14 +217,16 @@
             cursor = self._db_conn.execute(
                 "SELECT name FROM tx WHERE assert_before_seconds <= ? OR assert_before_height <= ?",
                 (timestamp, block_height),
             )
             to_remove = [bytes32(row[0]) for row in cursor]
 
         self.remove_from_pool(to_remove, MempoolRemoveReason.EXPIRED)
+        self._block_height = block_height
+        self._timestamp = timestamp
 
     def remove_from_pool(self, items: List[bytes32], reason: MempoolRemoveReason) -> None:
         """
         Removes an item from the mempool.
         """
         if items == []:
             return
@@ -250,39 +257,77 @@
         if reason != MempoolRemoveReason.BLOCK_INCLUSION:
             info = FeeMempoolInfo(
                 self.mempool_info, self.total_mempool_cost(), self.total_mempool_fees(), datetime.now()
             )
             for iteminfo in removed_items:
                 self.fee_estimator.remove_mempool_item(info, iteminfo)
 
-    def add_to_pool(self, item: MempoolItem) -> None:
+    def add_to_pool(self, item: MempoolItem) -> Optional[Err]:
         """
         Adds an item to the mempool by kicking out transactions (if it doesn't fit), in order of increasing fee per cost
         """
 
         assert item.fee < MEMPOOL_ITEM_FEE_LIMIT
         assert item.npc_result.conds is not None
         assert item.cost <= self.mempool_info.max_block_clvm_cost
 
         with self._db_conn:
+            # we have certain limits on transactions that will expire soon
+            # (in the next 15 minutes)
+            block_cutoff = self._block_height + 48
+            time_cutoff = self._timestamp + 900
+            if (item.assert_before_height is not None and item.assert_before_height < block_cutoff) or (
+                item.assert_before_seconds is not None and item.assert_before_seconds < time_cutoff
+            ):
+                # this lists only transactions that expire soon, in order of
+                # lowest fee rate along with the cumulative cost of such
+                # transactions counting from highest to lowest fee rate
+                cursor = self._db_conn.execute(
+                    """
+                    SELECT name,
+                        fee_per_cost,
+                        SUM(cost) OVER (ORDER BY fee_per_cost DESC, seq ASC) AS cumulative_cost
+                    FROM tx
+                    WHERE assert_before_seconds IS NOT NULL AND assert_before_seconds < ?
+                        OR assert_before_height IS NOT NULL AND assert_before_height < ?
+                    ORDER BY cumulative_cost DESC
+                    """,
+                    (time_cutoff, block_cutoff),
+                )
+                to_remove: List[bytes32] = []
+                for row in cursor:
+                    name, fee_per_cost, cumulative_cost = row
+
+                    # there's space for us, stop pruning
+                    if cumulative_cost + item.cost <= self.mempool_info.max_block_clvm_cost:
+                        break
+
+                    # we can't evict any more transactions, abort (and don't
+                    # evict what we put aside in "to_remove" list)
+                    if fee_per_cost > item.fee_per_cost:
+                        return Err.INVALID_FEE_LOW_FEE
+                    to_remove.append(name)
+                self.remove_from_pool(to_remove, MempoolRemoveReason.EXPIRED)
+                # if we don't find any entries, it's OK to add this entry
+
             total_cost = int(self.total_mempool_cost())
             if total_cost + item.cost > self.mempool_info.max_size_in_cost:
                 # pick the items with the lowest fee per cost to remove
                 cursor = self._db_conn.execute(
                     """SELECT name FROM tx
                     WHERE name NOT IN (
                         SELECT name FROM (
                             SELECT name,
                             SUM(cost) OVER (ORDER BY fee_per_cost DESC, seq ASC) AS total_cost
                             FROM tx) AS tx_with_cost
                         WHERE total_cost <= ?)
                     """,
                     (self.mempool_info.max_size_in_cost - item.cost,),
                 )
-                to_remove: List[bytes32] = [bytes32(row[0]) for row in cursor]
+                to_remove = [bytes32(row[0]) for row in cursor]
                 self.remove_from_pool(to_remove, MempoolRemoveReason.POOL_FULL)
 
             if SQLITE_NO_GENERATED_COLUMNS:
                 self._db_conn.execute(
                     "INSERT INTO "
                     "tx(name,cost,fee,assert_height,assert_before_height,assert_before_seconds,fee_per_cost) "
                     "VALUES(?, ?, ?, ?, ?, ?, ?)",
@@ -316,50 +361,49 @@
 
             self._items[item.name] = InternalMempoolItem(
                 item.spend_bundle, item.npc_result, item.height_added_to_mempool
             )
 
         info = FeeMempoolInfo(self.mempool_info, self.total_mempool_cost(), self.total_mempool_fees(), datetime.now())
         self.fee_estimator.add_mempool_item(info, MempoolItemInfo(item.cost, item.fee, item.height_added_to_mempool))
+        return None
 
     def at_full_capacity(self, cost: int) -> bool:
         """
         Checks whether the mempool is at full capacity and cannot accept a transaction with size cost.
         """
 
         return self.total_mempool_cost() + cost > self.mempool_info.max_size_in_cost
 
     def create_bundle_from_mempool_items(
         self, item_inclusion_filter: Callable[[bytes32], bool]
-    ) -> Optional[Tuple[SpendBundle, List[Coin], List[Coin]]]:
+    ) -> Optional[Tuple[SpendBundle, List[Coin]]]:
         cost_sum = 0  # Checks that total cost does not exceed block maximum
         fee_sum = 0  # Checks that total fees don't exceed 64 bits
         spend_bundles: List[SpendBundle] = []
-        removals: List[Coin] = []
         additions: List[Coin] = []
         log.info(f"Starting to make block, max cost: {self.mempool_info.max_block_clvm_cost}")
         for item in self.spends_by_feerate():
             if not item_inclusion_filter(item.name):
                 continue
             log.info("Cumulative cost: %d, fee per cost: %0.4f", cost_sum, item.fee_per_cost)
             if (
                 item.cost + cost_sum > self.mempool_info.max_block_clvm_cost
                 or item.fee + fee_sum > DEFAULT_CONSTANTS.MAX_COIN_AMOUNT
             ):
                 break
             spend_bundles.append(item.spend_bundle)
             cost_sum += item.cost
             fee_sum += item.fee
-            removals.extend(item.removals)
             if item.npc_result.conds is not None:
                 for spend in item.npc_result.conds.spends:
                     for puzzle_hash, amount, _ in spend.create_coin:
                         coin = Coin(spend.coin_id, puzzle_hash, amount)
                         additions.append(coin)
         if len(spend_bundles) == 0:
             return None
         log.info(
             f"Cumulative cost of block (real cost should be less) {cost_sum}. Proportion "
             f"full: {cost_sum / self.mempool_info.max_block_clvm_cost}"
         )
         agg = SpendBundle.aggregate(spend_bundles)
-        return agg, additions, removals
+        return agg, additions
```

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/mempool_check_conditions.py` & `chia-blockchain-1.8.0b6/chia/full_node/mempool_check_conditions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/mempool_manager.py` & `chia-blockchain-1.8.0b6/chia/full_node/mempool_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,18 +206,16 @@
         )
         self.mempool: Mempool = Mempool(mempool_info, self.fee_estimator)
 
     def shut_down(self) -> None:
         self.pool.shutdown(wait=True)
 
     def create_bundle_from_mempool(
-        self,
-        last_tb_header_hash: bytes32,
-        item_inclusion_filter: Optional[Callable[[bytes32], bool]] = None,
-    ) -> Optional[Tuple[SpendBundle, List[Coin], List[Coin]]]:
+        self, last_tb_header_hash: bytes32, item_inclusion_filter: Optional[Callable[[bytes32], bool]] = None
+    ) -> Optional[Tuple[SpendBundle, List[Coin]]]:
         """
         Returns aggregated spendbundle that can be used for creating new block,
         additions and removals in that spend_bundle
         """
         if self.peak is None or self.peak.header_hash != last_tb_header_hash:
             return None
         if item_inclusion_filter is None:
@@ -333,15 +331,17 @@
         err, item, remove_items = await self.validate_spend_bundle(
             new_spend, npc_result, spend_name, first_added_height
         )
         if err is None:
             # No error, immediately add to mempool, after removing conflicting TXs.
             assert item is not None
             self.mempool.remove_from_pool(remove_items, MempoolRemoveReason.CONFLICT)
-            self.mempool.add_to_pool(item)
+            err = self.mempool.add_to_pool(item)
+            if err is not None:
+                return item.cost, MempoolInclusionStatus.FAILED, err
             return item.cost, MempoolInclusionStatus.SUCCESS, None
         elif err is Err.MEMPOOL_CONFLICT and item is not None:
             # The transaction has a conflict with another item in the
             # mempool, put it aside and re-try it later
             self._conflict_cache.add(item)
             return item.cost, MempoolInclusionStatus.PENDING, err
         elif item is not None:
```

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/pending_tx_cache.py` & `chia-blockchain-1.8.0b6/chia/full_node/pending_tx_cache.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/subscriptions.py` & `chia-blockchain-1.8.0b6/chia/full_node/subscriptions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/sync_store.py` & `chia-blockchain-1.8.0b6/chia/full_node/sync_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/tx_processing_queue.py` & `chia-blockchain-1.8.0b6/chia/full_node/tx_processing_queue.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/full_node/weight_proof.py` & `chia-blockchain-1.8.0b6/chia/full_node/weight_proof.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/harvester/harvester.py` & `chia-blockchain-1.8.0b6/chia/harvester/harvester.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/harvester/harvester_api.py` & `chia-blockchain-1.8.0b6/chia/harvester/harvester_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/introducer/introducer.py` & `chia-blockchain-1.8.0b6/chia/introducer/introducer.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/introducer/introducer_api.py` & `chia-blockchain-1.8.0b6/chia/introducer/introducer_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         )
 
         peers = []
         for r_peer in rawpeers:
             if r_peer.vetted <= 0:
                 continue
 
-            if r_peer.host == peer.peer_host and r_peer.port == peer.peer_server_port:
+            if r_peer.host == peer.peer_info.host and r_peer.port == peer.peer_server_port:
                 continue
             peer_without_timestamp = TimestampedPeerInfo(
                 r_peer.host,
                 r_peer.port,
                 uint64(0),
             )
             peers.append(peer_without_timestamp)
```

### Comparing `chia-blockchain-1.8.0b5/chia/plot_sync/delta.py` & `chia-blockchain-1.8.0b6/chia/plot_sync/delta.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plot_sync/exceptions.py` & `chia-blockchain-1.8.0b6/chia/plot_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plot_sync/receiver.py` & `chia-blockchain-1.8.0b6/chia/plot_sync/receiver.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,16 +345,16 @@
                 "initial": self.initial_sync(),
                 "plot_files_processed": self._current_sync.plots_processed,
                 "plot_files_total": self._current_sync.plots_total,
             }
         return {
             "connection": {
                 "node_id": self._connection.peer_node_id,
-                "host": self._connection.peer_host,
-                "port": self._connection.peer_port,
+                "host": self._connection.peer_info.host,
+                "port": self._connection.peer_info.port,
             },
             "plots": get_list_or_len(list(self._plots.values()), counts_only),
             "failed_to_open_filenames": get_list_or_len(self._invalid, counts_only),
             "no_key_filenames": get_list_or_len(self._keys_missing, counts_only),
             "duplicates": get_list_or_len(self._duplicates, counts_only),
             "total_plot_size": self._total_plot_size,
             "syncing": syncing,
```

### Comparing `chia-blockchain-1.8.0b5/chia/plot_sync/sender.py` & `chia-blockchain-1.8.0b6/chia/plot_sync/sender.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plot_sync/util.py` & `chia-blockchain-1.8.0b6/chia/plot_sync/util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plotters/bladebit.py` & `chia-blockchain-1.8.0b6/chia/plotters/bladebit.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plotters/chiapos.py` & `chia-blockchain-1.8.0b6/chia/plotters/chiapos.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plotters/madmax.py` & `chia-blockchain-1.8.0b6/chia/plotters/madmax.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plotters/plotters.py` & `chia-blockchain-1.8.0b6/chia/plotters/plotters.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plotters/plotters_util.py` & `chia-blockchain-1.8.0b6/chia/plotters/plotters_util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plotting/cache.py` & `chia-blockchain-1.8.0b6/chia/plotting/cache.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plotting/check_plots.py` & `chia-blockchain-1.8.0b6/chia/plotting/check_plots.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plotting/create_plots.py` & `chia-blockchain-1.8.0b6/chia/plotting/create_plots.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plotting/manager.py` & `chia-blockchain-1.8.0b6/chia/plotting/manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/plotting/util.py` & `chia-blockchain-1.8.0b6/chia/plotting/util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/pools/pool_config.py` & `chia-blockchain-1.8.0b6/chia/pools/pool_config.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/pools/pool_puzzles.py` & `chia-blockchain-1.8.0b6/chia/pools/pool_puzzles.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/pools/pool_wallet.py` & `chia-blockchain-1.8.0b6/chia/pools/pool_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/pools/pool_wallet_info.py` & `chia-blockchain-1.8.0b6/chia/pools/pool_wallet_info.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/protocols/farmer_protocol.py` & `chia-blockchain-1.8.0b6/chia/protocols/farmer_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/protocols/full_node_protocol.py` & `chia-blockchain-1.8.0b6/chia/protocols/full_node_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/protocols/harvester_protocol.py` & `chia-blockchain-1.8.0b6/chia/protocols/harvester_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/protocols/introducer_protocol.py` & `chia-blockchain-1.8.0b6/chia/protocols/introducer_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/protocols/pool_protocol.py` & `chia-blockchain-1.8.0b6/chia/protocols/pool_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/protocols/protocol_message_types.py` & `chia-blockchain-1.8.0b6/chia/protocols/protocol_message_types.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/protocols/protocol_state_machine.py` & `chia-blockchain-1.8.0b6/chia/protocols/protocol_state_machine.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/protocols/shared_protocol.py` & `chia-blockchain-1.8.0b6/chia/protocols/shared_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/protocols/timelord_protocol.py` & `chia-blockchain-1.8.0b6/chia/protocols/timelord_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/protocols/wallet_protocol.py` & `chia-blockchain-1.8.0b6/chia/protocols/wallet_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/pyinstaller.spec` & `chia-blockchain-1.8.0b6/chia/pyinstaller.spec`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,15 @@
 
 for server in SERVERS:
     add_binary(f"start_{server}", f"{ROOT}/chia/server/start_{server}.py", COLLECT_ARGS)
 
 add_binary("start_crawler", f"{ROOT}/chia/seeder/start_crawler.py", COLLECT_ARGS)
 add_binary("start_seeder", f"{ROOT}/chia/seeder/dns_server.py", COLLECT_ARGS)
 add_binary("start_data_layer_http", f"{ROOT}/chia/data_layer/data_layer_server.py", COLLECT_ARGS)
+add_binary("start_data_layer_s3_plugin", f"{ROOT}/chia/data_layer/s3_plugin_service.py", COLLECT_ARGS)
 
 COLLECT_KWARGS = dict(
     strip=False,
     upx_exclude=[],
     name="daemon",
 )
```

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/crawler_rpc_api.py` & `chia-blockchain-1.8.0b6/chia/rpc/crawler_rpc_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/data_layer_rpc_api.py` & `chia-blockchain-1.8.0b6/chia/rpc/data_layer_rpc_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/data_layer_rpc_client.py` & `chia-blockchain-1.8.0b6/chia/rpc/data_layer_rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/data_layer_rpc_util.py` & `chia-blockchain-1.8.0b6/chia/rpc/data_layer_rpc_util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/farmer_rpc_api.py` & `chia-blockchain-1.8.0b6/chia/rpc/farmer_rpc_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/farmer_rpc_client.py` & `chia-blockchain-1.8.0b6/chia/rpc/farmer_rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/full_node_rpc_api.py` & `chia-blockchain-1.8.0b6/chia/rpc/full_node_rpc_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -806,14 +806,15 @@
             estimator.estimate_fee_rate(time_offset_seconds=time).mojos_per_clvm_cost * spend_cost
             for time in target_times
         ]
         # The Bitcoin Fee Estimator works by observing the most common fee rates that appear
         # at set times into the future. This can lead to situations that users do not expect,
         # such as estimating a higher fee for a longer transaction time.
         estimates = make_monotonically_decreasing(estimates)
+        estimates = [uint64(e) for e in estimates]
         current_fee_rate = estimator.estimate_fee_rate(time_offset_seconds=1)
         mempool_size = self.service.mempool_manager.mempool.total_mempool_cost()
         mempool_fees = self.service.mempool_manager.mempool.total_mempool_fees()
         num_mempool_spends = self.service.mempool_manager.mempool.size()
         mempool_max_size = estimator.mempool_max_size()
         blockchain_state = await self.get_blockchain_state({})
         synced = blockchain_state["blockchain_state"]["sync"]["synced"]
```

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/full_node_rpc_client.py` & `chia-blockchain-1.8.0b6/chia/rpc/full_node_rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/harvester_rpc_api.py` & `chia-blockchain-1.8.0b6/chia/rpc/harvester_rpc_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/harvester_rpc_client.py` & `chia-blockchain-1.8.0b6/chia/rpc/harvester_rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/rpc_client.py` & `chia-blockchain-1.8.0b6/chia/rpc/rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/rpc_server.py` & `chia-blockchain-1.8.0b6/chia/rpc/rpc_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,16 +116,16 @@
 
 def default_get_connections(server: ChiaServer, request_node_type: Optional[NodeType]) -> List[Dict[str, Any]]:
     connections = server.get_connections(request_node_type)
     con_info = [
         {
             "type": con.connection_type,
             "local_port": con.local_port,
-            "peer_host": con.peer_host,
-            "peer_port": con.peer_port,
+            "peer_host": con.peer_info.host,
+            "peer_port": con.peer_info.port,
             "peer_server_port": con.peer_server_port,
             "node_id": con.peer_node_id,
             "creation_time": con.creation_time,
             "bytes_read": con.bytes_read,
             "bytes_written": con.bytes_written,
             "last_message_time": con.last_message_time,
         }
```

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/timelord_rpc_api.py` & `chia-blockchain-1.8.0b6/chia/rpc/timelord_rpc_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/util.py` & `chia-blockchain-1.8.0b6/chia/rpc/util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/wallet_rpc_api.py` & `chia-blockchain-1.8.0b6/chia/rpc/wallet_rpc_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 from chia.wallet.nft_wallet.nft_puzzles import get_metadata_and_phs
 from chia.wallet.nft_wallet.nft_wallet import NFTWallet
 from chia.wallet.nft_wallet.uncurry_nft import UncurriedNFT
 from chia.wallet.notification_store import Notification
 from chia.wallet.outer_puzzles import AssetType
 from chia.wallet.puzzle_drivers import PuzzleInfo, Solver
 from chia.wallet.puzzles.p2_delegated_puzzle_or_hidden_puzzle import puzzle_hash_for_synthetic_public_key
-from chia.wallet.singleton import create_fullpuz
+from chia.wallet.singleton import create_singleton_puzzle
 from chia.wallet.trade_record import TradeRecord
 from chia.wallet.trading.offer import Offer
 from chia.wallet.transaction_record import TransactionRecord
 from chia.wallet.uncurried_puzzle import uncurry_puzzle
 from chia.wallet.util.address_type import AddressType, is_valid_address
 from chia.wallet.util.compute_hints import compute_coin_hints
 from chia.wallet.util.compute_memos import compute_memos
@@ -1889,50 +1889,50 @@
         else:
             our_inner_puzzle: Program = self.service.wallet_state_manager.main_wallet.puzzle_for_pk(
                 derivation_record.pubkey
             )
             did_puzzle = DID_INNERPUZ_MOD.curry(
                 our_inner_puzzle, recovery_list_hash, num_verification, singleton_struct, metadata
             )
-            full_puzzle = create_fullpuz(did_puzzle, launcher_id)
+            full_puzzle = create_singleton_puzzle(did_puzzle, launcher_id)
             did_puzzle_empty_recovery = DID_INNERPUZ_MOD.curry(
                 our_inner_puzzle, Program.to([]).get_tree_hash(), uint64(0), singleton_struct, metadata
             )
             # Check if we have the DID wallet
             did_wallet: Optional[DIDWallet] = None
             for wallet in self.service.wallet_state_manager.wallets.values():
                 if isinstance(wallet, DIDWallet):
                     assert wallet.did_info.origin_coin is not None
                     if wallet.did_info.origin_coin.name() == launcher_id:
                         did_wallet = wallet
                         break
 
-            full_puzzle_empty_recovery = create_fullpuz(did_puzzle_empty_recovery, launcher_id)
+            full_puzzle_empty_recovery = create_singleton_puzzle(did_puzzle_empty_recovery, launcher_id)
             if full_puzzle.get_tree_hash() != coin_state.coin.puzzle_hash:
                 if full_puzzle_empty_recovery.get_tree_hash() == coin_state.coin.puzzle_hash:
                     did_puzzle = did_puzzle_empty_recovery
                 elif (
                     did_wallet is not None
                     and did_wallet.did_info.current_inner is not None
-                    and create_fullpuz(did_wallet.did_info.current_inner, launcher_id).get_tree_hash()
+                    and create_singleton_puzzle(did_wallet.did_info.current_inner, launcher_id).get_tree_hash()
                     == coin_state.coin.puzzle_hash
                 ):
                     # Check if the old wallet has the inner puzzle
                     did_puzzle = did_wallet.did_info.current_inner
                 else:
                     # Try override
                     if "recovery_list_hash" in request:
                         recovery_list_hash = Program.from_bytes(bytes.fromhex(request["recovery_list_hash"]))
                     num_verification = request.get("num_verification", num_verification)
                     if "metadata" in request:
                         metadata = metadata_to_program(request["metadata"])
                     did_puzzle = DID_INNERPUZ_MOD.curry(
                         our_inner_puzzle, recovery_list_hash, num_verification, singleton_struct, metadata
                     )
-                    full_puzzle = create_fullpuz(did_puzzle, launcher_id)
+                    full_puzzle = create_singleton_puzzle(did_puzzle, launcher_id)
                     matched = True
                     if full_puzzle.get_tree_hash() != coin_state.coin.puzzle_hash:
                         matched = False
                         # Brute force addresses
                         index = 0
                         derivation_record = await self.service.wallet_state_manager.puzzle_store.get_derivation_record(
                             uint32(index), uint32(1), False
@@ -1940,15 +1940,15 @@
                         while derivation_record is not None:
                             our_inner_puzzle = self.service.wallet_state_manager.main_wallet.puzzle_for_pk(
                                 derivation_record.pubkey
                             )
                             did_puzzle = DID_INNERPUZ_MOD.curry(
                                 our_inner_puzzle, recovery_list_hash, num_verification, singleton_struct, metadata
                             )
-                            full_puzzle = create_fullpuz(did_puzzle, launcher_id)
+                            full_puzzle = create_singleton_puzzle(did_puzzle, launcher_id)
                             if full_puzzle.get_tree_hash() == coin_state.coin.puzzle_hash:
                                 matched = True
                                 break
                             index += 1
                             derivation_record = (
                                 await self.service.wallet_state_manager.puzzle_store.get_derivation_record(
                                     uint32(index), uint32(1), False
```

### Comparing `chia-blockchain-1.8.0b5/chia/rpc/wallet_rpc_client.py` & `chia-blockchain-1.8.0b6/chia/rpc/wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/seeder/crawl_store.py` & `chia-blockchain-1.8.0b6/chia/seeder/crawl_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/seeder/crawler.py` & `chia-blockchain-1.8.0b6/chia/seeder/crawler.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/seeder/crawler_api.py` & `chia-blockchain-1.8.0b6/chia/seeder/crawler_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/seeder/dns_server.py` & `chia-blockchain-1.8.0b6/chia/seeder/dns_server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/seeder/peer_record.py` & `chia-blockchain-1.8.0b6/chia/seeder/peer_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/seeder/start_crawler.py` & `chia-blockchain-1.8.0b6/chia/seeder/start_crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         config=config,
         node=api.crawler,
         peer_api=api,
         node_type=NodeType.FULL_NODE,
         advertised_port=service_config["port"],
         service_name="full_node",
         upnp_ports=[],
-        server_listen_ports=[service_config["port"]],
         on_connect_callback=crawler.on_connect,
         network_id=network_id,
         rpc_info=rpc_info,
         connect_to_daemon=connect_to_daemon,
     )
```

### Comparing `chia-blockchain-1.8.0b5/chia/server/address_manager.py` & `chia-blockchain-1.8.0b6/chia/server/address_manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/server/address_manager_sqlite_store.py` & `chia-blockchain-1.8.0b6/chia/server/address_manager_sqlite_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/server/address_manager_store.py` & `chia-blockchain-1.8.0b6/chia/server/address_manager_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/server/capabilities.py` & `chia-blockchain-1.8.0b6/chia/server/capabilities.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/server/chia_policy.py` & `chia-blockchain-1.8.0b6/chia/server/chia_policy.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/server/introducer_peers.py` & `chia-blockchain-1.8.0b6/chia/server/introducer_peers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/server/node_discovery.py` & `chia-blockchain-1.8.0b6/chia/server/node_discovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             peer.is_outbound is False
             and peer.peer_server_port is not None
             and peer.connection_type is NodeType.FULL_NODE
             and self.server._local_type is NodeType.FULL_NODE
             and self.address_manager is not None
         ):
             timestamped_peer_info = TimestampedPeerInfo(
-                peer.peer_host,
+                peer.peer_info.host,
                 peer.peer_server_port,
                 uint64(int(time.time())),
             )
             await self.address_manager.add_to_new_table([timestamped_peer_info], peer.get_peer_info(), 0)
             if self.relay_queue is not None:
                 self.relay_queue.put_nowait((timestamped_peer_info, 1))
         if (
```

### Comparing `chia-blockchain-1.8.0b5/chia/server/outbound_message.py` & `chia-blockchain-1.8.0b6/chia/server/outbound_message.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/server/peer_store_resolver.py` & `chia-blockchain-1.8.0b6/chia/server/peer_store_resolver.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/server/rate_limit_numbers.py` & `chia-blockchain-1.8.0b6/chia/server/rate_limit_numbers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/server/rate_limits.py` & `chia-blockchain-1.8.0b6/chia/server/rate_limits.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/server/server.py` & `chia-blockchain-1.8.0b6/chia/server/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,31 +32,31 @@
 from chia.server.outbound_message import Message, NodeType
 from chia.server.ssl_context import private_ssl_paths, public_ssl_paths
 from chia.server.ws_connection import ConnectionCallback, WSChiaConnection
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.types.peer_info import PeerInfo
 from chia.util.errors import Err, ProtocolError
 from chia.util.ints import uint16
-from chia.util.network import WebServer, is_in_network, is_localhost
+from chia.util.network import WebServer, is_in_network, is_localhost, is_trusted_peer
 from chia.util.ssl_check import verify_ssl_certs_and_keys
 
 max_message_size = 50 * 1024 * 1024  # 50MB
 
 
 def ssl_context_for_server(
     ca_cert: Path,
     ca_key: Path,
-    private_cert_path: Path,
-    private_key_path: Path,
+    cert_path: Path,
+    key_path: Path,
     *,
     check_permissions: bool = True,
     log: Optional[logging.Logger] = None,
 ) -> ssl.SSLContext:
     if check_permissions:
-        verify_ssl_certs_and_keys([ca_cert, private_cert_path], [ca_key, private_key_path], log)
+        verify_ssl_certs_and_keys([ca_cert, cert_path], [ca_key, key_path], log)
 
     ssl_context = ssl._create_unverified_context(purpose=ssl.Purpose.CLIENT_AUTH, cafile=str(ca_cert))
     ssl_context.check_hostname = False
     ssl_context.minimum_version = ssl.TLSVersion.TLSv1_2
     ssl_context.set_ciphers(
         (
             "ECDHE-ECDSA-AES256-GCM-SHA384:"
@@ -67,15 +67,15 @@
             "ECDHE-RSA-AES128-GCM-SHA256:"
             "ECDHE-ECDSA-AES256-SHA384:"
             "ECDHE-RSA-AES256-SHA384:"
             "ECDHE-ECDSA-AES128-SHA256:"
             "ECDHE-RSA-AES128-SHA256"
         )
     )
-    ssl_context.load_cert_chain(certfile=str(private_cert_path), keyfile=str(private_key_path))
+    ssl_context.load_cert_chain(certfile=str(cert_path), keyfile=str(key_path))
     ssl_context.verify_mode = ssl.CERT_REQUIRED
     return ssl_context
 
 
 def ssl_context_for_root(
     ca_cert_file: str, *, check_permissions: bool = True, log: Optional[logging.Logger] = None
 ) -> ssl.SSLContext:
@@ -85,26 +85,26 @@
     ssl_context = ssl.create_default_context(purpose=ssl.Purpose.SERVER_AUTH, cafile=ca_cert_file)
     return ssl_context
 
 
 def ssl_context_for_client(
     ca_cert: Path,
     ca_key: Path,
-    private_cert_path: Path,
-    private_key_path: Path,
+    cert_path: Path,
+    key_path: Path,
     *,
     check_permissions: bool = True,
     log: Optional[logging.Logger] = None,
 ) -> ssl.SSLContext:
     if check_permissions:
-        verify_ssl_certs_and_keys([ca_cert, private_cert_path], [ca_key, private_key_path], log)
+        verify_ssl_certs_and_keys([ca_cert, cert_path], [ca_key, key_path], log)
 
     ssl_context = ssl._create_unverified_context(purpose=ssl.Purpose.SERVER_AUTH, cafile=str(ca_cert))
     ssl_context.check_hostname = False
-    ssl_context.load_cert_chain(certfile=str(private_cert_path), keyfile=str(private_key_path))
+    ssl_context.load_cert_chain(certfile=str(cert_path), keyfile=str(key_path))
     ssl_context.verify_mode = ssl.CERT_REQUIRED
     return ssl_context
 
 
 def calculate_node_id(cert_path: Path) -> bytes32:
     pem_cert = x509.load_pem_x509_certificate(cert_path.read_bytes(), default_backend())
     der_cert_bytes = pem_cert.public_bytes(encoding=serialization.Encoding.DER)
@@ -172,38 +172,48 @@
         authenticated_client_types = {NodeType.HARVESTER}
         authenticated_server_types = {NodeType.HARVESTER, NodeType.FARMER, NodeType.WALLET, NodeType.DATA_LAYER}
 
         if local_type in authenticated_client_types:
             # Authenticated clients
             private_cert_path, private_key_path = private_ssl_paths(root_path, config)
             ssl_client_context = ssl_context_for_client(
-                ca_private_crt_path, ca_private_key_path, private_cert_path, private_key_path
+                ca_cert=ca_private_crt_path,
+                ca_key=ca_private_key_path,
+                cert_path=private_cert_path,
+                key_path=private_key_path,
             )
         else:
             # Public clients
             public_cert_path, public_key_path = public_ssl_paths(root_path, config)
             ssl_client_context = ssl_context_for_client(
-                chia_ca_crt_path, chia_ca_key_path, public_cert_path, public_key_path
+                ca_cert=chia_ca_crt_path,
+                ca_key=chia_ca_key_path,
+                cert_path=public_cert_path,
+                key_path=public_key_path,
             )
 
         if local_type in authenticated_server_types:
             # Authenticated servers
             private_cert_path, private_key_path = private_ssl_paths(root_path, config)
             ssl_context = ssl_context_for_server(
-                ca_private_crt_path,
-                ca_private_key_path,
-                private_cert_path,
-                private_key_path,
+                ca_cert=ca_private_crt_path,
+                ca_key=ca_private_key_path,
+                cert_path=private_cert_path,
+                key_path=private_key_path,
                 log=log,
             )
         else:
             # Public servers
             public_cert_path, public_key_path = public_ssl_paths(root_path, config)
             ssl_context = ssl_context_for_server(
-                chia_ca_crt_path, chia_ca_key_path, public_cert_path, public_key_path, log=log
+                ca_cert=chia_ca_crt_path,
+                ca_key=chia_ca_key_path,
+                cert_path=public_cert_path,
+                key_path=public_key_path,
+                log=log,
             )
 
         node_id_cert_path = private_cert_path if public_cert_path is None else public_cert_path
         assert node_id_cert_path is not None
 
         return cls(
             _port=port,
@@ -246,48 +256,51 @@
                     if is_crawler is not None:
                         if time.time() - connection.creation_time > 5:
                             to_remove.append(connection)
                     else:
                         if time.time() - connection.last_message_time > 1800:
                             to_remove.append(connection)
             for connection in to_remove:
-                self.log.debug(f"Garbage collecting connection {connection.peer_host} due to inactivity")
+                self.log.debug(f"Garbage collecting connection {connection.peer_info.host} due to inactivity")
                 if connection.closed:
                     self.all_connections.pop(connection.peer_node_id)
                 else:
                     await connection.close()
 
             # Also garbage collect banned_peers dict
             to_remove_ban = []
             for peer_ip, ban_until_time in self.banned_peers.items():
                 if time.time() > ban_until_time:
                     to_remove_ban.append(peer_ip)
             for peer_ip in to_remove_ban:
                 del self.banned_peers[peer_ip]
 
-    async def start_server(self, prefer_ipv6: bool, on_connect: Optional[ConnectionCallback] = None) -> None:
+    async def start(
+        self,
+        listen: bool,
+        prefer_ipv6: bool,
+        on_connect: Optional[ConnectionCallback] = None,
+    ) -> None:
         if self.webserver is not None:
             raise RuntimeError("ChiaServer already started")
         if self.gc_task is None:
             self.gc_task = asyncio.create_task(self.garbage_collect_connections_task())
 
-        if self._local_type in [NodeType.WALLET, NodeType.HARVESTER, NodeType.TIMELORD]:
-            return None
-
-        self.on_connect = on_connect
-        self.webserver = await WebServer.create(
-            hostname="",
-            port=uint16(self._port),
-            routes=[web.get("/ws", self.incoming_connection)],
-            ssl_context=self.ssl_context,
-            prefer_ipv6=prefer_ipv6,
-            logger=self.log,
-        )
-        self._port = int(self.webserver.listen_port)
-        self.log.info(f"Started listening on port: {self._port}")
+        if listen:
+            self.on_connect = on_connect
+            self.webserver = await WebServer.create(
+                hostname="",
+                port=uint16(self._port),
+                routes=[web.get("/ws", self.incoming_connection)],
+                ssl_context=self.ssl_context,
+                prefer_ipv6=prefer_ipv6,
+                logger=self.log,
+            )
+            self._port = int(self.webserver.listen_port)
+            self.log.info(f"Started listening on port: {self._port}")
 
     async def incoming_connection(self, request: web.Request) -> web.StreamResponse:
         if getattr(self.node, "crawl", None) is not None:
             raise web.HTTPForbidden(reason="incoming connections not allowed for crawler")
         if request.remote is None:
             raise web.HTTPInternalServerError(reason=f"remote is None for request {request}")
         if request.remote in self.banned_peers and time.time() < self.banned_peers[request.remote]:
@@ -305,34 +318,34 @@
         der_cert = x509.load_der_x509_certificate(cert_bytes)
         peer_id = bytes32(der_cert.fingerprint(hashes.SHA256()))
         if peer_id == self.node_id:
             return ws
         connection: Optional[WSChiaConnection] = None
         try:
             connection = WSChiaConnection.create(
-                self._local_type,
-                ws,
-                self.api,
-                self._port,
-                self.log,
-                False,
-                self.received_message_callback,
-                request.remote,
-                self.connection_closed,
-                peer_id,
-                self._inbound_rate_limit_percent,
-                self._outbound_rate_limit_percent,
-                self._local_capabilities_for_handshake,
+                local_type=self._local_type,
+                ws=ws,
+                api=self.api,
+                server_port=self._port,
+                log=self.log,
+                is_outbound=False,
+                received_message_callback=self.received_message_callback,
+                peer_host=request.remote,
+                close_callback=self.connection_closed,
+                peer_id=peer_id,
+                inbound_rate_limit_percent=self._inbound_rate_limit_percent,
+                outbound_rate_limit_percent=self._outbound_rate_limit_percent,
+                local_capabilities_for_handshake=self._local_capabilities_for_handshake,
             )
             await connection.perform_handshake(self._network_id, protocol_version, self._port, self._local_type)
             assert connection.connection_type is not None, "handshake failed to set connection type, still None"
 
             # Limit inbound connections to config's specifications.
             if not self.accept_inbound_connections(connection.connection_type) and not is_in_network(
-                connection.peer_host, self.exempt_peer_networks
+                connection.peer_info.host, self.exempt_peer_networks
             ):
                 self.log.info(
                     f"Not accepting inbound connection: {connection.get_peer_logging()}.Inbound limit reached."
                 )
                 await connection.close()
             else:
                 await self.connection_added(connection, self.on_connect)
@@ -365,15 +378,15 @@
 
     async def connection_added(
         self, connection: WSChiaConnection, on_connect: Optional[ConnectionCallback] = None
     ) -> None:
         # If we already had a connection to this peer_id, close the old one. This is secure because peer_ids are based
         # on TLS public keys
         if connection.closed:
-            self.log.debug(f"ignoring unexpected request to add closed connection {connection.peer_host} ")
+            self.log.debug(f"ignoring unexpected request to add closed connection {connection.peer_info.host} ")
             return
 
         if connection.peer_node_id in self.all_connections:
             con = self.all_connections[connection.peer_node_id]
             await con.close()
         self.all_connections[connection.peer_node_id] = connection
         if connection.connection_type is not None:
@@ -384,15 +397,15 @@
 
     def is_duplicate_or_self_connection(self, target_node: PeerInfo) -> bool:
         if is_localhost(target_node.host) and target_node.port == self._port:
             # Don't connect to self
             self.log.debug(f"Not connecting to {target_node}")
             return True
         for connection in self.all_connections.values():
-            if connection.peer_host == target_node.host and connection.peer_server_port == target_node.port:
+            if connection.peer_info.host == target_node.host and connection.peer_server_port == target_node.port:
                 self.log.debug(f"Not connecting to {target_node}, duplicate connection")
                 return True
         return False
 
     async def start_client(
         self,
         target_node: PeerInfo,
@@ -446,30 +459,31 @@
             ssl_object = ws.get_extra_info("ssl_object")
             if ssl_object is None:
                 raise ValueError(f"ssl_object is None for {ws}")
             cert_bytes = ssl_object.getpeercert(True)
             der_cert = x509.load_der_x509_certificate(cert_bytes, default_backend())
             peer_id = bytes32(der_cert.fingerprint(hashes.SHA256()))
             if peer_id == self.node_id:
-                raise RuntimeError(f"Trying to connect to a peer ({target_node}) with the same peer_id: {peer_id}")
+                self.log.info(f"Connected to a node with the same peer ID, disconnecting: {target_node} {peer_id}")
+                return False
 
             connection = WSChiaConnection.create(
-                self._local_type,
-                ws,
-                self.api,
-                self._port,
-                self.log,
-                True,
-                self.received_message_callback,
-                target_node.host,
-                self.connection_closed,
-                peer_id,
-                self._inbound_rate_limit_percent,
-                self._outbound_rate_limit_percent,
-                self._local_capabilities_for_handshake,
+                local_type=self._local_type,
+                ws=ws,
+                api=self.api,
+                server_port=self._port,
+                log=self.log,
+                is_outbound=True,
+                received_message_callback=self.received_message_callback,
+                peer_host=target_node.host,
+                close_callback=self.connection_closed,
+                peer_id=peer_id,
+                inbound_rate_limit_percent=self._inbound_rate_limit_percent,
+                outbound_rate_limit_percent=self._outbound_rate_limit_percent,
+                local_capabilities_for_handshake=self._local_capabilities_for_handshake,
                 session=session,
             )
             await connection.perform_handshake(self._network_id, protocol_version, self._port, self._local_type)
             await self.connection_added(connection, on_connect)
             # the session has been adopted by the connection, don't close it at
             # the end of the function
             session = None
@@ -506,36 +520,37 @@
         return False
 
     def connection_closed(self, connection: WSChiaConnection, ban_time: int, closed_connection: bool = False) -> None:
         # closed_connection is true if the callback is being called with a connection that was previously closed
         # in this case we still want to do the banning logic and remove the conection from the list
         # but the other cleanup should already have been done so we skip that
 
-        if is_localhost(connection.peer_host) and ban_time != 0:
+        if is_localhost(connection.peer_info.host) and ban_time != 0:
             self.log.warning(f"Trying to ban localhost for {ban_time}, but will not ban")
             ban_time = 0
         if ban_time > 0:
             ban_until: float = time.time() + ban_time
-            self.log.warning(f"Banning {connection.peer_host} for {ban_time} seconds")
-            if connection.peer_host in self.banned_peers:
-                if ban_until > self.banned_peers[connection.peer_host]:
-                    self.banned_peers[connection.peer_host] = ban_until
+            self.log.warning(f"Banning {connection.peer_info.host} for {ban_time} seconds")
+            if connection.peer_info.host in self.banned_peers:
+                if ban_until > self.banned_peers[connection.peer_info.host]:
+                    self.banned_peers[connection.peer_info.host] = ban_until
             else:
-                self.banned_peers[connection.peer_host] = ban_until
+                self.banned_peers[connection.peer_info.host] = ban_until
 
-        if connection.peer_node_id in self.all_connections:
+        present_connection = self.all_connections.get(connection.peer_node_id)
+        if present_connection is connection:
             self.all_connections.pop(connection.peer_node_id)
 
         if not closed_connection:
-            self.log.info(f"Connection closed: {connection.peer_host}, node id: {connection.peer_node_id}")
+            self.log.info(f"Connection closed: {connection.peer_info.host}, node id: {connection.peer_node_id}")
 
             if connection.connection_type is None:
                 # This means the handshake was never finished with this peer
                 self.log.debug(
-                    f"Invalid connection type for connection {connection.peer_host},"
+                    f"Invalid connection type for connection {connection.peer_info.host},"
                     f" while closing. Handshake never finished."
                 )
             connection.cancel_tasks()
             on_disconnect = getattr(self.node, "on_disconnect", None)
             if on_disconnect is not None:
                 on_disconnect(connection)
 
@@ -556,17 +571,17 @@
         for message in messages:
             if message_requires_reply(ProtocolMessageTypes(message.type)):
                 # Internal protocol logic error - we will raise, blocking messages to all peers
                 self.log.error(f"Attempt to broadcast message requiring protocol response: {message.type}")
                 for _, connection in self.all_connections.items():
                     if connection.connection_type is node_type:
                         await connection.close(
-                            self.invalid_protocol_ban_seconds,
-                            WSCloseCode.INTERNAL_ERROR,
-                            Err.INTERNAL_PROTOCOL_ERROR,
+                            ban_time=self.invalid_protocol_ban_seconds,
+                            ws_close_code=WSCloseCode.INTERNAL_ERROR,
+                            error=Err.INTERNAL_PROTOCOL_ERROR,
                         )
                 raise ProtocolError(Err.INTERNAL_PROTOCOL_ERROR, [message.type])
 
     async def send_to_all(
         self,
         messages: List[Message],
         node_type: NodeType,
@@ -670,18 +685,16 @@
         if node_type == NodeType.FARMER:
             return inbound_count < cast(int, self.config["max_inbound_farmer"])
         if node_type == NodeType.TIMELORD:
             return inbound_count < cast(int, self.config["max_inbound_timelord"])
         return True
 
     def is_trusted_peer(self, peer: WSChiaConnection, trusted_peers: Dict[str, Any]) -> bool:
-        if trusted_peers is None:
-            return False
-        if not self.config.get("testing", False) and peer.peer_host == "127.0.0.1":
-            return True
-        if peer.peer_node_id.hex() not in trusted_peers:
-            return False
-
-        return True
+        return is_trusted_peer(
+            host=peer.peer_info.host,
+            node_id=peer.peer_node_id,
+            trusted_peers=trusted_peers,
+            testing=self.config.get("testing", False),
+        )
 
     def set_capabilities(self, capabilities: List[Tuple[uint16, str]]) -> None:
         self._local_capabilities_for_handshake = capabilities
```

### Comparing `chia-blockchain-1.8.0b5/chia/server/ssl_context.py` & `chia-blockchain-1.8.0b6/chia/server/ssl_context.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/server/start_data_layer.py` & `chia-blockchain-1.8.0b6/chia/server/start_data_layer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 import pathlib
 import sys
-from typing import Any, Dict, Optional, cast
+from typing import Any, Dict, List, Optional, cast
 
 from chia.data_layer.data_layer import DataLayer
 from chia.data_layer.data_layer_api import DataLayerAPI
 from chia.rpc.data_layer_rpc_api import DataLayerRpcApi
 from chia.rpc.wallet_rpc_client import WalletRpcClient
 from chia.server.outbound_message import NodeType
 from chia.server.start_service import RpcInfo, Service, async_run
@@ -25,50 +25,63 @@
 log = logging.getLogger(__name__)
 
 
 # TODO: Review need for config and if retained then hint it properly.
 def create_data_layer_service(
     root_path: pathlib.Path,
     config: Dict[str, Any],
+    downloaders: List[str],
+    uploaders: List[str],  # dont add FilesystemUploader to this, it is the default uploader
     wallet_service: Optional[Service[WalletNode]] = None,
     connect_to_daemon: bool = True,
 ) -> Service[DataLayer]:
+    if uploaders is None:
+        uploaders = []
+    if downloaders is None:
+        downloaders = []
     service_config = config[SERVICE_NAME]
     self_hostname = config["self_hostname"]
     wallet_rpc_port = service_config["wallet_peer"]["port"]
     if wallet_service is None:
         wallet_root_path = root_path
         wallet_config = config
     else:
         wallet_root_path = wallet_service.root_path
         wallet_config = wallet_service.config
     wallet_rpc_init = WalletRpcClient.create(self_hostname, uint16(wallet_rpc_port), wallet_root_path, wallet_config)
-    data_layer = DataLayer(config=service_config, root_path=root_path, wallet_rpc_init=wallet_rpc_init)
+
+    data_layer = DataLayer(
+        config=service_config,
+        root_path=root_path,
+        wallet_rpc_init=wallet_rpc_init,
+        downloaders=downloaders,
+        uploaders=uploaders,
+    )  # dont add Fil)
     api = DataLayerAPI(data_layer)
     network_id = service_config["selected_network"]
     rpc_port = service_config.get("rpc_port")
     rpc_info: Optional[RpcInfo] = None
     if rpc_port is not None:
         rpc_info = (DataLayerRpcApi, cast(int, service_config["rpc_port"]))
 
     return Service(
-        server_listen_ports=[service_config["port"]],
         root_path=root_path,
         config=config,
         node=data_layer,
         # TODO: not for peers...
         peer_api=api,
         node_type=NodeType.DATA_LAYER,
         # TODO: no publicly advertised port, at least not yet
         advertised_port=service_config["port"],
         service_name=SERVICE_NAME,
         network_id=network_id,
         max_request_body_size=service_config.get("rpc_server_max_request_body_size", 26214400),
         rpc_info=rpc_info,
         connect_to_daemon=connect_to_daemon,
+        listen=False,
     )
 
 
 async def async_main() -> int:
     # TODO: refactor to avoid the double load
     config = load_config(DEFAULT_ROOT_PATH, "config.yaml", fill_missing_services=True)
     service_config = load_config_cli(DEFAULT_ROOT_PATH, "config.yaml", SERVICE_NAME, fill_missing_services=True)
@@ -82,15 +95,17 @@
     create_all_ssl(
         root_path=DEFAULT_ROOT_PATH,
         private_node_names=["data_layer"],
         public_node_names=["data_layer"],
         overwrite=False,
     )
 
-    service = create_data_layer_service(DEFAULT_ROOT_PATH, config)
+    uploaders: List[str] = config["data_layer"].get("uploaders", [])
+    downloaders: List[str] = config["data_layer"].get("downloaders", [])
+    service = create_data_layer_service(DEFAULT_ROOT_PATH, config, downloaders, uploaders)
     await service.setup_process_global_state()
     await service.run()
 
     return 0
 
 
 def main() -> int:
```

### Comparing `chia-blockchain-1.8.0b5/chia/server/start_farmer.py` & `chia-blockchain-1.8.0b6/chia/server/start_farmer.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 from chia.consensus.constants import ConsensusConstants
 from chia.consensus.default_constants import DEFAULT_CONSTANTS
 from chia.farmer.farmer import Farmer
 from chia.farmer.farmer_api import FarmerAPI
 from chia.rpc.farmer_rpc_api import FarmerRpcApi
 from chia.server.outbound_message import NodeType
 from chia.server.start_service import RpcInfo, Service, async_run
-from chia.types.peer_info import PeerInfo
+from chia.types.peer_info import UnresolvedPeerInfo
 from chia.util.chia_logging import initialize_service_logging
 from chia.util.config import load_config, load_config_cli
 from chia.util.default_root import DEFAULT_ROOT_PATH
 from chia.util.keychain import Keychain
-from chia.util.network import get_host_addr
 
 # See: https://bugs.python.org/issue29288
 "".encode("idna")
 
 SERVICE_NAME = "farmer"
 
 
@@ -30,20 +29,16 @@
     config_pool: Dict[str, Any],
     consensus_constants: ConsensusConstants,
     keychain: Optional[Keychain] = None,
     connect_to_daemon: bool = True,
 ) -> Service[Farmer]:
     service_config = config[SERVICE_NAME]
 
-    connect_peers = []
     fnp = service_config.get("full_node_peer")
-    if fnp is not None:
-        connect_peers.append(
-            PeerInfo(str(get_host_addr(fnp["host"], prefer_ipv6=config.get("prefer_ipv6", False))), fnp["port"])
-        )
+    connect_peers = set() if fnp is None else {UnresolvedPeerInfo(fnp["host"], fnp["port"])}
 
     overrides = service_config["network_overrides"]["constants"][service_config["selected_network"]]
     updated_constants = consensus_constants.replace_str_to_bytes(**overrides)
 
     farmer = Farmer(
         root_path, service_config, config_pool, consensus_constants=updated_constants, local_keychain=keychain
     )
@@ -56,15 +51,14 @@
         root_path=root_path,
         config=config,
         node=farmer,
         peer_api=peer_api,
         node_type=NodeType.FARMER,
         advertised_port=service_config["port"],
         service_name=SERVICE_NAME,
-        server_listen_ports=[service_config["port"]],
         connect_peers=connect_peers,
         on_connect_callback=farmer.on_connect,
         network_id=network_id,
         rpc_info=rpc_info,
         connect_to_daemon=connect_to_daemon,
     )
```

### Comparing `chia-blockchain-1.8.0b5/chia/server/start_full_node.py` & `chia-blockchain-1.8.0b6/chia/server/start_full_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         config=config,
         node=api.full_node,
         peer_api=api,
         node_type=NodeType.FULL_NODE,
         advertised_port=service_config["port"],
         service_name=SERVICE_NAME,
         upnp_ports=upnp_list,
-        server_listen_ports=[service_config["port"]],
         on_connect_callback=full_node.on_connect,
         network_id=network_id,
         rpc_info=rpc_info,
         connect_to_daemon=connect_to_daemon,
         override_capabilities=override_capabilities,
     )
```

### Comparing `chia-blockchain-1.8.0b5/chia/server/start_harvester.py` & `chia-blockchain-1.8.0b6/chia/server/start_harvester.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,31 +7,30 @@
 from chia.consensus.constants import ConsensusConstants
 from chia.consensus.default_constants import DEFAULT_CONSTANTS
 from chia.harvester.harvester import Harvester
 from chia.harvester.harvester_api import HarvesterAPI
 from chia.rpc.harvester_rpc_api import HarvesterRpcApi
 from chia.server.outbound_message import NodeType
 from chia.server.start_service import RpcInfo, Service, async_run
-from chia.types.peer_info import PeerInfo
+from chia.types.peer_info import UnresolvedPeerInfo
 from chia.util.chia_logging import initialize_service_logging
 from chia.util.config import load_config, load_config_cli
 from chia.util.default_root import DEFAULT_ROOT_PATH
-from chia.util.network import get_host_addr
 
 # See: https://bugs.python.org/issue29288
 "".encode("idna")
 
 SERVICE_NAME = "harvester"
 
 
 def create_harvester_service(
     root_path: pathlib.Path,
     config: Dict[str, Any],
     consensus_constants: ConsensusConstants,
-    farmer_peer: Optional[PeerInfo],
+    farmer_peer: Optional[UnresolvedPeerInfo],
     connect_to_daemon: bool = True,
 ) -> Service[Harvester]:
     service_config = config[SERVICE_NAME]
 
     overrides = service_config["network_overrides"]["constants"][service_config["selected_network"]]
     updated_constants = consensus_constants.replace_str_to_bytes(**overrides)
 
@@ -45,31 +44,29 @@
         root_path=root_path,
         config=config,
         node=harvester,
         peer_api=peer_api,
         node_type=NodeType.HARVESTER,
         advertised_port=service_config["port"],
         service_name=SERVICE_NAME,
-        server_listen_ports=[service_config["port"]],
-        connect_peers=[] if farmer_peer is None else [farmer_peer],
+        connect_peers=set() if farmer_peer is None else {farmer_peer},
         network_id=network_id,
         rpc_info=rpc_info,
         connect_to_daemon=connect_to_daemon,
+        listen=False,
     )
 
 
 async def async_main() -> int:
     # TODO: refactor to avoid the double load
     config = load_config(DEFAULT_ROOT_PATH, "config.yaml")
     service_config = load_config_cli(DEFAULT_ROOT_PATH, "config.yaml", SERVICE_NAME)
     config[SERVICE_NAME] = service_config
     initialize_service_logging(service_name=SERVICE_NAME, config=config)
-    farmer_peer = PeerInfo(
-        str(get_host_addr(service_config["farmer_peer"]["host"])), service_config["farmer_peer"]["port"]
-    )
+    farmer_peer = UnresolvedPeerInfo(service_config["farmer_peer"]["host"], service_config["farmer_peer"]["port"])
     service = create_harvester_service(DEFAULT_ROOT_PATH, config, DEFAULT_CONSTANTS, farmer_peer)
     await service.setup_process_global_state()
     await service.run()
 
     return 0
```

### Comparing `chia-blockchain-1.8.0b5/chia/server/start_introducer.py` & `chia-blockchain-1.8.0b6/chia/server/start_introducer.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     return Service(
         root_path=root_path,
         config=config,
         node=introducer,
         peer_api=node__api,
         node_type=NodeType.INTRODUCER,
         service_name=SERVICE_NAME,
-        server_listen_ports=[service_config["port"]],
         network_id=network_id,
         advertised_port=advertised_port,
         connect_to_daemon=connect_to_daemon,
     )
 
 
 async def async_main() -> int:
```

### Comparing `chia-blockchain-1.8.0b5/chia/server/start_service.py` & `chia-blockchain-1.8.0b6/chia/server/start_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 import logging
 import logging.config
 import os
 import signal
 import sys
 from pathlib import Path
 from types import FrameType
-from typing import Any, Awaitable, Callable, Coroutine, Dict, Generic, List, Optional, Tuple, Type, TypeVar
+from typing import Any, Awaitable, Callable, Coroutine, Dict, Generic, List, Optional, Set, Tuple, Type, TypeVar
 
 from chia.cmds.init_funcs import chia_full_version_str
 from chia.daemon.server import service_launch_lock_path
 from chia.rpc.rpc_server import RpcApiProtocol, RpcServer, RpcServiceProtocol, start_rpc_server
 from chia.server.chia_policy import set_chia_policy
 from chia.server.outbound_message import NodeType
 from chia.server.server import ChiaServer
 from chia.server.ssl_context import chia_ssl_ca_paths, private_ssl_ca_paths
 from chia.server.upnp import UPnP
 from chia.server.ws_connection import WSChiaConnection
-from chia.types.peer_info import PeerInfo
+from chia.types.peer_info import PeerInfo, UnresolvedPeerInfo
 from chia.util.ints import uint16
 from chia.util.lock import Lockfile, LockfileError
+from chia.util.network import get_host_addr
 from chia.util.setproctitle import setproctitle
 
 from ..protocols.shared_protocol import capabilities
-from .reconnect_task import start_reconnect_task
 
 # this is used to detect whether we are running in the main process or not, in
 # signal handlers. We need to ignore signals in the sub processes.
 main_pid: Optional[int] = None
 
 T = TypeVar("T")
 _T_RpcServiceProtocol = TypeVar("_T_RpcServiceProtocol", bound=RpcServiceProtocol)
@@ -51,35 +51,37 @@
         node_type: NodeType,
         advertised_port: int,
         service_name: str,
         network_id: str,
         *,
         config: Dict[str, Any],
         upnp_ports: List[int] = [],
-        server_listen_ports: List[int] = [],
-        connect_peers: List[PeerInfo] = [],
+        connect_peers: Set[UnresolvedPeerInfo] = set(),
         on_connect_callback: Optional[Callable[[WSChiaConnection], Awaitable[None]]] = None,
         rpc_info: Optional[RpcInfo] = None,
         connect_to_daemon: bool = True,
         max_request_body_size: Optional[int] = None,
         override_capabilities: Optional[List[Tuple[uint16, str]]] = None,
+        listen: bool = True,
     ) -> None:
         self.root_path = root_path
         self.config = config
         ping_interval = self.config.get("ping_interval")
         self.self_hostname = self.config.get("self_hostname")
         self.daemon_port = self.config.get("daemon_port")
         assert ping_interval is not None
         self._connect_to_daemon = connect_to_daemon
         self._node_type = node_type
         self._service_name = service_name
         self.rpc_server: Optional[RpcServer] = None
         self._rpc_close_task: Optional[asyncio.Task[None]] = None
         self._network_id: str = network_id
         self.max_request_body_size = max_request_body_size
+        self._listen = listen
+        self.reconnect_retry_seconds: int = 3
 
         self._log = logging.getLogger(service_name)
         self._log.info(f"Starting service {self._service_name} ...")
         self._log.info(f"chia-blockchain version: {chia_full_version_str()}")
 
         self.service_config = self.config[service_name]
 
@@ -115,27 +117,61 @@
         f = getattr(node, "set_server", None)
         if f:
             f(self._server)
         else:
             self._log.warning(f"No set_server method for {service_name}")
 
         self._upnp_ports = upnp_ports
-        self._server_listen_ports = server_listen_ports
 
         self._api = peer_api
         self._node = node
         self._did_start = False
         self._is_stopping = asyncio.Event()
         self._stopped_by_rpc = False
 
         self._on_connect_callback = on_connect_callback
         self._advertised_port = advertised_port
-        self._reconnect_tasks: Dict[PeerInfo, Optional[asyncio.Task[None]]] = {peer: None for peer in connect_peers}
+        self._connect_peers = connect_peers
+        self._connect_peers_task: Optional[asyncio.Task[None]] = None
         self.upnp: UPnP = UPnP()
 
+    async def _connect_peers_task_handler(self) -> None:
+        resolved_peers: Dict[UnresolvedPeerInfo, PeerInfo] = {}
+        prefer_ipv6 = self.config.get("prefer_ipv6", False)
+        while True:
+            for unresolved in self._connect_peers:
+                resolved = resolved_peers.get(unresolved)
+                if resolved is None:
+                    try:
+                        resolved = PeerInfo(get_host_addr(unresolved.host, prefer_ipv6=prefer_ipv6), unresolved.port)
+                    except Exception as e:
+                        self._log.warning(f"Failed to resolve {unresolved.host}: {e}")
+                        continue
+                    self._log.info(f"Add resolved {resolved}")
+                    resolved_peers[unresolved] = resolved
+
+                if any(connection.peer_info == resolved for connection in self._server.all_connections.values()):
+                    continue
+
+                if not await self._server.start_client(resolved, None):
+                    self._log.info(f"Failed to connect to {resolved}")
+                    # Re-resolve to make sure the IP didn't change, this helps for example to keep dyndns hostnames
+                    # up to date.
+                    try:
+                        resolved_new = PeerInfo(
+                            get_host_addr(unresolved.host, prefer_ipv6=prefer_ipv6), unresolved.port
+                        )
+                    except Exception as e:
+                        self._log.warning(f"Failed to resolve after connection failure {unresolved.host}: {e}")
+                        continue
+                    if resolved_new != resolved:
+                        self._log.info(f"Host {unresolved.host} changed from {resolved} to {resolved_new}")
+                        resolved_peers[unresolved] = resolved_new
+            await asyncio.sleep(self.reconnect_retry_seconds)
+
     async def start(self) -> None:
         # TODO: move those parameters to `__init__`
         if self._did_start:
             return None
 
         assert self.self_hostname is not None
         assert self.daemon_port is not None
@@ -147,19 +183,22 @@
 
         if len(self._upnp_ports) > 0:
             self.upnp.setup()
 
             for port in self._upnp_ports:
                 self.upnp.remap(port)
 
-        await self._server.start_server(self.config.get("prefer_ipv6", False), self._on_connect_callback)
+        await self._server.start(
+            listen=self._listen,
+            prefer_ipv6=self.config.get("prefer_ipv6", False),
+            on_connect=self._on_connect_callback,
+        )
         self._advertised_port = self._server.get_port()
 
-        for peer in self._reconnect_tasks.keys():
-            self.add_peer(peer)
+        self._connect_peers_task = asyncio.create_task(self._connect_peers_task_handler())
 
         self._log.info(
             f"Started {self._service_name} service on network_id: {self._network_id} "
             f"at port {self._advertised_port}"
         )
 
         self._rpc_close_task = None
@@ -182,19 +221,16 @@
             with Lockfile.create(service_launch_lock_path(self.root_path, self._service_name), timeout=1):
                 await self.start()
                 await self.wait_closed()
         except LockfileError as e:
             self._log.error(f"{self._service_name}: already running")
             raise ValueError(f"{self._service_name}: already running") from e
 
-    def add_peer(self, peer: PeerInfo) -> None:
-        if self._reconnect_tasks.get(peer) is not None:
-            raise ServiceException(f"Peer {peer} already added")
-
-        self._reconnect_tasks[peer] = start_reconnect_task(self._server, peer, self._log)
+    def add_peer(self, peer: UnresolvedPeerInfo) -> None:
+        self._connect_peers.add(peer)
 
     async def setup_process_global_state(self) -> None:
         # Being async forces this to be run from within an active event loop as is
         # needed for the signal handler setup.
         proctitle_name = f"chia_{self._service_name}"
         setproctitle(proctitle_name)
 
@@ -234,18 +270,16 @@
 
             # start with UPnP, since this can take a while, we want it to happen
             # in the background while shutting down everything else
             for port in self._upnp_ports:
                 self.upnp.release(port)
 
             self._log.info("Cancelling reconnect task")
-            for task in self._reconnect_tasks.values():
-                if task is not None:
-                    task.cancel()
-            self._reconnect_tasks.clear()
+            if self._connect_peers_task is not None:
+                self._connect_peers_task.cancel()
             self._log.info("Closing connections")
             self._server.close_all()
             self._node._close()
             self._node._shut_down = True
 
             self._log.info("Calling service stop callback")
```

### Comparing `chia-blockchain-1.8.0b5/chia/server/start_timelord.py` & `chia-blockchain-1.8.0b6/chia/server/start_timelord.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 from chia.consensus.constants import ConsensusConstants
 from chia.consensus.default_constants import DEFAULT_CONSTANTS
 from chia.rpc.timelord_rpc_api import TimelordRpcApi
 from chia.server.outbound_message import NodeType
 from chia.server.start_service import RpcInfo, Service, async_run
 from chia.timelord.timelord import Timelord
 from chia.timelord.timelord_api import TimelordAPI
-from chia.types.peer_info import PeerInfo
+from chia.types.peer_info import UnresolvedPeerInfo
 from chia.util.chia_logging import initialize_service_logging
 from chia.util.config import load_config, load_config_cli
 from chia.util.default_root import DEFAULT_ROOT_PATH
-from chia.util.network import get_host_addr
 
 # See: https://bugs.python.org/issue29288
 "".encode("idna")
 
 SERVICE_NAME = "timelord"
 
 
@@ -31,17 +30,17 @@
     root_path: pathlib.Path,
     config: Dict[str, Any],
     constants: ConsensusConstants,
     connect_to_daemon: bool = True,
 ) -> Service[Timelord]:
     service_config = config[SERVICE_NAME]
 
-    connect_peers = [
-        PeerInfo(str(get_host_addr(service_config["full_node_peer"]["host"])), service_config["full_node_peer"]["port"])
-    ]
+    connect_peers = {
+        UnresolvedPeerInfo(service_config["full_node_peer"]["host"], service_config["full_node_peer"]["port"])
+    }
     overrides = service_config["network_overrides"]["constants"][service_config["selected_network"]]
     updated_constants = constants.replace_str_to_bytes(**overrides)
 
     node = Timelord(root_path, service_config, updated_constants)
     peer_api = TimelordAPI(node)
     network_id = service_config["selected_network"]
 
@@ -53,19 +52,19 @@
         root_path=root_path,
         config=config,
         peer_api=peer_api,
         node=node,
         node_type=NodeType.TIMELORD,
         advertised_port=service_config["port"],
         service_name=SERVICE_NAME,
-        server_listen_ports=[service_config["port"]],
         connect_peers=connect_peers,
         network_id=network_id,
         rpc_info=rpc_info,
         connect_to_daemon=connect_to_daemon,
+        listen=False,
     )
 
 
 async def async_main() -> int:
     # TODO: refactor to avoid the double load
     config = load_config(DEFAULT_ROOT_PATH, "config.yaml")
     service_config = load_config_cli(DEFAULT_ROOT_PATH, "config.yaml", SERVICE_NAME)
```

### Comparing `chia-blockchain-1.8.0b5/chia/server/start_wallet.py` & `chia-blockchain-1.8.0b6/chia/server/start_wallet.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 from typing import Any, Dict, Optional
 
 from chia.consensus.constants import ConsensusConstants
 from chia.consensus.default_constants import DEFAULT_CONSTANTS
 from chia.rpc.wallet_rpc_api import WalletRpcApi
 from chia.server.outbound_message import NodeType
 from chia.server.start_service import RpcInfo, Service, async_run
-from chia.types.peer_info import PeerInfo
+from chia.types.peer_info import UnresolvedPeerInfo
 from chia.util.chia_logging import initialize_service_logging
 from chia.util.config import load_config, load_config_cli
 from chia.util.default_root import DEFAULT_ROOT_PATH
 from chia.util.keychain import Keychain
-from chia.util.network import get_host_addr
 from chia.util.task_timing import maybe_manage_task_instrumentation
 from chia.wallet.wallet_node import WalletNode
 
 # See: https://bugs.python.org/issue29288
 from chia.wallet.wallet_node_api import WalletNodeAPI
 
 "".encode("idna")
@@ -46,33 +45,28 @@
         service_config,
         root_path,
         constants=updated_constants,
         local_keychain=keychain,
     )
     peer_api = WalletNodeAPI(node)
     fnp = service_config.get("full_node_peer")
+    connect_peers = set() if fnp is None else {UnresolvedPeerInfo(fnp["host"], fnp["port"])}
 
-    if fnp:
-        connect_peers = [
-            PeerInfo(str(get_host_addr(fnp["host"], prefer_ipv6=config.get("prefer_ipv6", False))), fnp["port"])
-        ]
-    else:
-        connect_peers = []
     network_id = service_config["selected_network"]
     rpc_port = service_config.get("rpc_port")
     rpc_info: Optional[RpcInfo] = None
     if rpc_port is not None:
         rpc_info = (WalletRpcApi, service_config["rpc_port"])
 
     return Service(
-        server_listen_ports=[service_config["port"]],
         root_path=root_path,
         config=config,
         node=node,
         peer_api=peer_api,
+        listen=False,
         node_type=NodeType.WALLET,
         service_name=SERVICE_NAME,
         on_connect_callback=node.on_connect,
         connect_peers=connect_peers,
         network_id=network_id,
         rpc_info=rpc_info,
         advertised_port=service_config["port"],
```

### Comparing `chia-blockchain-1.8.0b5/chia/server/upnp.py` & `chia-blockchain-1.8.0b6/chia/server/upnp.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/server/ws_connection.py` & `chia-blockchain-1.8.0b6/chia/server/ws_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,16 +66,15 @@
 
     ws: WebSocket = field(repr=False)
     api: Any = field(repr=False)
     local_type: NodeType
     local_port: int
     local_capabilities_for_handshake: List[Tuple[uint16, str]] = field(repr=False)
     local_capabilities: List[Capability]
-    peer_host: str
-    peer_port: uint16
+    peer_info: PeerInfo
     peer_node_id: bytes32
     log: logging.Logger = field(repr=False)
 
     close_callback: Optional[ConnectionClosedCallbackProtocol] = field(repr=False)
     outbound_rate_limiter: RateLimiter
     inbound_rate_limiter: RateLimiter
 
@@ -153,16 +152,15 @@
         return cls(
             ws=ws,
             api=api,
             local_type=local_type,
             local_port=server_port,
             local_capabilities_for_handshake=local_capabilities_for_handshake,
             local_capabilities=known_active_capabilities(local_capabilities_for_handshake),
-            peer_host=peer_host,
-            peer_port=peername[1],
+            peer_info=PeerInfo(peer_host, peername[1]),
             peer_node_id=peer_id,
             log=log,
             close_callback=close_callback,
             request_nonce=request_nonce,
             outbound_rate_limiter=RateLimiter(incoming=False, percentage_of_limit=outbound_rate_limit_percent),
             inbound_rate_limiter=RateLimiter(incoming=True, percentage_of_limit=inbound_rate_limit_percent),
             is_outbound=is_outbound,
@@ -267,15 +265,15 @@
         """
         Closes the connection, and finally calls the close_callback on the server, so the connection gets removed
         from the global list.
         """
         if self.closed:
             # always try to call the callback even for closed connections
             with log_exceptions(self.log, consume=True):
-                self.log.debug(f"Closing already closed connection for {self.peer_host}")
+                self.log.debug(f"Closing already closed connection for {self.peer_info.host}")
                 if self.close_callback is not None:
                     self.close_callback(self, ban_time, closed_connection=True)
             self._close_event.set()
             return None
         self.closed = True
 
         if error is None:
@@ -308,15 +306,15 @@
 
     async def wait_until_closed(self) -> None:
         await self._close_event.wait()
 
     async def ban_peer_bad_protocol(self, log_err_msg: str) -> None:
         """Ban peer for protocol violation"""
         ban_seconds = INTERNAL_PROTOCOL_ERROR_BAN_SECONDS
-        self.log.error(f"Banning peer for {ban_seconds} seconds: {self.peer_host} {log_err_msg}")
+        self.log.error(f"Banning peer for {ban_seconds} seconds: {self.peer_info.host} {log_err_msg}")
         await self.close(ban_seconds, WSCloseCode.PROTOCOL_ERROR, Err.INVALID_PROTOCOL_MESSAGE)
 
     def cancel_pending_requests(self) -> None:
         for message_id, event in self.pending_requests.items():
             try:
                 event.set()
             except Exception as e:
@@ -341,28 +339,28 @@
             if isinstance(e, (BrokenPipeError, ConnectionResetError, TimeoutError)):
                 expected = True
             elif isinstance(e, OSError):
                 if e.errno in {113}:
                     expected = True
 
             if expected:
-                self.log.warning(f"{e} {self.peer_host}")
+                self.log.warning(f"{e} {self.peer_info.host}")
             else:
                 error_stack = traceback.format_exc()
-                self.log.error(f"Exception: {e} with {self.peer_host}")
+                self.log.error(f"Exception: {e} with {self.peer_info.host}")
                 self.log.error(f"Exception Stack: {error_stack}")
 
     async def _api_call(self, full_message: Message, task_id: bytes32) -> None:
         start_time = time.time()
         message_type = ""
         try:
             if self.received_message_callback is not None:
                 await self.received_message_callback(self)
             self.log.debug(
-                f"<- {ProtocolMessageTypes(full_message.type).name} from peer {self.peer_node_id} {self.peer_host}"
+                f"<- {ProtocolMessageTypes(full_message.type).name} from peer {self.peer_node_id} {self.peer_info.host}"
             )
             message_type = ProtocolMessageTypes(full_message.type).name
 
             f = getattr(self.api, message_type, None)
 
             if f is None:
                 self.log.error(f"Non existing function: {message_type}")
@@ -537,15 +535,17 @@
             await asyncio.wait_for(event.wait(), timeout=timeout)
 
         self.pending_requests.pop(message.id)
         result: Optional[Message] = None
         if message.id in self.request_results:
             result = self.request_results[message.id]
             assert result is not None
-            self.log.debug(f"<- {ProtocolMessageTypes(result.type).name} from: {self.peer_host}:{self.peer_port}")
+            self.log.debug(
+                f"<- {ProtocolMessageTypes(result.type).name} from: {self.peer_info.host}:{self.peer_info.port}"
+            )
             self.request_results.pop(message.id)
 
         return result
 
     async def send_messages(self, messages: List[Message]) -> None:
         if self.closed:
             return None
@@ -563,36 +563,38 @@
     async def _send_message(self, message: Message) -> None:
         encoded: bytes = bytes(message)
         size = len(encoded)
         assert len(encoded) < (2 ** (LENGTH_BYTES * 8))
         if not self.outbound_rate_limiter.process_msg_and_check(
             message, self.local_capabilities, self.peer_capabilities
         ):
-            if not is_localhost(self.peer_host):
+            if not is_localhost(self.peer_info.host):
                 message_type = ProtocolMessageTypes(message.type)
                 last_time = self.log_rate_limit_last_time[message_type]
                 now = time.monotonic()
                 self.log_rate_limit_last_time[message_type] = now
                 if now - last_time >= 60:
-                    msg = f"Rate limiting ourselves. message type: {message_type.name}, peer: {self.peer_host}"
+                    msg = f"Rate limiting ourselves. message type: {message_type.name}, peer: {self.peer_info.host}"
                     self.log.debug(msg)
 
                 # TODO: fix this special case. This function has rate limits which are too low.
                 if ProtocolMessageTypes(message.type) != ProtocolMessageTypes.respond_peers:
                     asyncio.create_task(self._wait_and_retry(message))
 
                 return None
             else:
                 self.log.debug(
                     f"Not rate limiting ourselves. message type: {ProtocolMessageTypes(message.type).name}, "
-                    f"peer: {self.peer_host}"
+                    f"peer: {self.peer_info.host}"
                 )
 
         await self.ws.send_bytes(encoded)
-        self.log.debug(f"-> {ProtocolMessageTypes(message.type).name} to peer {self.peer_host} {self.peer_node_id}")
+        self.log.debug(
+            f"-> {ProtocolMessageTypes(message.type).name} to peer {self.peer_info.host} {self.peer_node_id}"
+        )
         self.bytes_written += size
 
     async def _read_one_message(self) -> Optional[Message]:
         try:
             message: WSMessage = await self.ws.receive(30)
         except asyncio.TimeoutError:
             # self.ws._closed if we didn't receive a ping / pong
@@ -604,25 +606,25 @@
 
         if self.connection_type is not None:
             connection_type_str = NodeType(self.connection_type).name.lower()
         else:
             connection_type_str = ""
         if message.type == WSMsgType.CLOSING:
             self.log.debug(
-                f"Closing connection to {connection_type_str} {self.peer_host}:"
+                f"Closing connection to {connection_type_str} {self.peer_info.host}:"
                 f"{self.peer_server_port}/"
-                f"{self.peer_port}"
+                f"{self.peer_info.port}"
             )
             asyncio.create_task(self.close())
             await asyncio.sleep(3)
         elif message.type == WSMsgType.CLOSE:
             self.log.debug(
-                f"Peer closed connection {connection_type_str} {self.peer_host}:"
+                f"Peer closed connection {connection_type_str} {self.peer_info.host}:"
                 f"{self.peer_server_port}/"
-                f"{self.peer_port}"
+                f"{self.peer_info.port}"
             )
             asyncio.create_task(self.close())
             await asyncio.sleep(3)
         elif message.type == WSMsgType.CLOSED:
             if not self.closed:
                 asyncio.create_task(self.close())
                 await asyncio.sleep(3)
@@ -635,27 +637,27 @@
             try:
                 message_type = ProtocolMessageTypes(full_message_loaded.type).name
             except Exception:
                 message_type = "Unknown"
             if not self.inbound_rate_limiter.process_msg_and_check(
                 full_message_loaded, self.local_capabilities, self.peer_capabilities
             ):
-                if self.local_type == NodeType.FULL_NODE and not is_localhost(self.peer_host):
+                if self.local_type == NodeType.FULL_NODE and not is_localhost(self.peer_info.host):
                     self.log.error(
-                        f"Peer has been rate limited and will be disconnected: {self.peer_host}, "
+                        f"Peer has been rate limited and will be disconnected: {self.peer_info.host}, "
                         f"message: {message_type}"
                     )
                     # Only full node disconnects peers, to prevent abuse and crashing timelords, farmers, etc
                     asyncio.create_task(self.close(300))
                     await asyncio.sleep(3)
                     return None
                 else:
                     self.log.debug(
-                        f"Peer surpassed rate limit {self.peer_host}, message: {message_type}, "
-                        f"port {self.peer_port} but not disconnecting"
+                        f"Peer surpassed rate limit {self.peer_info.host}, message: {message_type}, "
+                        f"port {self.peer_info.port} but not disconnecting"
                     )
                     return full_message_loaded
             return full_message_loaded
         elif message.type == WSMsgType.ERROR:
             self.log.error(f"WebSocket Error: {message}")
             if message.data.code == WSCloseCode.MESSAGE_TOO_BIG:
                 asyncio.create_task(self.close(300))
@@ -681,21 +683,21 @@
             return "unknown"
 
     def get_peer_info(self) -> Optional[PeerInfo]:
         result = self._get_extra_info("peername")
         if result is None:
             return None
         connection_host = result[0]
-        port = self.peer_server_port if self.peer_server_port is not None else self.peer_port
+        port = self.peer_server_port if self.peer_server_port is not None else self.peer_info.port
         return PeerInfo(connection_host, port)
 
     def get_peer_logging(self) -> PeerInfo:
         info: Optional[PeerInfo] = self.get_peer_info()
         if info is None:
-            # in this case, we will use self.peer_host which is friendlier for logging
-            port = self.peer_server_port if self.peer_server_port is not None else self.peer_port
-            return PeerInfo(self.peer_host, port)
+            # in this case, we will use self.peer_info.host which is friendlier for logging
+            port = self.peer_server_port if self.peer_server_port is not None else self.peer_info.port
+            return PeerInfo(self.peer_info.host, port)
         else:
             return info
 
     def has_capability(self, capability: Capability) -> bool:
         return capability in self.peer_capabilities
```

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/block_tools.py` & `chia-blockchain-1.8.0b6/chia/simulator/block_tools.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/full_node_simulator.py` & `chia-blockchain-1.8.0b6/chia/simulator/full_node_simulator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/keyring.py` & `chia-blockchain-1.8.0b6/chia/simulator/keyring.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/setup_nodes.py` & `chia-blockchain-1.8.0b6/chia/simulator/setup_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     setup_vdf_clients,
     setup_wallet_node,
 )
 from chia.simulator.socket import find_available_listen_port
 from chia.simulator.time_out_assert import time_out_assert_custom_interval
 from chia.timelord.timelord import Timelord
 from chia.types.blockchain_format.sized_bytes import bytes32
-from chia.types.peer_info import PeerInfo
+from chia.types.peer_info import UnresolvedPeerInfo
 from chia.util.hash import std_hash
 from chia.util.ints import uint16, uint32
 from chia.util.keychain import Keychain
 from chia.wallet.wallet_node import WalletNode
 
 SimulatorsAndWallets = Tuple[List[FullNodeSimulator], List[Tuple[WalletNode, ChiaServer]], BlockTools]
 SimulatorsAndWalletsServices = Tuple[List[Service[FullNode]], List[Service[WalletNode]], BlockTools]
@@ -298,15 +298,15 @@
             consensus_constants,
             port=uint16(0),
             start_service=start_services,
         )
     ]
     farmer_service = await farmer_node_iterators[0].__anext__()
     if start_services:
-        farmer_peer = PeerInfo(block_tools.config["self_hostname"], uint16(farmer_service._server._port))
+        farmer_peer = UnresolvedPeerInfo(block_tools.config["self_hostname"], uint16(farmer_service._server._port))
     else:
         farmer_peer = None
     harvester_node_iterators = []
     for i in range(0, harvester_count):
         root_path: Path = temp_dir / f"harvester_{i}"
         harvester_node_iterators.append(
             setup_harvester(
@@ -428,15 +428,15 @@
         consensus_constants,
         full_node_0_port,
     )
     farmer_service = await farmer_iter.__anext__()
     harvester_iter = setup_harvester(
         shared_b_tools,
         shared_b_tools.root_path / "harvester",
-        PeerInfo(shared_b_tools.config["self_hostname"], farmer_service._server.get_port()),
+        UnresolvedPeerInfo(shared_b_tools.config["self_hostname"], farmer_service._server.get_port()),
         consensus_constants,
     )
     vdf1_port = uint16(find_available_listen_port("vdf1"))
     vdf2_port = uint16(find_available_listen_port("vdf2"))
     timelord_iter = setup_timelord(full_node_0_port, False, consensus_constants, b_tools, vdf_port=vdf1_port)
     timelord_bluebox_iter = setup_timelord(uint16(1000), True, consensus_constants, b_tools_1, vdf_port=vdf2_port)
     harvester_service = await harvester_iter.__anext__()
```

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/setup_services.py` & `chia-blockchain-1.8.0b6/chia/simulator/setup_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from chia.server.start_timelord import create_timelord_service
 from chia.server.start_wallet import create_wallet_service
 from chia.simulator.block_tools import BlockTools
 from chia.simulator.keyring import TempKeyring
 from chia.simulator.start_simulator import create_full_node_simulator_service
 from chia.timelord.timelord import Timelord
 from chia.timelord.timelord_launcher import kill_processes, spawn_process
-from chia.types.peer_info import PeerInfo
+from chia.types.peer_info import UnresolvedPeerInfo
 from chia.util.bech32m import encode_puzzle_hash
 from chia.util.config import config_path_for_filename, lock_and_load_config, save_config
 from chia.util.ints import uint16
 from chia.util.keychain import bytes_to_mnemonic
 from chia.util.lock import Lockfile
 from chia.wallet.wallet_node import WalletNode
 
@@ -238,15 +238,15 @@
             db_path.unlink()
         keychain.delete_all_keys()
 
 
 async def setup_harvester(
     b_tools: BlockTools,
     root_path: Path,
-    farmer_peer: Optional[PeerInfo],
+    farmer_peer: Optional[UnresolvedPeerInfo],
     consensus_constants: ConsensusConstants,
     start_service: bool = True,
 ) -> AsyncGenerator[Service[Harvester], None]:
     with create_lock_and_load_config(b_tools.root_path / "config" / "ssl" / "ca", root_path) as config:
         config["logging"]["log_stdout"] = True
         config["selected_network"] = "testnet0"
         config["harvester"]["selected_network"] = "testnet0"
```

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/simulator_constants.py` & `chia-blockchain-1.8.0b6/chia/simulator/simulator_constants.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/simulator_full_node_rpc_api.py` & `chia-blockchain-1.8.0b6/chia/simulator/simulator_full_node_rpc_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/simulator_full_node_rpc_client.py` & `chia-blockchain-1.8.0b6/chia/simulator/simulator_full_node_rpc_client.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/simulator_protocol.py` & `chia-blockchain-1.8.0b6/chia/simulator/simulator_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/simulator_test_tools.py` & `chia-blockchain-1.8.0b6/chia/simulator/simulator_test_tools.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/socket.py` & `chia-blockchain-1.8.0b6/chia/simulator/socket.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/ssl_certs.py` & `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_1.py` & `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_1.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_10.py` & `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_10.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_2.py` & `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_2.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_3.py` & `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_3.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_4.py` & `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_4.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_5.py` & `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_5.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_6.py` & `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_6.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_7.py` & `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_7.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_8.py` & `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_8.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/ssl_certs_9.py` & `chia-blockchain-1.8.0b6/chia/simulator/ssl_certs_9.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/start_simulator.py` & `chia-blockchain-1.8.0b6/chia/simulator/start_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         root_path=root_path,
         config=config,
         node=node,
         peer_api=peer_api,
         node_type=NodeType.FULL_NODE,
         advertised_port=service_config["port"],
         service_name=SERVICE_NAME,
-        server_listen_ports=[service_config["port"]],
         on_connect_callback=node.on_connect,
         network_id=network_id,
         rpc_info=(SimulatorFullNodeRpcApi, service_config["rpc_port"]),
         connect_to_daemon=connect_to_daemon,
         override_capabilities=override_capabilities,
     )
```

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/time_out_assert.py` & `chia-blockchain-1.8.0b6/chia/simulator/time_out_assert.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/simulator/wallet_tools.py` & `chia-blockchain-1.8.0b6/chia/simulator/wallet_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.serialized_program import SerializedProgram
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.types.coin_spend import CoinSpend
 from chia.types.condition_opcodes import ConditionOpcode
 from chia.types.condition_with_args import ConditionWithArgs
 from chia.types.spend_bundle import SpendBundle
-from chia.util.condition_tools import conditions_by_opcode, conditions_for_solution
+from chia.util.condition_tools import conditions_dict_for_solution
 from chia.util.hash import std_hash
 from chia.util.ints import uint32, uint64
 from chia.wallet.derive_keys import master_sk_to_wallet_sk
 from chia.wallet.puzzles.p2_delegated_puzzle_or_hidden_puzzle import (
     DEFAULT_HIDDEN_PUZZLE_HASH,
     calculate_synthetic_secret_key,
     puzzle_for_pk,
@@ -176,20 +176,17 @@
         return spends
 
     def sign_transaction(self, coin_spends: List[CoinSpend]) -> SpendBundle:
         signatures = []
         for coin_spend in coin_spends:  # noqa
             secret_key = self.get_private_key_for_puzzle_hash(coin_spend.coin.puzzle_hash)
             synthetic_secret_key = calculate_synthetic_secret_key(secret_key, DEFAULT_HIDDEN_PUZZLE_HASH)
-            err, con, cost = conditions_for_solution(
+            conditions_dict = conditions_dict_for_solution(
                 coin_spend.puzzle_reveal, coin_spend.solution, self.constants.MAX_BLOCK_COST_CLVM
             )
-            if not con:
-                raise ValueError(err)
-            conditions_dict = conditions_by_opcode(con)
 
             for cwa in conditions_dict.get(ConditionOpcode.AGG_SIG_UNSAFE, []):
                 msg = cwa.vars[1]
                 signature = AugSchemeMPL.sign(synthetic_secret_key, msg)
                 signatures.append(signature)
 
             for cwa in conditions_dict.get(ConditionOpcode.AGG_SIG_ME, []):
```

### Comparing `chia-blockchain-1.8.0b5/chia/ssl/chia_ca.crt` & `chia-blockchain-1.8.0b6/chia/ssl/chia_ca.crt`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/ssl/chia_ca.key` & `chia-blockchain-1.8.0b6/chia/ssl/chia_ca.key`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/ssl/create_ssl.py` & `chia-blockchain-1.8.0b6/chia/ssl/create_ssl.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/ssl/dst_root_ca.pem` & `chia-blockchain-1.8.0b6/chia/ssl/dst_root_ca.pem`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/timelord/iters_from_block.py` & `chia-blockchain-1.8.0b6/chia/timelord/iters_from_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/timelord/timelord.py` & `chia-blockchain-1.8.0b6/chia/timelord/timelord.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,14 @@
             Chain.REWARD_CHAIN,
             Chain.INFUSED_CHALLENGE_CHAIN,
         ]
         # Chains that currently accept iterations.
         self.allows_iters: List[Chain] = []
         # Last peak received, None if it's already processed.
         self.new_peak: Optional[timelord_protocol.NewPeakTimelord] = None
-        # Last end of subslot bundle, None if we built a peak on top of it.
-        self.new_subslot_end: Optional[EndOfSubSlotBundle] = None
         # Last state received. Can either be a new peak or a new EndOfSubslotBundle.
         # Unfinished block info, iters adjusted to the last peak.
         self.unfinished_blocks: List[timelord_protocol.NewUnfinishedBlockTimelord] = []
         # Signage points iters, adjusted to the last peak.
         self.signage_point_iters: List[Tuple[uint64, uint8]] = []
         # For each chain, send those info when the process spawns.
         self.iters_to_submit: Dict[Chain, List[uint64]] = {}
@@ -372,22 +370,14 @@
                 f"Total infused blocks: {self.total_infused}. "
                 f"Infusion rate: {infusion_rate}%."
             )
 
         self.new_peak = None
         await self._reset_chains()
 
-    async def _handle_subslot_end(self):
-        self.last_state.set_state(self.new_subslot_end)
-        for block in self.unfinished_blocks:
-            if self._can_infuse_unfinished_block(block) is not None:
-                self.total_unfinished += 1
-        self.new_subslot_end = None
-        await self._reset_chains()
-
     async def _map_chains_with_vdf_clients(self):
         while not self._shut_down:
             picked_chain = None
             async with self.lock:
                 if len(self.free_clients) == 0:
                     break
                 ip, reader, writer = self.free_clients[0]
@@ -822,17 +812,20 @@
 
             if next_ses is None or next_ses.new_difficulty is None:
                 self.unfinished_blocks = self.overflow_blocks.copy()
             else:
                 # No overflow blocks in a new epoch
                 self.unfinished_blocks = []
             self.overflow_blocks = []
-            self.new_subslot_end = eos_bundle
 
-            await self._handle_subslot_end()
+            self.last_state.set_state(eos_bundle)
+            for block in self.unfinished_blocks:
+                if self._can_infuse_unfinished_block(block) is not None:
+                    self.total_unfinished += 1
+            await self._reset_chains()
 
     async def _handle_failures(self):
         if len(self.vdf_failures) > 0:
             # This can happen if one of the VDF processes has an issue. In this case, we abort all other
             # infusion points and signage points, and go straight to the end of slot, so we avoid potential
             # issues with the number of iterations that failed.
```

### Comparing `chia-blockchain-1.8.0b5/chia/timelord/timelord_api.py` & `chia-blockchain-1.8.0b6/chia/timelord/timelord_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,20 +39,18 @@
                 self.timelord.state_changed("new_peak", {"height": new_peak.reward_chain_block.height})
             elif (
                 self.timelord.last_state.peak is not None
                 and self.timelord.last_state.peak.reward_chain_block == new_peak.reward_chain_block
             ):
                 log.info("Skipping peak, already have.")
                 self.timelord.state_changed("skipping_peak", {"height": new_peak.reward_chain_block.height})
-                return None
             else:
                 log.warning("block that we don't have, changing to it.")
                 self.timelord.new_peak = new_peak
                 self.timelord.state_changed("new_peak", {"height": new_peak.reward_chain_block.height})
-                self.timelord.new_subslot_end = None
 
     @api_request()
     async def new_unfinished_block_timelord(self, new_unfinished_block: timelord_protocol.NewUnfinishedBlockTimelord):
         if self.timelord.last_state is None:
             return None
         async with self.timelord.lock:
             if self.timelord.bluebox_mode:
```

### Comparing `chia-blockchain-1.8.0b5/chia/timelord/timelord_launcher.py` & `chia-blockchain-1.8.0b6/chia/timelord/timelord_launcher.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/timelord/timelord_state.py` & `chia-blockchain-1.8.0b6/chia/timelord/timelord_state.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/announcement.py` & `chia-blockchain-1.8.0b6/chia/types/announcement.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/block_protocol.py` & `chia-blockchain-1.8.0b6/chia/types/block_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/blockchain_format/classgroup.py` & `chia-blockchain-1.8.0b6/chia/types/blockchain_format/classgroup.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/blockchain_format/coin.py` & `chia-blockchain-1.8.0b6/chia/types/blockchain_format/coin.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/blockchain_format/foliage.py` & `chia-blockchain-1.8.0b6/chia/types/blockchain_format/foliage.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/blockchain_format/program.py` & `chia-blockchain-1.8.0b6/chia/types/blockchain_format/program.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/blockchain_format/proof_of_space.py` & `chia-blockchain-1.8.0b6/chia/types/blockchain_format/proof_of_space.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/blockchain_format/reward_chain_block.py` & `chia-blockchain-1.8.0b6/chia/types/blockchain_format/reward_chain_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/blockchain_format/serialized_program.py` & `chia-blockchain-1.8.0b6/chia/types/blockchain_format/serialized_program.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/blockchain_format/slots.py` & `chia-blockchain-1.8.0b6/chia/types/blockchain_format/slots.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/blockchain_format/sub_epoch_summary.py` & `chia-blockchain-1.8.0b6/chia/types/blockchain_format/sub_epoch_summary.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/blockchain_format/tree_hash.py` & `chia-blockchain-1.8.0b6/chia/types/blockchain_format/tree_hash.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/blockchain_format/vdf.py` & `chia-blockchain-1.8.0b6/chia/types/blockchain_format/vdf.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/coin_record.py` & `chia-blockchain-1.8.0b6/chia/types/coin_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/coin_spend.py` & `chia-blockchain-1.8.0b6/chia/types/coin_spend.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/condition_opcodes.py` & `chia-blockchain-1.8.0b6/chia/types/condition_opcodes.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/end_of_slot_bundle.py` & `chia-blockchain-1.8.0b6/chia/types/end_of_slot_bundle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/fee_rate.py` & `chia-blockchain-1.8.0b6/chia/types/fee_rate.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/full_block.py` & `chia-blockchain-1.8.0b6/chia/types/full_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/generator_types.py` & `chia-blockchain-1.8.0b6/chia/types/generator_types.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/header_block.py` & `chia-blockchain-1.8.0b6/chia/types/header_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/mempool_item.py` & `chia-blockchain-1.8.0b6/chia/types/mempool_item.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/mempool_submission_status.py` & `chia-blockchain-1.8.0b6/chia/types/mempool_submission_status.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/peer_info.py` & `chia-blockchain-1.8.0b6/chia/types/peer_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 from typing import Union
 
 from chia.util.ints import uint16, uint64
 from chia.util.network import IPAddress
 from chia.util.streamable import Streamable, streamable
 
 
+@dataclass(frozen=True)
+class UnresolvedPeerInfo:
+    host: str
+    port: uint16
+
+
 # TODO, Replace unsafe_hash with frozen and drop the __init__ as soon as all PeerInfo call sites pass in an IPAddress.
 @dataclass(unsafe_hash=True)
 class PeerInfo:
     _ip: IPAddress
     _port: uint16
 
     # TODO, Drop this as soon as all call PeerInfo calls pass in an IPAddress
```

### Comparing `chia-blockchain-1.8.0b5/chia/types/signing_mode.py` & `chia-blockchain-1.8.0b6/chia/types/signing_mode.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/spend_bundle.py` & `chia-blockchain-1.8.0b6/chia/types/spend_bundle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/transaction_queue_entry.py` & `chia-blockchain-1.8.0b6/chia/types/transaction_queue_entry.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/unfinished_block.py` & `chia-blockchain-1.8.0b6/chia/types/unfinished_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/unfinished_header_block.py` & `chia-blockchain-1.8.0b6/chia/types/unfinished_header_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/types/weight_proof.py` & `chia-blockchain-1.8.0b6/chia/types/weight_proof.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/api_decorators.py` & `chia-blockchain-1.8.0b6/chia/util/api_decorators.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/bech32m.py` & `chia-blockchain-1.8.0b6/chia/util/bech32m.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/beta_metrics.py` & `chia-blockchain-1.8.0b6/chia/util/beta_metrics.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/block_cache.py` & `chia-blockchain-1.8.0b6/chia/util/block_cache.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/byte_types.py` & `chia-blockchain-1.8.0b6/chia/util/byte_types.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/cached_bls.py` & `chia-blockchain-1.8.0b6/chia/util/cached_bls.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/check_fork_next_block.py` & `chia-blockchain-1.8.0b6/chia/util/check_fork_next_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/chia_logging.py` & `chia-blockchain-1.8.0b6/chia/util/chia_logging.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/condition_tools.py` & `chia-blockchain-1.8.0b6/chia/util/condition_tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Dict, List, Optional, Tuple
+from typing import Dict, List, Tuple
 
 from clvm.casts import int_from_bytes
 
 from chia.types.blockchain_format.coin import Coin
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.serialized_program import SerializedProgram
 from chia.types.blockchain_format.sized_bytes import bytes32, bytes48
@@ -14,27 +14,25 @@
 from chia.util.errors import ConsensusError, Err
 from chia.util.ints import uint64
 
 # TODO: review each `assert` and consider replacing with explicit checks
 #       since asserts can be stripped with python `-OO` flag
 
 
-def parse_sexp_to_condition(
-    sexp: Program,
-) -> Tuple[Optional[Err], Optional[ConditionWithArgs]]:
+def parse_sexp_to_condition(sexp: Program) -> ConditionWithArgs:
     """
     Takes a ChiaLisp sexp and returns a ConditionWithArgs.
-    If it fails, returns an Error
+    Raises an ConsensusError if it fails.
     """
     first = sexp.pair
     if first is None:
-        return Err.INVALID_CONDITION, None
+        raise ConsensusError(Err.INVALID_CONDITION, ["first is None"])
     op = first[0].atom
     if op is None or len(op) != 1:
-        return Err.INVALID_CONDITION, None
+        raise ConsensusError(Err.INVALID_CONDITION, ["invalid op"])
 
     # since the ConditionWithArgs only has atoms as the args, we can't parse
     # hints and memos with this function. We just exit the loop if we encounter
     # a pair instead of an atom
     vars: List[bytes] = []
     for arg in Program(first[1]).as_iter():
         a = arg.atom
@@ -42,49 +40,23 @@
             break
         vars.append(a)
         # no condition (currently) has more than 3 arguments. Additional
         # arguments are allowed but ignored
         if len(vars) > 3:
             break
 
-    return None, ConditionWithArgs(ConditionOpcode(op), vars)
+    return ConditionWithArgs(ConditionOpcode(op), vars)
 
 
-def parse_sexp_to_conditions(
-    sexp: Program,
-) -> Tuple[Optional[Err], Optional[List[ConditionWithArgs]]]:
+def parse_sexp_to_conditions(sexp: Program) -> List[ConditionWithArgs]:
     """
     Takes a ChiaLisp sexp (list) and returns the list of ConditionWithArgss
-    If it fails, returns as Error
+    Raises an ConsensusError if it fails.
     """
-    results: List[ConditionWithArgs] = []
-    try:
-        for _ in sexp.as_iter():
-            error, cvp = parse_sexp_to_condition(_)
-            if error:
-                return error, None
-            results.append(cvp)  # type: ignore # noqa
-    except ConsensusError:
-        return Err.INVALID_CONDITION, None
-    return None, results
-
-
-def conditions_by_opcode(
-    conditions: List[ConditionWithArgs],
-) -> Dict[ConditionOpcode, List[ConditionWithArgs]]:
-    """
-    Takes a list of ConditionWithArgss(CVP) and return dictionary of CVPs keyed of their opcode
-    """
-    d: Dict[ConditionOpcode, List[ConditionWithArgs]] = {}
-    cvp: ConditionWithArgs
-    for cvp in conditions:
-        if cvp.opcode not in d:
-            d[cvp.opcode] = list()
-        d[cvp.opcode].append(cvp)
-    return d
+    return [parse_sexp_to_condition(s) for s in sexp.as_iter()]
 
 
 def pkm_pairs(
     conditions: SpendBundleConditions, additional_data: bytes, *, soft_fork: bool
 ) -> Tuple[List[bytes48], List[bytes]]:
     ret: Tuple[List[bytes48], List[bytes]] = ([], [])
 
@@ -136,26 +108,25 @@
     return output_coins
 
 
 def conditions_dict_for_solution(
     puzzle_reveal: SerializedProgram,
     solution: SerializedProgram,
     max_cost: int,
-) -> Tuple[Optional[Err], Optional[Dict[ConditionOpcode, List[ConditionWithArgs]]], uint64]:
-    error, result, cost = conditions_for_solution(puzzle_reveal, solution, max_cost)
-    if error or result is None:
-        return error, None, uint64(0)
-    return None, conditions_by_opcode(result), cost
+) -> Dict[ConditionOpcode, List[ConditionWithArgs]]:
+    conditions_dict: Dict[ConditionOpcode, List[ConditionWithArgs]] = {}
+    for cvp in conditions_for_solution(puzzle_reveal, solution, max_cost):
+        conditions_dict.setdefault(cvp.opcode, list()).append(cvp)
+    return conditions_dict
 
 
 def conditions_for_solution(
     puzzle_reveal: SerializedProgram,
     solution: SerializedProgram,
     max_cost: int,
-) -> Tuple[Optional[Err], Optional[List[ConditionWithArgs]], uint64]:
+) -> List[ConditionWithArgs]:
     # get the standard script for a puzzle hash and feed in the solution
     try:
         cost, r = puzzle_reveal.run_with_cost(max_cost, solution)
-        error, result = parse_sexp_to_conditions(r)
-        return error, result, uint64(cost)
-    except Program.EvalError:
-        return Err.SEXP_ERROR, None, uint64(0)
+        return parse_sexp_to_conditions(r)
+    except Program.EvalError as e:
+        raise ConsensusError(Err.SEXP_ERROR, [str(e)]) from e
```

### Comparing `chia-blockchain-1.8.0b5/chia/util/config.py` & `chia-blockchain-1.8.0b6/chia/util/config.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/create_alert_file.py` & `chia-blockchain-1.8.0b6/chia/util/create_alert_file.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/db_synchronous.py` & `chia-blockchain-1.8.0b6/chia/util/db_synchronous.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/db_version.py` & `chia-blockchain-1.8.0b6/chia/util/db_version.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/db_wrapper.py` & `chia-blockchain-1.8.0b6/chia/util/db_wrapper.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/dump_keyring.py` & `chia-blockchain-1.8.0b6/chia/util/dump_keyring.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/english.txt` & `chia-blockchain-1.8.0b6/chia/util/english.txt`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/errors.py` & `chia-blockchain-1.8.0b6/chia/util/errors.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/file_keyring.py` & `chia-blockchain-1.8.0b6/chia/util/file_keyring.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import shutil
 import sys
 import threading
 from dataclasses import asdict, dataclass, field
 from hashlib import pbkdf2_hmac
 from pathlib import Path
 from secrets import token_bytes
-from typing import Any, Dict, Iterator, Optional, Union
+from typing import Any, Dict, Iterator, Optional, Union, cast
 
 import yaml
 from cryptography.hazmat.primitives.ciphers.aead import ChaCha20Poly1305  # pyright: reportMissingModuleSource=false
 from typing_extensions import final
 from watchdog.events import DirModifiedEvent, FileSystemEvent, FileSystemEventHandler
 from watchdog.observers import Observer
 
@@ -382,15 +382,17 @@
         # Merge in other properties like "passphrase_hint"
         if "passphrase_hint" in self.file_content_properties_for_next_write:
             self.cached_file_content.passphrase_hint = self.file_content_properties_for_next_write["passphrase_hint"]
 
         # When writing for the first time, we should have a cached passphrase which hasn't been
         # validated (because it can't be validated yet...)
         if not self.has_content() and KeyringWrapper.get_shared_instance().has_cached_master_passphrase():
-            passphrase = KeyringWrapper.get_shared_instance().get_cached_master_passphrase()[0]
+            # TODO: The above checks, at the time of writing, make sure we get a str here.  A reconsideration of this
+            #       interface would be good.
+            passphrase = cast(str, KeyringWrapper.get_shared_instance().get_cached_master_passphrase()[0])
         else:
             # TODO, this prompts for the passphrase interactively, move this out
             passphrase = obtain_current_passphrase(use_passphrase_cache=True)
 
         try:
             self.cached_file_content.update_encrypted_data_dict(passphrase, self.cached_data_dict, fresh_salt)
             self.cached_file_content.write_to_path(self.keyring_path)
```

### Comparing `chia-blockchain-1.8.0b5/chia/util/files.py` & `chia-blockchain-1.8.0b6/chia/util/files.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from aiofiles import tempfile
 from typing_extensions import Literal
 
 log = logging.getLogger(__name__)
 
 
-def move_file(src: Path, dst: Path):
+def move_file(src: Path, dst: Path) -> None:
     """
     Attempts to move the file at src to dst, falling back to a copy if the move fails.
     """
 
     dir_perms: int = 0o700
     # Create the parent directory if necessary
     os.makedirs(dst.parent, mode=dir_perms, exist_ok=True)
@@ -31,15 +31,15 @@
             # If that fails, use the more robust shutil.move(), though it may internally initiate a copy
             shutil.move(os.fspath(src), os.fspath(dst))
         except Exception:
             log.exception(f"Failed to move {src} to {dst} using shutil.move")
             raise
 
 
-async def move_file_async(src: Path, dst: Path, *, reattempts: int = 6, reattempt_delay: float = 0.5):
+async def move_file_async(src: Path, dst: Path, *, reattempts: int = 6, reattempt_delay: float = 0.5) -> None:
     """
     Attempts to move the file at src to dst, making multiple attempts if the move fails.
     """
 
     remaining_attempts: int = reattempts
     while True:
         try:
@@ -56,25 +56,29 @@
 
     if not dst.exists():
         raise FileNotFoundError(f"Failed to move {src} to {dst}")
     else:
         log.debug(f"Moved {src} to {dst}")
 
 
-async def write_file_async(file_path: Path, data: Union[str, bytes], *, file_mode: int = 0o600, dir_mode: int = 0o700):
+async def write_file_async(
+    file_path: Path, data: Union[str, bytes], *, file_mode: int = 0o600, dir_mode: int = 0o700
+) -> None:
     """
     Writes the provided data to a temporary file and then moves it to the final destination.
     """
 
     # Create the parent directory if necessary
     os.makedirs(file_path.parent, mode=dir_mode, exist_ok=True)
 
     mode: Literal["w+", "w+b"] = "w+" if type(data) == str else "w+b"
     temp_file_path: Path
     async with tempfile.NamedTemporaryFile(dir=file_path.parent, mode=mode, delete=False) as f:
+        # Ignoring type error since it is not obvious how to tie the type of the data
+        # being passed in to the type of the file object, etc.
         temp_file_path = f.name  # type: ignore[assignment]
         await f.write(data)  # type: ignore[arg-type]
         await f.flush()
         os.fsync(f.fileno())
 
     try:
         await move_file_async(temp_file_path, file_path)
```

### Comparing `chia-blockchain-1.8.0b5/chia/util/full_block_utils.py` & `chia-blockchain-1.8.0b6/chia/util/full_block_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/generator_tools.py` & `chia-blockchain-1.8.0b6/chia/util/generator_tools.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/initial-config.yaml` & `chia-blockchain-1.8.0b6/chia/util/initial-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -103,31 +103,29 @@
   crt: "config/ssl/ca/private_ca.crt"
   key: "config/ssl/ca/private_ca.key"
 
 chia_ssl_ca:
   crt: "config/ssl/ca/chia_ca.crt"
   key: "config/ssl/ca/chia_ca.key"
 
-
 daemon_ssl:
   private_crt: "config/ssl/daemon/private_daemon.crt"
   private_key: "config/ssl/daemon/private_daemon.key"
 
-
 # Controls logging of all servers (harvester, farmer, etc..). Each one can be overridden.
 logging: &logging
-  log_stdout: False  # If True, outputs to stdout instead of a file
+  log_stdout: False # If True, outputs to stdout instead of a file
   log_filename: "log/debug.log"
-  log_level: "WARNING"  # Can be CRITICAL, ERROR, WARNING, INFO, DEBUG, NOTSET
+  log_level: "WARNING" # Can be CRITICAL, ERROR, WARNING, INFO, DEBUG, NOTSET
   log_maxfilesrotation: 7 #  Max files in rotation. Default value 7 if the key is not set
   log_maxbytesrotation: 52428800 #  Max bytes logged before rotating logs
   log_use_gzip: False #  Use gzip to compress rotated logs
-  log_syslog: False  # If True, outputs to SysLog host and port specified
-  log_syslog_host: "localhost"  # Send logging messages to a remote or local Unix syslog
-  log_syslog_port: 514  # UDP port of the remote or local Unix syslog
+  log_syslog: False # If True, outputs to SysLog host and port specified
+  log_syslog_host: "localhost" # Send logging messages to a remote or local Unix syslog
+  log_syslog_port: 514 # UDP port of the remote or local Unix syslog
 
 seeder:
   # The fake full node used for crawling will run on this port.
   port: 8444
   # Most full nodes on the network run on this port. (i.e. 8444 for mainnet, 58444 for testnet).
   other_peers_port: 8444
   # This will override the default full_node.peer_connect_timeout for the crawler full node
@@ -175,29 +173,28 @@
   num_threads: 30
   plots_refresh_parameter:
     interval_seconds: 120 # The interval in seconds to refresh the plot file manager
     retry_invalid_seconds: 1200 # How long to wait before re-trying plots which failed to load
     batch_size: 300 # How many plot files the harvester processes before it waits batch_sleep_milliseconds
     batch_sleep_milliseconds: 1 # Milliseconds the harvester sleeps between batch processing
 
-
   # If True use parallel reads in chiapos
   parallel_read: True
 
   logging: *logging
   network_overrides: *network_overrides
   selected_network: *selected_network
 
   # Plots are searched for in the following directories
   plot_directories: []
   recursive_plot_scan: False # If True the harvester scans plots recursively in the provided directories.
 
   ssl:
-    private_crt:  "config/ssl/harvester/private_harvester.crt"
-    private_key:  "config/ssl/harvester/private_harvester.key"
+    private_crt: "config/ssl/harvester/private_harvester.crt"
+    private_key: "config/ssl/harvester/private_harvester.key"
 
   private_ssl_ca:
     crt: "config/ssl/ca/private_ca.crt"
     key: "config/ssl/ca/private_ca.key"
 
   chia_ssl_ca:
     crt: "config/ssl/ca/chia_ca.crt"
@@ -206,15 +203,14 @@
 pool:
   # Replace this with a real receive address
   # xch_target_address: txch102gkhhzs60grx7cfnpng5n6rjecr89r86l5s8xux2za8k820cxsq64ssdg
   logging: *logging
   network_overrides: *network_overrides
   selected_network: *selected_network
 
-
 farmer:
   # The farmer server (if run) will run on this port
   port: 8447
   # The farmer will attempt to connect to this full node and harvester
   full_node_peer:
     host: *self_hostname
     port: 8444
@@ -234,44 +230,43 @@
   # To send a share to a pool, a proof of space must have required_iters less than this number
   pool_share_threshold: 1000
   logging: *logging
   network_overrides: *network_overrides
   selected_network: *selected_network
 
   ssl:
-    private_crt:  "config/ssl/farmer/private_farmer.crt"
-    private_key:  "config/ssl/farmer/private_farmer.key"
-    public_crt:  "config/ssl/farmer/public_farmer.crt"
-    public_key:  "config/ssl/farmer/public_farmer.key"
+    private_crt: "config/ssl/farmer/private_farmer.crt"
+    private_key: "config/ssl/farmer/private_farmer.key"
+    public_crt: "config/ssl/farmer/public_farmer.crt"
+    public_key: "config/ssl/farmer/public_farmer.key"
 
 # Don't run this unless you want to run VDF clients on the local machine.
 timelord_launcher:
   # The server where the VDF clients will connect to.
   host: *self_hostname
   port: 8000
   # Number of VDF client processes to keep alive in the local machine.
   process_count: 3
   logging: *logging
 
-
 timelord:
   # The timelord server (if run) will run on this port
   port: 8446
   # Provides a list of VDF clients expected to connect to this timelord.
   # For each client, an IP is provided, together with the estimated iterations per second.
   vdf_clients:
     ip:
       - *self_hostname
       - localhost
       - 127.0.0.1
     ips_estimate:
       - 150000
   full_node_peer:
-      host: *self_hostname
-      port: 8444
+    host: *self_hostname
+    port: 8444
   # Maximum number of seconds allowed for a client to reconnect to the server.
   max_connection_time: 60
   # The ip and port where the TCP clients will connect.
   vdf_server:
     host: *self_hostname
     port: 8000
   logging: *logging
@@ -302,18 +297,18 @@
 
   multiprocessing_start_method: default
 
   start_rpc_server: True
   rpc_port: 8557
 
   ssl:
-    private_crt:  "config/ssl/timelord/private_timelord.crt"
-    private_key:  "config/ssl/timelord/private_timelord.key"
-    public_crt:  "config/ssl/timelord/public_timelord.crt"
-    public_key:  "config/ssl/timelord/public_timelord.key"
+    private_crt: "config/ssl/timelord/private_timelord.crt"
+    private_key: "config/ssl/timelord/private_timelord.key"
+    public_crt: "config/ssl/timelord/public_timelord.crt"
+    public_key: "config/ssl/timelord/public_timelord.key"
 
 full_node:
   # The full node server (if run) will run on this port
   port: 8444
 
   # controls the sync-to-disk behavior of the database connection. Can be one of:
   # "on"    enables syncing to disk, minimizes risk of corrupting the DB in
@@ -421,42 +416,42 @@
     - "dns-introducer.chia.net"
     - "chia.ctrlaltdel.ch"
     - "seeder.dexie.space"
     - "chia-seeder.h9.com"
     - "chia.hoffmang.com"
     - "seeder.xchpool.org"
   farmer_peer:
-      host: *self_hostname
-      port: 8447
+    host: *self_hostname
+    port: 8447
   timelord_peer:
-      host: *self_hostname
-      port: 8446
+    host: *self_hostname
+    port: 8446
   introducer_peer:
-      host: introducer.chia.net  # Chia AWS introducer IPv4/IPv6
-      port: 8444
+    host: introducer.chia.net # Chia AWS introducer IPv4/IPv6
+    port: 8444
   wallet_peer:
     host: *self_hostname
     port: 8449
   logging: *logging
   network_overrides: *network_overrides
   selected_network: *selected_network
 
   # Node IDs of trusted wallet peers, allows using more permissive limits on sync
   trusted_peers:
     0ThisisanexampleNodeID7ff9d60f1c3fa270c213c0ad0cb89c01274634a7c3cb7: Does_not_matter
 
   ssl:
-    private_crt:  "config/ssl/full_node/private_full_node.crt"
-    private_key:  "config/ssl/full_node/private_full_node.key"
-    public_crt:  "config/ssl/full_node/public_full_node.crt"
-    public_key:  "config/ssl/full_node/public_full_node.key"
+    private_crt: "config/ssl/full_node/private_full_node.crt"
+    private_key: "config/ssl/full_node/private_full_node.key"
+    public_crt: "config/ssl/full_node/public_full_node.crt"
+    public_key: "config/ssl/full_node/public_full_node.key"
   use_chia_loop_policy: True
 
 ui:
-   # The ui node server (if run) will run on this port
+  # The ui node server (if run) will run on this port
   port: 8222
 
   # Which port to use to communicate with the full node
   rpc_port: 8555
 
   # This SSH key is for the ui SSH server
   ssh_filename: config/ssh_host_key
@@ -480,16 +475,16 @@
   # recent_peer_threshold seconds
   recent_peer_threshold: 6000
   logging: *logging
   network_overrides: *network_overrides
   selected_network: *selected_network
 
   ssl:
-    public_crt:  "config/ssl/full_node/public_full_node.crt"
-    public_key:  "config/ssl/full_node/public_full_node.key"
+    public_crt: "config/ssl/full_node/public_full_node.crt"
+    public_key: "config/ssl/full_node/public_full_node.key"
 
 wallet:
   port: 8449
   rpc_port: 9256
 
   enable_profiler: False
 
@@ -543,18 +538,18 @@
   recent_peer_threshold: 6000
 
   introducer_peer:
     host: introducer.chia.net # Chia AWS introducer IPv4/IPv6
     port: 8444
 
   ssl:
-    private_crt:  "config/ssl/wallet/private_wallet.crt"
-    private_key:  "config/ssl/wallet/private_wallet.key"
-    public_crt:  "config/ssl/wallet/public_wallet.crt"
-    public_key:  "config/ssl/wallet/public_wallet.key"
+    private_crt: "config/ssl/wallet/private_wallet.crt"
+    private_key: "config/ssl/wallet/private_wallet.key"
+    public_crt: "config/ssl/wallet/public_wallet.crt"
+    public_key: "config/ssl/wallet/public_wallet.key"
 
   # Node IDs of trusted full node peers, for performing a fast trusted wallet sync
   trusted_peers:
     0ThisisanexampleNodeID7ff9d60f1c3fa270c213c0ad0cb89c01274634a7c3cb9: Does_not_matter
 
   short_sync_blocks_behind_threshold: 20
 
@@ -615,21 +610,22 @@
   rpc_server_max_request_body_size: 26214400
   fee: 1000000000
   logging: *logging
 
   # TODO: which of these are really appropriate?
 
   ssl:
-    private_crt:  "config/ssl/data_layer/private_data_layer.crt"
-    private_key:  "config/ssl/data_layer/private_data_layer.key"
-    public_crt:  "config/ssl/data_layer/public_data_layer.crt"
-    public_key:  "config/ssl/data_layer/public_data_layer.key"
+    private_crt: "config/ssl/data_layer/private_data_layer.crt"
+    private_key: "config/ssl/data_layer/private_data_layer.key"
+    public_crt: "config/ssl/data_layer/public_data_layer.crt"
+    public_key: "config/ssl/data_layer/public_data_layer.key"
 
+  uploaders: []
+  downloaders: []
 simulator:
-
   # Should the simulator farm a block whenever a transaction is in mempool
   auto_farm: True
 
   # The key used by the simulator to farm blocks and send transactions
   key_fingerprint:
 
   # The target address for any blocks that are farmed
```

### Comparing `chia-blockchain-1.8.0b5/chia/util/inline_executor.py` & `chia-blockchain-1.8.0b6/chia/util/inline_executor.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/ints.py` & `chia-blockchain-1.8.0b6/chia/util/ints.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/json_util.py` & `chia-blockchain-1.8.0b6/chia/util/json_util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/keychain.py` & `chia-blockchain-1.8.0b6/chia/util/keychain.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,18 +478,22 @@
     @staticmethod
     def is_keyring_locked() -> bool:
         """
         Returns whether the keyring is in a locked state. If the keyring doesn't have a master passphrase set,
         or if a master passphrase is set and the cached passphrase is valid, the keyring is "unlocked"
         """
         # Unlocked: If a master passphrase isn't set, or if the cached passphrase is valid
-        if not Keychain.has_master_passphrase() or (
-            Keychain.has_cached_passphrase()
-            and Keychain.master_passphrase_is_valid(Keychain.get_cached_master_passphrase())
-        ):
+        if not Keychain.has_master_passphrase():
+            return False
+
+        passphrase = Keychain.get_cached_master_passphrase()
+        if passphrase is None:
+            return True
+
+        if Keychain.master_passphrase_is_valid(passphrase):
             return False
 
         # Locked: Everything else
         return True
 
     @staticmethod
     def passphrase_is_optional() -> bool:
@@ -541,15 +545,15 @@
     def has_cached_passphrase() -> bool:
         """
         Returns whether the master passphrase has been cached (it may need to be validated)
         """
         return KeyringWrapper.get_shared_instance().has_cached_master_passphrase()
 
     @staticmethod
-    def get_cached_master_passphrase() -> str:
+    def get_cached_master_passphrase() -> Optional[str]:
         """
         Returns the cached master passphrase
         """
         passphrase, _ = KeyringWrapper.get_shared_instance().get_cached_master_passphrase()
         return passphrase
 
     @staticmethod
```

### Comparing `chia-blockchain-1.8.0b5/chia/util/keyring_wrapper.py` & `chia-blockchain-1.8.0b6/chia/util/keyring_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 from pathlib import Path
 from sys import platform
-from typing import Optional, Tuple, Union
+from typing import Optional, Tuple, Union, overload
 
 from keyring.backends.macOS import Keyring as MacKeyring
 from keyring.backends.Windows import WinVaultKeyring as WinKeyring
 from keyring.errors import KeyringError, PasswordDeleteError
+from typing_extensions import Literal
 
 from chia.util.default_root import DEFAULT_KEYS_ROOT_PATH
 from chia.util.file_keyring import FileKeyring
 
 # We want to protect the keyring, even if a user-specified master passphrase isn't provided
 #
 # WARNING: Changing the default passphrase will prevent passphrase-less users from accessing
@@ -105,16 +106,31 @@
     @staticmethod
     def set_keys_root_path(keys_root_path: Path):
         """
         Used to set the keys_root_path prior to instantiating the __shared_instance
         """
         KeyringWrapper.__keys_root_path = keys_root_path
 
+    @overload
     @staticmethod
-    def get_shared_instance(create_if_necessary: bool = True):
+    def get_shared_instance() -> KeyringWrapper:
+        ...
+
+    @overload
+    @staticmethod
+    def get_shared_instance(create_if_necessary: Literal[True]) -> KeyringWrapper:
+        ...
+
+    @overload
+    @staticmethod
+    def get_shared_instance(create_if_necessary: bool) -> Optional[KeyringWrapper]:
+        ...
+
+    @staticmethod
+    def get_shared_instance(create_if_necessary: bool = True) -> Optional[KeyringWrapper]:
         if not KeyringWrapper.__shared_instance and create_if_necessary:
             KeyringWrapper.__shared_instance = KeyringWrapper(keys_root_path=KeyringWrapper.__keys_root_path)
 
         return KeyringWrapper.__shared_instance
 
     @staticmethod
     def cleanup_shared_instance() -> None:
```

### Comparing `chia-blockchain-1.8.0b5/chia/util/limited_semaphore.py` & `chia-blockchain-1.8.0b6/chia/util/limited_semaphore.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/lock.py` & `chia-blockchain-1.8.0b6/chia/util/lock.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/logging.py` & `chia-blockchain-1.8.0b6/chia/util/logging.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/lru_cache.py` & `chia-blockchain-1.8.0b6/chia/util/lru_cache.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/merkle_set.py` & `chia-blockchain-1.8.0b6/chia/util/merkle_set.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/misc.py` & `chia-blockchain-1.8.0b6/chia/util/misc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/network.py` & `chia-blockchain-1.8.0b6/chia/util/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,15 +106,19 @@
         peer_host_ip = ip_address(peer_host)
         return any(peer_host_ip in network for network in networks)
     except ValueError:
         return False
 
 
 def is_localhost(peer_host: str) -> bool:
-    return peer_host == "127.0.0.1" or peer_host == "localhost" or peer_host == "::1" or peer_host == "0:0:0:0:0:0:0:1"
+    return peer_host in ["127.0.0.1", "localhost", "::1", "0:0:0:0:0:0:0:1"]
+
+
+def is_trusted_peer(host: str, node_id: bytes32, trusted_peers: Dict[str, Any], testing: bool = False) -> bool:
+    return not testing and is_localhost(host) or node_id.hex() in trusted_peers
 
 
 def class_for_type(type: NodeType) -> Any:
     if type is NodeType.FULL_NODE:
         from chia.full_node.full_node_api import FullNodeAPI
 
         return FullNodeAPI
@@ -163,25 +167,14 @@
         return preferred[0]
     elif len(alternative) > 0:
         return alternative[0]
     else:
         raise ValueError(f"failed to resolve {host} into an IP address")
 
 
-def is_trusted_inner(peer_host: str, peer_node_id: bytes32, trusted_peers: Dict, testing: bool) -> bool:
-    if trusted_peers is None:
-        return False
-    if not testing and peer_host == "127.0.0.1":
-        return True
-    if peer_node_id.hex() not in trusted_peers:
-        return False
-
-    return True
-
-
 def select_port(prefer_ipv6: bool, addresses: List[Any]) -> uint16:
     selected_port: uint16
     for address_string, port, *_ in addresses:
         address = ip_address(address_string)
         if address.version == 6 and prefer_ipv6:
             selected_port = port
             break
```

### Comparing `chia-blockchain-1.8.0b5/chia/util/paginator.py` & `chia-blockchain-1.8.0b6/chia/util/paginator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/partial_func.py` & `chia-blockchain-1.8.0b6/chia/util/partial_func.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/path.py` & `chia-blockchain-1.8.0b6/chia/util/path.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/pprint.py` & `chia-blockchain-1.8.0b6/chia/util/pprint.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/prev_transaction_block.py` & `chia-blockchain-1.8.0b6/chia/util/prev_transaction_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/profiler.py` & `chia-blockchain-1.8.0b6/chia/util/profiler.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/service_groups.py` & `chia-blockchain-1.8.0b6/chia/util/service_groups.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/significant_bits.py` & `chia-blockchain-1.8.0b6/chia/util/significant_bits.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/ssl_check.py` & `chia-blockchain-1.8.0b6/chia/util/ssl_check.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/streamable.py` & `chia-blockchain-1.8.0b6/chia/util/streamable.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/struct_stream.py` & `chia-blockchain-1.8.0b6/chia/util/struct_stream.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/task_timing.py` & `chia-blockchain-1.8.0b6/chia/util/task_timing.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/validate_alert.py` & `chia-blockchain-1.8.0b6/chia/util/validate_alert.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/vdf_prover.py` & `chia-blockchain-1.8.0b6/chia/util/vdf_prover.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/util/ws_message.py` & `chia-blockchain-1.8.0b6/chia/util/ws_message.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/block_record.py` & `chia-blockchain-1.8.0b6/chia/wallet/block_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/cat_constants.py` & `chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_constants.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/cat_info.py` & `chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_info.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/cat_outer_puzzle.py` & `chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_outer_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/cat_utils.py` & `chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,22 +107,19 @@
     """
 
     N = len(spendable_cat_list)
 
     # figure out what the deltas are by running the inner puzzles & solutions
     deltas: List[int] = []
     for spend_info in spendable_cat_list:
-        error, conditions, cost = conditions_dict_for_solution(
-            spend_info.inner_puzzle, spend_info.inner_solution, INFINITE_COST
-        )
+        conditions = conditions_dict_for_solution(spend_info.inner_puzzle, spend_info.inner_solution, INFINITE_COST)
         total = spend_info.extra_delta * -1
-        if conditions:
-            for _ in conditions.get(ConditionOpcode.CREATE_COIN, []):
-                if _.vars[1] != b"\x8f":  # -113 in bytes
-                    total += Program.to(_.vars[1]).as_int()
+        for _ in conditions.get(ConditionOpcode.CREATE_COIN, []):
+            if _.vars[1] != b"\x8f":  # -113 in bytes
+                total += Program.to(_.vars[1]).as_int()
         deltas.append(spend_info.coin.amount - total)
 
     if sum(deltas) != 0:
         raise ValueError("input and output amounts don't match")
 
     subtotals = subtotals_for_deltas(deltas)
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/cat_wallet.py` & `chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/cat_wallet.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,29 +502,28 @@
                 puzzle_hash = inner_puzzle.get_tree_hash()
                 ret = await self.wallet_state_manager.get_keys(puzzle_hash)
                 if ret is None:
                     # Abort signing the entire SpendBundle - sign all or none
                     raise RuntimeError(f"Failed to get keys for puzzle_hash {puzzle_hash}")
                 pubkey, private = ret
                 synthetic_secret_key = calculate_synthetic_secret_key(private, DEFAULT_HIDDEN_PUZZLE_HASH)
-                error, conditions, cost = conditions_dict_for_solution(
+                conditions = conditions_dict_for_solution(
                     spend.puzzle_reveal.to_program(),
                     spend.solution.to_program(),
                     self.wallet_state_manager.constants.MAX_BLOCK_COST_CLVM,
                 )
-                if conditions is not None:
-                    synthetic_pk = synthetic_secret_key.get_g1()
-                    for pk, msg in pkm_pairs_for_conditions_dict(
-                        conditions, spend.coin.name(), self.wallet_state_manager.constants.AGG_SIG_ME_ADDITIONAL_DATA
-                    ):
-                        try:
-                            assert bytes(synthetic_pk) == pk
-                            sigs.append(AugSchemeMPL.sign(synthetic_secret_key, msg))
-                        except AssertionError:
-                            raise ValueError("This spend bundle cannot be signed by the CAT wallet")
+                synthetic_pk = synthetic_secret_key.get_g1()
+                for pk, msg in pkm_pairs_for_conditions_dict(
+                    conditions, spend.coin.name(), self.wallet_state_manager.constants.AGG_SIG_ME_ADDITIONAL_DATA
+                ):
+                    try:
+                        assert bytes(synthetic_pk) == pk
+                        sigs.append(AugSchemeMPL.sign(synthetic_secret_key, msg))
+                    except AssertionError:
+                        raise ValueError("This spend bundle cannot be signed by the CAT wallet")
 
         agg_sig = AugSchemeMPL.aggregate(sigs)
         return SpendBundle.aggregate([spend_bundle, SpendBundle([], agg_sig)])
 
     async def inner_puzzle_for_cat_puzhash(self, cat_hash: bytes32) -> Program:
         record: Optional[
             DerivationRecord
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/cat_wallet/lineage_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/cat_wallet/lineage_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/chialisp.py` & `chia-blockchain-1.8.0b6/chia/wallet/chialisp.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/coin_selection.py` & `chia-blockchain-1.8.0b6/chia/wallet/coin_selection.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/db_wallet/db_wallet_puzzles.py` & `chia-blockchain-1.8.0b6/chia/wallet/db_wallet/db_wallet_puzzles.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/derivation_record.py` & `chia-blockchain-1.8.0b6/chia/wallet/derivation_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/derive_keys.py` & `chia-blockchain-1.8.0b6/chia/wallet/derive_keys.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/did_wallet/did_info.py` & `chia-blockchain-1.8.0b6/chia/wallet/did_wallet/did_info.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/did_wallet/did_wallet.py` & `chia-blockchain-1.8.0b6/chia/wallet/did_wallet/did_wallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import re
 import time
 from secrets import token_bytes
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Tuple
 
 from blspy import AugSchemeMPL, G1Element, G2Element
 
-import chia.wallet.singleton
 from chia.full_node.full_node_api import FullNodeAPI
 from chia.protocols import wallet_protocol
 from chia.protocols.wallet_protocol import CoinState
 from chia.server.ws_connection import WSChiaConnection
 from chia.types.announcement import Announcement
 from chia.types.blockchain_format.coin import Coin
 from chia.types.blockchain_format.program import Program
@@ -32,15 +31,20 @@
 from chia.wallet.lineage_proof import LineageProof
 from chia.wallet.puzzles.p2_delegated_puzzle_or_hidden_puzzle import (
     DEFAULT_HIDDEN_PUZZLE_HASH,
     calculate_synthetic_secret_key,
     puzzle_for_pk,
     puzzle_hash_for_pk,
 )
-from chia.wallet.singleton import create_fullpuz
+from chia.wallet.singleton import (
+    SINGLETON_LAUNCHER_PUZZLE,
+    create_singleton_puzzle,
+    create_singleton_puzzle_hash,
+    get_inner_puzzle_from_singleton,
+)
 from chia.wallet.transaction_record import TransactionRecord
 from chia.wallet.util.compute_memos import compute_memos
 from chia.wallet.util.transaction_type import TransactionType
 from chia.wallet.util.wallet_types import WalletType
 from chia.wallet.wallet import CHIP_0002_SIGN_MESSAGE_PREFIX, Wallet
 from chia.wallet.wallet_coin_record import WalletCoinRecord
 from chia.wallet.wallet_info import WalletInfo
@@ -380,15 +384,15 @@
             assert parent_state.spent_height is not None
             puzzle_solution_request = wallet_protocol.RequestPuzzleSolution(
                 coin.parent_coin_info, uint32(parent_state.spent_height)
             )
             response = await peer.call_api(FullNodeAPI.request_puzzle_solution, puzzle_solution_request)
             req_puz_sol = response.response
             assert req_puz_sol.puzzle is not None
-            parent_innerpuz = chia.wallet.singleton.get_innerpuzzle_from_puzzle(req_puz_sol.puzzle.to_program())
+            parent_innerpuz = get_inner_puzzle_from_singleton(req_puz_sol.puzzle.to_program())
             if parent_innerpuz:
                 parent_info = LineageProof(
                     parent_state.coin.parent_coin_info,
                     parent_innerpuz.get_tree_hash(),
                     uint64(parent_state.coin.amount),
                 )
 
@@ -399,15 +403,15 @@
         self.log.info(f"DID wallet has been notified that coin was added: {coin.name()}:{coin}")
         inner_puzzle = await self.inner_puzzle_for_did_puzzle(coin.puzzle_hash)
         # Check inner puzzle consistency
         assert self.did_info.origin_coin is not None
 
         # TODO: if not the first singleton, and solution mode == recovery
         if not self._coin_is_first_singleton(coin):
-            full_puzzle = create_fullpuz(inner_puzzle, self.did_info.origin_coin.name())
+            full_puzzle = create_singleton_puzzle(inner_puzzle, self.did_info.origin_coin.name())
             assert full_puzzle.get_tree_hash() == coin.puzzle_hash
         if self.did_info.temp_coin is not None:
             self.wallet_state_manager.state_changed("did_coin_added", self.wallet_info.id)
 
         new_info = DIDInfo(
             self.did_info.origin_coin,
             self.did_info.backup_ids,
@@ -499,80 +503,52 @@
                     did_info.metadata,
                 )
 
                 await self.save_info(did_info)
                 assert children_state.created_height
                 parent_spend = await wallet_node.fetch_puzzle_solution(children_state.created_height, parent_coin, peer)
                 assert parent_spend is not None
-                parent_innerpuz = chia.wallet.singleton.get_innerpuzzle_from_puzzle(
-                    parent_spend.puzzle_reveal.to_program()
-                )
+                parent_innerpuz = get_inner_puzzle_from_singleton(parent_spend.puzzle_reveal.to_program())
                 assert parent_innerpuz is not None
                 parent_info = LineageProof(
                     parent_coin.parent_coin_info,
                     parent_innerpuz.get_tree_hash(),
                     uint64(parent_coin.amount),
                 )
                 await self.add_parent(child_coin.parent_coin_info, parent_info)
             parent_coin = child_coin
         assert parent_info is not None
 
-    async def create_tandem_xch_tx(
-        self,
-        fee: uint64,
-        announcement_to_assert: Optional[Announcement] = None,
-        reuse_puzhash: Optional[bool] = None,
-    ) -> TransactionRecord:
-        chia_coins = await self.standard_wallet.select_coins(fee)
-        if reuse_puzhash is None:
-            reuse_puzhash_config = self.wallet_state_manager.config.get("reuse_public_key_for_change", None)
-            if reuse_puzhash_config is None:
-                reuse_puzhash = False
-            else:
-                reuse_puzhash = reuse_puzhash_config.get(
-                    str(self.wallet_state_manager.wallet_node.logged_in_fingerprint), False
-                )
-        chia_tx = await self.standard_wallet.generate_signed_transaction(
-            uint64(0),
-            (await self.standard_wallet.get_puzzle_hash(not reuse_puzhash)),
-            fee=fee,
-            coins=chia_coins,
-            coin_announcements_to_consume={announcement_to_assert} if announcement_to_assert is not None else None,
-            reuse_puzhash=reuse_puzhash,
-        )
-        assert chia_tx.spend_bundle is not None
-        return chia_tx
-
     def puzzle_for_pk(self, pubkey: G1Element) -> Program:
         if self.did_info.origin_coin is not None:
             innerpuz = did_wallet_puzzles.create_innerpuz(
                 puzzle_for_pk(pubkey),
                 self.did_info.backup_ids,
                 self.did_info.num_of_backup_ids_needed,
                 self.did_info.origin_coin.name(),
                 did_wallet_puzzles.metadata_to_program(json.loads(self.did_info.metadata)),
             )
-            return chia.wallet.singleton.create_fullpuz(innerpuz, self.did_info.origin_coin.name())
+            return create_singleton_puzzle(innerpuz, self.did_info.origin_coin.name())
         else:
             innerpuz = Program.to((8, 0))
-            return chia.wallet.singleton.create_fullpuz(innerpuz, bytes32([0] * 32))
+            return create_singleton_puzzle(innerpuz, bytes32([0] * 32))
 
     def puzzle_hash_for_pk(self, pubkey: G1Element) -> bytes32:
         if self.did_info.origin_coin is None:
             # TODO: this seem dumb. Why bother with this case? Is it ever used?
             return puzzle_for_pk(pubkey).get_tree_hash()
         origin_coin_name = self.did_info.origin_coin.name()
         innerpuz_hash = did_wallet_puzzles.get_inner_puzhash_by_p2(
             puzzle_hash_for_pk(pubkey),
             self.did_info.backup_ids,
             self.did_info.num_of_backup_ids_needed,
             origin_coin_name,
             did_wallet_puzzles.metadata_to_program(json.loads(self.did_info.metadata)),
         )
-        return chia.wallet.singleton.create_fullpuz_hash(innerpuz_hash, origin_coin_name)
+        return create_singleton_puzzle_hash(innerpuz_hash, origin_coin_name)
 
     async def get_new_puzzle(self) -> Program:
         return self.puzzle_for_pk(
             (await self.wallet_state_manager.get_unused_derivation_record(self.wallet_info.id)).pubkey
         )
 
     def get_my_DID(self) -> str:
@@ -612,15 +588,15 @@
             ],
             coin_announcements={coin.name()},
         )
         innersol: Program = Program.to([1, p2_solution])
         # full solution is (corehash parent_info my_amount innerpuz_reveal solution)
         innerpuz: Program = self.did_info.current_inner
 
-        full_puzzle: Program = chia.wallet.singleton.create_fullpuz(
+        full_puzzle: Program = create_singleton_puzzle(
             innerpuz,
             self.did_info.origin_coin.name(),
         )
         parent_info = self.get_parent_for_coin(coin)
         assert parent_info is not None
         fullsol = Program.to(
             [
@@ -630,15 +606,15 @@
                     parent_info.amount,
                 ],
                 coin.amount,
                 innersol,
             ]
         )
         # Create an additional spend to confirm the change on-chain
-        new_full_puzzle: Program = chia.wallet.singleton.create_fullpuz(
+        new_full_puzzle: Program = create_singleton_puzzle(
             new_inner_puzzle,
             self.did_info.origin_coin.name(),
         )
         new_full_sol = Program.to(
             [
                 [
                     coin.parent_coin_info,
@@ -651,15 +627,15 @@
         )
         new_coin = Coin(coin.name(), new_full_puzzle.get_tree_hash(), coin.amount)
         list_of_coinspends = [CoinSpend(coin, full_puzzle, fullsol), CoinSpend(new_coin, new_full_puzzle, new_full_sol)]
         unsigned_spend_bundle = SpendBundle(list_of_coinspends, G2Element())
         spend_bundle = await self.sign(unsigned_spend_bundle)
         if fee > 0:
             announcement_to_make = coin.name()
-            chia_tx = await self.create_tandem_xch_tx(
+            chia_tx = await self.standard_wallet.create_tandem_xch_tx(
                 fee, Announcement(coin.name(), announcement_to_make), reuse_puzhash=reuse_puzhash
             )
         else:
             announcement_to_make = None
             chia_tx = None
         if chia_tx is not None and chia_tx.spend_bundle is not None:
             spend_bundle = SpendBundle.aggregate([spend_bundle, chia_tx.spend_bundle])
@@ -732,15 +708,15 @@
         # innerpuz solution is
         # (mode, p2_solution)
         innersol: Program = Program.to([2, p2_solution])
         if with_recovery:
             innersol = Program.to([2, p2_solution, [], [], [], self.did_info.backup_ids])
         # full solution is (corehash parent_info my_amount innerpuz_reveal solution)
 
-        full_puzzle: Program = chia.wallet.singleton.create_fullpuz(
+        full_puzzle: Program = create_singleton_puzzle(
             self.did_info.current_inner,
             self.did_info.origin_coin.name(),
         )
         parent_info = self.get_parent_for_coin(coin)
         assert parent_info is not None
         fullsol = Program.to(
             [
@@ -754,15 +730,15 @@
             ]
         )
         list_of_coinspends = [CoinSpend(coin, full_puzzle, fullsol)]
         unsigned_spend_bundle = SpendBundle(list_of_coinspends, G2Element())
         spend_bundle = await self.sign(unsigned_spend_bundle)
         if fee > 0:
             announcement_to_make = coin.name()
-            chia_tx = await self.create_tandem_xch_tx(
+            chia_tx = await self.standard_wallet.create_tandem_xch_tx(
                 fee, Announcement(coin.name(), announcement_to_make), reuse_puzhash=reuse_puzhash
             )
         else:
             chia_tx = None
         if chia_tx is not None and chia_tx.spend_bundle is not None:
             spend_bundle = SpendBundle.aggregate([spend_bundle, chia_tx.spend_bundle])
             chia_tx = dataclasses.replace(chia_tx, spend_bundle=None)
@@ -818,15 +794,15 @@
             puzzle_announcements=puzzle_announcements,
             coin_announcements=coin_announcements,
         )
         # innerpuz solution is (mode p2_solution)
         innersol: Program = Program.to([1, p2_solution])
 
         # full solution is (corehash parent_info my_amount innerpuz_reveal solution)
-        full_puzzle: Program = chia.wallet.singleton.create_fullpuz(
+        full_puzzle: Program = create_singleton_puzzle(
             innerpuz,
             self.did_info.origin_coin.name(),
         )
         parent_info = self.get_parent_for_coin(coin)
         assert parent_info is not None
         fullsol = Program.to(
             [
@@ -853,15 +829,15 @@
         message_puz = Program.to((1, [[51, puzhash, coin.amount - 1, [puzhash]], [51, 0x00, -113]]))
 
         # innerpuz solution is (mode p2_solution)
         innersol: Program = Program.to([1, [[], message_puz, []]])
         # full solution is (corehash parent_info my_amount innerpuz_reveal solution)
         innerpuz: Program = self.did_info.current_inner
 
-        full_puzzle: Program = chia.wallet.singleton.create_fullpuz(
+        full_puzzle: Program = create_singleton_puzzle(
             innerpuz,
             self.did_info.origin_coin.name(),
         )
         parent_info = self.get_parent_for_coin(coin)
         assert parent_info is not None
         fullsol = Program.to(
             [
@@ -932,15 +908,15 @@
                 },
                 {"puzzlehash": innermessage, "amount": uint64(0), "memos": []},
             ],
         )
         innersol = Program.to([1, p2_solution])
 
         # full solution is (corehash parent_info my_amount innerpuz_reveal solution)
-        full_puzzle: Program = chia.wallet.singleton.create_fullpuz(
+        full_puzzle: Program = create_singleton_puzzle(
             innerpuz,
             self.did_info.origin_coin.name(),
         )
         parent_info = self.get_parent_for_coin(coin)
         assert parent_info is not None
 
         fullsol = Program.to(
@@ -1049,15 +1025,15 @@
                 self.did_info.backup_ids,
                 coin.name(),
             ]
         )
         # full solution is (parent_info my_amount solution)
         assert self.did_info.current_inner is not None
         innerpuz: Program = self.did_info.current_inner
-        full_puzzle: Program = chia.wallet.singleton.create_fullpuz(
+        full_puzzle: Program = create_singleton_puzzle(
             innerpuz,
             self.did_info.origin_coin.name(),
         )
         parent_info = self.get_parent_for_coin(coin)
         assert parent_info is not None
         fullsol = Program.to(
             [
@@ -1230,50 +1206,48 @@
         for spend in spend_bundle.coin_spends:
             puzzle_args = did_wallet_puzzles.match_did_puzzle(*spend.puzzle_reveal.to_program().uncurry())
             if puzzle_args is not None:
                 p2_puzzle, _, _, _, _ = puzzle_args
                 puzzle_hash = p2_puzzle.get_tree_hash()
                 pubkey, private = await self.wallet_state_manager.get_keys(puzzle_hash)
                 synthetic_secret_key = calculate_synthetic_secret_key(private, DEFAULT_HIDDEN_PUZZLE_HASH)
-                error, conditions, cost = conditions_dict_for_solution(
+                conditions = conditions_dict_for_solution(
                     spend.puzzle_reveal.to_program(),
                     spend.solution.to_program(),
                     self.wallet_state_manager.constants.MAX_BLOCK_COST_CLVM,
                 )
-
-                if conditions is not None:
-                    synthetic_pk = synthetic_secret_key.get_g1()
-                    for pk, msg in pkm_pairs_for_conditions_dict(
-                        conditions, spend.coin.name(), self.wallet_state_manager.constants.AGG_SIG_ME_ADDITIONAL_DATA
-                    ):
-                        try:
-                            assert bytes(synthetic_pk) == pk
-                            sigs.append(AugSchemeMPL.sign(synthetic_secret_key, msg))
-                        except AssertionError:
-                            raise ValueError("This spend bundle cannot be signed by the DID wallet")
+                synthetic_pk = synthetic_secret_key.get_g1()
+                for pk, msg in pkm_pairs_for_conditions_dict(
+                    conditions, spend.coin.name(), self.wallet_state_manager.constants.AGG_SIG_ME_ADDITIONAL_DATA
+                ):
+                    try:
+                        assert bytes(synthetic_pk) == pk
+                        sigs.append(AugSchemeMPL.sign(synthetic_secret_key, msg))
+                    except AssertionError:
+                        raise ValueError("This spend bundle cannot be signed by the DID wallet")
 
         agg_sig = AugSchemeMPL.aggregate(sigs)
         return SpendBundle.aggregate([spend_bundle, SpendBundle([], agg_sig)])
 
     async def generate_new_decentralised_id(self, amount: uint64, fee: uint64 = uint64(0)) -> Optional[SpendBundle]:
         """
         This must be called under the wallet state manager lock
         """
 
         coins = await self.standard_wallet.select_coins(uint64(amount + fee))
         if coins is None:
             return None
 
         origin = coins.copy().pop()
-        genesis_launcher_puz = chia.wallet.singleton.LAUNCHER_PUZZLE
+        genesis_launcher_puz = SINGLETON_LAUNCHER_PUZZLE
         launcher_coin = Coin(origin.name(), genesis_launcher_puz.get_tree_hash(), amount)
 
         did_inner: Program = await self.get_new_did_innerpuz(launcher_coin.name())
         did_inner_hash = did_inner.get_tree_hash()
-        did_full_puz = chia.wallet.singleton.create_fullpuz(did_inner, launcher_coin.name())
+        did_full_puz = create_singleton_puzzle(did_inner, launcher_coin.name())
         did_puzzle_hash = did_full_puz.get_tree_hash()
 
         announcement_set: Set[Announcement] = set()
         announcement_message = Program.to([did_puzzle_hash, amount, bytes(0x80)]).get_tree_hash()
         announcement_set.add(Announcement(launcher_coin.name(), announcement_message))
 
         tx_record: Optional[TransactionRecord] = await self.standard_wallet.generate_signed_transaction(
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/did_wallet/did_wallet_puzzles.py` & `chia-blockchain-1.8.0b6/chia/wallet/did_wallet/did_wallet_puzzles.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.types.coin_spend import CoinSpend
 from chia.types.condition_opcodes import ConditionOpcode
 from chia.util.ints import uint64
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 from chia.wallet.singleton import (
-    LAUNCHER_PUZZLE_HASH,
+    SINGLETON_LAUNCHER_PUZZLE_HASH,
     SINGLETON_TOP_LAYER_MOD,
     SINGLETON_TOP_LAYER_MOD_HASH,
     is_singleton,
 )
 from chia.wallet.util.curry_and_treehash import calculate_hash_of_quoted_mod_hash, curry_and_treehash
 
 DID_INNERPUZ_MOD = load_clvm_maybe_recompile("did_innerpuz.clvm")
@@ -41,15 +41,15 @@
     :param metadata: DID customized metadata
     :param recovery_list_hash: Recovery list hash
     :return: DID inner puzzle
     """
     backup_ids_hash = Program(Program.to(recovery_list)).get_tree_hash()
     if recovery_list_hash is not None:
         backup_ids_hash = recovery_list_hash
-    singleton_struct = Program.to((SINGLETON_TOP_LAYER_MOD_HASH, (launcher_id, LAUNCHER_PUZZLE_HASH)))
+    singleton_struct = Program.to((SINGLETON_TOP_LAYER_MOD_HASH, (launcher_id, SINGLETON_LAUNCHER_PUZZLE_HASH)))
     return DID_INNERPUZ_MOD.curry(p2_puzzle, backup_ids_hash, num_of_backup_ids_needed, singleton_struct, metadata)
 
 
 def get_inner_puzhash_by_p2(
     p2_puzhash: bytes32,
     recovery_list: List[bytes32],
     num_of_backup_ids_needed: uint64,
@@ -63,15 +63,15 @@
     :param num_of_backup_ids_needed: Need how many DIDs for the recovery
     :param launcher_id: ID of the launch coin
     :param metadata: DID customized metadata
     :return: DID inner puzzle hash
     """
 
     backup_ids_hash = Program(Program.to(recovery_list)).get_tree_hash()
-    singleton_struct = Program.to((SINGLETON_TOP_LAYER_MOD_HASH, (launcher_id, LAUNCHER_PUZZLE_HASH)))
+    singleton_struct = Program.to((SINGLETON_TOP_LAYER_MOD_HASH, (launcher_id, SINGLETON_LAUNCHER_PUZZLE_HASH)))
 
     quoted_mod_hash = calculate_hash_of_quoted_mod_hash(DID_INNERPUZ_MOD_HASH)
 
     return curry_and_treehash(
         quoted_mod_hash,
         p2_puzhash,
         Program.to(backup_ids_hash).get_tree_hash(),
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/driver_protocol.py` & `chia-blockchain-1.8.0b6/chia/wallet/driver_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/key_val_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/key_val_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/lineage_proof.py` & `chia-blockchain-1.8.0b6/chia/wallet/lineage_proof.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/metadata_outer_puzzle.py` & `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/metadata_outer_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/nft_info.py` & `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/nft_info.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/nft_puzzles.py` & `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/nft_puzzles.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/nft_wallet.py` & `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/nft_wallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,32 +460,31 @@
             for ph in puzzle_hashes:
                 keys = await self.wallet_state_manager.get_keys(ph)
                 assert keys
                 pks[bytes(keys[0])] = private = keys[1]
                 synthetic_secret_key = calculate_synthetic_secret_key(private, DEFAULT_HIDDEN_PUZZLE_HASH)
                 synthetic_pk = synthetic_secret_key.get_g1()
                 pks[bytes(synthetic_pk)] = synthetic_secret_key
-            error, conditions, cost = conditions_dict_for_solution(
+            conditions = conditions_dict_for_solution(
                 spend.puzzle_reveal.to_program(),
                 spend.solution.to_program(),
                 self.wallet_state_manager.constants.MAX_BLOCK_COST_CLVM,
             )
-            if conditions is not None:
-                for pk, msg in pkm_pairs_for_conditions_dict(
-                    conditions, spend.coin.name(), self.wallet_state_manager.constants.AGG_SIG_ME_ADDITIONAL_DATA
-                ):
-                    try:
-                        sk = pks.get(pk)
-                        if sk:
-                            self.log.debug("Found key, signing for pk: %s", pk)
-                            sigs.append(AugSchemeMPL.sign(sk, msg))
-                        else:
-                            self.log.warning("Couldn't find key for: %s", pk)
-                    except AssertionError:
-                        raise ValueError("This spend bundle cannot be signed by the NFT wallet")
+            for pk, msg in pkm_pairs_for_conditions_dict(
+                conditions, spend.coin.name(), self.wallet_state_manager.constants.AGG_SIG_ME_ADDITIONAL_DATA
+            ):
+                try:
+                    sk = pks.get(pk)
+                    if sk:
+                        self.log.debug("Found key, signing for pk: %s", pk)
+                        sigs.append(AugSchemeMPL.sign(sk, msg))
+                    else:
+                        self.log.warning("Couldn't find key for: %s", pk)
+                except AssertionError:
+                    raise ValueError("This spend bundle cannot be signed by the NFT wallet")
 
         agg_sig = AugSchemeMPL.aggregate(sigs)
         return SpendBundle.aggregate([spend_bundle, SpendBundle([], agg_sig)])
 
     async def update_metadata(
         self,
         nft_coin_info: NFTCoinInfo,
@@ -606,40 +605,14 @@
         return await cls.create_new_nft_wallet(
             wallet_state_manager,
             wallet,
             None,
             name,
         )
 
-    async def create_tandem_xch_tx(
-        self,
-        fee: uint64,
-        announcement_to_assert: Optional[Announcement] = None,
-        reuse_puzhash: Optional[bool] = None,
-    ) -> TransactionRecord:
-        chia_coins = await self.standard_wallet.select_coins(fee)
-        if reuse_puzhash is None:
-            reuse_puzhash_config = self.wallet_state_manager.config.get("reuse_public_key_for_change", None)
-            if reuse_puzhash_config is None:
-                reuse_puzhash = False
-            else:
-                reuse_puzhash = reuse_puzhash_config.get(
-                    str(self.wallet_state_manager.wallet_node.logged_in_fingerprint), False
-                )
-        chia_tx = await self.standard_wallet.generate_signed_transaction(
-            uint64(0),
-            (await self.standard_wallet.get_puzzle_hash(not reuse_puzhash)),
-            fee=fee,
-            coins=chia_coins,
-            coin_announcements_to_consume={announcement_to_assert} if announcement_to_assert is not None else None,
-            reuse_puzhash=reuse_puzhash,
-        )
-        assert chia_tx.spend_bundle is not None
-        return chia_tx
-
     async def generate_signed_transaction(
         self,
         amounts: List[uint64],
         puzzle_hashes: List[bytes32],
         fee: uint64 = uint64(0),
         coins: Optional[Set[Coin]] = None,
         nft_coin: Optional[NFTCoinInfo] = None,
@@ -747,15 +720,15 @@
 
         primaries: List[AmountWithPuzzlehash] = []
         for payment in payments:
             primaries.append({"puzzlehash": payment.puzzle_hash, "amount": payment.amount, "memos": payment.memos})
 
         if fee > 0:
             announcement_to_make = nft_coin.coin.name()
-            chia_tx = await self.create_tandem_xch_tx(
+            chia_tx = await self.standard_wallet.create_tandem_xch_tx(
                 fee, Announcement(nft_coin.coin.name(), announcement_to_make), reuse_puzhash=reuse_puzhash
             )
         else:
             announcement_to_make = None
             chia_tx = None
 
         innersol: Program = self.standard_wallet.make_solution(
@@ -1367,15 +1340,15 @@
         p2_inner_puzzle = await self.standard_wallet.get_new_puzzle()
         p2_inner_ph = p2_inner_puzzle.get_tree_hash()
 
         # Loop to create each intermediate coin, launcher, eve and (optional) transfer spends
         for mint_number in range(mint_number_start, mint_number_end):
             # Create  the puzzle, solution and coin spend for the intermediate launcher
             intermediate_launcher_puz = did_wallet_puzzles.INTERMEDIATE_LAUNCHER_MOD.curry(
-                chia.wallet.singleton.LAUNCHER_PUZZLE_HASH, mint_number, mint_total
+                chia.wallet.singleton.SINGLETON_LAUNCHER_PUZZLE_HASH, mint_number, mint_total
             )
             intermediate_launcher_ph = intermediate_launcher_puz.get_tree_hash()
             primaries.append(
                 AmountWithPuzzlehash(
                     {
                         "puzzlehash": intermediate_launcher_ph,
                         "amount": uint64(0),
@@ -1393,15 +1366,17 @@
             # create an ASSERT_COIN_ANNOUNCEMENT for the DID spend. The
             # intermediate launcher coin issues a CREATE_COIN_ANNOUNCEMENT of
             # the mint_number and mint_total for the launcher coin it creates
             intermediate_announcement_message = std_hash(int_to_bytes(mint_number) + int_to_bytes(mint_total))
             did_announcements.add(std_hash(intermediate_launcher_coin.name() + intermediate_announcement_message))
 
             # Create the launcher coin, and add its id to a list to be asserted in the DID spend
-            launcher_coin = Coin(intermediate_launcher_coin.name(), chia.wallet.singleton.LAUNCHER_PUZZLE_HASH, amount)
+            launcher_coin = Coin(
+                intermediate_launcher_coin.name(), chia.wallet.singleton.SINGLETON_LAUNCHER_PUZZLE_HASH, amount
+            )
             launcher_ids.append(launcher_coin.name())
 
             # Grab the metadata from metadata_list. The index for metadata_list
             # needs to be offset by mint_number_start
             metadata = metadata_list[mint_number - mint_number_start]
 
             # Create the inner and full puzzles for the eve spend
@@ -1418,15 +1393,17 @@
 
             # Annnouncements for eve spend. These are asserted by the DID spend
             announcement_message = Program.to([eve_fullpuz.get_tree_hash(), amount, []]).get_tree_hash()
             did_announcements.add(std_hash(launcher_coin.name() + announcement_message))
 
             genesis_launcher_solution = Program.to([eve_fullpuz.get_tree_hash(), amount, []])
 
-            launcher_cs = CoinSpend(launcher_coin, chia.wallet.singleton.LAUNCHER_PUZZLE, genesis_launcher_solution)
+            launcher_cs = CoinSpend(
+                launcher_coin, chia.wallet.singleton.SINGLETON_LAUNCHER_PUZZLE, genesis_launcher_solution
+            )
             launcher_spends.append(launcher_cs)
 
             eve_coin = Coin(launcher_coin.name(), eve_fullpuz.get_tree_hash(), uint64(amount))
 
             # To make the eve transaction we need to construct the NFTCoinInfo
             # for the NFT (which doesn't exist yet)
             nft_coin = NFTCoinInfo(
@@ -1514,15 +1491,15 @@
         did_p2_solution = self.standard_wallet.make_solution(
             primaries=primaries,
             coin_announcements=did_coin_announcement,
             coin_announcements_to_assert=did_announcements,
             puzzle_announcements_to_assert=puzzle_assertions,
         )
         did_inner_sol: Program = Program.to([1, did_p2_solution])
-        did_full_puzzle: Program = chia.wallet.singleton.create_fullpuz(
+        did_full_puzzle: Program = chia.wallet.singleton.create_singleton_puzzle(
             innerpuz,
             did_wallet.did_info.origin_coin.name(),
         )
         # The DID lineage parent won't not exist if we're bulk minting from a future DID coin
         if did_lineage_parent:
             did_parent_info: Optional[LineageProof] = LineageProof(
                 parent_name=did_lineage_parent,
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/ownership_outer_puzzle.py` & `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/ownership_outer_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/singleton_outer_puzzle.py` & `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/singleton_outer_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/transfer_program_puzzle.py` & `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/transfer_program_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/nft_wallet/uncurry_nft.py` & `chia-blockchain-1.8.0b6/chia/wallet/nft_wallet/uncurry_nft.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/notification_manager.py` & `chia-blockchain-1.8.0b6/chia/wallet/notification_manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/notification_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/notification_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/outer_puzzles.py` & `chia-blockchain-1.8.0b6/chia/wallet/outer_puzzles.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/payment.py` & `chia-blockchain-1.8.0b6/chia/wallet/payment.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzle_drivers.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzle_drivers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/block_program_zero.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/block_program_zero.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/cat_truths.clib` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_truths.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/cat_v2.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_v2.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/cat_v2.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/cat_v2.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/chialisp_deserialisation.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/chialisp_deserialisation.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/chialisp_deserialisation.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/chialisp_deserialisation.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/condition_codes.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/condition_codes.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/create-lock-puzzlehash.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/create-lock-puzzlehash.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/curry-and-treehash.clinc` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/curry-and-treehash.clinc`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/curry.clib` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/curry.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/delegated_tail.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/delegated_tail.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/did_innerpuz.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/did_innerpuz.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/did_innerpuz.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/did_innerpuz.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/genesis_by_coin_id.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_coin_id.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/genesis_by_puzzle_hash.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/genesis_by_puzzle_hash.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/graftroot_dl_offers.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/graftroot_dl_offers.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/graftroot_dl_offers.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/graftroot_dl_offers.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/json.clib` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/json.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/load_clvm.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/load_clvm.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/merkle_utils.clib` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/merkle_utils.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_metadata_updater_default.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_default.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_metadata_updater_updateable.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_metadata_updater_updateable.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_ownership_layer.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_layer.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_ownership_layer.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_layer.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_ownership_transfer_program_one_way_claim_with_royalties.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_state_layer.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_state_layer.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/nft_state_layer.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/nft_state_layer.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_conditions.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_conditions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_conditions.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_conditions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_puzzle.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_delegated_puzzle_or_hidden_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_m_of_n_delegate_direct.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_m_of_n_delegate_direct.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_puzzle_hash.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_puzzle_hash.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_singleton.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_singleton.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/p2_singleton_or_delayed_puzhash.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/pool_member_innerpuz.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_member_innerpuz.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/pool_member_innerpuz.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_member_innerpuz.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/pool_waitingroom_innerpuz.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/prefarm/make_prefarm_ph.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/prefarm/make_prefarm_ph.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,28 +36,22 @@
 
     solution = "()"
     prefix = "xch"
     print("PH", puzzle_hash)
     print(f"Address: {encode_puzzle_hash(puzzle_hash, prefix)}")
 
     result = puzzle_prog.run(solution)
-    error, result_human = parse_sexp_to_conditions(result)
-
     total_chia = 0
-    if error:
-        print(f"Error: {error}")
-    else:
-        assert result_human is not None
-        for cvp in result_human:
-            assert len(cvp.vars) == 2
-            total_chia += int_from_bytes(cvp.vars[1])
-            print(
-                f"{ConditionOpcode(cvp.opcode).name}: {encode_puzzle_hash(bytes32(cvp.vars[0]), prefix)},"
-                f" amount: {int_from_bytes(cvp.vars[1])}"
-            )
+    for cvp in parse_sexp_to_conditions(result):
+        assert len(cvp.vars) == 2
+        total_chia += int_from_bytes(cvp.vars[1])
+        print(
+            f"{ConditionOpcode(cvp.opcode).name}: {encode_puzzle_hash(bytes32(cvp.vars[0]), prefix)},"
+            f" amount: {int_from_bytes(cvp.vars[1])}"
+        )
     return total_chia
 
 
 total_chia = 0
 print("Pool address: ")
 total_chia += make_puzzle(pool_amounts)
 print("\nFarmer address: ")
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/prefarm/spend_prefarm.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/prefarm/spend_prefarm.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,15 @@
 from chia.util.ints import uint16, uint32
 
 
 def print_conditions(spend_bundle: SpendBundle):
     print("\nConditions:")
     for coin_spend in spend_bundle.coin_spends:
         result = Program.from_bytes(bytes(coin_spend.puzzle_reveal)).run(Program.from_bytes(bytes(coin_spend.solution)))
-        error, result_human = parse_sexp_to_conditions(result)
-        assert error is None
-        assert result_human is not None
-        for cvp in result_human:
+        for cvp in parse_sexp_to_conditions(result):
             print(f"{ConditionOpcode(cvp.opcode).name}: {[var.hex() for var in cvp.vars]}")
     print("")
 
 
 async def main() -> None:
     rpc_port: uint16 = uint16(8555)
     self_hostname = "localhost"
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/puzzle_utils.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/puzzle_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/rom_bootstrap_generator.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/rom_bootstrap_generator.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/rom_bootstrap_generator.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/rom_bootstrap_generator.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/settlement_payments.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/settlement_payments.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/settlement_payments_old.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments_old.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/settlement_payments_old.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/settlement_payments_old.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm.hex` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.clvm.hex`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_top_layer_v1_1.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_top_layer_v1_1.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/singleton_truths.clib` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/singleton_truths.clib`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/tails.py` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/tails.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm` & `chia-blockchain-1.8.0b6/chia/wallet/puzzles/test_multiple_generator_input_arguments.clvm`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/secret_key_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/secret_key_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/sign_coin_spends.py` & `chia-blockchain-1.8.0b6/chia/wallet/sign_coin_spends.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,21 +35,15 @@
     wallet rpc's get_private_key method).
     """
     signatures: List[blspy.G2Element] = []
     pk_list: List[blspy.G1Element] = []
     msg_list: List[bytes] = []
     for coin_spend in coin_spends:
         # Get AGG_SIG conditions
-        err, conditions_dict, cost = conditions_dict_for_solution(
-            coin_spend.puzzle_reveal, coin_spend.solution, max_cost
-        )
-        if err or conditions_dict is None:
-            error_msg = f"Sign transaction failed, con:{conditions_dict}, error: {err}"
-            raise ValueError(error_msg)
-
+        conditions_dict = conditions_dict_for_solution(coin_spend.puzzle_reveal, coin_spend.solution, max_cost)
         # Create signature
         for pk_bytes, msg in pkm_pairs_for_conditions_dict(conditions_dict, coin_spend.coin.name(), additional_data):
             pk = blspy.G1Element.from_bytes(pk_bytes)
             pk_list.append(pk)
             msg_list.append(msg)
             if inspect.iscoroutinefunction(secret_key_for_public_key_f):
                 secret_key = await secret_key_for_public_key_f(pk)
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/singleton.py` & `chia-blockchain-1.8.0b6/chia/wallet/singleton.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.wallet.puzzles.load_clvm import load_clvm_maybe_recompile
 from chia.wallet.util.curry_and_treehash import calculate_hash_of_quoted_mod_hash, curry_and_treehash
 
 SINGLETON_TOP_LAYER_MOD = load_clvm_maybe_recompile("singleton_top_layer_v1_1.clvm")
 SINGLETON_TOP_LAYER_MOD_HASH = SINGLETON_TOP_LAYER_MOD.get_tree_hash()
 SINGLETON_TOP_LAYER_MOD_HASH_QUOTED = calculate_hash_of_quoted_mod_hash(SINGLETON_TOP_LAYER_MOD_HASH)
-LAUNCHER_PUZZLE = load_clvm_maybe_recompile("singleton_launcher.clvm")
-LAUNCHER_PUZZLE_HASH = LAUNCHER_PUZZLE.get_tree_hash()
+SINGLETON_LAUNCHER_PUZZLE = load_clvm_maybe_recompile("singleton_launcher.clvm")
+SINGLETON_LAUNCHER_PUZZLE_HASH = SINGLETON_LAUNCHER_PUZZLE.get_tree_hash()
 
 
-def get_innerpuzzle_from_puzzle(puzzle: Program) -> Optional[Program]:
+def get_inner_puzzle_from_singleton(puzzle: Program) -> Optional[Program]:
     """
     Extract the inner puzzle of a singleton
     :param puzzle: Singleton puzzle
     :return: Inner puzzle
     """
     r = puzzle.uncurry()
     if r is None:
@@ -35,30 +35,30 @@
     Check if a puzzle is a singleton mod
     :param inner_f: puzzle
     :return: Boolean
     """
     return inner_f == SINGLETON_TOP_LAYER_MOD
 
 
-def create_fullpuz_hash(innerpuz_hash: bytes32, launcher_id: bytes32) -> bytes32:
+def create_singleton_puzzle_hash(innerpuz_hash: bytes32, launcher_id: bytes32) -> bytes32:
     """
     Return Hash ID of the whole Singleton Puzzle
     :param innerpuz_hash: Singleton inner puzzle tree hash
     :param launcher_id: launcher coin name
     :return: Singleton full puzzle hash
     """
     # singleton_struct = (MOD_HASH . (LAUNCHER_ID . LAUNCHER_PUZZLE_HASH))
-    singleton_struct = Program.to((SINGLETON_TOP_LAYER_MOD_HASH, (launcher_id, LAUNCHER_PUZZLE_HASH)))
+    singleton_struct = Program.to((SINGLETON_TOP_LAYER_MOD_HASH, (launcher_id, SINGLETON_LAUNCHER_PUZZLE_HASH)))
 
     return curry_and_treehash(SINGLETON_TOP_LAYER_MOD_HASH_QUOTED, singleton_struct.get_tree_hash(), innerpuz_hash)
 
 
-def create_fullpuz(innerpuz: Program, launcher_id: bytes32) -> Program:
+def create_singleton_puzzle(innerpuz: Program, launcher_id: bytes32) -> Program:
     """
     Create a full Singleton puzzle
     :param innerpuz: Singleton inner puzzle
     :param launcher_id:
     :return: Singleton full puzzle
     """
     # singleton_struct = (MOD_HASH . (LAUNCHER_ID . LAUNCHER_PUZZLE_HASH))
-    singleton_struct = Program.to((SINGLETON_TOP_LAYER_MOD_HASH, (launcher_id, LAUNCHER_PUZZLE_HASH)))
+    singleton_struct = Program.to((SINGLETON_TOP_LAYER_MOD_HASH, (launcher_id, SINGLETON_LAUNCHER_PUZZLE_HASH)))
     return SINGLETON_TOP_LAYER_MOD.curry(singleton_struct, innerpuz)
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/trade_manager.py` & `chia-blockchain-1.8.0b6/chia/wallet/trade_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -503,16 +503,20 @@
                                     f"Cannot offer assets from wallet id {wallet.id()} without more information"
                                 )
                     else:
                         asset_id = id
                         wallet = await self.wallet_state_manager.get_wallet_for_asset_id(asset_id.hex())
                     if not callable(getattr(wallet, "get_coins_to_offer", None)):  # ATTENTION: new wallets
                         raise ValueError(f"Cannot offer coins from wallet id {wallet.id()}")
+                    # For the XCH wallet also include the fee amount to the coins we use to pay this offer
+                    amount_to_select = abs(amount)
+                    if wallet.type() == WalletType.STANDARD_WALLET:
+                        amount_to_select += fee
                     coins_to_offer[id] = await wallet.get_coins_to_offer(
-                        asset_id, uint64(abs(amount)), min_coin_amount, max_coin_amount
+                        asset_id, uint64(amount_to_select), min_coin_amount, max_coin_amount
                     )
                     # Note: if we use check_for_special_offer_making, this is not used.
                 elif amount == 0:
                     raise ValueError("You cannot offer nor request 0 amount of something")
 
                 offer_dict_no_ints[asset_id] = amount
 
@@ -543,15 +547,18 @@
             notarized_payments: Dict[Optional[bytes32], List[NotarizedPayment]] = Offer.notarize_payments(
                 requested_payments, all_coins
             )
             announcements_to_assert = Offer.calculate_announcements(notarized_payments, driver_dict, old)
 
             all_transactions: List[TransactionRecord] = []
             fee_left_to_pay: uint64 = fee
-            for id, selected_coins in coins_to_offer.items():
+            # The access of the sorted keys here makes sure we create the XCH transaction first to make sure we pay fee
+            # with the XCH side of the offer and don't create an extra fee transaction in other wallets.
+            for id in sorted(coins_to_offer.keys()):
+                selected_coins = coins_to_offer[id]
                 if isinstance(id, int):
                     wallet = self.wallet_state_manager.wallets[id]
                 else:
                     wallet = await self.wallet_state_manager.get_wallet_for_asset_id(id.hex())
                 # This should probably not switch on whether or not we're spending XCH but it has to for now
                 if wallet.type() == WalletType.STANDARD_WALLET:
                     tx = await wallet.generate_signed_transaction(
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/trade_record.py` & `chia-blockchain-1.8.0b6/chia/wallet/trade_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/trading/offer.py` & `chia-blockchain-1.8.0b6/chia/wallet/trading/offer.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/trading/trade_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/trading/trade_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/transaction_record.py` & `chia-blockchain-1.8.0b6/chia/wallet/transaction_record.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/address_type.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/address_type.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/compute_hints.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/compute_hints.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/compute_memos.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/compute_memos.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/curry_and_treehash.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/curry_and_treehash.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/debug_spend_bundle.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/debug_spend_bundle.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,51 +69,48 @@
             print("*" * 80)
             continue
 
         print(f"consuming coin {dump_coin(coin)}")
         print(f"  with id {coin_name.hex()}")
         print()
         print(f"\nbrun -y main.sym '{bu_disassemble(puzzle_reveal)}' '{bu_disassemble(solution)}'")
-        error, conditions, cost = conditions_dict_for_solution(puzzle_reveal, solution, INFINITE_COST)
-        if error:
-            print(f"*** error {error}")
-        elif conditions is not None:
-            for pk_bytes, m in pkm_pairs_for_conditions_dict(conditions, coin_name, agg_sig_additional_data):
-                pks.append(G1Element.from_bytes(pk_bytes))
-                msgs.append(m)
-            print()
-            cost, r = puzzle_reveal.run_with_cost(INFINITE_COST, solution)  # type: ignore
-            print(disassemble(r))
-            print()
-            if conditions and len(conditions) > 0:
-                print("grouped conditions:")
-                for condition_programs in conditions.values():
-                    print()
-                    for c in condition_programs:
-                        if len(c.vars) == 1:
-                            as_prog = Program.to([c.opcode, c.vars[0]])
-                        if len(c.vars) == 2:
-                            as_prog = Program.to([c.opcode, c.vars[0], c.vars[1]])
-                        print(f"  {disassemble(as_prog)}")
-                created_coin_announcements.extend(
-                    [coin_name] + _.vars for _ in conditions.get(ConditionOpcode.CREATE_COIN_ANNOUNCEMENT, [])
-                )
-                asserted_coin_announcements.extend(
-                    [_.vars[0].hex() for _ in conditions.get(ConditionOpcode.ASSERT_COIN_ANNOUNCEMENT, [])]
-                )
-                created_puzzle_announcements.extend(
-                    [puzzle_reveal.get_tree_hash()] + _.vars
-                    for _ in conditions.get(ConditionOpcode.CREATE_PUZZLE_ANNOUNCEMENT, [])
-                )
-                asserted_puzzle_announcements.extend(
-                    [_.vars[0].hex() for _ in conditions.get(ConditionOpcode.ASSERT_PUZZLE_ANNOUNCEMENT, [])]
-                )
+        conditions = conditions_dict_for_solution(puzzle_reveal, solution, INFINITE_COST)
+        for pk_bytes, m in pkm_pairs_for_conditions_dict(conditions, coin_name, agg_sig_additional_data):
+            pks.append(G1Element.from_bytes(pk_bytes))
+            msgs.append(m)
+        print()
+        cost, r = puzzle_reveal.run_with_cost(INFINITE_COST, solution)
+        print(disassemble(r))
+        print()
+        if conditions and len(conditions) > 0:
+            print("grouped conditions:")
+            for condition_programs in conditions.values():
                 print()
-            else:
-                print("(no output conditions generated)")
+                for c in condition_programs:
+                    if len(c.vars) == 1:
+                        as_prog = Program.to([c.opcode, c.vars[0]])
+                    if len(c.vars) == 2:
+                        as_prog = Program.to([c.opcode, c.vars[0], c.vars[1]])
+                    print(f"  {disassemble(as_prog)}")
+            created_coin_announcements.extend(
+                [coin_name] + _.vars for _ in conditions.get(ConditionOpcode.CREATE_COIN_ANNOUNCEMENT, [])
+            )
+            asserted_coin_announcements.extend(
+                [_.vars[0].hex() for _ in conditions.get(ConditionOpcode.ASSERT_COIN_ANNOUNCEMENT, [])]
+            )
+            created_puzzle_announcements.extend(
+                [puzzle_reveal.get_tree_hash()] + _.vars
+                for _ in conditions.get(ConditionOpcode.CREATE_PUZZLE_ANNOUNCEMENT, [])
+            )
+            asserted_puzzle_announcements.extend(
+                [_.vars[0].hex() for _ in conditions.get(ConditionOpcode.ASSERT_PUZZLE_ANNOUNCEMENT, [])]
+            )
+            print()
+        else:
+            print("(no output conditions generated)")
         print()
         print("-------")
 
     created = set(spend_bundle.additions())
     spent = set(spend_bundle.removals())
 
     zero_coin_set = set(coin.name() for coin in created if coin.amount == 0)
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/json_clvm_utils.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/json_clvm_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/merkle_tree.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/merkle_tree.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/merkle_utils.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/merkle_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/new_peak_queue.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/new_peak_queue.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/peer_request_cache.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/peer_request_cache.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/puzzle_compression.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/puzzle_compression.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/wallet_sync_utils.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/wallet_sync_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     Tells full nodes that we are interested in puzzle hashes, and returns the response.
     """
     msg = wallet_protocol.RegisterForPhUpdates(puzzle_hashes, uint32(max(min_height, uint32(0))))
     all_coins_state: Optional[RespondToPhUpdates] = await peer.call_api(
         FullNodeAPI.register_interest_in_puzzle_hash, msg, timeout=300
     )
     if all_coins_state is None:
-        raise ValueError(f"None response from peer {peer.peer_host} for register_interest_in_puzzle_hash")
+        raise ValueError(f"None response from peer {peer.peer_info.host} for register_interest_in_puzzle_hash")
     return all_coins_state.coin_states
 
 
 async def subscribe_to_coin_updates(
     coin_names: List[bytes32],
     peer: WSChiaConnection,
     min_height: int,
@@ -89,15 +89,15 @@
     """
     msg = wallet_protocol.RegisterForCoinUpdates(coin_names, uint32(max(0, min_height)))
     all_coins_state: Optional[RespondToCoinUpdates] = await peer.call_api(
         FullNodeAPI.register_interest_in_coin, msg, timeout=300
     )
 
     if all_coins_state is None:
-        raise ValueError(f"None response from peer {peer.peer_host} for register_interest_in_coin")
+        raise ValueError(f"None response from peer {peer.peer_info.host} for register_interest_in_coin")
     return all_coins_state.coin_states
 
 
 def validate_additions(
     coins: List[Tuple[bytes32, List[Coin]]],
     proofs: Optional[List[Tuple[bytes32, bytes, Optional[bytes]]]],
     root: bytes32,
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/util/wallet_types.py` & `chia-blockchain-1.8.0b6/chia/wallet/util/wallet_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,19 @@
     DECENTRALIZED_ID = 8
     POOLING_WALLET = 9
     NFT = 10
     DATA_LAYER = 11
     DATA_LAYER_OFFER = 12
 
 
+class CoinType(IntEnum):
+    NORMAL = 0
+    CLAWBACK = 1
+
+
 class AmountWithPuzzlehash(TypedDict):
     amount: uint64
     puzzlehash: bytes32
     memos: List[bytes]
 
 
 @dataclass(frozen=True)
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet.py`

 * *Files 16% similar despite different names*

```diff
@@ -375,27 +375,16 @@
         assert len(coins) > 0
         self.log.info(f"coins is not None {coins}")
         spend_value = sum([coin.amount for coin in coins])
         self.log.info(f"spend_value is {spend_value} and total_amount is {total_amount}")
         change = spend_value - total_amount
         if negative_change_allowed:
             change = max(0, change)
-        # only kicks in if fee is missing
-        if change < 0 and fee + amount == total_amount:
-            fee_coins = await self.select_coins(
-                # change already includes fee amount
-                uint64(abs(change)),
-                excluded_coin_amounts=exclude_coin_amounts,
-                exclude=([] if exclude_coins is None else list(exclude_coins)) + list(coins or []),
-            )
-            coins = coins.union(fee_coins)
-            spend_value = sum([coin.amount for coin in coins])
-            self.log.info(f"Updated spend_value is {spend_value} and total_amount is {total_amount}")
-            change = spend_value - total_amount
-        assert change >= 0, f"change is negative: {change}"
+
+        assert change >= 0
 
         if coin_announcements_to_consume is not None:
             coin_announcements_bytes: Optional[Set[bytes32]] = {a.name() for a in coin_announcements_to_consume}
         else:
             coin_announcements_bytes = None
         if puzzle_announcements_to_consume is not None:
             puzzle_announcements_bytes: Optional[Set[bytes32]] = {a.name() for a in puzzle_announcements_to_consume}
@@ -580,59 +569,45 @@
             sent_to=[],
             trade_id=None,
             type=uint32(TransactionType.OUTGOING_TX.value),
             name=spend_bundle.name(),
             memos=list(compute_memos(spend_bundle).items()),
         )
 
+    async def create_tandem_xch_tx(
+        self,
+        fee: uint64,
+        announcement_to_assert: Optional[Announcement] = None,
+        reuse_puzhash: Optional[bool] = None,
+    ) -> TransactionRecord:
+        chia_coins = await self.select_coins(fee)
+        if reuse_puzhash is None:
+            reuse_puzhash_config = self.wallet_state_manager.config.get("reuse_public_key_for_change", None)
+            if reuse_puzhash_config is None:
+                reuse_puzhash = False
+            else:
+                reuse_puzhash = reuse_puzhash_config.get(
+                    str(self.wallet_state_manager.wallet_node.logged_in_fingerprint), False
+                )
+        chia_tx = await self.generate_signed_transaction(
+            uint64(0),
+            (await self.get_puzzle_hash(not reuse_puzhash)),
+            fee=fee,
+            coins=chia_coins,
+            coin_announcements_to_consume={announcement_to_assert} if announcement_to_assert is not None else None,
+            reuse_puzhash=reuse_puzhash,
+        )
+        assert chia_tx.spend_bundle is not None
+        return chia_tx
+
     async def push_transaction(self, tx: TransactionRecord) -> None:
         """Use this API to send transactions."""
         await self.wallet_state_manager.add_pending_transaction(tx)
         await self.wallet_state_manager.wallet_node.update_ui()
 
-    # This is to be aggregated together with a CAT offer to ensure that the trade happens
-    async def create_spend_bundle_relative_chia(self, chia_amount: int, exclude: List[Coin] = []) -> SpendBundle:
-        list_of_solutions = []
-        utxos = None
-
-        # If we're losing value then get coins with at least that much value
-        # If we're gaining value then our amount doesn't matter
-        if chia_amount < 0:
-            utxos = await self.select_coins(uint64(abs(chia_amount)), exclude)
-        else:
-            utxos = await self.select_coins(uint64(0), exclude)
-
-        assert len(utxos) > 0
-
-        # Calculate output amount given sum of utxos
-        spend_value = sum([coin.amount for coin in utxos])
-        chia_amount = spend_value + chia_amount
-
-        # Create coin solutions for each utxo
-        output_created = None
-        for coin in utxos:
-            puzzle = await self.puzzle_for_puzzle_hash(coin.puzzle_hash)
-            if output_created is None:
-                newpuzhash = await self.get_new_puzzlehash()
-                primaries: List[AmountWithPuzzlehash] = [
-                    {"puzzlehash": newpuzhash, "amount": uint64(chia_amount), "memos": []}
-                ]
-                solution = self.make_solution(primaries=primaries)
-                output_created = coin
-            list_of_solutions.append(CoinSpend(coin, puzzle, solution))
-
-        await self.hack_populate_secret_keys_for_coin_spends(list_of_solutions)
-        spend_bundle = await sign_coin_spends(
-            list_of_solutions,
-            self.secret_key_store.secret_key_for_public_key,
-            self.wallet_state_manager.constants.AGG_SIG_ME_ADDITIONAL_DATA,
-            self.wallet_state_manager.constants.MAX_BLOCK_COST_CLVM,
-        )
-        return spend_bundle
-
     async def get_coins_to_offer(
         self,
         asset_id: Optional[bytes32],
         amount: uint64,
         min_coin_amount: Optional[uint64] = None,
         max_coin_amount: Optional[uint64] = None,
     ) -> Set[Coin]:
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_action.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_action.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_blockchain.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_blockchain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_coin_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_coin_store.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import sqlite3
 from typing import Dict, List, Optional, Set
 
 from chia.types.blockchain_format.coin import Coin
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.util.db_wrapper import DBWrapper2, execute_fetchone
 from chia.util.ints import uint32, uint64
-from chia.wallet.util.wallet_types import WalletType
+from chia.util.misc import VersionedBlob
+from chia.wallet.util.wallet_types import CoinType, WalletType
 from chia.wallet.wallet_coin_record import WalletCoinRecord
 
 
 class WalletCoinStore:
     """
     This object handles CoinRecords in DB used by wallet.
     """
@@ -50,43 +51,53 @@
 
             await conn.execute("CREATE INDEX IF NOT EXISTS coin_record_wallet_type on coin_record(wallet_type)")
 
             await conn.execute("CREATE INDEX IF NOT EXISTS wallet_id on coin_record(wallet_id)")
 
             await conn.execute("CREATE INDEX IF NOT EXISTS coin_amount on coin_record(amount)")
 
+            try:
+                await conn.execute("ALTER TABLE coin_record ADD COLUMN coin_type int DEFAULT 0")
+                await conn.execute("ALTER TABLE coin_record ADD COLUMN metadata blob")
+                await conn.execute("CREATE INDEX IF NOT EXISTS coin_record_coin_type on coin_record(coin_type)")
+            except sqlite3.OperationalError:
+                pass
         return self
 
-    async def count_small_unspent(self, cutoff: int) -> int:
+    async def count_small_unspent(self, cutoff: int, coin_type: CoinType = CoinType.NORMAL) -> int:
         amount_bytes = bytes(uint64(cutoff))
         async with self.db_wrapper.reader_no_transaction() as conn:
             row = await execute_fetchone(
-                conn, "SELECT COUNT(*) FROM coin_record WHERE amount < ? AND spent=0", (amount_bytes,)
+                conn,
+                "SELECT COUNT(*) FROM coin_record WHERE coin_type=? AND amount < ? AND spent=0",
+                (coin_type, amount_bytes),
             )
             return int(0 if row is None else row[0])
 
     # Store CoinRecord in DB and ram cache
     async def add_coin_record(self, record: WalletCoinRecord, name: Optional[bytes32] = None) -> None:
         if name is None:
             name = record.name()
         assert record.spent == (record.spent_block_height != 0)
         async with self.db_wrapper.writer_maybe_transaction() as conn:
             await conn.execute_insert(
-                "INSERT OR REPLACE INTO coin_record VALUES(?, ?, ?, ?, ?, ?, ?, ?, ?, ?)",
+                "INSERT OR REPLACE INTO coin_record VALUES(?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)",
                 (
                     name.hex(),
                     record.confirmed_block_height,
                     record.spent_block_height,
                     int(record.spent),
                     int(record.coinbase),
                     str(record.coin.puzzle_hash.hex()),
                     str(record.coin.parent_coin_info.hex()),
                     bytes(uint64(record.coin.amount)),
                     record.wallet_type,
                     record.wallet_id,
+                    record.coin_type,
+                    None if record.metadata is None else bytes(record.metadata),
                 ),
             )
 
     # Sometimes we realize that a coin is actually not interesting to us so we need to delete it
     async def delete_coin_record(self, coin_name: bytes32) -> None:
         async with self.db_wrapper.writer_maybe_transaction() as conn:
             await (await conn.execute("DELETE FROM coin_record WHERE coin_name=?", (coin_name.hex(),))).close()
@@ -102,15 +113,23 @@
                     coin_name.hex(),
                 ),
             )
 
     def coin_record_from_row(self, row: sqlite3.Row) -> WalletCoinRecord:
         coin = Coin(bytes32.fromhex(row[6]), bytes32.fromhex(row[5]), uint64.from_bytes(row[7]))
         return WalletCoinRecord(
-            coin, uint32(row[1]), uint32(row[2]), bool(row[3]), bool(row[4]), WalletType(row[8]), row[9]
+            coin,
+            uint32(row[1]),
+            uint32(row[2]),
+            bool(row[3]),
+            bool(row[4]),
+            WalletType(row[8]),
+            row[9],
+            CoinType(row[10]),
+            None if row[11] is None else VersionedBlob.from_bytes(row[11]),
         )
 
     async def get_coin_record(self, coin_name: bytes32) -> Optional[WalletCoinRecord]:
         """Returns CoinRecord with specified coin id."""
         async with self.db_wrapper.reader_no_transaction() as conn:
             rows = list(await conn.execute_fetchall("SELECT * from coin_record WHERE coin_name=?", (coin_name.hex(),)))
 
@@ -140,36 +159,58 @@
         for row in rows:
             record = self.coin_record_from_row(row)
             coin_name = bytes32.fromhex(row[0])
             ret[coin_name] = record
 
         return ret
 
+    async def get_coin_records_between(
+        self, wallet_id: int, start: int, end: int, reverse: bool = False, coin_type: CoinType = CoinType.NORMAL
+    ) -> List[WalletCoinRecord]:
+        """Return a list of coins between start and end index. List is in reverse chronological order.
+        start = 0 is most recent transaction
+        """
+        limit = end - start
+        query_str = "ORDER BY confirmed_height " + ("DESC" if reverse else "ASC")
+
+        async with self.db_wrapper.reader_no_transaction() as conn:
+            rows = await conn.execute_fetchall(
+                f"SELECT * FROM coin_record WHERE coin_type=? AND"
+                f" wallet_id=? {query_str}, rowid LIMIT {start}, {limit}",
+                (coin_type, wallet_id),
+            )
+        return [self.coin_record_from_row(row) for row in rows]
+
     async def get_first_coin_height(self) -> Optional[uint32]:
         """Returns height of first confirmed coin"""
         async with self.db_wrapper.reader_no_transaction() as conn:
             rows = list(await conn.execute_fetchall("SELECT MIN(confirmed_height) FROM coin_record"))
 
         if len(rows) != 0 and rows[0][0] is not None:
             return uint32(rows[0][0])
 
         return None
 
-    async def get_unspent_coins_for_wallet(self, wallet_id: int) -> Set[WalletCoinRecord]:
+    async def get_unspent_coins_for_wallet(
+        self, wallet_id: int, coin_type: CoinType = CoinType.NORMAL
+    ) -> Set[WalletCoinRecord]:
         """Returns set of CoinRecords that have not been spent yet for a wallet."""
         async with self.db_wrapper.reader_no_transaction() as conn:
             rows = await conn.execute_fetchall(
-                "SELECT * FROM coin_record WHERE wallet_id=? AND spent_height=0", (wallet_id,)
+                "SELECT * FROM coin_record WHERE coin_type=? AND wallet_id=? AND spent_height=0",
+                (coin_type, wallet_id),
             )
         return set(self.coin_record_from_row(row) for row in rows)
 
-    async def get_all_unspent_coins(self) -> Set[WalletCoinRecord]:
+    async def get_all_unspent_coins(self, coin_type: CoinType = CoinType.NORMAL) -> Set[WalletCoinRecord]:
         """Returns set of CoinRecords that have not been spent yet for a wallet."""
         async with self.db_wrapper.reader_no_transaction() as conn:
-            rows = await conn.execute_fetchall("SELECT * FROM coin_record WHERE spent_height=0")
+            rows = await conn.execute_fetchall(
+                "SELECT * FROM coin_record WHERE coin_type=? AND spent_height=0", (coin_type,)
+            )
         return set(self.coin_record_from_row(row) for row in rows)
 
     # Checks DB and DiffStores for CoinRecords with puzzle_hash and returns them
     async def get_coin_records_by_puzzle_hash(self, puzzle_hash: bytes32) -> List[WalletCoinRecord]:
         """Returns a list of all coin records with the given puzzle hash"""
         async with self.db_wrapper.reader_no_transaction() as conn:
             rows = await conn.execute_fetchall("SELECT * from coin_record WHERE puzzle_hash=?", (puzzle_hash.hex(),))
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_info.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_info.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_interested_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_interested_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_nft_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_nft_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_node.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 import aiosqlite
 from blspy import AugSchemeMPL, G1Element, G2Element, PrivateKey
 from packaging.version import Version
 
-from chia.consensus.block_record import BlockRecord
 from chia.consensus.blockchain import AddBlockResult
 from chia.consensus.constants import ConsensusConstants
 from chia.daemon.keychain_proxy import KeychainProxy, connect_to_keychain_and_validate, wrap_local_keychain
 from chia.full_node.full_node_api import FullNodeAPI
 from chia.protocols import wallet_protocol
 from chia.protocols.full_node_protocol import RequestProofOfWeight, RespondProofOfWeight
 from chia.protocols.protocol_message_types import ProtocolMessageTypes
@@ -28,15 +27,14 @@
 from chia.server.node_discovery import WalletPeers
 from chia.server.outbound_message import Message, NodeType, make_msg
 from chia.server.peer_store_resolver import PeerStoreResolver
 from chia.server.server import ChiaServer
 from chia.server.ws_connection import WSChiaConnection
 from chia.types.blockchain_format.coin import Coin
 from chia.types.blockchain_format.sized_bytes import bytes32
-from chia.types.blockchain_format.sub_epoch_summary import SubEpochSummary
 from chia.types.coin_spend import CoinSpend
 from chia.types.header_block import HeaderBlock
 from chia.types.mempool_inclusion_status import MempoolInclusionStatus
 from chia.types.spend_bundle import SpendBundle
 from chia.types.weight_proof import WeightProof
 from chia.util.chunks import chunks
 from chia.util.config import (
@@ -728,15 +726,15 @@
             if cs.spent_height is not None and cs.spent_height >= fork_height:
                 return True
             if cs.created_height is not None and cs.created_height >= fork_height:
                 return True
             return False
 
         trusted: bool = self.is_trusted(full_node)
-        self.log.info(f"Starting sync trusted: {trusted} to peer {full_node.peer_host}")
+        self.log.info(f"Starting sync trusted: {trusted} to peer {full_node.peer_info.host}")
         start_time = time.time()
 
         if rollback:
             # we should clear all peers since this is a full rollback
             await self.perform_atomic_rollback(fork_height)
             await self.update_ui()
 
@@ -872,15 +870,15 @@
         chunk_size: int = 900 if trusted else 10
         for states in chunks(items, chunk_size):
             if self._server is None:
                 self.log.error("No server")
                 await asyncio.gather(*all_tasks)
                 return False
             if peer.peer_node_id not in self.server.all_connections:
-                self.log.error(f"Disconnected from peer {peer.peer_node_id} host {peer.peer_host}")
+                self.log.error(f"Disconnected from peer {peer.peer_node_id} host {peer.peer_info.host}")
                 await asyncio.gather(*all_tasks)
                 return False
             if trusted:
                 async with self.wallet_state_manager.db_wrapper.writer():
                     self.log.info(f"new coin state received ({idx}-{idx + len(states) - 1}/ {len(items)})")
                     if not await self.wallet_state_manager.add_coin_states(states, peer, fork_height):
                         return False
@@ -1106,40 +1104,33 @@
             self.log.exception(f"Error syncing to {peer.get_peer_info()}")
             await peer.close()
             return False
         return True
 
     async def long_sync_from_untrusted(self, syncing: bool, new_peak_hb: HeaderBlock, peer: WSChiaConnection) -> None:
         current_height: uint32 = await self.wallet_state_manager.blockchain.get_finished_sync_up_to()
-        weight_proof, summaries, block_records = await self.fetch_and_validate_the_weight_proof(peer, new_peak_hb)
-        old_proof = self.wallet_state_manager.blockchain.synced_weight_proof
-        # In this case we will not rollback so it's OK to check some older updates as well, to ensure
-        # that no recent transactions are being hidden.
-        fork_point: int = 0
-        if syncing:
-            # This usually happens the first time we start up the wallet. We roll back slightly to be
-            # safe, but we don't want to rollback too much (hence 16)
-            fork_point = max(0, current_height - 16)
-        if old_proof is not None:
-            # If the weight proof fork point is in the past, rollback more to ensure we don't have duplicate
-            # state.
-            fork_point = min(fork_point, get_wp_fork_point(self.constants, old_proof, weight_proof))
-
-        await self.wallet_state_manager.blockchain.new_valid_weight_proof(weight_proof, block_records)
+        fork_point_weight_proof = await self.fetch_and_update_weight_proof(peer, new_peak_hb)
+        # This usually happens the first time we start up the wallet. We roll back slightly to be
+        # safe, but we don't want to rollback too much (hence 16)
+        fork_point_rollback: int = max(0, current_height - 16)
+        # If the weight proof fork point is in the past, rollback more to ensure we don't have duplicate
+        fork_point_syncing = min(fork_point_rollback, fork_point_weight_proof)
 
         if syncing:
             async with self.wallet_state_manager.set_sync_mode(new_peak_hb.height):
-                await self.long_sync(new_peak_hb.height, peer, fork_point, rollback=True)
+                await self.long_sync(new_peak_hb.height, peer, fork_point_syncing, rollback=True)
             return
 
         # we exit earlier in the case where syncing is False and a Secondary sync is running
         assert self._secondary_peer_sync_task is None or self._secondary_peer_sync_task.done()
         self.log.info("Secondary peer syncing")
+        # In this case we will not rollback so it's OK to check some older updates as well, to ensure
+        # that no recent transactions are being hidden.
         self._secondary_peer_sync_task = asyncio.create_task(
-            self.long_sync(new_peak_hb.height, peer, fork_point, rollback=False)
+            self.long_sync(new_peak_hb.height, peer, 0, rollback=False)
         )
 
     async def sync_from_untrusted_close_to_peak(self, new_peak_hb: HeaderBlock, peer: WSChiaConnection) -> bool:
         async with self.wallet_state_manager.lock:
             peak_hb = await self.wallet_state_manager.blockchain.get_peak_block()
             if peak_hb is None or new_peak_hb.weight > peak_hb.weight:
                 backtrack_fork_height: int = await self.wallet_short_sync_backtrack(new_peak_hb, peer)
@@ -1222,17 +1213,15 @@
         return fork_height
 
     async def update_ui(self) -> None:
         for wallet_id, wallet in self.wallet_state_manager.wallets.items():
             self.wallet_state_manager.state_changed("coin_removed", wallet_id)
             self.wallet_state_manager.state_changed("coin_added", wallet_id)
 
-    async def fetch_and_validate_the_weight_proof(
-        self, peer: WSChiaConnection, peak: HeaderBlock
-    ) -> Tuple[WeightProof, List[SubEpochSummary], List[BlockRecord]]:
+    async def fetch_and_update_weight_proof(self, peer: WSChiaConnection, peak: HeaderBlock) -> int:
         assert self._weight_proof_handler is not None
         weight_request = RequestProofOfWeight(peak.height, peak.header_hash)
         wp_timeout = self.config.get("weight_proof_timeout", 360)
         self.log.debug(f"weight proof timeout is {wp_timeout} sec")
         weight_proof_response: RespondProofOfWeight = await peer.call_api(
             FullNodeAPI.request_proof_of_weight, weight_request, timeout=wp_timeout
         )
@@ -1246,26 +1235,19 @@
             raise Exception("weight proof height does not match peak")
         if weight_proof.recent_chain_data[-1].weight != peak.weight:
             raise Exception("weight proof weight does not match peak")
         if weight_proof.recent_chain_data[-1].header_hash != peak.header_hash:
             raise Exception("weight proof peak hash does not match peak")
 
         old_proof = self.wallet_state_manager.blockchain.synced_weight_proof
-        start_validation = time.time()
-        (
-            valid,
-            summaries,
-            block_records,
-        ) = await self._weight_proof_handler.validate_weight_proof(weight_proof, False, old_proof)
-        if not valid:
-            raise Exception("weight proof failed validation")
-
-        end_validation = time.time()
-        self.log.info(f"It took {end_validation - start_validation} time to validate the weight proof")
-        return weight_proof, summaries, block_records
+        block_records = await self._weight_proof_handler.validate_weight_proof(weight_proof, False, old_proof)
+
+        await self.wallet_state_manager.blockchain.new_valid_weight_proof(weight_proof, block_records)
+
+        return get_wp_fork_point(self.constants, old_proof, weight_proof)
 
     async def get_puzzle_hashes_to_subscribe(self) -> List[bytes32]:
         all_puzzle_hashes = await self.wallet_state_manager.puzzle_store.get_all_puzzle_hashes()
         # Get all phs from interested store
         interested_puzzle_hashes = [
             t[0] for t in await self.wallet_state_manager.interested_store.get_interested_puzzle_hashes()
         ]
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_node_api.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_node_api.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_pool_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_pool_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_protocol.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_puzzle_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_puzzle_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_retry_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_retry_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_state_manager.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_state_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import asyncio
-import json
 import logging
 import multiprocessing.context
 import time
 import traceback
 from contextlib import asynccontextmanager
 from pathlib import Path
 from secrets import token_bytes
@@ -49,27 +48,25 @@
     _derive_path,
     _derive_path_unhardened,
     master_sk_to_wallet_sk,
     master_sk_to_wallet_sk_intermediate,
     master_sk_to_wallet_sk_unhardened,
     master_sk_to_wallet_sk_unhardened_intermediate,
 )
-from chia.wallet.did_wallet.did_info import DIDInfo
 from chia.wallet.did_wallet.did_wallet import DIDWallet
 from chia.wallet.did_wallet.did_wallet_puzzles import DID_INNERPUZ_MOD, match_did_puzzle
 from chia.wallet.key_val_store import KeyValStore
-from chia.wallet.nft_wallet.nft_info import NFTWalletInfo
 from chia.wallet.nft_wallet.nft_puzzles import get_metadata_and_phs, get_new_owner_did
 from chia.wallet.nft_wallet.nft_wallet import NFTWallet
 from chia.wallet.nft_wallet.uncurry_nft import UncurriedNFT
 from chia.wallet.notification_manager import NotificationManager
 from chia.wallet.outer_puzzles import AssetType
 from chia.wallet.puzzle_drivers import PuzzleInfo
 from chia.wallet.puzzles.cat_loader import CAT_MOD, CAT_MOD_HASH
-from chia.wallet.singleton import create_fullpuz
+from chia.wallet.singleton import create_singleton_puzzle
 from chia.wallet.trade_manager import TradeManager
 from chia.wallet.trading.trade_status import TradeStatus
 from chia.wallet.transaction_record import TransactionRecord
 from chia.wallet.uncurried_puzzle import uncurry_puzzle
 from chia.wallet.util.address_type import AddressType
 from chia.wallet.util.compute_hints import compute_coin_hints
 from chia.wallet.util.transaction_type import TransactionType
@@ -769,40 +766,41 @@
                 break
 
         launch_id: bytes32 = bytes32(bytes(singleton_struct.rest().first())[1:])
         if derivation_record is None:
             self.log.info(f"Received state for the coin that doesn't belong to us {coin_state}")
             # Check if it was owned by us
             removed_wallet_ids = []
-            for wallet_info in await self.get_all_wallet_info_entries(wallet_type=WalletType.DECENTRALIZED_ID):
-                did_info: DIDInfo = DIDInfo.from_json_dict(json.loads(wallet_info.data))
+            for wallet in self.wallets.values():
+                if not isinstance(wallet, DIDWallet):
+                    continue
                 if (
-                    did_info.origin_coin is not None
-                    and launch_id == did_info.origin_coin.name()
-                    and not did_info.sent_recovery_transaction
+                    wallet.did_info.origin_coin is not None
+                    and launch_id == wallet.did_info.origin_coin.name()
+                    and not wallet.did_info.sent_recovery_transaction
                 ):
-                    await self.user_store.delete_wallet(wallet_info.id)
-                    removed_wallet_ids.append(wallet_info.id)
+                    await self.user_store.delete_wallet(wallet.id())
+                    removed_wallet_ids.append(wallet.id())
             for remove_id in removed_wallet_ids:
                 self.wallets.pop(remove_id)
                 self.log.info(f"Removed DID wallet {remove_id}, Launch_ID: {launch_id.hex()}")
                 self.state_changed("wallet_removed", remove_id)
             return None
         else:
             our_inner_puzzle: Program = self.main_wallet.puzzle_for_pk(derivation_record.pubkey)
 
             self.log.info(f"Found DID, launch_id {launch_id}.")
             did_puzzle = DID_INNERPUZ_MOD.curry(
                 our_inner_puzzle, recovery_list_hash, num_verification, singleton_struct, metadata
             )
-            full_puzzle = create_fullpuz(did_puzzle, launch_id)
+            full_puzzle = create_singleton_puzzle(did_puzzle, launch_id)
             did_puzzle_empty_recovery = DID_INNERPUZ_MOD.curry(
                 our_inner_puzzle, Program.to([]).get_tree_hash(), uint64(0), singleton_struct, metadata
             )
-            full_puzzle_empty_recovery = create_fullpuz(did_puzzle_empty_recovery, launch_id)
+            full_puzzle_empty_recovery = create_singleton_puzzle(did_puzzle_empty_recovery, launch_id)
             if full_puzzle.get_tree_hash() != coin_state.coin.puzzle_hash:
                 if full_puzzle_empty_recovery.get_tree_hash() == coin_state.coin.puzzle_hash:
                     did_puzzle = did_puzzle_empty_recovery
                     self.log.info("DID recovery list was reset by the previous owner.")
                 else:
                     self.log.error("DID puzzle hash doesn't match, please check curried parameters.")
                     return None
@@ -916,46 +914,45 @@
         ] = await self.puzzle_store.get_derivation_record_for_puzzle_hash(old_p2_puzhash)
         if new_derivation_record is None and old_derivation_record is None:
             self.log.debug(
                 "Cannot find a P2 puzzle hash for NFT:%s, this NFT belongs to others.",
                 uncurried_nft.singleton_launcher_id.hex(),
             )
             return wallet_identifier
-        for wallet_info in await self.get_all_wallet_info_entries(wallet_type=WalletType.NFT):
-            nft_wallet_info: NFTWalletInfo = NFTWalletInfo.from_json_dict(json.loads(wallet_info.data))
-            if nft_wallet_info.did_id == old_did_id and old_derivation_record is not None:
+        for nft_wallet in self.wallets.values():
+            if not isinstance(nft_wallet, NFTWallet):
+                continue
+            if nft_wallet.nft_wallet_info.did_id == old_did_id and old_derivation_record is not None:
                 self.log.info(
                     "Removing old NFT, NFT_ID:%s, DID_ID:%s",
                     uncurried_nft.singleton_launcher_id.hex(),
                     old_did_id,
                 )
-                nft_wallet = self.get_wallet(id=wallet_info.id, required_type=NFTWallet)
                 if parent_coin_state.spent_height is not None:
                     await nft_wallet.remove_coin(coin_spend.coin, uint32(parent_coin_state.spent_height))
                     is_empty = await nft_wallet.is_empty()
                     has_did = False
-                    for did_wallet_info in await self.get_all_wallet_info_entries(
-                        wallet_type=WalletType.DECENTRALIZED_ID
-                    ):
-                        did_wallet: DIDInfo = DIDInfo.from_json_dict(json.loads(did_wallet_info.data))
-                        assert did_wallet.origin_coin is not None
-                        if did_wallet.origin_coin.name() == old_did_id:
+                    for did_wallet in self.wallets.values():
+                        if not isinstance(did_wallet, DIDWallet):
+                            continue
+                        assert did_wallet.did_info.origin_coin is not None
+                        if did_wallet.did_info.origin_coin.name() == old_did_id:
                             has_did = True
                             break
                     if is_empty and nft_wallet.did_id is not None and not has_did:
                         self.log.info(f"No NFT, deleting wallet {nft_wallet.did_id.hex()} ...")
                         await self.user_store.delete_wallet(nft_wallet.wallet_info.id)
                         self.wallets.pop(nft_wallet.wallet_info.id)
-            if nft_wallet_info.did_id == new_did_id and new_derivation_record is not None:
+            if nft_wallet.nft_wallet_info.did_id == new_did_id and new_derivation_record is not None:
                 self.log.info(
                     "Adding new NFT, NFT_ID:%s, DID_ID:%s",
                     uncurried_nft.singleton_launcher_id.hex(),
                     new_did_id,
                 )
-                wallet_identifier = WalletIdentifier(wallet_info.id, WalletType.NFT)
+                wallet_identifier = WalletIdentifier.create(nft_wallet)
 
         if wallet_identifier is None and new_derivation_record is not None:
             # Cannot find an existed NFT wallet for the new NFT
             self.log.info(
                 "Cannot find a NFT wallet for NFT_ID: %s DID_ID: %s, creating a new one.",
                 uncurried_nft.singleton_launcher_id,
                 new_did_id,
@@ -1470,14 +1467,15 @@
                 type=uint32(tx_type),
                 name=coin_name,
                 memos=[],
             )
             if tx_record.amount > 0:
                 await self.tx_store.add_transaction_record(tx_record)
 
+        # We only add normal coins here
         coin_record: WalletCoinRecord = WalletCoinRecord(
             coin, height, uint32(0), False, coinbase, wallet_type, wallet_id
         )
         await self.coin_store.add_coin_record(coin_record, coin_name)
 
         await self.wallets[wallet_id].coin_added(coin, height, peer)
```

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_transaction_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_transaction_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_user_store.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_user_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/chia/wallet/wallet_weight_proof_handler.py` & `chia-blockchain-1.8.0b6/chia/wallet/wallet_weight_proof_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import tempfile
+import time
 from concurrent.futures.process import ProcessPoolExecutor
 from multiprocessing.context import BaseContext
-from typing import IO, List, Optional, Tuple
+from typing import IO, List, Optional
 
 from chia.consensus.block_record import BlockRecord
 from chia.consensus.constants import ConsensusConstants
 from chia.full_node.weight_proof import _validate_sub_epoch_summaries, validate_weight_proof_inner
-from chia.types.blockchain_format.sub_epoch_summary import SubEpochSummary
 from chia.types.weight_proof import WeightProof
 from chia.util.ints import uint32
 from chia.util.setproctitle import getproctitle, setproctitle
 
 log = logging.getLogger(__name__)
 
 
@@ -33,50 +33,43 @@
         self._executor_shutdown_tempfile: IO[bytes] = _create_shutdown_file()
         self._executor: ProcessPoolExecutor = ProcessPoolExecutor(
             self._num_processes,
             mp_context=multiprocessing_context,
             initializer=setproctitle,
             initargs=(f"{getproctitle()}_worker",),
         )
-        self._weight_proof_tasks: List[asyncio.Task[Tuple[bool, List[BlockRecord]]]] = []
 
     def cancel_weight_proof_tasks(self) -> None:
-        for task in self._weight_proof_tasks:
-            if not task.done():
-                task.cancel()
-        self._weight_proof_tasks = []
         self._executor_shutdown_tempfile.close()
         self._executor.shutdown(wait=True)
 
     async def validate_weight_proof(
         self, weight_proof: WeightProof, skip_segment_validation: bool = False, old_proof: Optional[WeightProof] = None
-    ) -> Tuple[bool, List[SubEpochSummary], List[BlockRecord]]:
+    ) -> List[BlockRecord]:
+        start_time = time.time()
         summaries, sub_epoch_weight_list = _validate_sub_epoch_summaries(self._constants, weight_proof)
         await asyncio.sleep(0)  # break up otherwise multi-second sync code
         if summaries is None or sub_epoch_weight_list is None:
-            log.error("weight proof failed sub epoch data validation")
-            return False, [], []
+            raise ValueError("weight proof failed sub epoch data validation")
         validate_from = get_fork_ses_idx(old_proof, weight_proof)
-        task = asyncio.create_task(
-            validate_weight_proof_inner(
-                self._constants,
-                self._executor,
-                self._executor_shutdown_tempfile.name,
-                self._num_processes,
-                weight_proof,
-                summaries,
-                sub_epoch_weight_list,
-                skip_segment_validation,
-                validate_from,
-            )
+        valid, block_records = await validate_weight_proof_inner(
+            self._constants,
+            self._executor,
+            self._executor_shutdown_tempfile.name,
+            self._num_processes,
+            weight_proof,
+            summaries,
+            sub_epoch_weight_list,
+            skip_segment_validation,
+            validate_from,
         )
-        self._weight_proof_tasks.append(task)
-        valid, block_records = await task
-        self._weight_proof_tasks.remove(task)
-        return valid, summaries, block_records
+        if not valid:
+            raise ValueError("weight proof validation failed")
+        log.info(f"It took {time.time() - start_time} time to validate the weight proof {weight_proof.get_hash()}")
+        return block_records
 
 
 def get_wp_fork_point(constants: ConsensusConstants, old_wp: Optional[WeightProof], new_wp: WeightProof) -> uint32:
     """
     iterate through sub epoch summaries to find fork point. This method is conservative, it does not return the
     actual fork point, it can return a height that is before the actual fork point.
     """
```

### Comparing `chia-blockchain-1.8.0b5/chia_blockchain.egg-info/PKG-INFO` & `chia-blockchain-1.8.0b6/chia_blockchain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chia-blockchain
-Version: 1.8.0b5
+Version: 1.8.0b6
 Summary: Chia blockchain full node, farmer, timelord, and wallet.
 Home-page: https://chia.net/
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
 Project-URL: Source, https://github.com/Chia-Network/chia-blockchain/
 Project-URL: Changelog, https://github.com/Chia-Network/chia-blockchain/blob/main/CHANGELOG.md
```

### Comparing `chia-blockchain-1.8.0b5/chia_blockchain.egg-info/SOURCES.txt` & `chia-blockchain-1.8.0b6/chia_blockchain.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 build_scripts/npm_macos/__init__.py
 build_scripts/npm_macos/package-lock.json
 build_scripts/npm_macos/package.json
 build_scripts/npm_windows/__init__.py
 build_scripts/npm_windows/package-lock.json
 build_scripts/npm_windows/package.json
 chia/__init__.py
+chia/__main__.py
 chia/py.typed
 chia/pyinstaller.spec
 chia/clvm/__init__.py
 chia/clvm/singleton.py
 chia/clvm/spend_sim.py
 chia/cmds/__init__.py
 chia/cmds/beta.py
@@ -193,14 +194,16 @@
 chia/data_layer/data_layer_errors.py
 chia/data_layer/data_layer_server.py
 chia/data_layer/data_layer_util.py
 chia/data_layer/data_layer_wallet.py
 chia/data_layer/data_store.py
 chia/data_layer/dl_wallet_store.py
 chia/data_layer/download_data.py
+chia/data_layer/s3_plugin_config.yml
+chia/data_layer/s3_plugin_service.py
 chia/data_layer/util/__init__.py
 chia/data_layer/util/benchmark.py
 chia/farmer/__init__.py
 chia/farmer/farmer.py
 chia/farmer/farmer_api.py
 chia/full_node/__init__.py
 chia/full_node/bitcoin_fee_estimator.py
@@ -306,15 +309,14 @@
 chia/server/chia_policy.py
 chia/server/introducer_peers.py
 chia/server/node_discovery.py
 chia/server/outbound_message.py
 chia/server/peer_store_resolver.py
 chia/server/rate_limit_numbers.py
 chia/server/rate_limits.py
-chia/server/reconnect_task.py
 chia/server/server.py
 chia/server/ssl_context.py
 chia/server/start_data_layer.py
 chia/server/start_farmer.py
 chia/server/start_full_node.py
 chia/server/start_harvester.py
 chia/server/start_introducer.py
@@ -927,14 +929,15 @@
 tests/util/test_network.py
 tests/util/test_network_protocol_files.py
 tests/util/test_network_protocol_json.py
 tests/util/test_network_protocol_test.py
 tests/util/test_paginator.py
 tests/util/test_pprint.py
 tests/util/test_struct_stream.py
+tests/util/test_trusted_peer.py
 tests/wallet/__init__.py
 tests/wallet/config.py
 tests/wallet/test_address_type.py
 tests/wallet/test_bech32m.py
 tests/wallet/test_chialisp.py
 tests/wallet/test_coin_selection.py
 tests/wallet/test_nft_store.py
```

### Comparing `chia-blockchain-1.8.0b5/chia_blockchain.egg-info/entry_points.txt` & `chia-blockchain-1.8.0b6/chia_blockchain.egg-info/entry_points.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [console_scripts]
 chia = chia.cmds.chia:main
 chia_crawler = chia.seeder.start_crawler:main
 chia_daemon = chia.daemon.server:main
 chia_data_layer = chia.server.start_data_layer:main
 chia_data_layer_http = chia.data_layer.data_layer_server:main
+chia_data_layer_s3_plugin = chia.data_layer.s3_plugin_service:run_server
 chia_farmer = chia.server.start_farmer:main
 chia_full_node = chia.server.start_full_node:main
 chia_full_node_simulator = chia.simulator.start_simulator:main
 chia_harvester = chia.server.start_harvester:main
 chia_introducer = chia.server.start_introducer:main
 chia_seeder = chia.seeder.dns_server:main
 chia_timelord = chia.server.start_timelord:main
```

### Comparing `chia-blockchain-1.8.0b5/chia_blockchain.egg-info/requires.txt` & `chia-blockchain-1.8.0b6/chia_blockchain.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 aiofiles==23.1.0
 anyio==3.6.2
+boto3==1.26.111
 blspy==1.0.16
 chiavdf==1.0.8
 chiabip158==1.2
 chiapos==1.0.11
 clvm==0.9.7
 clvm_tools==0.4.6
 chia_rs==0.2.5
```

### Comparing `chia-blockchain-1.8.0b5/install-gui.sh` & `chia-blockchain-1.8.0b6/install-gui.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/install-plotter.sh` & `chia-blockchain-1.8.0b6/install-plotter.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/install-timelord.sh` & `chia-blockchain-1.8.0b6/install-timelord.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/install.sh` & `chia-blockchain-1.8.0b6/install.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/installhelper.py` & `chia-blockchain-1.8.0b6/installhelper.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/mozilla-ca/cacert.pem` & `chia-blockchain-1.8.0b6/mozilla-ca/cacert.pem`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/mypy.ini` & `chia-blockchain-1.8.0b6/mypy.ini`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 no_implicit_optional = True
 warn_return_any = True
 no_implicit_reexport = True
 strict_equality = True
 warn_redundant_casts = True
 
 # list created by: venv/bin/mypy | sed -n 's/.py:.*//p' | sort | uniq | tr '/' '.' | tr '\n' ','
-[mypy-chia.cmds.passphrase,chia.cmds.passphrase_funcs,chia.cmds.plots,chia.cmds.plotters,chia.cmds.show,chia.cmds.start_funcs,chia.cmds.wallet,chia.cmds.wallet_funcs,chia.daemon.server,chia.farmer.farmer_api,chia.full_node.weight_proof,chia.introducer.introducer,chia.introducer.introducer_api,chia.plotters.bladebit,chia.plotters.chiapos,chia.plotters.madmax,chia.plotters.plotters,chia.plotters.plotters_util,chia.plotting.create_plots,chia.plotting.manager,chia.plotting.util,chia.pools.pool_puzzles,chia.pools.pool_wallet,chia.pools.pool_wallet_info,chia.rpc.full_node_rpc_client,chia.rpc.harvester_rpc_api,chia.rpc.harvester_rpc_client,chia.rpc.rpc_client,chia.rpc.timelord_rpc_api,chia.rpc.util,chia.rpc.wallet_rpc_api,chia.rpc.wallet_rpc_client,chia.seeder.crawler,chia.seeder.crawler_api,chia.seeder.crawl_store,chia.seeder.dns_server,chia.seeder.peer_record,chia.seeder.start_crawler,chia.simulator.full_node_simulator,chia.simulator.start_simulator,chia.ssl.create_ssl,chia.timelord.iters_from_block,chia.timelord.timelord,chia.timelord.timelord_api,chia.timelord.timelord_launcher,chia.timelord.timelord_state,chia.types.blockchain_format.program,chia.util.block_cache,chia.util.check_fork_next_block,chia.util.chia_logging,chia.util.config,chia.util.db_wrapper,chia.util.dump_keyring,chia.util.files,chia.util.hash,chia.util.json_util,chia.util.keychain,chia.util.keyring_wrapper,chia.util.log_exceptions,chia.util.make_test_constants,chia.util.merkle_set,chia.util.network,chia.util.partial_func,chia.util.profiler,chia.util.safe_cancel_task,chia.util.service_groups,chia.util.ssl_check,chia.util.validate_alert,chia.wallet.block_record,chia.wallet.chialisp,chia.wallet.did_wallet.did_wallet,chia.wallet.did_wallet.did_wallet_puzzles,chia.wallet.key_val_store,chia.wallet.lineage_proof,chia.wallet.payment,chia.wallet.puzzles.load_clvm,chia.wallet.puzzles.p2_conditions,chia.wallet.puzzles.p2_delegated_conditions,chia.wallet.puzzles.p2_delegated_puzzle,chia.wallet.puzzles.p2_delegated_puzzle_or_hidden_puzzle,chia.wallet.puzzles.p2_m_of_n_delegate_direct,chia.wallet.puzzles.p2_puzzle_hash,chia.wallet.puzzles.prefarm.spend_prefarm,chia.wallet.puzzles.puzzle_utils,chia.wallet.puzzles.singleton_top_layer,chia.wallet.puzzles.tails,chia.wallet.secret_key_store,chia.wallet.trade_record,chia.wallet.trading.trade_store,chia.wallet.transaction_record,chia.wallet.util.debug_spend_bundle,chia.wallet.util.new_peak_queue,chia.wallet.wallet,chia.wallet.wallet_coin_store,chia.wallet.wallet_interested_store,chia.wallet.wallet_node_api,chia.wallet.wallet_pool_store,chia.wallet.wallet_puzzle_store,chia.wallet.wallet_state_manager,chia.wallet.wallet_sync_store,chia.wallet.wallet_transaction_store,chia.wallet.wallet_user_store,installhelper,tests.blockchain.blockchain_test_utils,tests.blockchain.test_blockchain,tests.blockchain.test_blockchain_transactions,chia.simulator.block_tools,tests.build-init-files,tests.build-workflows,tests.clvm.coin_store,tests.clvm.test_chialisp_deserialization,tests.clvm.test_clvm_compilation,tests.clvm.test_program,tests.clvm.test_puzzle_compression,tests.clvm.test_puzzles,tests.clvm.test_serialized_program,tests.clvm.test_singletons,tests.clvm.test_spend_sim,tests.conftest,tests.connection_utils,tests.core.cmds.test_keys,tests.core.consensus.test_pot_iterations,tests.core.custom_types.test_coin,tests.core.custom_types.test_proof_of_space,tests.core.custom_types.test_spend_bundle,tests.core.daemon.test_daemon,tests.core.full_node.full_sync.test_full_sync,tests.core.full_node.stores.test_block_store,tests.core.full_node.stores.test_coin_store,tests.core.full_node.stores.test_full_node_store,tests.core.full_node.stores.test_hint_store,tests.core.full_node.stores.test_sync_store,tests.core.full_node.test_address_manager,tests.core.full_node.test_block_height_map,tests.core.full_node.test_conditions,tests.core.full_node.test_full_node,tests.core.mempool.test_mempool,tests.core.mempool.test_mempool_performance,tests.core.full_node.test_node_load,tests.core.full_node.test_peer_store_resolver,tests.core.full_node.test_performance,tests.core.full_node.test_transactions,tests.core.make_block_generator,tests.core.node_height,tests.core.server.test_dos,tests.core.server.test_rate_limits,tests.core.ssl.test_ssl,tests.core.test_cost_calculation,tests.core.test_crawler_rpc,tests.core.test_daemon_rpc,tests.core.test_db_conversion,tests.core.test_db_validation,tests.core.test_farmer_harvester_rpc,tests.core.test_filter,tests.core.test_full_node_rpc,tests.core.test_merkle_set,tests.core.test_setproctitle,tests.core.util.test_cached_bls,tests.core.util.test_config,tests.core.util.test_file_keyring_synchronization,tests.core.util.test_files,tests.core.util.test_keychain,tests.core.util.test_keyring_wrapper,tests.core.util.test_lru_cache,tests.core.util.test_significant_bits,tests.farmer_harvester.test_farmer_harvester,tests.generator.test_compression,tests.generator.test_generator_types,tests.generator.test_list_to_batches,tests.generator.test_rom,tests.generator.test_scan,tests.plotting.test_plot_manager,tests.pools.test_pool_cmdline,tests.pools.test_pool_config,tests.pools.test_pool_puzzles_lifecycle,tests.pools.test_wallet_pool_store,tests.simulation.test_simulation,chia.simulator.time_out_assert,tests.tools.test_full_sync,tests.tools.test_run_block,tests.util.alert_server,tests.util.benchmark_cost,tests.util.blockchain,tests.util.build_network_protocol_files,tests.util.db_connection,tests.util.generator_tools_testing,chia.simulator.keyring,tests.util.key_tool,tests.util.test_full_block_utils,tests.util.test_lock_queue,tests.util.test_misc,tests.util.test_network,tests.util.test_network_protocol_files,tests.wallet.cat_wallet.test_cat_lifecycle,tests.wallet.cat_wallet.test_cat_wallet,tests.wallet.cat_wallet.test_offer_lifecycle,tests.wallet.cat_wallet.test_trades,tests.wallet.did_wallet.test_did,tests.wallet.did_wallet.test_did_rpc,tests.wallet.did_wallet.test_nft_rpc,tests.wallet.did_wallet.test_nft_wallet,tests.wallet.rpc.test_wallet_rpc,tests.wallet.simple_sync.test_simple_sync_protocol,tests.wallet.sync.test_wallet_sync,tests.wallet.test_bech32m,tests.wallet.test_chialisp,tests.wallet.test_puzzle_store,tests.wallet.test_singleton,tests.wallet.test_singleton_lifecycle,tests.wallet.test_singleton_lifecycle_fast,tests.wallet.test_taproot,tests.wallet.test_wallet_blockchain,tests.wallet.test_wallet_interested_store,tests.wallet.test_wallet_key_val_store,tests.wallet.test_wallet_user_store,chia.simulator.wallet_tools,tests.weight_proof.test_weight_proof,tools.analyze-chain,tools.run_block,tools.test_full_sync,tests.wallet.nft_wallet.test_nft_wallet,chia.wallet.nft_wallet.nft_puzzles,tests.wallet.nft_wallet.test_nft_puzzles]
+[mypy-chia.cmds.passphrase,chia.cmds.passphrase_funcs,chia.cmds.plots,chia.cmds.plotters,chia.cmds.show,chia.cmds.start_funcs,chia.cmds.wallet,chia.cmds.wallet_funcs,chia.daemon.server,chia.farmer.farmer_api,chia.full_node.weight_proof,chia.introducer.introducer,chia.introducer.introducer_api,chia.plotters.bladebit,chia.plotters.chiapos,chia.plotters.madmax,chia.plotters.plotters,chia.plotters.plotters_util,chia.plotting.create_plots,chia.plotting.manager,chia.plotting.util,chia.pools.pool_puzzles,chia.pools.pool_wallet,chia.pools.pool_wallet_info,chia.rpc.full_node_rpc_client,chia.rpc.harvester_rpc_api,chia.rpc.harvester_rpc_client,chia.rpc.rpc_client,chia.rpc.timelord_rpc_api,chia.rpc.util,chia.rpc.wallet_rpc_api,chia.rpc.wallet_rpc_client,chia.seeder.crawler,chia.seeder.crawler_api,chia.seeder.crawl_store,chia.seeder.dns_server,chia.seeder.peer_record,chia.seeder.start_crawler,chia.simulator.full_node_simulator,chia.simulator.start_simulator,chia.ssl.create_ssl,chia.timelord.iters_from_block,chia.timelord.timelord,chia.timelord.timelord_api,chia.timelord.timelord_launcher,chia.timelord.timelord_state,chia.types.blockchain_format.program,chia.util.block_cache,chia.util.check_fork_next_block,chia.util.chia_logging,chia.util.config,chia.util.db_wrapper,chia.util.dump_keyring,chia.util.hash,chia.util.json_util,chia.util.keychain,chia.util.keyring_wrapper,chia.util.log_exceptions,chia.util.make_test_constants,chia.util.merkle_set,chia.util.network,chia.util.partial_func,chia.util.profiler,chia.util.safe_cancel_task,chia.util.service_groups,chia.util.ssl_check,chia.util.validate_alert,chia.wallet.block_record,chia.wallet.chialisp,chia.wallet.did_wallet.did_wallet,chia.wallet.did_wallet.did_wallet_puzzles,chia.wallet.key_val_store,chia.wallet.lineage_proof,chia.wallet.payment,chia.wallet.puzzles.load_clvm,chia.wallet.puzzles.p2_conditions,chia.wallet.puzzles.p2_delegated_conditions,chia.wallet.puzzles.p2_delegated_puzzle,chia.wallet.puzzles.p2_delegated_puzzle_or_hidden_puzzle,chia.wallet.puzzles.p2_m_of_n_delegate_direct,chia.wallet.puzzles.p2_puzzle_hash,chia.wallet.puzzles.prefarm.spend_prefarm,chia.wallet.puzzles.puzzle_utils,chia.wallet.puzzles.singleton_top_layer,chia.wallet.puzzles.tails,chia.wallet.secret_key_store,chia.wallet.trade_record,chia.wallet.trading.trade_store,chia.wallet.transaction_record,chia.wallet.util.debug_spend_bundle,chia.wallet.util.new_peak_queue,chia.wallet.wallet,chia.wallet.wallet_coin_store,chia.wallet.wallet_interested_store,chia.wallet.wallet_node_api,chia.wallet.wallet_pool_store,chia.wallet.wallet_puzzle_store,chia.wallet.wallet_state_manager,chia.wallet.wallet_sync_store,chia.wallet.wallet_transaction_store,chia.wallet.wallet_user_store,installhelper,tests.blockchain.blockchain_test_utils,tests.blockchain.test_blockchain,tests.blockchain.test_blockchain_transactions,chia.simulator.block_tools,tests.build-init-files,tests.build-workflows,tests.clvm.coin_store,tests.clvm.test_chialisp_deserialization,tests.clvm.test_clvm_compilation,tests.clvm.test_program,tests.clvm.test_puzzle_compression,tests.clvm.test_puzzles,tests.clvm.test_serialized_program,tests.clvm.test_singletons,tests.clvm.test_spend_sim,tests.conftest,tests.connection_utils,tests.core.cmds.test_keys,tests.core.consensus.test_pot_iterations,tests.core.custom_types.test_coin,tests.core.custom_types.test_proof_of_space,tests.core.custom_types.test_spend_bundle,tests.core.daemon.test_daemon,tests.core.full_node.full_sync.test_full_sync,tests.core.full_node.stores.test_block_store,tests.core.full_node.stores.test_coin_store,tests.core.full_node.stores.test_full_node_store,tests.core.full_node.stores.test_hint_store,tests.core.full_node.stores.test_sync_store,tests.core.full_node.test_address_manager,tests.core.full_node.test_block_height_map,tests.core.full_node.test_conditions,tests.core.full_node.test_full_node,tests.core.mempool.test_mempool,tests.core.mempool.test_mempool_performance,tests.core.full_node.test_node_load,tests.core.full_node.test_peer_store_resolver,tests.core.full_node.test_performance,tests.core.full_node.test_transactions,tests.core.make_block_generator,tests.core.node_height,tests.core.server.test_dos,tests.core.server.test_rate_limits,tests.core.ssl.test_ssl,tests.core.test_cost_calculation,tests.core.test_crawler_rpc,tests.core.test_daemon_rpc,tests.core.test_db_conversion,tests.core.test_db_validation,tests.core.test_farmer_harvester_rpc,tests.core.test_filter,tests.core.test_full_node_rpc,tests.core.test_merkle_set,tests.core.test_setproctitle,tests.core.util.test_cached_bls,tests.core.util.test_config,tests.core.util.test_file_keyring_synchronization,tests.core.util.test_files,tests.core.util.test_keychain,tests.core.util.test_keyring_wrapper,tests.core.util.test_lru_cache,tests.core.util.test_significant_bits,tests.farmer_harvester.test_farmer_harvester,tests.generator.test_compression,tests.generator.test_generator_types,tests.generator.test_list_to_batches,tests.generator.test_rom,tests.generator.test_scan,tests.plotting.test_plot_manager,tests.pools.test_pool_cmdline,tests.pools.test_pool_config,tests.pools.test_pool_puzzles_lifecycle,tests.pools.test_wallet_pool_store,tests.simulation.test_simulation,chia.simulator.time_out_assert,tests.tools.test_full_sync,tests.tools.test_run_block,tests.util.alert_server,tests.util.benchmark_cost,tests.util.blockchain,tests.util.build_network_protocol_files,tests.util.db_connection,tests.util.generator_tools_testing,chia.simulator.keyring,tests.util.key_tool,tests.util.test_full_block_utils,tests.util.test_lock_queue,tests.util.test_misc,tests.util.test_network,tests.util.test_network_protocol_files,tests.wallet.cat_wallet.test_cat_lifecycle,tests.wallet.cat_wallet.test_cat_wallet,tests.wallet.cat_wallet.test_offer_lifecycle,tests.wallet.cat_wallet.test_trades,tests.wallet.did_wallet.test_did,tests.wallet.did_wallet.test_did_rpc,tests.wallet.did_wallet.test_nft_rpc,tests.wallet.did_wallet.test_nft_wallet,tests.wallet.rpc.test_wallet_rpc,tests.wallet.simple_sync.test_simple_sync_protocol,tests.wallet.sync.test_wallet_sync,tests.wallet.test_bech32m,tests.wallet.test_chialisp,tests.wallet.test_puzzle_store,tests.wallet.test_singleton,tests.wallet.test_singleton_lifecycle,tests.wallet.test_singleton_lifecycle_fast,tests.wallet.test_taproot,tests.wallet.test_wallet_blockchain,tests.wallet.test_wallet_interested_store,tests.wallet.test_wallet_key_val_store,tests.wallet.test_wallet_user_store,chia.simulator.wallet_tools,tests.weight_proof.test_weight_proof,tools.analyze-chain,tools.run_block,tools.test_full_sync,tests.wallet.nft_wallet.test_nft_wallet,chia.wallet.nft_wallet.nft_puzzles,tests.wallet.nft_wallet.test_nft_puzzles]
 disable_error_code = annotation-unchecked
 disallow_any_generics = False
 disallow_subclassing_any = False
 disallow_untyped_calls = False
 disallow_untyped_defs = False
 disallow_incomplete_defs = False
 check_untyped_defs = False
```

### Comparing `chia-blockchain-1.8.0b5/pylintrc` & `chia-blockchain-1.8.0b6/pylintrc`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/pytest.ini` & `chia-blockchain-1.8.0b6/pytest.ini`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/setup.py` & `chia-blockchain-1.8.0b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 
 from setuptools import setup
 
 dependencies = [
     "aiofiles==23.1.0",  # Async IO for files
     "anyio==3.6.2",
+    "boto3==1.26.111",  # AWS S3 for DL s3 plugin
     "blspy==1.0.16",  # Signature library
     "chiavdf==1.0.8",  # timelord and vdf verification
     "chiabip158==1.2",  # bip158-style wallet filters
     "chiapos==1.0.11",  # proof of space
     "clvm==0.9.7",
     "clvm_tools==0.4.6",  # Currying, Program.to, other conveniences
     "chia_rs==0.2.5",
@@ -136,14 +137,15 @@
             "chia_crawler = chia.seeder.start_crawler:main",
             "chia_seeder = chia.seeder.dns_server:main",
             "chia_timelord = chia.server.start_timelord:main",
             "chia_timelord_launcher = chia.timelord.timelord_launcher:main",
             "chia_full_node_simulator = chia.simulator.start_simulator:main",
             "chia_data_layer = chia.server.start_data_layer:main",
             "chia_data_layer_http = chia.data_layer.data_layer_server:main",
+            "chia_data_layer_s3_plugin = chia.data_layer.s3_plugin_service:run_server",
         ]
     },
     package_data={
         "chia": ["pyinstaller.spec"],
         "": ["*.clvm", "*.clvm.hex", "*.clib", "*.clinc", "*.clsp", "py.typed"],
         "chia.util": ["initial-*.yaml", "english.txt"],
         "chia.ssl": ["chia_ca.crt", "chia_ca.key", "dst_root_ca.pem"],
```

### Comparing `chia-blockchain-1.8.0b5/start-gui.sh` & `chia-blockchain-1.8.0b6/start-gui.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/README.md` & `chia-blockchain-1.8.0b6/tests/README.md`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/blockchain/blockchain_test_utils.py` & `chia-blockchain-1.8.0b6/tests/blockchain/blockchain_test_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/blockchain/test_blockchain.py` & `chia-blockchain-1.8.0b6/tests/blockchain/test_blockchain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/blockchain/test_blockchain_transactions.py` & `chia-blockchain-1.8.0b6/tests/blockchain/test_blockchain_transactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,18 +54,17 @@
 
         await full_node_api_1.send_transaction(tx)
 
         sb = full_node_1.mempool_manager.get_spendbundle(spend_bundle.name())
         assert sb == spend_bundle
 
         last_block = blocks[-1]
-        next_spendbundle, additions, removals = full_node_1.mempool_manager.create_bundle_from_mempool(
-            last_block.header_hash
-        )
-        assert next_spendbundle is not None
+        result = full_node_1.mempool_manager.create_bundle_from_mempool(last_block.header_hash)
+        assert result is not None
+        next_spendbundle, _ = result
 
         new_blocks = bt.get_consecutive_blocks(
             1,
             block_list_input=blocks,
             farmer_reward_puzzle_hash=coinbase_puzzlehash,
             transaction_data=next_spendbundle,
             guarantee_transaction_block=True,
```

### Comparing `chia-blockchain-1.8.0b5/tests/build-init-files.py` & `chia-blockchain-1.8.0b6/tests/build-init-files.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/build-job-matrix.py` & `chia-blockchain-1.8.0b6/tests/build-job-matrix.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/check_pytest_monitor_output.py` & `chia-blockchain-1.8.0b6/tests/check_pytest_monitor_output.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/check_sql_statements.py` & `chia-blockchain-1.8.0b6/tests/check_sql_statements.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/chia-start-sim` & `chia-blockchain-1.8.0b6/tests/chia-start-sim`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/clvm/benchmark_costs.py` & `chia-blockchain-1.8.0b6/tests/clvm/benchmark_costs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/clvm/coin_store.py` & `chia-blockchain-1.8.0b6/tests/clvm/coin_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/clvm/test_chialisp_deserialization.py` & `chia-blockchain-1.8.0b6/tests/clvm/test_chialisp_deserialization.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/clvm/test_clvm_step.py` & `chia-blockchain-1.8.0b6/tests/clvm/test_clvm_step.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/clvm/test_curry_and_treehash.py` & `chia-blockchain-1.8.0b6/tests/clvm/test_curry_and_treehash.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/clvm/test_program.py` & `chia-blockchain-1.8.0b6/tests/clvm/test_program.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/clvm/test_puzzle_compression.py` & `chia-blockchain-1.8.0b6/tests/clvm/test_puzzle_compression.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/clvm/test_puzzle_drivers.py` & `chia-blockchain-1.8.0b6/tests/clvm/test_puzzle_drivers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/clvm/test_puzzles.py` & `chia-blockchain-1.8.0b6/tests/clvm/test_puzzles.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from unittest import TestCase
 
 from blspy import AugSchemeMPL, BasicSchemeMPL, G1Element, G2Element
 
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.types.coin_spend import CoinSpend
-from chia.types.condition_opcodes import ConditionOpcode
 from chia.types.spend_bundle import SpendBundle
 from chia.util.hash import std_hash
 from chia.wallet.puzzles import (
     p2_conditions,
     p2_delegated_conditions,
     p2_delegated_puzzle,
     p2_delegated_puzzle_or_hidden_puzzle,
     p2_m_of_n_delegate_direct,
     p2_puzzle_hash,
 )
+from chia.wallet.puzzles.puzzle_utils import make_create_coin_condition
 from tests.util.key_tool import KeyTool
 
 from ..core.make_block_generator import int_to_public_key
 from .coin_store import CoinStore, CoinTimestamp
 
 T1 = CoinTimestamp(1, 10000000)
 T2 = CoinTimestamp(5, 10003000)
@@ -97,22 +97,18 @@
 ) -> Tuple[List[Tuple[bytes32, int]], Program]:
     # the coin we get from coin_db.farm_coin only has amount 1024, so we can
     # only make small payments to avoid failing with MINTING_COIN
     payments = [
         (throwaway_puzzle_hash(initial_index + 1, key_lookup), initial_index * 10),
         (throwaway_puzzle_hash(initial_index + 2, key_lookup), (initial_index + 1) * 10),
     ]
-    conditions = Program.to([make_create_coin_condition(ph, amount) for ph, amount in payments])
+    conditions = Program.to([make_create_coin_condition(ph, amount, None) for ph, amount in payments])
     return payments, conditions
 
 
-def make_create_coin_condition(puzzle_hash, amount):
-    return Program.to([ConditionOpcode.CREATE_COIN, puzzle_hash, amount])
-
-
 class TestPuzzles(TestCase):
     def test_p2_conditions(self):
         key_lookup = KeyTool()
         payments, conditions = default_payments_and_conditions(1, key_lookup)
 
         puzzle = p2_conditions.puzzle_for_conditions(conditions)
         solution = p2_conditions.solution_for_conditions(conditions)
```

### Comparing `chia-blockchain-1.8.0b5/tests/clvm/test_serialized_program.py` & `chia-blockchain-1.8.0b6/tests/clvm/test_serialized_program.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/clvm/test_singletons.py` & `chia-blockchain-1.8.0b6/tests/clvm/test_singletons.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/clvm/test_spend_sim.py` & `chia-blockchain-1.8.0b6/tests/clvm/test_spend_sim.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/cmds/test_wallet_check.py` & `chia-blockchain-1.8.0b6/tests/cmds/test_wallet_check.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/conftest.py` & `chia-blockchain-1.8.0b6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/connection_utils.py` & `chia-blockchain-1.8.0b6/tests/connection_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/cmds/test_beta.py` & `chia-blockchain-1.8.0b6/tests/core/cmds/test_beta.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/cmds/test_keys.py` & `chia-blockchain-1.8.0b6/tests/core/cmds/test_keys.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/cmds/test_wallet.py` & `chia-blockchain-1.8.0b6/tests/core/cmds/test_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/consensus/test_pot_iterations.py` & `chia-blockchain-1.8.0b6/tests/core/consensus/test_pot_iterations.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/custom_types/test_coin.py` & `chia-blockchain-1.8.0b6/tests/core/custom_types/test_coin.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/custom_types/test_proof_of_space.py` & `chia-blockchain-1.8.0b6/tests/core/custom_types/test_proof_of_space.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/custom_types/test_spend_bundle.py` & `chia-blockchain-1.8.0b6/tests/core/custom_types/test_spend_bundle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/daemon/test_daemon.py` & `chia-blockchain-1.8.0b6/tests/core/daemon/test_daemon.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/daemon/test_daemon_register.py` & `chia-blockchain-1.8.0b6/tests/core/daemon/test_daemon_register.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/daemon/test_keychain_proxy.py` & `chia-blockchain-1.8.0b6/tests/core/daemon/test_keychain_proxy.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/data_layer/conftest.py` & `chia-blockchain-1.8.0b6/tests/core/data_layer/conftest.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/data_layer/test_data_cli.py` & `chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_cli.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/data_layer/test_data_layer_util.py` & `chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_layer_util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/data_layer/test_data_rpc.py` & `chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,17 @@
     config["data_layer"]["wallet_peer"]["port"] = int(wallet_rpc_port)
     # TODO: running the data server causes the RPC tests to hang at the end
     config["data_layer"]["run_server"] = False
     config["data_layer"]["port"] = 0
     config["data_layer"]["rpc_port"] = 0
     config["data_layer"]["database_path"] = str(db_path.joinpath("db.sqlite"))
     save_config(bt.root_path, "config.yaml", config)
-    service = create_data_layer_service(root_path=bt.root_path, config=config, wallet_service=wallet_service)
+    service = create_data_layer_service(
+        root_path=bt.root_path, config=config, wallet_service=wallet_service, downloaders=[], uploaders=[]
+    )
     await service.start()
     try:
         yield service._api.data_layer
     finally:
         service.stop()
         await service.wait_closed()
```

### Comparing `chia-blockchain-1.8.0b5/tests/core/data_layer/test_data_store.py` & `chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/data_layer/test_data_store_schema.py` & `chia-blockchain-1.8.0b6/tests/core/data_layer/test_data_store_schema.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/data_layer/util.py` & `chia-blockchain-1.8.0b6/tests/core/data_layer/util.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/conftest.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/conftest.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/full_sync/test_full_sync.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/full_sync/test_full_sync.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/ram_db.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/ram_db.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/stores/test_block_store.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_block_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/stores/test_coin_store.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_coin_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/stores/test_full_node_store.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_full_node_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/stores/test_hint_store.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_hint_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/stores/test_sync_store.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/stores/test_sync_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/test_address_manager.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/test_address_manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/test_block_height_map.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/test_block_height_map.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/test_conditions.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/test_conditions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/test_full_node.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/test_full_node.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/test_generator_tools.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/test_generator_tools.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/test_hint_management.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/test_hint_management.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/test_node_load.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/test_node_load.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/test_peer_store_resolver.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/test_peer_store_resolver.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/test_performance.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/test_performance.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/test_subscriptions.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/test_transactions.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/test_transactions.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/full_node/test_tx_processing_queue.py` & `chia-blockchain-1.8.0b6/tests/core/full_node/test_tx_processing_queue.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/large_block.py` & `chia-blockchain-1.8.0b6/tests/core/large_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/make_block_generator.py` & `chia-blockchain-1.8.0b6/tests/core/make_block_generator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/mempool/test_mempool.py` & `chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,34 +24,29 @@
 from chia.server.outbound_message import Message
 from chia.server.ws_connection import WSChiaConnection
 from chia.simulator.simulator_protocol import FarmNewBlockProtocol
 from chia.simulator.time_out_assert import time_out_assert
 from chia.simulator.wallet_tools import WalletTool
 from chia.types.announcement import Announcement
 from chia.types.blockchain_format.coin import Coin
-from chia.types.blockchain_format.program import INFINITE_COST, Program
+from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.serialized_program import SerializedProgram
 from chia.types.blockchain_format.sized_bytes import bytes32, bytes48
 from chia.types.clvm_cost import CLVMCost
 from chia.types.coin_spend import CoinSpend
 from chia.types.condition_opcodes import ConditionOpcode
 from chia.types.condition_with_args import ConditionWithArgs
 from chia.types.fee_rate import FeeRate
 from chia.types.generator_types import BlockGenerator
 from chia.types.mempool_inclusion_status import MempoolInclusionStatus
 from chia.types.mempool_item import MempoolItem
 from chia.types.spend_bundle import SpendBundle
 from chia.types.spend_bundle_conditions import Spend, SpendBundleConditions
 from chia.util.api_decorators import api_request
-from chia.util.condition_tools import (
-    conditions_for_solution,
-    parse_sexp_to_conditions,
-    pkm_pairs,
-    pkm_pairs_for_conditions_dict,
-)
+from chia.util.condition_tools import parse_sexp_to_conditions, pkm_pairs, pkm_pairs_for_conditions_dict
 from chia.util.errors import ConsensusError, Err
 from chia.util.hash import std_hash
 from chia.util.ints import uint32, uint64
 from chia.util.recursive_replace import recursive_replace
 from tests.blockchain.blockchain_test_utils import _validate_and_add_block
 from tests.connection_utils import add_dummy_connection, connect_and_get_peer
 from tests.core.mempool.test_mempool_manager import make_test_coins, mk_item
@@ -1688,22 +1683,19 @@
 
         coin = await next_block(full_node_1, wallet_a, bt)
         # coin = list(blocks[-1].get_included_reward_coins())[0]
         spend_bundle_0 = generate_test_spend_bundle(wallet_a, coin)
         unsigned: List[CoinSpend] = spend_bundle_0.coin_spends
 
         assert len(unsigned) == 1
-        coin_spend: CoinSpend = unsigned[0]
-
-        err, con, cost = conditions_for_solution(coin_spend.puzzle_reveal, coin_spend.solution, INFINITE_COST)
-        assert con is not None
+        # coin_spend: CoinSpend = unsigned[0]
 
         # TODO(straya): fix this test
         # puzzle, solution = list(coin_spend.solution.as_iter())
-        # conditions_dict = conditions_by_opcode(con)
+        # conditions_dict = conditions_dict_for_solution(coin_spend.puzzle_reveal, coin_spend.solution, INFINITE_COST)
 
         # pkm_pairs = pkm_pairs_for_conditions_dict(conditions_dict, coin_spend.coin.name())
         # assert len(pkm_pairs) == 1
         #
         # assert pkm_pairs[0][1] == solution.rest().first().get_tree_hash() + coin_spend.coin.name()
         #
         # spend_bundle = wallet_a.sign_transaction(unsigned)
@@ -2624,46 +2616,39 @@
 
         with pytest.raises(ConsensusError, match="INVALID_CONDITION"):
             pkm_pairs_for_conditions_dict(conds, self.h1, b"g2")
 
 
 class TestParseSexpCondition:
     def test_basic(self) -> None:
-        err, conds = parse_sexp_to_conditions(Program.to([[bytes([49]), b"foo", b"bar"]]))
-        assert err is None
+        conds = parse_sexp_to_conditions(Program.to([[bytes([49]), b"foo", b"bar"]]))
         assert conds == [ConditionWithArgs(ConditionOpcode.AGG_SIG_UNSAFE, [b"foo", b"bar"])]
 
     def test_oversized_op(self) -> None:
-        err, conds = parse_sexp_to_conditions(Program.to([[bytes([49, 49]), b"foo", b"bar"]]))
-        assert err is Err.INVALID_CONDITION
-        assert conds is None
+        with pytest.raises(ConsensusError):
+            parse_sexp_to_conditions(Program.to([[bytes([49, 49]), b"foo", b"bar"]]))
 
     def test_empty_op(self) -> None:
-        err, conds = parse_sexp_to_conditions(Program.to([[b"", b"foo", b"bar"]]))
-        assert err is Err.INVALID_CONDITION
-        assert conds is None
+        with pytest.raises(ConsensusError):
+            parse_sexp_to_conditions(Program.to([[b"", b"foo", b"bar"]]))
 
     def test_list_op(self) -> None:
-        err, conds = parse_sexp_to_conditions(Program.to([[[bytes([49])], b"foo", b"bar"]]))
-        assert err is Err.INVALID_CONDITION
-        assert conds is None
+        with pytest.raises(ConsensusError):
+            parse_sexp_to_conditions(Program.to([[[bytes([49])], b"foo", b"bar"]]))
 
     def test_list_arg(self) -> None:
-        err, conds = parse_sexp_to_conditions(Program.to([[bytes([49]), [b"foo", b"bar"]]]))
-        assert err is None
+        conds = parse_sexp_to_conditions(Program.to([[bytes([49]), [b"foo", b"bar"]]]))
         assert conds == [ConditionWithArgs(ConditionOpcode.AGG_SIG_UNSAFE, [])]
 
     def test_list_arg_truncate(self) -> None:
-        err, conds = parse_sexp_to_conditions(Program.to([[bytes([49]), b"baz", [b"foo", b"bar"]]]))
-        assert err is None
+        conds = parse_sexp_to_conditions(Program.to([[bytes([49]), b"baz", [b"foo", b"bar"]]]))
         assert conds == [ConditionWithArgs(ConditionOpcode.AGG_SIG_UNSAFE, [b"baz"])]
 
     def test_arg_limit(self) -> None:
-        err, conds = parse_sexp_to_conditions(Program.to([[bytes([49]), b"1", b"2", b"3", b"4", b"5", b"6"]]))
-        assert err is None
+        conds = parse_sexp_to_conditions(Program.to([[bytes([49]), b"1", b"2", b"3", b"4", b"5", b"6"]]))
         assert conds == [ConditionWithArgs(ConditionOpcode.AGG_SIG_UNSAFE, [b"1", b"2", b"3", b"4"])]
 
 
 coins = make_test_coins()
 
 
 # This test makes sure we're properly sorting items by fee rate
@@ -2773,7 +2758,78 @@
 
     ordered_items = list(mempool.spends_by_feerate())
 
     assert len(ordered_items) == len(expected)
 
     for mi, expected_cost in zip(ordered_items, expected):
         assert mi.cost == expected_cost
+
+
+@pytest.mark.parametrize("height", [True, False])
+@pytest.mark.parametrize(
+    "items,expected,increase_fee",
+    [
+        # the max size is 100
+        # the max block size is 50
+        # which is also the max size for expiring transactions
+        # the increasing fee will order the transactions in the reverse
+        # insertion order
+        ([10, 11, 12, 13, 14], [14, 13, 12, 11], True),
+        # decreasing fee rate will make the last one fail to be inserted
+        ([10, 11, 12, 13, 14], [10, 11, 12, 13], False),
+        # the last is big enough to evict all previous ones
+        ([10, 11, 12, 13, 50], [50], True),
+        # the last one will not evict any earlier ones, because the fee rate is
+        # lower
+        ([10, 11, 12, 13, 50], [10, 11, 12, 13], False),
+    ],
+)
+def test_limit_expiring_transactions(height: bool, items: List[int], expected: List[int], increase_fee: bool) -> None:
+    fee_estimator = create_bitcoin_fee_estimator(uint64(11000000000))
+
+    mempool_info = MempoolInfo(
+        CLVMCost(uint64(100)),
+        FeeRate(uint64(1000000)),
+        CLVMCost(uint64(50)),
+    )
+    mempool = Mempool(mempool_info, fee_estimator)
+    mempool.new_tx_block(uint32(10), uint64(100000))
+
+    # fill the mempool with regular transactions (without expiration)
+    fee_rate: float = 3.0
+    for i in range(1, 20):
+        mempool.add_to_pool(item_cost(i, fee_rate))
+        fee_rate -= 0.1
+
+    # now add the expiring transactions from the test case
+    fee_rate = 2.7
+    for cost in items:
+        fee = cost * fee_rate
+        amount = int(fee + 100)
+        coin = Coin(rand_hash(), rand_hash(), amount)
+        if height:
+            ret = mempool.add_to_pool(mk_item([coin], cost=cost, fee=int(cost * fee_rate), assert_before_height=15))
+        else:
+            ret = mempool.add_to_pool(mk_item([coin], cost=cost, fee=int(cost * fee_rate), assert_before_seconds=10400))
+        if increase_fee:
+            fee_rate += 0.1
+            assert ret is None
+        else:
+            fee_rate -= 0.1
+
+    ordered_costs = [
+        item.cost
+        for item in mempool.spends_by_feerate()
+        if item.assert_before_height is not None or item.assert_before_seconds is not None
+    ]
+
+    assert ordered_costs == expected
+
+    print("")
+    for item in mempool.spends_by_feerate():
+        if item.assert_before_seconds is not None or item.assert_before_height is not None:
+            ttl = "yes"
+        else:
+            ttl = "No"
+        print(f"- cost: {item.cost} TTL: {ttl}")
+
+    assert mempool.total_mempool_cost() > 90
```

### Comparing `chia-blockchain-1.8.0b5/tests/core/mempool/test_mempool_fee_estimator.py` & `chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_fee_estimator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/mempool/test_mempool_fee_protocol.py` & `chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_fee_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/mempool/test_mempool_manager.py` & `chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,30 +134,32 @@
     seconds_relative: Optional[int] = None,
     seconds_absolute: int = 0,
     before_height_relative: Optional[int] = None,
     before_height_absolute: Optional[int] = None,
     before_seconds_relative: Optional[int] = None,
     before_seconds_absolute: Optional[int] = None,
     cost: int = 0,
+    spend_ids: List[bytes32] = [TEST_COIN_ID],
 ) -> SpendBundleConditions:
     return SpendBundleConditions(
         [
             Spend(
-                TEST_COIN.name(),
+                spend_id,
                 IDENTITY_PUZZLE_HASH,
                 None if height_relative is None else uint32(height_relative),
                 None if seconds_relative is None else uint64(seconds_relative),
                 None if before_height_relative is None else uint32(before_height_relative),
                 None if before_seconds_relative is None else uint64(before_seconds_relative),
                 None if birth_height is None else uint32(birth_height),
                 None if birth_seconds is None else uint64(birth_seconds),
                 [],
                 [],
                 0,
             )
+            for spend_id in spend_ids
         ],
         0,
         uint32(height_absolute),
         uint64(seconds_absolute),
         None if before_height_absolute is None else uint32(before_height_absolute),
         None if before_seconds_absolute is None else uint64(before_seconds_absolute),
         [],
@@ -615,19 +617,19 @@
     assert_before_height: Optional[int] = None,
     assert_before_seconds: Optional[int] = None,
 ) -> MempoolItem:
     # we don't actually care about the puzzle and solutions for the purpose of
     # can_replace()
     spends = [CoinSpend(c, SerializedProgram(), SerializedProgram()) for c in coins]
     spend_bundle = SpendBundle(spends, G2Element())
-    npc_results = NPCResult(None, make_test_conds(cost=cost), uint64(cost))
+    npc_result = NPCResult(None, make_test_conds(cost=cost, spend_ids=[c.name() for c in coins]), uint64(cost))
     return MempoolItem(
         spend_bundle,
         uint64(fee),
-        npc_results,
+        npc_result,
         spend_bundle.name(),
         uint32(0),
         None if assert_height is None else uint32(assert_height),
         None if assert_before_height is None else uint32(assert_before_height),
         None if assert_before_seconds is None else uint64(assert_before_seconds),
     )
 
@@ -913,20 +915,20 @@
     # Combined with the first spend bundle, we'd exceed the maximum block clvm cost
     conditions = [[ConditionOpcode.CREATE_COIN, IDENTITY_PUZZLE_HASH, coins[1].amount - 2]]
     sb2, _, res = await generate_and_add_spendbundle(mempool_manager, conditions, coins[1])
     assert res[1] == MempoolInclusionStatus.SUCCESS
     assert mempool_manager.peak is not None
     result = mempool_manager.create_bundle_from_mempool(mempool_manager.peak.header_hash)
     assert result is not None
-    agg, additions, removals = result
+    agg, additions = result
     # The second spend bundle has a higher FPC so it should get picked first
     assert agg == sb2
     # The first spend bundle hits the maximum block clvm cost and gets skipped
     assert additions == [Coin(coins[1].name(), IDENTITY_PUZZLE_HASH, coins[1].amount - 2)]
-    assert removals == [coins[1]]
+    assert agg.removals() == [coins[1]]
 
 
 @pytest.mark.parametrize(
     "opcode,arg,expect_eviction, expect_limit",
     [
         # current height: 10 current_time: 10000
         # we step the chain forward 1 block and 19 seconds
```

### Comparing `chia-blockchain-1.8.0b5/tests/core/mempool/test_mempool_performance.py` & `chia-blockchain-1.8.0b6/tests/core/mempool/test_mempool_performance.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/node_height.py` & `chia-blockchain-1.8.0b6/tests/core/node_height.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/server/flood.py` & `chia-blockchain-1.8.0b6/tests/core/server/flood.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/server/serve.py` & `chia-blockchain-1.8.0b6/tests/core/server/serve.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/server/test_capabilities.py` & `chia-blockchain-1.8.0b6/tests/core/server/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/server/test_dos.py` & `chia-blockchain-1.8.0b6/tests/core/server/test_dos.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,16 +167,16 @@
         await server_2.start_client(PeerInfo(self_hostname, uint16(server_1._port)), full_node_2.full_node.on_connect)
 
         assert len(server_1.all_connections) == 1
 
         ws_con: WSChiaConnection = list(server_1.all_connections.values())[0]
         ws_con_2: WSChiaConnection = list(server_2.all_connections.values())[0]
 
-        ws_con.peer_host = "1.2.3.4"
-        ws_con_2.peer_host = "1.2.3.4"
+        ws_con.peer_info = PeerInfo("1.2.3.4", ws_con.peer_info.port)
+        ws_con_2.peer_info = PeerInfo("1.2.3.4", ws_con_2.peer_info.port)
 
         new_tx_message = make_msg(
             ProtocolMessageTypes.new_transaction,
             full_node_protocol.NewTransaction(bytes([9] * 32), uint64(0), uint64(0)),
         )
         for i in range(4000):
             await ws_con._send_message(new_tx_message)
@@ -222,16 +222,16 @@
         await server_2.start_client(PeerInfo(self_hostname, uint16(server_1._port)), full_node_2.full_node.on_connect)
 
         assert len(server_1.all_connections) == 1
 
         ws_con: WSChiaConnection = list(server_1.all_connections.values())[0]
         ws_con_2: WSChiaConnection = list(server_2.all_connections.values())[0]
 
-        ws_con.peer_host = "1.2.3.4"
-        ws_con_2.peer_host = "1.2.3.4"
+        ws_con.peer_info = PeerInfo("1.2.3.4", ws_con.peer_info.port)
+        ws_con_2.peer_info = PeerInfo("1.2.3.4", ws_con_2.peer_info.port)
 
         def is_closed():
             return ws_con.closed
 
         new_message = make_msg(
             ProtocolMessageTypes.request_mempool_transactions,
             full_node_protocol.RequestMempoolTransactions(bytes([])),
@@ -271,16 +271,16 @@
         await server_2.start_client(PeerInfo(self_hostname, uint16(server_1._port)), full_node_2.full_node.on_connect)
 
         assert len(server_1.all_connections) == 1
 
         ws_con: WSChiaConnection = list(server_1.all_connections.values())[0]
         ws_con_2: WSChiaConnection = list(server_2.all_connections.values())[0]
 
-        ws_con.peer_host = "1.2.3.4"
-        ws_con_2.peer_host = "1.2.3.4"
+        ws_con.peer_info = PeerInfo("1.2.3.4", ws_con.peer_info.port)
+        ws_con_2.peer_info = PeerInfo("1.2.3.4", ws_con_2.peer_info.port)
 
         def is_closed():
             return ws_con.closed
 
         new_message = make_msg(
             ProtocolMessageTypes.request_mempool_transactions,
             full_node_protocol.RequestMempoolTransactions(bytes([0] * 5 * 1024 * 1024)),
```

### Comparing `chia-blockchain-1.8.0b5/tests/core/server/test_event_loop.py` & `chia-blockchain-1.8.0b6/tests/core/server/test_event_loop.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/server/test_loop.py` & `chia-blockchain-1.8.0b6/tests/core/server/test_loop.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/server/test_rate_limits.py` & `chia-blockchain-1.8.0b6/tests/core/server/test_rate_limits.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/server/test_server.py` & `chia-blockchain-1.8.0b6/tests/core/server/test_server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/ssl/test_ssl.py` & `chia-blockchain-1.8.0b6/tests/core/ssl/test_ssl.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/test_coins.py` & `chia-blockchain-1.8.0b6/tests/core/test_coins.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/test_cost_calculation.py` & `chia-blockchain-1.8.0b6/tests/core/test_cost_calculation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/test_crawler_rpc.py` & `chia-blockchain-1.8.0b6/tests/core/test_crawler_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/test_daemon_rpc.py` & `chia-blockchain-1.8.0b6/tests/core/test_daemon_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/test_db_conversion.py` & `chia-blockchain-1.8.0b6/tests/core/test_db_conversion.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/test_db_validation.py` & `chia-blockchain-1.8.0b6/tests/core/test_db_validation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/test_farmer_harvester_rpc.py` & `chia-blockchain-1.8.0b6/tests/core/test_farmer_harvester_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/test_filter.py` & `chia-blockchain-1.8.0b6/tests/core/test_filter.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/test_full_node_rpc.py` & `chia-blockchain-1.8.0b6/tests/core/test_full_node_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/test_merkle_set.py` & `chia-blockchain-1.8.0b6/tests/core/test_merkle_set.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/test_services.py` & `chia-blockchain-1.8.0b6/tests/core/test_services.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/util/test_cached_bls.py` & `chia-blockchain-1.8.0b6/tests/core/util/test_cached_bls.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/util/test_config.py` & `chia-blockchain-1.8.0b6/tests/core/util/test_config.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/util/test_file_keyring_synchronization.py` & `chia-blockchain-1.8.0b6/tests/core/util/test_file_keyring_synchronization.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/util/test_files.py` & `chia-blockchain-1.8.0b6/tests/core/util/test_files.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/util/test_jsonify.py` & `chia-blockchain-1.8.0b6/tests/core/util/test_jsonify.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/util/test_keychain.py` & `chia-blockchain-1.8.0b6/tests/core/util/test_keychain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/util/test_keyring_wrapper.py` & `chia-blockchain-1.8.0b6/tests/core/util/test_keyring_wrapper.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/util/test_lockfile.py` & `chia-blockchain-1.8.0b6/tests/core/util/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/util/test_lru_cache.py` & `chia-blockchain-1.8.0b6/tests/core/util/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/util/test_significant_bits.py` & `chia-blockchain-1.8.0b6/tests/core/util/test_significant_bits.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/core/util/test_streamable.py` & `chia-blockchain-1.8.0b6/tests/core/util/test_streamable.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/db/test_db_wrapper.py` & `chia-blockchain-1.8.0b6/tests/db/test_db_wrapper.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/farmer_harvester/test_farmer_harvester.py` & `chia-blockchain-1.8.0b6/tests/farmer_harvester/test_farmer_harvester.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 import asyncio
 
 import pytest
 
 from chia.farmer.farmer import Farmer
 from chia.simulator.time_out_assert import time_out_assert
-from chia.types.peer_info import PeerInfo
+from chia.types.peer_info import UnresolvedPeerInfo
 from chia.util.keychain import generate_mnemonic
 
 
 def farmer_is_started(farmer):
     return farmer.started
 
 
 @pytest.mark.asyncio
 async def test_start_with_empty_keychain(farmer_one_harvester_not_started):
     _, farmer_service, bt = farmer_one_harvester_not_started
     farmer: Farmer = farmer_service._node
+    farmer_service.reconnect_retry_seconds = 1
     # First remove all keys from the keychain
     bt.local_keychain.delete_all_keys()
     # Make sure the farmer service is not initialized yet
     assert not farmer.started
     # Start it, wait 5 seconds and make sure it still isn't initialized (since the keychain is empty)
     await farmer_service.start()
     await asyncio.sleep(5)
@@ -38,14 +39,17 @@
 @pytest.mark.asyncio
 async def test_harvester_handshake(farmer_one_harvester_not_started):
     harvesters, farmer_service, bt = farmer_one_harvester_not_started
     harvester_service = harvesters[0]
     harvester = harvester_service._node
     farmer = farmer_service._node
 
+    farmer_service.reconnect_retry_seconds = 1
+    harvester_service.reconnect_retry_seconds = 1
+
     def farmer_has_connections():
         return len(farmer.server.get_connections()) > 0
 
     def handshake_task_active():
         return farmer.harvester_handshake_task is not None
 
     async def handshake_done() -> bool:
@@ -56,15 +60,15 @@
     bt.local_keychain.delete_all_keys()
     # Handshake task and plot manager thread should not be running yet
     assert farmer.harvester_handshake_task is None
     assert harvester.plot_manager._refresh_thread is None
     # Start both services and wait a bit
     await farmer_service.start()
     await harvester_service.start()
-    harvester_service.add_peer(PeerInfo(str(farmer_service.self_hostname), farmer_service._server.get_port()))
+    harvester_service.add_peer(UnresolvedPeerInfo(str(farmer_service.self_hostname), farmer_service._server.get_port()))
     # Handshake task should be started but the handshake should not be done
     await time_out_assert(5, handshake_task_active, True)
     assert not await handshake_done()
     # Stop the harvester service and wait for the farmer to lose the connection
     harvester_service.stop()
     await harvester_service.wait_closed()
     await time_out_assert(10, farmer_has_connections, False)
@@ -72,15 +76,15 @@
     # Handshake task should be stopped again
     await time_out_assert(5, handshake_task_active, False)
     await asyncio.sleep(1)
     assert harvester.plot_manager._refresh_thread is None
     assert len(harvester.plot_manager.farmer_public_keys) == 0
     # Re-start the harvester and make sure the handshake task gets started but the handshake still doesn't go through
     await harvester_service.start()
-    harvester_service.add_peer(PeerInfo(str(farmer_service.self_hostname), farmer_service._server.get_port()))
+    harvester_service.add_peer(UnresolvedPeerInfo(str(farmer_service.self_hostname), farmer_service._server.get_port()))
     await time_out_assert(5, handshake_task_active, True)
     assert not await handshake_done()
     # Stop the farmer and make sure the handshake_task doesn't block the shutdown
     farmer_service.stop()
     await farmer_service.wait_closed()
     await time_out_assert(5, handshake_task_active, False)
     # Re-start the farmer and make sure the handshake task succeeds if a key get added to the keychain
```

### Comparing `chia-blockchain-1.8.0b5/tests/fee_estimation/cmdline_test.py` & `chia-blockchain-1.8.0b6/tests/fee_estimation/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/fee_estimation/test_fee_estimation_integration.py` & `chia-blockchain-1.8.0b6/tests/fee_estimation/test_fee_estimation_integration.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/fee_estimation/test_fee_estimation_rpc.py` & `chia-blockchain-1.8.0b6/tests/fee_estimation/test_fee_estimation_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/fee_estimation/test_fee_estimation_unit_tests.py` & `chia-blockchain-1.8.0b6/tests/fee_estimation/test_fee_estimation_unit_tests.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/fee_estimation/test_mempoolitem_height_added.py` & `chia-blockchain-1.8.0b6/tests/fee_estimation/test_mempoolitem_height_added.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/generator/test_compression.py` & `chia-blockchain-1.8.0b6/tests/generator/test_compression.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/generator/test_generator_types.py` & `chia-blockchain-1.8.0b6/tests/generator/test_generator_types.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/generator/test_list_to_batches.py` & `chia-blockchain-1.8.0b6/tests/generator/test_list_to_batches.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/generator/test_rom.py` & `chia-blockchain-1.8.0b6/tests/generator/test_rom.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/generator/test_scan.py` & `chia-blockchain-1.8.0b6/tests/generator/test_scan.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/plot_sync/test_delta.py` & `chia-blockchain-1.8.0b6/tests/plot_sync/test_delta.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/plot_sync/test_plot_sync.py` & `chia-blockchain-1.8.0b6/tests/plot_sync/test_plot_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,14 +295,15 @@
 
     # Invalidate the plots in `dir_invalid`
     for path in dir_invalid.path_list():
         with open(path, "wb") as file:
             file.write(bytes(100))
 
     harvester_services, farmer_service, bt = farmer_two_harvester_not_started
+    farmer_service.reconnect_retry_seconds = 1
     farmer: Farmer = farmer_service._node
     await farmer_service.start()
     harvesters: List[Harvester] = [
         await start_harvester_service(service, farmer_service) for service in harvester_services
     ]
     for harvester in harvesters:
         # Remove default plot directory for this tests
```

### Comparing `chia-blockchain-1.8.0b5/tests/plot_sync/test_receiver.py` & `chia-blockchain-1.8.0b6/tests/plot_sync/test_receiver.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,16 +243,16 @@
     assert get_list_or_len(plot_sync_dict_1["no_key_filenames"], not counts_only) == 0
     assert get_list_or_len(plot_sync_dict_1["duplicates"], not counts_only) == 0
     assert plot_sync_dict_1["total_plot_size"] == sum(plot.file_size for plot in receiver.plots().values())
     assert plot_sync_dict_1["syncing"] is None
     assert plot_sync_dict_1["last_sync_time"] is None
     assert plot_sync_dict_1["connection"] == {
         "node_id": receiver.connection().peer_node_id,
-        "host": receiver.connection().peer_host,
-        "port": receiver.connection().peer_port,
+        "host": receiver.connection().peer_info.host,
+        "port": receiver.connection().peer_info.port,
     }
 
     # We should get equal dicts
     assert plot_sync_dict_1 == receiver.to_dict(counts_only)
     # But unequal dicts wit the opposite counts_only value
     assert plot_sync_dict_1 != receiver.to_dict(not counts_only)
```

### Comparing `chia-blockchain-1.8.0b5/tests/plot_sync/test_sender.py` & `chia-blockchain-1.8.0b6/tests/plot_sync/test_sender.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/plot_sync/test_sync_simulated.py` & `chia-blockchain-1.8.0b6/tests/plot_sync/test_sync_simulated.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/plot_sync/util.py` & `chia-blockchain-1.8.0b6/tests/plot_sync/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 from chia.harvester.harvester import Harvester
 from chia.plot_sync.sender import Sender
 from chia.protocols.harvester_protocol import PlotSyncIdentifier
 from chia.server.outbound_message import Message, NodeType
 from chia.server.start_service import Service
 from chia.simulator.time_out_assert import time_out_assert
 from chia.types.blockchain_format.sized_bytes import bytes32
-from chia.types.peer_info import PeerInfo
-from chia.util.ints import uint64
+from chia.types.peer_info import PeerInfo, UnresolvedPeerInfo
+from chia.util.ints import uint16, uint64
 
 
 @dataclass
 class WSChiaConnectionDummy:
     connection_type: NodeType
     peer_node_id: bytes32
-    peer_host: str = "localhost"
-    peer_port: int = 0
+    peer_info: PeerInfo = PeerInfo("127.0.0.1", uint16(0))
     last_sent_message: Optional[Message] = None
 
     async def send_message(self, message: Message) -> None:
         self.last_sent_message = message
 
 
 def get_dummy_connection(node_type: NodeType, peer_id: Optional[bytes32] = None) -> WSChiaConnectionDummy:
@@ -37,16 +36,17 @@
     return PlotSyncIdentifier(uint64(int(time.time())), current_sync_id, message_id)
 
 
 async def start_harvester_service(harvester_service: Service[Harvester], farmer_service: Service[Farmer]) -> Harvester:
     # Set the `last_refresh_time` of the plot manager to avoid initial plot loading
     harvester: Harvester = harvester_service._node
     harvester.plot_manager.last_refresh_time = time.time()
+    harvester_service.reconnect_retry_seconds = 1
     await harvester_service.start()
-    harvester_service.add_peer(PeerInfo(str(farmer_service.self_hostname), farmer_service._server.get_port()))
+    harvester_service.add_peer(UnresolvedPeerInfo(str(farmer_service.self_hostname), farmer_service._server.get_port()))
     harvester.plot_manager.stop_refreshing()
 
     assert harvester.plot_sync_sender._sync_id == 0
     assert harvester.plot_sync_sender._next_message_id == 0
     assert harvester.plot_sync_sender._last_sync_id == 0
     assert harvester.plot_sync_sender._messages == []
```

### Comparing `chia-blockchain-1.8.0b5/tests/plotting/test_plot_manager.py` & `chia-blockchain-1.8.0b6/tests/plotting/test_plot_manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/pools/test_pool_cmdline.py` & `chia-blockchain-1.8.0b6/tests/pools/test_pool_cmdline.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/pools/test_pool_config.py` & `chia-blockchain-1.8.0b6/tests/pools/test_pool_config.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/pools/test_pool_puzzles_lifecycle.py` & `chia-blockchain-1.8.0b6/tests/pools/test_pool_puzzles_lifecycle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/pools/test_pool_rpc.py` & `chia-blockchain-1.8.0b6/tests/pools/test_pool_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/pools/test_pool_wallet.py` & `chia-blockchain-1.8.0b6/tests/pools/test_pool_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/pools/test_wallet_pool_store.py` & `chia-blockchain-1.8.0b6/tests/pools/test_wallet_pool_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/simulation/test_simulation.py` & `chia-blockchain-1.8.0b6/tests/simulation/test_simulation.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/simulation/test_simulator.py` & `chia-blockchain-1.8.0b6/tests/simulation/test_simulator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/simulation/test_start_simulator.py` & `chia-blockchain-1.8.0b6/tests/simulation/test_start_simulator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/tools/1315537.json` & `chia-blockchain-1.8.0b6/tests/tools/1315537.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/tools/1315544.json` & `chia-blockchain-1.8.0b6/tests/tools/1315544.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/tools/1315630.json` & `chia-blockchain-1.8.0b6/tests/tools/1315630.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/tools/300000.json` & `chia-blockchain-1.8.0b6/tests/tools/300000.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/tools/442734.json` & `chia-blockchain-1.8.0b6/tests/tools/442734.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/tools/466212.json` & `chia-blockchain-1.8.0b6/tests/tools/466212.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/tools/test-blockchain-db.sqlite` & `chia-blockchain-1.8.0b6/tests/tools/test-blockchain-db.sqlite`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/tools/test_full_sync.py` & `chia-blockchain-1.8.0b6/tests/tools/test_full_sync.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/tools/test_legacy_keyring.py` & `chia-blockchain-1.8.0b6/tests/tools/test_legacy_keyring.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/tools/test_run_block.py` & `chia-blockchain-1.8.0b6/tests/tools/test_run_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/alert_server.py` & `chia-blockchain-1.8.0b6/tests/util/alert_server.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/benchmark_cost.py` & `chia-blockchain-1.8.0b6/tests/util/benchmark_cost.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/bip39_test_vectors.json` & `chia-blockchain-1.8.0b6/tests/util/bip39_test_vectors.json`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/blockchain.py` & `chia-blockchain-1.8.0b6/tests/util/blockchain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/build_network_protocol_files.py` & `chia-blockchain-1.8.0b6/tests/util/build_network_protocol_files.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/db_connection.py` & `chia-blockchain-1.8.0b6/tests/util/db_connection.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/gen_ssl_certs.py` & `chia-blockchain-1.8.0b6/tests/util/gen_ssl_certs.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/generator_tools_testing.py` & `chia-blockchain-1.8.0b6/tests/util/generator_tools_testing.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/key_tool.py` & `chia-blockchain-1.8.0b6/tests/util/key_tool.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import List
 
 from blspy import AugSchemeMPL, G2Element, PrivateKey
 
 from chia.simulator.block_tools import test_constants
 from chia.types.coin_spend import CoinSpend
-from chia.util.condition_tools import conditions_by_opcode, conditions_for_solution, pkm_pairs_for_conditions_dict
+from chia.util.condition_tools import conditions_dict_for_solution, pkm_pairs_for_conditions_dict
 from tests.core.make_block_generator import GROUP_ORDER, int_to_public_key
 
 
 class KeyTool(dict):
     @classmethod
     def __new__(cls, *args):
         return dict.__new__(*args)
@@ -24,18 +24,16 @@
         if not secret_exponent:
             raise ValueError("unknown pubkey %s" % public_key.hex())
         bls_private_key = PrivateKey.from_bytes(secret_exponent.to_bytes(32, "big"))
         return AugSchemeMPL.sign(bls_private_key, message)
 
     def signature_for_solution(self, coin_spend: CoinSpend, additional_data: bytes) -> AugSchemeMPL:
         signatures = []
-        err, conditions, cost = conditions_for_solution(
+        conditions_dict = conditions_dict_for_solution(
             coin_spend.puzzle_reveal, coin_spend.solution, test_constants.MAX_BLOCK_COST_CLVM
         )
-        assert conditions is not None
-        conditions_dict = conditions_by_opcode(conditions)
         for public_key, message in pkm_pairs_for_conditions_dict(
             conditions_dict, coin_spend.coin.name(), additional_data
         ):
             signature = self.sign(public_key, message)
             signatures.append(signature)
         return AugSchemeMPL.aggregate(signatures)
```

### Comparing `chia-blockchain-1.8.0b5/tests/util/misc.py` & `chia-blockchain-1.8.0b6/tests/util/misc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/network_protocol_data.py` & `chia-blockchain-1.8.0b6/tests/util/network_protocol_data.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/protocol_messages_bytes-v1.0` & `chia-blockchain-1.8.0b6/tests/util/protocol_messages_bytes-v1.0`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/protocol_messages_json.py` & `chia-blockchain-1.8.0b6/tests/util/protocol_messages_json.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/rpc.py` & `chia-blockchain-1.8.0b6/tests/util/rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_chunks.py` & `chia-blockchain-1.8.0b6/tests/util/test_chunks.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_full_block_utils.py` & `chia-blockchain-1.8.0b6/tests/util/test_full_block_utils.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_limited_semaphore.py` & `chia-blockchain-1.8.0b6/tests/util/test_limited_semaphore.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_lock_queue.py` & `chia-blockchain-1.8.0b6/tests/util/test_lock_queue.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_logging_filter.py` & `chia-blockchain-1.8.0b6/tests/util/test_logging_filter.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_misc.py` & `chia-blockchain-1.8.0b6/tests/util/test_misc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_network.py` & `chia-blockchain-1.8.0b6/tests/util/test_network.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_network_protocol_files.py` & `chia-blockchain-1.8.0b6/tests/util/test_network_protocol_files.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_network_protocol_json.py` & `chia-blockchain-1.8.0b6/tests/util/test_network_protocol_json.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_network_protocol_test.py` & `chia-blockchain-1.8.0b6/tests/util/test_network_protocol_test.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_paginator.py` & `chia-blockchain-1.8.0b6/tests/util/test_paginator.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_pprint.py` & `chia-blockchain-1.8.0b6/tests/util/test_pprint.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/util/test_struct_stream.py` & `chia-blockchain-1.8.0b6/tests/util/test_struct_stream.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/test_cat_lifecycle.py` & `chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_cat_lifecycle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/test_cat_outer_puzzle.py` & `chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_cat_outer_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/test_cat_wallet.py` & `chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_cat_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/test_offer_lifecycle.py` & `chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_offer_lifecycle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/cat_wallet/test_trades.py` & `chia-blockchain-1.8.0b6/tests/wallet/cat_wallet/test_trades.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/db_wallet/test_db_graftroot.py` & `chia-blockchain-1.8.0b6/tests/wallet/db_wallet/test_db_graftroot.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/db_wallet/test_dl_offers.py` & `chia-blockchain-1.8.0b6/tests/wallet/db_wallet/test_dl_offers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/db_wallet/test_dl_wallet.py` & `chia-blockchain-1.8.0b6/tests/wallet/db_wallet/test_dl_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/did_wallet/test_did.py` & `chia-blockchain-1.8.0b6/tests/wallet/did_wallet/test_did.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from chia.types.condition_opcodes import ConditionOpcode
 from chia.types.peer_info import PeerInfo
 from chia.types.spend_bundle import SpendBundle
 from chia.util.bech32m import decode_puzzle_hash, encode_puzzle_hash
 from chia.util.condition_tools import conditions_dict_for_solution
 from chia.util.ints import uint16, uint32, uint64
 from chia.wallet.did_wallet.did_wallet import DIDWallet
-from chia.wallet.singleton import create_fullpuz
+from chia.wallet.singleton import create_singleton_puzzle
 from chia.wallet.util.address_type import AddressType
 from chia.wallet.util.wallet_types import WalletType
 from chia.wallet.wallet import CHIP_0002_SIGN_MESSAGE_PREFIX
 
 
 async def get_wallet_num(wallet_manager):
     return len(await wallet_manager.get_all_wallet_info_entries())
@@ -1015,15 +1015,15 @@
         await full_node_api.wait_for_wallet_synced(wallet_node=wallet_node, timeout=15)
 
         assert await did_wallet_1.get_confirmed_balance() == did_amount
         assert await did_wallet_1.get_unconfirmed_balance() == did_amount
         response = await api_0.did_get_info({"coin_id": did_wallet_1.did_info.origin_coin.name().hex()})
 
         assert response["launcher_id"] == did_wallet_1.did_info.origin_coin.name().hex()
-        assert response["full_puzzle"] == create_fullpuz(
+        assert response["full_puzzle"] == create_singleton_puzzle(
             did_wallet_1.did_info.current_inner, did_wallet_1.did_info.origin_coin.name()
         )
         assert response["metadata"]["twitter"] == "twitter"
         assert response["latest_coin"] == (await did_wallet_1.select_coins(uint64(1))).pop().name().hex()
         assert response["num_verification"] == 0
         assert response["recovery_list_hash"] == Program(Program.to([])).get_tree_hash().hex()
         assert decode_puzzle_hash(response["p2_address"]).hex() == response["hints"][0]
@@ -1113,15 +1113,15 @@
         await time_out_assert(15, did_wallet_1.get_confirmed_balance, 101)
         await time_out_assert(15, did_wallet_1.get_unconfirmed_balance, 101)
         response = await api_0.did_message_spend(
             {"wallet_id": did_wallet_1.wallet_id, "coin_announcements": ["0abc"], "puzzle_announcements": ["0def"]}
         )
         assert "spend_bundle" in response
         spend = response["spend_bundle"].coin_spends[0]
-        error, conditions, cost = conditions_dict_for_solution(
+        conditions = conditions_dict_for_solution(
             spend.puzzle_reveal.to_program(),
             spend.solution.to_program(),
             wallet.wallet_state_manager.constants.MAX_BLOCK_COST_CLVM,
         )
 
         assert len(conditions[ConditionOpcode.CREATE_COIN_ANNOUNCEMENT]) == 1
         assert conditions[ConditionOpcode.CREATE_COIN_ANNOUNCEMENT][0].vars[0].hex() == "0abc"
```

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_nft_1_offers.py` & `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_1_offers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_nft_bulk_mint.py` & `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_bulk_mint.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_nft_lifecycle.py` & `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_lifecycle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_nft_offers.py` & `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_offers.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_nft_puzzles.py` & `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_puzzles.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_nft_wallet.py` & `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_nft_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/nft_wallet/test_ownership_outer_puzzle.py` & `chia-blockchain-1.8.0b6/tests/wallet/nft_wallet/test_ownership_outer_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/rpc/test_dl_wallet_rpc.py` & `chia-blockchain-1.8.0b6/tests/wallet/rpc/test_dl_wallet_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/rpc/test_wallet_rpc.py` & `chia-blockchain-1.8.0b6/tests/wallet/rpc/test_wallet_rpc.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/simple_sync/test_simple_sync_protocol.py` & `chia-blockchain-1.8.0b6/tests/wallet/simple_sync/test_simple_sync_protocol.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/sync/test_wallet_sync.py` & `chia-blockchain-1.8.0b6/tests/wallet/sync/test_wallet_sync.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_address_type.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_address_type.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_bech32m.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_bech32m.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_chialisp.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_chialisp.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_coin_selection.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_coin_selection.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_nft_store.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_nft_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_notifications.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_notifications.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_offer_parsing_performance.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_offer_parsing_performance.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_puzzle_store.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_puzzle_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_singleton.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_singleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,14 @@
     p2_singleton_coin_id = Program.to(["test_hash"]).get_tree_hash()
     expected_announcement = Announcement(singleton_full_puzzle.get_tree_hash(), p2_singleton_coin_id).name()
 
     # create a `p2_singleton` puzzle. This should call driver code.
     p2_singleton_full = p2_singleton_puzzle(launcher_id, LAUNCHER_PUZZLE_HASH)
     solution = Program.to([innerpuz.get_tree_hash(), p2_singleton_coin_id])
     cost, result = p2_singleton_full.run_with_cost(INFINITE_COST, solution)
-    err, conditions = parse_sexp_to_conditions(result)
-    assert err is None
+    conditions = parse_sexp_to_conditions(result)
 
     p2_singleton_full = p2_singleton_puzzle(launcher_id, LAUNCHER_PUZZLE_HASH)
     solution = Program.to([innerpuz.get_tree_hash(), p2_singleton_coin_id])
     cost, result = p2_singleton_full.run_with_cost(INFINITE_COST, solution)
     assert result.first().rest().first().as_atom() == expected_announcement
     assert conditions[0].vars[0] == expected_announcement
```

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_singleton_lifecycle.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_singleton_lifecycle.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_singleton_lifecycle_fast.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_singleton_lifecycle_fast.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_taproot.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_taproot.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_transaction_store.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_transaction_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_wallet.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_wallet.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_wallet_blockchain.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_blockchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,23 +36,19 @@
 
         res_3 = await full_node_api.request_proof_of_weight(
             full_node_protocol.RequestProofOfWeight(
                 default_1000_blocks[505].height + 1, default_1000_blocks[505].header_hash
             )
         )
         weight_proof: WeightProof = full_node_protocol.RespondProofOfWeight.from_bytes(res.data).wp
-        success, _, records = await wallet_node._weight_proof_handler.validate_weight_proof(weight_proof, True)
+        records = await wallet_node._weight_proof_handler.validate_weight_proof(weight_proof, True)
         weight_proof_short: WeightProof = full_node_protocol.RespondProofOfWeight.from_bytes(res_2.data).wp
-        success, _, records_short = await wallet_node._weight_proof_handler.validate_weight_proof(
-            weight_proof_short, True
-        )
+        records_short = await wallet_node._weight_proof_handler.validate_weight_proof(weight_proof_short, True)
         weight_proof_long: WeightProof = full_node_protocol.RespondProofOfWeight.from_bytes(res_3.data).wp
-        success, _, records_long = await wallet_node._weight_proof_handler.validate_weight_proof(
-            weight_proof_long, True
-        )
+        records_long = await wallet_node._weight_proof_handler.validate_weight_proof(weight_proof_long, True)
 
         async with DBConnection(1) as db_wrapper:
             store = await KeyValStore.create(db_wrapper)
             chain = await WalletBlockchain.create(store, test_constants)
 
             assert (await chain.get_peak_block()) is None
             assert chain.get_latest_timestamp() == 0
```

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_wallet_coin_store.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_coin_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import annotations
 
 from secrets import token_bytes
 
 import pytest
 
 from chia.types.blockchain_format.coin import Coin
-from chia.util.ints import uint32, uint64
-from chia.wallet.util.wallet_types import WalletType
+from chia.util.ints import uint16, uint32, uint64
+from chia.util.misc import VersionedBlob
+from chia.wallet.util.wallet_types import CoinType, WalletType
 from chia.wallet.wallet_coin_record import WalletCoinRecord
 from chia.wallet.wallet_coin_store import WalletCoinStore
 from tests.util.db_connection import DBConnection
 
 coin_1 = Coin(token_bytes(32), token_bytes(32), uint64(12312))
 coin_2 = Coin(coin_1.parent_coin_info, token_bytes(32), uint64(12311))
 coin_3 = Coin(token_bytes(32), token_bytes(32), uint64(12312))
 coin_4 = Coin(token_bytes(32), token_bytes(32), uint64(12312))
 coin_5 = Coin(token_bytes(32), token_bytes(32), uint64(12312))
 coin_6 = Coin(token_bytes(32), coin_4.puzzle_hash, uint64(12312))
 coin_7 = Coin(token_bytes(32), token_bytes(32), uint64(12312))
+coin_8 = Coin(token_bytes(32), token_bytes(32), uint64(2))
 record_replaced = WalletCoinRecord(coin_1, uint32(8), uint32(0), False, True, WalletType.STANDARD_WALLET, 0)
 record_1 = WalletCoinRecord(coin_1, uint32(4), uint32(0), False, True, WalletType.STANDARD_WALLET, 0)
 record_2 = WalletCoinRecord(coin_2, uint32(5), uint32(0), False, True, WalletType.STANDARD_WALLET, 0)
 record_3 = WalletCoinRecord(
     coin_3,
     uint32(5),
     uint32(10),
@@ -62,14 +64,25 @@
     uint32(5),
     uint32(0),
     False,
     False,
     WalletType.POOLING_WALLET,
     2,
 )
+record_8 = WalletCoinRecord(
+    coin_8,
+    uint32(1),
+    uint32(0),
+    False,
+    False,
+    WalletType.STANDARD_WALLET,
+    1,
+    CoinType.CLAWBACK,
+    VersionedBlob(uint16(1), b"TEST"),
+)
 
 
 @pytest.mark.asyncio
 async def test_add_replace_get() -> None:
     async with DBConnection(1) as db_wrapper:
         store = await WalletCoinStore.create(db_wrapper)
 
@@ -99,14 +112,15 @@
 async def test_bulk_get() -> None:
     async with DBConnection(1) as db_wrapper:
         store = await WalletCoinStore.create(db_wrapper)
         await store.add_coin_record(record_1)
         await store.add_coin_record(record_2)
         await store.add_coin_record(record_3)
         await store.add_coin_record(record_4)
+        await store.add_coin_record(record_8)
 
         store = await WalletCoinStore.create(db_wrapper)
         records = await store.get_coin_records([coin_1.name(), coin_2.name(), token_bytes(32), coin_4.name()])
         assert records == {coin_1.name(): record_1, coin_2.name(): record_2, coin_4.name(): record_4}
 
 
 @pytest.mark.asyncio
@@ -147,14 +161,15 @@
 
         assert await store.get_unspent_coins_for_wallet(1) == set()
 
         await store.add_coin_record(record_4)  # this is spent and wallet 0
         await store.add_coin_record(record_5)  # wallet 1
         await store.add_coin_record(record_6)  # this is spent and wallet 2
         await store.add_coin_record(record_7)  # wallet 2
+        await store.add_coin_record(record_8)
 
         assert await store.get_unspent_coins_for_wallet(1) == set([record_5])
         assert await store.get_unspent_coins_for_wallet(2) == set([record_7])
         assert await store.get_unspent_coins_for_wallet(3) == set()
 
         await store.set_spent(coin_4.name(), uint32(12))
 
@@ -170,25 +185,28 @@
 
         await store.set_spent(coin_5.name(), uint32(12))
 
         assert await store.get_unspent_coins_for_wallet(1) == set()
         assert await store.get_unspent_coins_for_wallet(2) == set()
         assert await store.get_unspent_coins_for_wallet(3) == set()
 
+        assert await store.get_unspent_coins_for_wallet(1, coin_type=CoinType.CLAWBACK) == set([record_8])
+
 
 @pytest.mark.asyncio
 async def test_get_all_unspent_coins() -> None:
     async with DBConnection(1) as db_wrapper:
         store = await WalletCoinStore.create(db_wrapper)
 
         assert await store.get_all_unspent_coins() == set()
 
         await store.add_coin_record(record_1)  # not spent
         await store.add_coin_record(record_2)  # not spent
         await store.add_coin_record(record_3)  # spent
+        await store.add_coin_record(record_8)  # spent
         assert await store.get_all_unspent_coins() == set([record_1, record_2])
 
         await store.add_coin_record(record_4)  # spent
         await store.add_coin_record(record_5)  # not spent
         await store.add_coin_record(record_6)  # spent
         assert await store.get_all_unspent_coins() == set([record_1, record_2, record_5])
 
@@ -204,14 +222,16 @@
         await store.set_spent(coin_5.name(), uint32(12))
         assert await store.get_all_unspent_coins() == set([record_1, record_2])
 
         await store.set_spent(coin_2.name(), uint32(12))
         await store.set_spent(coin_1.name(), uint32(12))
         assert await store.get_all_unspent_coins() == set()
 
+        assert await store.get_all_unspent_coins(coin_type=CoinType.CLAWBACK) == set([record_8])
+
 
 @pytest.mark.asyncio
 async def test_get_records_by_parent_id() -> None:
     async with DBConnection(1) as db_wrapper:
         store = await WalletCoinStore.create(db_wrapper)
 
         await store.add_coin_record(record_1)
@@ -374,21 +394,47 @@
         r1 = record(coin_1, confirmed=1, spent=0)
         r2 = record(coin_2, confirmed=2, spent=0)
         r3 = record(coin_3, confirmed=3, spent=0)
 
         await store.add_coin_record(r1)
         await store.add_coin_record(r2)
         await store.add_coin_record(r3)
+        await store.add_coin_record(record_8)
 
         assert await store.count_small_unspent(5) == 3
         assert await store.count_small_unspent(4) == 2
         assert await store.count_small_unspent(3) == 2
         assert await store.count_small_unspent(2) == 1
         assert await store.count_small_unspent(1) == 0
+        assert await store.count_small_unspent(3, coin_type=CoinType.CLAWBACK) == 1
 
         await store.set_spent(coin_2.name(), uint32(12))
+        await store.set_spent(coin_8.name(), uint32(12))
 
         assert await store.count_small_unspent(5) == 2
         assert await store.count_small_unspent(4) == 1
         assert await store.count_small_unspent(3) == 1
         assert await store.count_small_unspent(2) == 1
+        assert await store.count_small_unspent(3, coin_type=CoinType.CLAWBACK) == 0
         assert await store.count_small_unspent(1) == 0
+
+
+@pytest.mark.asyncio
+async def test_get_coin_records_between() -> None:
+    async with DBConnection(1) as db_wrapper:
+        store = await WalletCoinStore.create(db_wrapper)
+
+        assert await store.get_all_unspent_coins() == set()
+
+        await store.add_coin_record(record_1)  # not spent
+        await store.add_coin_record(record_2)  # not spent
+        await store.add_coin_record(record_5)  # spent
+        await store.add_coin_record(record_8)  # spent
+
+        records = await store.get_coin_records_between(1, 0, 0)
+        assert len(records) == 0
+        records = await store.get_coin_records_between(1, 0, 3)
+        assert len(records) == 1
+        assert records[0] == record_5
+        records = await store.get_coin_records_between(1, 0, 4, coin_type=CoinType.CLAWBACK)
+        assert len(records) == 1
+        assert records[0] == record_8
```

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_wallet_interested_store.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_interested_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_wallet_key_val_store.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_key_val_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_wallet_node.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_node.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_wallet_retry.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_retry.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_wallet_state_manager.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_state_manager.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_wallet_trade_store.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_trade_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/wallet/test_wallet_user_store.py` & `chia-blockchain-1.8.0b6/tests/wallet/test_wallet_user_store.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tests/weight_proof/test_weight_proof.py` & `chia-blockchain-1.8.0b6/tests/weight_proof/test_weight_proof.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tools/analyze-chain.py` & `chia-blockchain-1.8.0b6/tools/analyze-chain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tools/analyze_memory_profile.py` & `chia-blockchain-1.8.0b6/tools/analyze_memory_profile.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tools/cpu_utilization.py` & `chia-blockchain-1.8.0b6/tools/cpu_utilization.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tools/generate_chain.py` & `chia-blockchain-1.8.0b6/tools/generate_chain.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tools/legacy_keyring.py` & `chia-blockchain-1.8.0b6/tools/legacy_keyring.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tools/manage_clvm.py` & `chia-blockchain-1.8.0b6/tools/manage_clvm.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
             print(f"    {exclude}")
 
     if use_cache and cache_modified:
         cache_path.parent.mkdir(parents=True, exist_ok=True)
         with cache_path.open(mode="w") as file:
             dump_cache(cache=cache, file=file)
 
-    return 1 if overall_fail else 0
+    sys.exit(1 if overall_fail else 0)
 
 
 @main.command()
 def build() -> int:
     overall_fail = False
 
     found_stems = find_stems(top_levels, suffixes={"clvm": clvm_suffix})
@@ -340,11 +340,11 @@
                 print(error)
         else:
             print(f"    built: {clvm_path}")
 
         if file_fail:
             overall_fail = True
 
-    return 1 if overall_fail else 0
+    sys.exit(1 if overall_fail else 0)
 
 
-sys.exit(main(auto_envvar_prefix="CHIA_MANAGE_CLVM"))
+main(auto_envvar_prefix="CHIA_MANAGE_CLVM")
```

### Comparing `chia-blockchain-1.8.0b5/tools/plot-log.gnuplot` & `chia-blockchain-1.8.0b6/tools/plot-log.gnuplot`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tools/run_benchmark.sh` & `chia-blockchain-1.8.0b6/tools/run_benchmark.sh`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tools/run_block.py` & `chia-blockchain-1.8.0b6/tools/run_block.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tools/test_constants.py` & `chia-blockchain-1.8.0b6/tools/test_constants.py`

 * *Files identical despite different names*

### Comparing `chia-blockchain-1.8.0b5/tools/test_full_sync.py` & `chia-blockchain-1.8.0b6/tools/test_full_sync.py`

 * *Files identical despite different names*


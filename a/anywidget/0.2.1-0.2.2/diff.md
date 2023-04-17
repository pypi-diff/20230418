# Comparing `tmp/anywidget-0.2.1.tar.gz` & `tmp/anywidget-0.2.2.tar.gz`

## Comparing `anywidget-0.2.1.tar` & `anywidget-0.2.2.tar`

### file list

```diff
@@ -1,101 +1,100 @@
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 anywidget-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 anywidget-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget.json
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 anywidget-0.2.1/package.json
--rw-r--r--   0        0        0   251374 2020-02-02 00:00:00.000000 anywidget-0.2.1/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.2.1/pnpm-workspace.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.2.1/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/__init__.py
--rw-r--r--   0        0        0    24459 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/_protocols.py
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/widget.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/labextension/static/138.4955823d1827e11e8ec1.js
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/labextension/static/326.1ce804f5af553a793872.js
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/labextension/static/remoteEntry.d443ca0ab408b6568c07.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 anywidget-0.2.1/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/astro.config.mjs
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/scripts/render.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Counter.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.2.1/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.2.1/examples/Counter.ipynb
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 anywidget-0.2.1/examples/minimal_example.ipynb
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.2.1/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.2.1/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.2.1/packages/anywidget/package.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.2.1/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.2.1/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 anywidget-0.2.1/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 anywidget-0.2.1/tests/test_descriptor.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.2.1/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.2.1/tests/test_protocols.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 anywidget-0.2.1/tests/test_utils.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.2.1/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.2.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.2.1/LICENSE
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.2.1/README.md
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 anywidget-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 anywidget-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 anywidget-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget.json
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 anywidget-0.2.2/package.json
+-rw-r--r--   0        0        0   251374 2020-02-02 00:00:00.000000 anywidget-0.2.2/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.2.2/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.2.2/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/__init__.py
+-rw-r--r--   0        0        0    24459 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/widget.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/labextension/static/138.59057bd63ab1c21ed356.js
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/labextension/static/326.d1451d7ac916a323dd4d.js
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/labextension/static/remoteEntry.2212decbf8760b4ac856.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 anywidget-0.2.2/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/astro.config.mjs
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/scripts/render.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Counter.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.2.2/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.2.2/examples/Counter.ipynb
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 anywidget-0.2.2/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 anywidget-0.2.2/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.2.2/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.2.2/packages/anywidget/package.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.2.2/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.2.2/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 anywidget-0.2.2/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 anywidget-0.2.2/tests/test_descriptor.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.2.2/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.2.2/tests/test_protocols.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 anywidget-0.2.2/tests/test_utils.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.2.2/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.2.2/README.md
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 anywidget-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 anywidget-0.2.2/PKG-INFO
```

### Comparing `anywidget-0.2.1/.pre-commit-config.yaml` & `anywidget-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/CHANGELOG.md` & `anywidget-0.2.2/packages/anywidget/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # anywidget
 
+## 0.2.2
+
+### Patch Changes
+
+- feat: log an re-raise error on ESM import failure ([#105](https://github.com/manzt/anywidget/pull/105))
+
+## 0.2.1
+
+### Patch Changes
+
+- fix: allow more flexible semver resolution for `@jupyter-widgets/base` ([`fe00cdf`](https://github.com/manzt/anywidget/commit/fe00cdfa56e983bdc7b2c6c00b30efae75814057))
+
 ## 0.2.0
 
 ### Minor Changes
 
 - feat: auto-create (and watch) `FileContents` for valid file paths ([#79](https://github.com/manzt/anywidget/pull/79))
 
   ```python
```

### Comparing `anywidget-0.2.1/package.json` & `anywidget-0.2.2/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/pnpm-lock.yaml` & `anywidget-0.2.2/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/anywidget/_descriptor.py` & `anywidget-0.2.2/anywidget/_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/anywidget/_file_contents.py` & `anywidget-0.2.2/anywidget/_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/anywidget/_protocols.py` & `anywidget-0.2.2/anywidget/_protocols.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/anywidget/_util.py` & `anywidget-0.2.2/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/anywidget/widget.py` & `anywidget-0.2.2/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/anywidget/labextension/package.json` & `anywidget-0.2.2/anywidget/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95703125%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.2212decbf8760b4ac856.js'}}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -22,15 +22,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.d443ca0ab408b6568c07.js"
+            "load": "static/remoteEntry.2212decbf8760b4ac856.js"
         },
         "extension": "src/plugin",
         "outputDir": "../../anywidget/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -42,9 +42,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `anywidget-0.2.1/anywidget/labextension/static/138.4955823d1827e11e8ec1.js` & `anywidget-0.2.2/anywidget/labextension/static/138.59057bd63ab1c21ed356.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -37,18 +37,22 @@
                     });
                     n.appendChild(document.createTextNode(e)), document.head.appendChild(n)
                 }(e, t)
             }
             async function d(e) {
                 if (a(e)) return import(e);
                 let t = URL.createObjectURL(new Blob([e], {
-                        type: "text/javascript"
-                    })),
-                    i = await import(t);
-                return URL.revokeObjectURL(t), i
+                    type: "text/javascript"
+                }));
+                try {
+                    await import(t)
+                } catch (e) {
+                    throw console.log(e), e
+                }
+                return URL.revokeObjectURL(t), widget
             }
 
             function c(e) {
                 class t extends e.DOMWidgetModel {
                     static model_name = "AnyModel";
                     static model_module = n.u2;
                     static model_module_version = n.i8;
@@ -88,11 +92,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.2.1"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.2.2"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.2.1/anywidget/labextension/static/326.1ce804f5af553a793872.js` & `anywidget-0.2.2/anywidget/labextension/static/326.d1451d7ac916a323dd4d.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -55,18 +55,22 @@
                     });
                     n.appendChild(document.createTextNode(e)), document.head.appendChild(n)
                 }(e, t)
             }
             async function d(e) {
                 if (a(e)) return import(e);
                 let t = URL.createObjectURL(new Blob([e], {
-                        type: "text/javascript"
-                    })),
-                    i = await import(t);
-                return URL.revokeObjectURL(t), i
+                    type: "text/javascript"
+                }));
+                try {
+                    await import(t)
+                } catch (e) {
+                    throw console.log(e), e
+                }
+                return URL.revokeObjectURL(t), widget
             }
 
             function c(e) {
                 class t extends e.DOMWidgetModel {
                     static model_name = "AnyModel";
                     static model_module = n.u2;
                     static model_module_version = n.i8;
@@ -106,11 +110,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.2.1"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.2.2"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.2.1/anywidget/labextension/static/remoteEntry.d443ca0ab408b6568c07.js` & `anywidget-0.2.2/anywidget/labextension/static/remoteEntry.2212decbf8760b4ac856.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, d, f, p, c, h, v = {
+    var e, r, t, n, o, a, i, u, d, l, s, f, c, p, h, v = {
             408: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(138).then((() => () => t(138))),
                         "./extension": () => t.e(326).then((() => () => t(326)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -41,45 +41,45 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        138: "4955823d1827e11e8ec1",
-        326: "1ce804f5af553a793872"
+        138: "59057bd63ab1c21ed356",
+        326: "d1451d7ac916a323dd4d"
     } [e] + ".js?v=" + {
-        138: "4955823d1827e11e8ec1",
-        326: "1ce804f5af553a793872"
+        138: "59057bd63ab1c21ed356",
+        326: "d1451d7ac916a323dd4d"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var d = l[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        i = d;
+                for (var d = document.getElementsByTagName("script"), l = 0; l < d.length; l++) {
+                    var s = d[l];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -104,15 +104,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => m.e(138).then((() => () => m(138))),
                         from: i,
                         eager: !1
                     })
-                })("anywidget", "0.2.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.2.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -147,94 +147,94 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
         for (a = 1; a < e.length; a++) {
             var u = e[a];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+            i.push(0 === u ? "not(" + d() + ")" : 1 === u ? "(" + d() + " || " + d() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
-        return l();
+        return d();
 
-        function l() {
+        function d() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
-                if ("u" == d) {
-                    if (!l || "u" != f) return !1
-                } else if (l)
-                    if (f == d)
+            for (var i = 0, u = 1, d = !0;; u++, i++) {
+                var l, s, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(l = r[i]))[0])) return !d || ("u" == f ? u > n && !o : "" == f != o);
+                if ("u" == s) {
+                    if (!d || "u" != f) return !1
+                } else if (d)
+                    if (f == s)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (l != e[u]) return !1
                         } else {
-                            if (o ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (o ? l > e[u] : l < e[u]) return !1;
+                            l != e[u] && (d = !1)
                         }
                 else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
-                    l = !1, u--
+                    d = !1, u--
                 } else {
-                    if (u <= n || d < f != o) return !1;
-                    l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                    if (u <= n || s < f != o) return !1;
+                    d = !1
+                } else "s" != f && "n" != f && (d = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
         var t = m.S[e];
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), d(e[t][o])
-    }, d = e => (e.loaded = 1, e.get()), f = (e => function(r, t, n, o) {
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(d(e, t, o, n)), s(e[t][o])
+    }, s = e => (e.loaded = 1, e.get()), f = (e => function(r, t, n, o) {
         var a = m.I(r);
         return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), p = {}, c = {
+    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), c = {}, p = {
         395: () => f("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ])
     }, h = {
         326: [395]
     }, m.f.consumes = (e, r) => {
         m.o(h, e) && h[e].forEach((e => {
-            if (m.o(p, e)) return r.push(p[e]);
+            if (m.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    p[e] = 0, m.m[e] = t => {
+                    c[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete p[e], m.m[e] = t => {
+                    delete c[e], m.m[e] = t => {
                         throw delete m.c[e], r
                     }
                 };
             try {
-                var o = c[e]();
-                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
+                var o = p[e]();
+                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             957: 0
@@ -255,20 +255,20 @@
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
-                    l = 0;
+                    d = 0;
                 if (a.some((r => 0 !== e[r]))) {
                     for (n in i) m.o(i, n) && (m.m[n] = i[n]);
                     u && u(m)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); d < a.length; d++) o = a[d], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkanywidget = self.webpackChunkanywidget || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var y = m(408);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = y
 })();
```

### Comparing `anywidget-0.2.1/anywidget/nbextension/index.js` & `anywidget-0.2.2/anywidget/nbextension/index.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.2.1";
+var version = "0.2.2";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
@@ -56,18 +56,23 @@
         );
     }
     let url = URL.createObjectURL(
         new Blob([esm], {
             type: "text/javascript"
         })
     );
-    let widget = await import(
-        /* webpackIgnore: true */
-        url
-    );
+    try {
+        let widget2 = await import(
+            /* webpackIgnore: true */
+            url
+        );
+    } catch (e) {
+        console.log(e);
+        throw e;
+    }
     URL.revokeObjectURL(url);
     return widget;
 }
 
 function widget_default(base) {
     class AnyModel extends base.DOMWidgetModel {
         static model_name = "AnyModel";
@@ -88,31 +93,31 @@
             });
             this.on("change:_esm", async () => {
                 let id = this.get("_anywidget_id");
                 if (!id)
                     return;
                 console.debug(`[anywidget] esm hot updated: ${id}`);
                 for await (let view of Object.values(this.views ?? {})) {
-                    let widget = await load_esm(this.get("_esm"));
+                    let widget2 = await load_esm(this.get("_esm"));
                     await /** @type {AnyView} */
                     view._anywidget_cached_cleanup();
                     view.$el.empty();
                     view.stopListening(this);
-                    let cleanup = await widget.render(view);
+                    let cleanup = await widget2.render(view);
                     if (cleanup)
                         this._anywidget_cached_cleanup = cleanup;
                 }
             });
         }
     }
     class AnyView extends base.DOMWidgetView {
         async render() {
             await load_css(this.model.get("_css"), this.model.get("_anywidget_id"));
-            let widget = await load_esm(this.model.get("_esm"));
-            let cleanup = await widget.render(this);
+            let widget2 = await load_esm(this.model.get("_esm"));
+            let cleanup = await widget2.render(this);
             if (cleanup)
                 this._anywidget_cached_cleanup = cleanup;
         }
         async _anywidget_cached_cleanup() {}
         async remove() {
             await this._anywidget_cached_cleanup();
             return super.remove();
```

### Comparing `anywidget-0.2.1/docs/README.md` & `anywidget-0.2.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/astro.config.mjs` & `anywidget-0.2.2/docs/astro.config.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/package.json` & `anywidget-0.2.2/docs/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/public/anywidget-overview.png` & `anywidget-0.2.2/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/public/banner-dark.png` & `anywidget-0.2.2/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/public/banner-light.png` & `anywidget-0.2.2/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/public/banner-minimal.png` & `anywidget-0.2.2/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/public/client-js-diagram.png` & `anywidget-0.2.2/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/public/default-og-image.png` & `anywidget-0.2.2/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/public/favicon.svg` & `anywidget-0.2.2/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/public/widget-overview.png` & `anywidget-0.2.2/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/scripts/ipynb.mjs` & `anywidget-0.2.2/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/scripts/utils.mjs` & `anywidget-0.2.2/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/consts.ts` & `anywidget-0.2.2/docs/src/consts.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/CodeHero.astro` & `anywidget-0.2.2/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/CounterButton.astro` & `anywidget-0.2.2/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/HeadCommon.astro` & `anywidget-0.2.2/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/HeadSEO.astro` & `anywidget-0.2.2/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Hero.astro` & `anywidget-0.2.2/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.2.2/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.2.2/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.2.2/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Header/Header.astro` & `anywidget-0.2.2/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Header/HeaderButton.css` & `anywidget-0.2.2/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.2.2/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.2.2/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Header/Search.css` & `anywidget-0.2.2/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Header/Search.tsx` & `anywidget-0.2.2/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.2.2/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.2.2/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.2.2/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.2.2/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.2.2/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.2.2/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.2.2/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.2.2/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/components/examples/Counter.astro` & `anywidget-0.2.2/docs/src/components/examples/Counter.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/layouts/MainLayout.astro` & `anywidget-0.2.2/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/layouts/SplashLayout.astro` & `anywidget-0.2.2/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.2.2/docs/src/pages/blog/anywidget-02.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.2.2/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/pages/en/bundling.md` & `anywidget-0.2.2/docs/src/pages/en/bundling.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/pages/en/getting-started.mdx` & `anywidget-0.2.2/docs/src/pages/en/getting-started.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.2.2/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.2.2/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/styles/index.css` & `anywidget-0.2.2/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/docs/src/styles/theme.css` & `anywidget-0.2.2/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/examples/Counter.ipynb` & `anywidget-0.2.2/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/examples/minimal_example.ipynb` & `anywidget-0.2.2/examples/minimal_example.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/packages/anywidget/build.mjs` & `anywidget-0.2.2/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/packages/anywidget/package.json` & `anywidget-0.2.2/packages/anywidget/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -38,9 +38,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `anywidget-0.2.1/packages/anywidget/src/widget.js` & `anywidget-0.2.2/packages/anywidget/src/widget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -90,15 +90,20 @@
         return import( /* webpackIgnore: true */ esm);
     }
     let url = URL.createObjectURL(
         new Blob([esm], {
             type: "text/javascript"
         }),
     );
-    let widget = await import( /* webpackIgnore: true */ url);
+    try {
+        let widget = await import( /* webpackIgnore: true */ url);
+    } catch (e) {
+        console.log(e);
+        throw e;
+    }
     URL.revokeObjectURL(url);
     return widget;
 }
 
 /** @param {typeof import("@jupyter-widgets/base")} base */
 export default function(base) {
     class AnyModel extends base.DOMWidgetModel {
```

### Comparing `anywidget-0.2.1/tests/test_descriptor.py` & `anywidget-0.2.2/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/tests/test_file_contents.py` & `anywidget-0.2.2/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/tests/test_utils.py` & `anywidget-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/tests/test_widget.py` & `anywidget-0.2.2/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/LICENSE` & `anywidget-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/README.md` & `anywidget-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/pyproject.toml` & `anywidget-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anywidget-0.2.1/PKG-INFO` & `anywidget-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.2.1
+Version: 0.2.2
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
```


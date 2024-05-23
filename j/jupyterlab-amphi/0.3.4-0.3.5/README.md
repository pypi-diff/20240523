# Comparing `tmp/jupyterlab_amphi-0.3.4.tar.gz` & `tmp/jupyterlab_amphi-0.3.5.tar.gz`

## Comparing `jupyterlab_amphi-0.3.4.tar` & `jupyterlab_amphi-0.3.5.tar`

### file list

```diff
@@ -1,153 +1,153 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/.yarnrc.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/MANIFEST.in
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/install.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/lerna.json
--rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/output.json
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/package.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/setup.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/tsconfig.eslint.json
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/tsconfigbase.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/_version.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/package.json
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js
--rw-r--r--   0        0        0    22345 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js.LICENSE.txt
--rw-r--r--   0        0        0  1441949 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/687.e44561a1742c6083cba0.js
--rw-r--r--   0        0        0    35011 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/687.e44561a1742c6083cba0.js.LICENSE.txt
--rw-r--r--   0        0        0   542717 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt
--rw-r--r--   0        0        0   143367 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/792.7de2deb742ba9e036dda.js
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/remoteEntry.1144a177b5daf1c9977c.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/style.js
--rw-r--r--   0        0        0   120113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/third-party-licenses.json
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/package.json
--rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
--rw-r--r--   0        0        0    56966 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/142.acbbd4c680da3a899eb9.js
--rw-r--r--   0        0        0    27269 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js.LICENSE.txt
--rw-r--r--   0        0        0    61091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js
--rw-r--r--   0        0        0  1437675 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/422.27a4f789109562c256e8.js
--rw-r--r--   0        0        0    29737 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/422.27a4f789109562c256e8.js.LICENSE.txt
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js
--rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
--rw-r--r--   0        0        0   150147 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt
--rw-r--r--   0        0        0   439969 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/841.6f47bec498543a801840.js
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/841.6f47bec498543a801840.js.LICENSE.txt
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
--rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/remoteEntry.001fdc1b89863b0cb38e.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/style.js
--rw-r--r--   0        0        0   140477 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/third-party-licenses.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/package.json
--rw-r--r--   0        0        0   152553 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt
--rw-r--r--   0        0        0    33113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/412.23a82146827c21626eae.js
--rw-r--r--   0        0        0    27297 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/631.20cdac1e84cf987a8781.js
--rw-r--r--   0        0        0  1447644 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/735.711b3b299b885104b862.js
--rw-r--r--   0        0        0    36421 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/735.711b3b299b885104b862.js.LICENSE.txt
--rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/remoteEntry.bfb171550404534afb06.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/style.js
--rw-r--r--   0        0        0   118882 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/third-party-licenses.json
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/package.json
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js
--rw-r--r--   0        0        0   751992 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/595.853e8b63deafdcf653a9.js
--rw-r--r--   0        0        0    13950 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/595.853e8b63deafdcf653a9.js.LICENSE.txt
--rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/684.06766aa445a023bc4adf.js
--rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/remoteEntry.871deda2d395cf3ebdb5.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/style.js
--rw-r--r--   0        0        0    64970 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/third-party-licenses.json
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/package.json
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js
--rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/732.1ea6cff032a5ee2821e8.js
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/remoteEntry.9bc842b6cc0c70b4b0c3.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/third-party-licenses.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi_extension/_version.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/install.json
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/tsconfig.json
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
--rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/CodeGenerator.tsx
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/CustomHandle.tsx
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/DndProviderWrapper.tsx
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/PipelineComponent.tsx
--rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/PipelineService.tsx
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/RequestService.tsx
--rw-r--r--   0        0        0    20670 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/configUtils.tsx
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/connectionUtils.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/declarations.d.ts
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/generatorUtils.tsx
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/icons.ts
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/index.ts
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/rendererUtils.tsx
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/InputRegular.tsx
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/connectionSelector.tsx
--rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/dataMapping.tsx
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectColumn.tsx
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectColumns.tsx
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectRegular.tsx
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/transferData.tsx
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/base.css
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/index.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/crosshair-16.svg
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/minus-16.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/play-16.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/play-circle-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/plus-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/plus-24.svg
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/search-16.svg
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/search-24.svg
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/settings-16.svg
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/settings-24.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/trash-16.svg
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/trash-24.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/x-16.svg
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/x-square-16.svg
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/install.json
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/package.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/pipeline-16.svg
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/pipeline-24.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/tailwind.config.js
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/tsconfig.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/schema/extension.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/schema/plugin copy.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/schema/plugin.json
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/Dropzone.tsx
--rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/PipelineEditorWidget.tsx
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/customEdge.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/declarations.d.ts
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/icons.ts
--rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/index.ts
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/canvas.css
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/index.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/index.js
--rw-r--r--   0        0        0    22125 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/output.css
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/pipeline-category-icon.svg
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/react-icon.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/tailwinds_preflight.css
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/api-24.svg
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/file-plus-24.svg
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/file-text-24.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/monitor-24.svg
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/.gitignore
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/README.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/.yarnrc.yml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/MANIFEST.in
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/install.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/lerna.json
+-rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/output.json
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/package.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/tsconfig.eslint.json
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/tsconfigbase.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/_version.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/package.json
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js
+-rw-r--r--   0        0        0    22345 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js.LICENSE.txt
+-rw-r--r--   0        0        0  1442297 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/687.3718223fe5543295ebcd.js
+-rw-r--r--   0        0        0    35011 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/687.3718223fe5543295ebcd.js.LICENSE.txt
+-rw-r--r--   0        0        0   542717 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt
+-rw-r--r--   0        0        0   143367 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/792.7de2deb742ba9e036dda.js
+-rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/remoteEntry.f71216c42efa6af2ddcd.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/style.js
+-rw-r--r--   0        0        0   120113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
+-rw-r--r--   0        0        0    56966 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/142.acbbd4c680da3a899eb9.js
+-rw-r--r--   0        0        0    27269 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js.LICENSE.txt
+-rw-r--r--   0        0        0    61091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js
+-rw-r--r--   0        0        0  1438023 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/422.bbb456b73e63e5a1e7d4.js
+-rw-r--r--   0        0        0    29737 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/422.bbb456b73e63e5a1e7d4.js.LICENSE.txt
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js
+-rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
+-rw-r--r--   0        0        0   150147 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt
+-rw-r--r--   0        0        0   440126 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/841.0203c999f04b4e256cd6.js
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/841.0203c999f04b4e256cd6.js.LICENSE.txt
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/remoteEntry.5ec1e44c8f356f845b6f.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/style.js
+-rw-r--r--   0        0        0   140477 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/package.json
+-rw-r--r--   0        0        0   152553 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt
+-rw-r--r--   0        0        0    33113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/412.23a82146827c21626eae.js
+-rw-r--r--   0        0        0    27297 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/631.20cdac1e84cf987a8781.js
+-rw-r--r--   0        0        0  1447990 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/735.59d5dbc617bf0dc8cc9f.js
+-rw-r--r--   0        0        0    36421 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/735.59d5dbc617bf0dc8cc9f.js.LICENSE.txt
+-rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/remoteEntry.54de67c179f201c5e11a.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/style.js
+-rw-r--r--   0        0        0   118882 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/package.json
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js
+-rw-r--r--   0        0        0   752340 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/595.7fd40f4a8673fc24185a.js
+-rw-r--r--   0        0        0    13950 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/595.7fd40f4a8673fc24185a.js.LICENSE.txt
+-rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/684.06766aa445a023bc4adf.js
+-rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/remoteEntry.432f146e752b80daa98d.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/style.js
+-rw-r--r--   0        0        0    64970 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/package.json
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js
+-rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/732.1ea6cff032a5ee2821e8.js
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/remoteEntry.da6df8ad6b7fdf2715dc.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/third-party-licenses.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi_extension/_version.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/install.json
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/tsconfig.json
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
+-rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/CodeGenerator.tsx
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/CustomHandle.tsx
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/DndProviderWrapper.tsx
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/PipelineComponent.tsx
+-rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/PipelineService.tsx
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/RequestService.tsx
+-rw-r--r--   0        0        0    20670 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/configUtils.tsx
+-rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/connectionUtils.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/declarations.d.ts
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/generatorUtils.tsx
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/icons.ts
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/index.ts
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/rendererUtils.tsx
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/InputRegular.tsx
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/connectionSelector.tsx
+-rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/dataMapping.tsx
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectColumn.tsx
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectColumns.tsx
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectRegular.tsx
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/transferData.tsx
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/base.css
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/index.js
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/crosshair-16.svg
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/minus-16.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/play-16.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/play-circle-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/plus-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/plus-24.svg
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/search-16.svg
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/search-24.svg
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/settings-16.svg
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/settings-24.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/trash-16.svg
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/trash-24.svg
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/x-16.svg
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/x-square-16.svg
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/install.json
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/package.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/pipeline-16.svg
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/pipeline-24.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/tailwind.config.js
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/tsconfig.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/schema/extension.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/schema/plugin copy.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/schema/plugin.json
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/Dropzone.tsx
+-rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/PipelineEditorWidget.tsx
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/customEdge.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/declarations.d.ts
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/icons.ts
+-rw-r--r--   0        0        0    18171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/index.ts
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/canvas.css
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/index.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/index.js
+-rw-r--r--   0        0        0    22125 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/output.css
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/pipeline-category-icon.svg
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/react-icon.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/tailwinds_preflight.css
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/api-24.svg
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/file-plus-24.svg
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/file-text-24.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/monitor-24.svg
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/.gitignore
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/README.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/PKG-INFO
```

### Comparing `jupyterlab_amphi-0.3.4/output.json` & `jupyterlab_amphi-0.3.5/output.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/package.json` & `jupyterlab_amphi-0.3.5/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.3.5'"}*

```diff
@@ -66,15 +66,15 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.yaml}\"",
         "prettier:check": "jlpm prettier:base --check",
         "quickstart": "npm run setup:py && jlpm && jlpm deduplicate && jlpm clean:all && jlpm lint && jlpm build:prod && jlpm dist && jlpm docs && jlpm test",
         "setup:py": "python -m pip install -e \".[dev,lint,test,docs]\"",
         "test": "jlpm test:py",
         "test:py": "pytest"
     },
-    "version": "0.3.4",
+    "version": "0.3.5",
     "workspaces": {
         "packages": [
             "packages/pipeline-editor",
             "packages/pipeline-components-manager",
             "packages/pipeline-components-core",
             "packages/pipeline-console",
             "packages/pipeline-metadata-panel"
```

### Comparing `jupyterlab_amphi-0.3.4/tsconfigbase.json` & `jupyterlab_amphi-0.3.5/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/package.json` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8468079539508111%*

 * *Differences: {"'author'": "{'email': 'tgourdel@amphi.ai'}",*

 * * "'dependencies'": "{'@jupyterlab/apputils': '^4.1.5', '@uiw/react-codemirror': '^4.22.0', "*

 * *                   "'ace-builds': '^1.33.1', 'react-ace': '^11.0.1', 'react-dnd': '^16.0.1', "*

 * *                   "'react-dnd-html5-backend': '^16.0.1', 'react-dom': '^18.2.0', "*

 * *                   "'react-flow-renderer': '^10.3.17', 'react-mentions': '^4.4.10', "*

 * *                   "'react-select': '^5.8.0', 'styled-components': '^6.1.8', delete: "*

 * *                   " […]*

```diff
@@ -1,36 +1,46 @@
 {
     "author": {
-        "email": "",
+        "email": "tgourdel@amphi.ai",
         "name": "Thibaut Gourdel"
     },
     "bugs": {
         "url": "https://github.com/amphi-ai/jupyterlab-amphi/issues"
     },
     "dependencies": {
-        "@amphi/pipeline-components-manager": "file:./../pipeline-components-manager",
         "@jupyterlab/application": "^4.1.5",
+        "@jupyterlab/apputils": "^4.1.5",
         "@lumino/widgets": "^2.0.0",
+        "@uiw/react-codemirror": "^4.22.0",
+        "ace-builds": "^1.33.1",
         "antd": "5.16.4",
-        "reactflow": "11.9.4"
+        "react-ace": "^11.0.1",
+        "react-dnd": "^16.0.1",
+        "react-dnd-html5-backend": "^16.0.1",
+        "react-dom": "^18.2.0",
+        "react-flow-renderer": "^10.3.17",
+        "react-mentions": "^4.4.10",
+        "react-select": "^5.8.0",
+        "styled-components": "^6.1.8"
     },
-    "description": "Amphi Pipeline Core Components",
+    "description": "Amphi Pipeline Components Manager",
     "devDependencies": {
         "@jupyterlab/builder": "^4.1.5",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
+        "antd": "5.16.4",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "reactflow": "11.7.2",
         "rimraf": "^3.0.2",
-        "typescript": "~5.0.4",
+        "typescript": "~5.2.2",
         "yarn-deduplicate": "^6.0.2"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/*.d.ts",
@@ -39,53 +49,59 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1144a177b5daf1c9977c.js",
+            "load": "static/remoteEntry.5ec1e44c8f356f845b6f.js",
             "style": "./style"
         },
         "extension": true,
-        "outputDir": "../../amphi/pipeline-components-core",
+        "outputDir": "../../amphi/pipeline-components-manager",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
-                "bundled": false,
+                "bundle": false,
                 "singleton": true
             }
         }
     },
     "license": "Elastic License 2.0",
     "main": "lib/index.js",
-    "name": "@amphi/pipeline-components-core",
+    "name": "@amphi/pipeline-components-manager",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/amphi-ai/jupyterlab-amphi.git"
     },
+    "resolutions": {
+        "@jupyterlab/rendermime-interfaces": "^3.8.9",
+        "@lumino/widgets": "^2.0.0",
+        "@types/react": "^18.2.7",
+        "antd": "5.16.4"
+    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --build --verbose",
-        "build:prod": "jlpm run build:lib && jlpm run build:labextension",
+        "build:prod": "jlpm run build:lib && jlpm run build:labextension && jlpm install",
         "clean": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf ../../amphi/labextension",
+        "clean:labextension": "rimraf ../../amphi/pipeline-components-manager",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "eslint": "eslint . --ext .ts,.tsx --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.3"
+    "version": "0.3.4"
 }
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/687.e44561a1742c6083cba0.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/687.3718223fe5543295ebcd.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 687.e44561a1742c6083cba0.js.LICENSE.txt */
+/*! For license information please see 687.3718223fe5543295ebcd.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_components_core = self.webpackChunk_amphi_pipeline_components_core || []).push([
     [687], {
         7687: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 Affix: () => Ko,
                 Alert: () => $i,
@@ -14773,28 +14773,30 @@
                         n(e)
                     }), []);
                 return o.cloneElement(t, {
                     ref: r
                 })
             }
             const vm = "object" === ("undefined" == typeof navigator ? "undefined" : (0, p.A)(navigator)) && /Firefox/i.test(navigator.userAgent),
-                bm = function(e, t) {
-                    var n = (0, o.useRef)(!1),
-                        r = (0, o.useRef)(null),
-                        i = (0, o.useRef)({
+                bm = function(e, t, n, r) {
+                    var i = (0, o.useRef)(!1),
+                        a = (0, o.useRef)(null),
+                        l = (0, o.useRef)({
                             top: e,
-                            bottom: t
+                            bottom: t,
+                            left: n,
+                            right: r
                         });
-                    return i.current.top = e, i.current.bottom = t,
-                        function(e) {
-                            var t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1],
-                                o = e < 0 && i.current.top || e > 0 && i.current.bottom;
-                            return t && o ? (clearTimeout(r.current), n.current = !1) : o && !n.current || (clearTimeout(r.current), n.current = !0, r.current = setTimeout((function() {
-                                n.current = !1
-                            }), 50)), !n.current && o
+                    return l.current.top = e, l.current.bottom = t, l.current.left = n, l.current.right = r,
+                        function(e, t) {
+                            var n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2],
+                                o = e ? t < 0 && l.current.left || t > 0 && l.current.right : t < 0 && l.current.top || t > 0 && l.current.bottom;
+                            return n && o ? (clearTimeout(a.current), i.current = !1) : o && !i.current || (clearTimeout(a.current), i.current = !0, a.current = setTimeout((function() {
+                                i.current = !1
+                            }), 50)), !i.current && o
                         }
                 };
             const ym = function() {
                 function e() {
                     X(this, e), (0, Ee.A)(this, "maps", void 0), (0, Ee.A)(this, "id", 0), this.maps = Object.create(null)
                 }
                 return Y(e, [{
@@ -15169,142 +15171,151 @@
                         return Em(we.height, he)
                     }), [we.height, he]),
                     Me = he - c,
                     je = (0, o.useRef)(Me);
                 je.current = Me;
                 var Pe = U <= 0,
                     Re = U >= Me,
-                    ze = bm(Pe, Re),
-                    Te = function() {
+                    ze = ee <= 0,
+                    Te = ee >= $,
+                    He = bm(Pe, Re, ze, Te),
+                    Be = function() {
                         return {
                             x: W ? -ee : ee,
                             y: U
                         }
                     },
-                    He = (0, o.useRef)(Te()),
-                    Be = wn((function(e) {
+                    De = (0, o.useRef)(Be()),
+                    Le = wn((function(e) {
                         if (k) {
-                            var t = (0, d.A)((0, d.A)({}, Te()), e);
-                            He.current.x === t.x && He.current.y === t.y || (k(t), He.current = t)
+                            var t = (0, d.A)((0, d.A)({}, Be()), e);
+                            De.current.x === t.x && De.current.y === t.y || (k(t), De.current = t)
                         }
                     }));
 
-                function De(e, t) {
+                function Fe(e, t) {
                     var n = e;
                     t ? ((0, f.flushSync)((function() {
                         te(n)
-                    })), Be()) : ue(n)
+                    })), Le()) : ue(n)
                 }
-                var Le = function(e) {
+                var We = function(e) {
                         var t = e,
                             n = $ ? $ - we.width : 0;
                         return t = Math.max(t, 0), Math.min(t, n)
                     },
-                    Fe = wn((function(e, t) {
+                    _e = wn((function(e, t) {
                         t ? ((0, f.flushSync)((function() {
                             te((function(t) {
-                                return Le(t + (W ? -e : e))
+                                return We(t + (W ? -e : e))
                             }))
-                        })), Be()) : ue((function(t) {
+                        })), Le()) : ue((function(t) {
                             return t + e
                         }))
                     })),
-                    We = function(e, t, n, r, i) {
-                        var a = (0, o.useRef)(0),
-                            l = (0, o.useRef)(null),
-                            c = (0, o.useRef)(null),
-                            s = (0, o.useRef)(!1),
-                            u = bm(t, n),
-                            d = (0, o.useRef)(null),
-                            p = (0, o.useRef)(null);
+                    Ve = function(e, t, n, r, i, a, l) {
+                        var c = (0, o.useRef)(0),
+                            s = (0, o.useRef)(null),
+                            u = (0, o.useRef)(null),
+                            d = (0, o.useRef)(!1),
+                            p = bm(t, n, r, i),
+                            f = (0, o.useRef)(null),
+                            m = (0, o.useRef)(null);
                         return [function(t) {
                             if (e) {
-                                Ce.cancel(p.current), p.current = Ce((function() {
-                                    d.current = null
+                                Ce.cancel(m.current), m.current = Ce((function() {
+                                    f.current = null
                                 }), 2);
                                 var n = t.deltaX,
                                     o = t.deltaY,
-                                    f = t.shiftKey,
-                                    m = n,
+                                    r = t.shiftKey,
+                                    i = n,
                                     g = o;
-                                ("sx" === d.current || !d.current && f && o && !n) && (m = o, g = 0, d.current = "sx");
-                                var h = Math.abs(m),
+                                ("sx" === f.current || !f.current && r && o && !n) && (i = o, g = 0, f.current = "sx");
+                                var h = Math.abs(i),
                                     v = Math.abs(g);
-                                null === d.current && (d.current = r && h > v ? "x" : "y"), "y" === d.current ? function(e, t) {
-                                    Ce.cancel(l.current), a.current += t, c.current = t, u(t) || (vm || e.preventDefault(), l.current = Ce((function() {
-                                        var e = s.current ? 10 : 1;
-                                        i(a.current * e), a.current = 0
+                                null === f.current && (f.current = a && h > v ? "x" : "y"), "y" === f.current ? function(e, t) {
+                                    Ce.cancel(s.current), c.current += t, u.current = t, p(!1, t) || (vm || e.preventDefault(), s.current = Ce((function() {
+                                        var e = d.current ? 10 : 1;
+                                        l(c.current * e), c.current = 0
                                     })))
                                 }(t, g) : function(e, t) {
-                                    i(t, !0), vm || e.preventDefault()
-                                }(t, m)
+                                    l(t, !0), vm || e.preventDefault()
+                                }(t, i)
                             }
                         }, function(t) {
-                            e && (s.current = t.detail === c.current)
+                            e && (d.current = t.detail === u.current)
                         }]
-                    }(D, Pe, Re, !!$, Fe),
-                    _e = (0, ke.A)(We, 2),
-                    Ve = _e[0],
-                    Ke = _e[1];
+                    }(D, Pe, Re, ze, Te, !!$, _e),
+                    Ke = (0, ke.A)(Ve, 2),
+                    Xe = Ke[0],
+                    qe = Ke[1];
                 ! function(e, t, n) {
                     var r, i = (0, o.useRef)(!1),
                         a = (0, o.useRef)(0),
-                        l = (0, o.useRef)(null),
+                        l = (0, o.useRef)(0),
                         c = (0, o.useRef)(null),
-                        s = function(e) {
+                        s = (0, o.useRef)(null),
+                        u = function(e) {
                             if (i.current) {
-                                var t = Math.ceil(e.touches[0].pageY),
-                                    o = a.current - t;
-                                a.current = t, n(o) && e.preventDefault(), clearInterval(c.current), c.current = setInterval((function() {
-                                    (!n(o *= Cm, !0) || Math.abs(o) <= .1) && clearInterval(c.current)
+                                var t = Math.ceil(e.touches[0].pageX),
+                                    o = Math.ceil(e.touches[0].pageY),
+                                    r = a.current - t,
+                                    c = l.current - o,
+                                    u = Math.abs(r) > Math.abs(c);
+                                u ? a.current = t : l.current = o, n(u, u ? r : c) && e.preventDefault(), clearInterval(s.current), s.current = setInterval((function() {
+                                    u ? r *= Cm : c *= Cm;
+                                    var e = Math.floor(u ? r : c);
+                                    (!n(u, e, !0) || Math.abs(e) <= .1) && clearInterval(s.current)
                                 }), 16)
                             }
                         },
-                        u = function() {
+                        d = function() {
                             i.current = !1, r()
                         },
-                        d = function(e) {
-                            r(), 1 !== e.touches.length || i.current || (i.current = !0, a.current = Math.ceil(e.touches[0].pageY), l.current = e.target, l.current.addEventListener("touchmove", s), l.current.addEventListener("touchend", u))
+                        p = function(e) {
+                            r(), 1 !== e.touches.length || i.current || (i.current = !0, a.current = Math.ceil(e.touches[0].pageX), l.current = Math.ceil(e.touches[0].pageY), c.current = e.target, c.current.addEventListener("touchmove", u), c.current.addEventListener("touchend", d))
                         };
                     r = function() {
-                        l.current && (l.current.removeEventListener("touchmove", s), l.current.removeEventListener("touchend", u))
+                        c.current && (c.current.removeEventListener("touchmove", u), c.current.removeEventListener("touchend", d))
                     }, it((function() {
-                        return e && t.current.addEventListener("touchstart", d),
+                        return e && t.current.addEventListener("touchstart", p),
                             function() {
                                 var e;
-                                null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", d), r(), clearInterval(c.current)
+                                null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", p), r(), clearInterval(s.current)
                             }
                     }), [e])
-                }(D, K, (function(e, t) {
-                    return !ze(e, t) && (Ve({
+                }(D, K, (function(e, t, n) {
+                    return !He(e, t, n) && (Xe({
                         preventDefault: function() {},
-                        deltaY: e
+                        deltaX: e ? t : 0,
+                        deltaY: e ? 0 : t
                     }), !0)
                 })), it((function() {
                     function e(e) {
                         D && e.preventDefault()
                     }
                     var t = K.current;
-                    return t.addEventListener("wheel", Ve), t.addEventListener("DOMMouseScroll", Ke), t.addEventListener("MozMousePixelScroll", e),
+                    return t.addEventListener("wheel", Xe), t.addEventListener("DOMMouseScroll", qe), t.addEventListener("MozMousePixelScroll", e),
                         function() {
-                            t.removeEventListener("wheel", Ve), t.removeEventListener("DOMMouseScroll", Ke), t.removeEventListener("MozMousePixelScroll", e)
+                            t.removeEventListener("wheel", Xe), t.removeEventListener("DOMMouseScroll", qe), t.removeEventListener("MozMousePixelScroll", e)
                         }
                 }), [D]), it((function() {
                     if ($) {
-                        var e = Le(ee);
-                        te(e), Be({
+                        var e = We(ee);
+                        te(e), Le({
                             x: e
                         })
                     }
                 }), [we.width, $]);
-                var Xe = function() {
+                var Ge = function() {
                         var e, t;
                         null === (e = Oe.current) || void 0 === e || e.delayHidden(), null === (t = Ae.current) || void 0 === t || t.delayHidden()
                     },
-                    qe = function(e, t, n, r, i, a, l, c) {
+                    Ye = function(e, t, n, r, i, a, l, c) {
                         var s = o.useRef(),
                             u = o.useState(null),
                             f = (0, ke.A)(u, 2),
                             m = f[0],
                             g = f[1];
                         return it((function() {
                                 if (m && m.times < 10) {
@@ -15372,31 +15383,31 @@
                                             originAlign: o
                                         })
                                     }
                                 } else c()
                             }
                     }(K, V, H, s, j, (function() {
                         return T(!0)
-                    }), ue, Xe);
+                    }), ue, Ge);
                 o.useImperativeHandle(t, (function() {
                     return {
                         nativeElement: q.current,
-                        getScrollInfo: Te,
+                        getScrollInfo: Be,
                         scrollTo: function(e) {
                             var t;
-                            (t = e) && "object" === (0, p.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && te(Le(e.left)), qe(e.top)) : qe(e)
+                            (t = e) && "object" === (0, p.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && te(We(e.left)), Ye(e.top)) : Ye(e)
                         }
                     }
                 })), it((function() {
                     if (O) {
                         var e = V.slice(ve, be + 1);
                         O(e, V)
                     }
                 }), [ve, be, V]);
-                var Ge = function(e, t, n, r) {
+                var Ue = function(e, t, n, r) {
                         var i = o.useMemo((function() {
                                 return [new Map, []]
                             }), [e, n.id, r]),
                             a = (0, ke.A)(i, 2),
                             l = a[0],
                             c = a[1];
                         return function(o) {
@@ -15413,24 +15424,24 @@
                                 }
                             return {
                                 top: c[a - 1] || 0,
                                 bottom: c[s]
                             }
                         }
                     }(V, j, H, s),
-                    Ye = null == I ? void 0 : I({
+                    Qe = null == I ? void 0 : I({
                         start: ve,
                         end: be,
                         virtual: F,
                         offsetX: ee,
                         offsetY: ye,
                         rtl: W,
-                        getSize: Ge
+                        getSize: Ue
                     }),
-                    Ue = function(e, t, n, r, i, a, l, c) {
+                    Ze = function(e, t, n, r, i, a, l, c) {
                         var s = c.getKey;
                         return e.slice(t, n + 1).map((function(e, n) {
                             var c = l(e, t + n, {
                                     style: {
                                         width: r
                                     },
                                     offsetX: i
@@ -15440,70 +15451,70 @@
                                 key: u,
                                 setRef: function(t) {
                                     return a(e, t)
                                 }
                             }, c)
                         }))
                     }(V, ve, be, $, ee, z, b, se),
-                    Qe = null;
-                c && (Qe = (0, d.A)((0, Ee.A)({}, m ? "height" : "maxHeight", c), Am), D && (Qe.overflowY = "hidden", $ && (Qe.overflowX = "hidden"), re && (Qe.pointerEvents = "none")));
-                var Ze = {};
-                return W && (Ze.dir = "rtl"), o.createElement("div", (0, l.A)({
+                    Je = null;
+                c && (Je = (0, d.A)((0, Ee.A)({}, m ? "height" : "maxHeight", c), Am), D && (Je.overflowY = "hidden", $ && (Je.overflowX = "hidden"), re && (Je.pointerEvents = "none")));
+                var et = {};
+                return W && (et.dir = "rtl"), o.createElement("div", (0, l.A)({
                     ref: q,
                     style: (0, d.A)((0, d.A)({}, g), {}, {
                         position: "relative"
                     }),
                     className: _
-                }, Ze, M), o.createElement(ce, {
+                }, et, M), o.createElement(ce, {
                     onResize: function(e) {
                         Se({
                             width: e.width || e.offsetWidth,
                             height: e.height || e.offsetHeight
                         })
                     }
                 }, o.createElement(S, {
                     className: "".concat(r, "-holder"),
-                    style: Qe,
+                    style: Je,
                     ref: K,
                     onScroll: function(e) {
                         var t = e.currentTarget.scrollTop;
-                        t !== U && ue(t), null == E || E(e), Be()
+                        t !== U && ue(t), null == E || E(e), Le()
                     },
-                    onMouseEnter: Xe
+                    onMouseEnter: Ge
                 }, o.createElement(gm, {
                     prefixCls: r,
                     height: he,
                     offsetX: ee,
                     offsetY: ye,
                     scrollWidth: $,
                     onInnerResize: T,
                     ref: X,
                     innerProps: A,
                     rtl: W,
-                    extra: Ye
-                }, Ue))), F && he > c && o.createElement(wm, {
+                    extra: Qe
+                }, Ze))), F && he > c && o.createElement(wm, {
                     ref: Oe,
                     prefixCls: r,
                     scrollOffset: U,
                     scrollRange: he,
                     rtl: W,
-                    onScroll: De,
+                    onScroll: Fe,
                     onStartMove: ae,
                     onStopMove: le,
                     spinSize: Ne,
                     containerSize: we.height,
                     style: null == N ? void 0 : N.verticalScrollBar,
                     thumbStyle: null == N ? void 0 : N.verticalScrollBarThumb
                 }), F && $ > we.width && o.createElement(wm, {
                     ref: Ae,
                     prefixCls: r,
                     scrollOffset: ee,
                     scrollRange: $,
                     rtl: W,
-                    onScroll: De,
+                    onScroll: Fe,
                     onStartMove: ae,
                     onStopMove: le,
                     spinSize: Ie,
                     containerSize: we.width,
                     horizontal: !0,
                     style: null == N ? void 0 : N.horizontalScrollBar,
                     thumbStyle: null == N ? void 0 : N.horizontalScrollBarThumb
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/687.e44561a1742c6083cba0.js.LICENSE.txt` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/687.3718223fe5543295ebcd.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/792.7de2deb742ba9e036dda.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/792.7de2deb742ba9e036dda.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/remoteEntry.1144a177b5daf1c9977c.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/remoteEntry.f71216c42efa6af2ddcd.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, u, s, c, p, f, d, h, b, v, m, g, y, w = {
+    var e, r, t, n, o, a, i, l, u, s, f, p, c, d, h, v, m, b, g, y, w = {
             2212: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(518), t.e(345), t.e(792)]).then((() => () => t(5792))),
                         "./extension": () => Promise.all([t.e(518), t.e(345), t.e(792)]).then((() => () => t(5792))),
                         "./style": () => t.e(432).then((() => () => t(1432)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -47,23 +47,23 @@
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         345: "d33854e26caa385d0f56",
         432: "0fc640989ce2150a2305",
         518: "f70a8c5cdb51fc55b510",
         628: "6bee9242bd295a15f79b",
-        687: "e44561a1742c6083cba0",
+        687: "3718223fe5543295ebcd",
         713: "986c30f40fc55619b937",
         792: "7de2deb742ba9e036dda"
     } [e] + ".js?v=" + {
         345: "d33854e26caa385d0f56",
         432: "0fc640989ce2150a2305",
         518: "f70a8c5cdb51fc55b510",
         628: "6bee9242bd295a15f79b",
-        687: "e44561a1742c6083cba0",
+        687: "3718223fe5543295ebcd",
         713: "986c30f40fc55619b937",
         792: "7de2deb742ba9e036dda"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -71,27 +71,27 @@
         }
     }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-components-core:", S.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
             if (void 0 !== o)
                 for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
-                    var c = u[s];
-                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + o) {
-                        i = c;
+                    var f = u[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var p = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(f);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                f = setTimeout(p.bind(null, void 0, {
+                c = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -117,15 +117,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@amphi/pipeline-components-core", "0.3.3", (() => Promise.all([S.e(518), S.e(345), S.e(792)]).then((() => () => S(5792))))), l("antd", "5.16.4", (() => Promise.all([S.e(687), S.e(518), S.e(628), S.e(345)]).then((() => () => S(7687))))), l("reactflow", "11.7.2", (() => Promise.all([S.e(713), S.e(628), S.e(345)]).then((() => () => S(5713)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@amphi/pipeline-components-core", "0.3.4", (() => Promise.all([S.e(518), S.e(345), S.e(792)]).then((() => () => S(5792))))), l("antd", "5.16.4", (() => Promise.all([S.e(687), S.e(518), S.e(628), S.e(345)]).then((() => () => S(7687))))), l("reactflow", "11.7.2", (() => Promise.all([S.e(713), S.e(628), S.e(345)]).then((() => () => S(5713)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -175,92 +175,92 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var s, c, p = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (c = (typeof(s = r[i]))[0])) return !u || ("u" == p ? l > n && !o : "" == p != o);
-                if ("u" == c) {
+                var s, f, p = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !u || ("u" == p ? l > n && !o : "" == p != o);
+                if ("u" == f) {
                     if (!u || "u" != p) return !1
                 } else if (u)
-                    if (p == c)
+                    if (p == f)
                         if (l <= n) {
                             if (s != e[l]) return !1
                         } else {
                             if (o ? s > e[l] : s < e[l]) return !1;
                             s != e[l] && (u = !1)
                         }
                 else if ("s" != p && "n" != p) {
                     if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || c < p != o) return !1;
+                    if (l <= n || f < p != o) return !1;
                     u = !1
                 } else "s" != p && "n" != p && (u = !1, l--)
             }
         }
-        var f = [],
-            d = f.pop.bind(f);
+        var c = [],
+            d = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            f.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? a(h, r) : !d())
+            c.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? a(h, r) : !d())
         }
         return !!d()
     }, i = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || p(u(e, t, o, n)), f(e[t][o])
-    }, c = (e, r, t) => {
+        return a(n, o) || p(u(e, t, o, n)), c(e[t][o])
+    }, f = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, f = e => (e.loaded = 1, e.get()), h = (d = e => function(r, t, n, o) {
+    }, c = e => (e.loaded = 1, e.get()), h = (d = e => function(r, t, n, o) {
         var a = S.I(r);
         return a && a.then ? a.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), b = d(((e, r, t, n, o) => {
-        var a = r && S.o(r, t) && c(r, t, n);
-        return a ? f(a) : o()
-    })), v = {}, m = {
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = d(((e, r, t, n, o) => {
+        var a = r && S.o(r, t) && f(r, t, n);
+        return a ? c(a) : o()
+    })), m = {}, b = {
         3345: () => h("default", "react", [1, 18, 2, 0]),
         1527: () => h("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
-        2473: () => b("default", "reactflow", [4, 11, 9, 4], (() => Promise.all([S.e(713), S.e(628)]).then((() => () => S(5713))))),
+        2473: () => v("default", "reactflow", [4, 11, 9, 4], (() => Promise.all([S.e(713), S.e(628)]).then((() => () => S(5713))))),
         3254: () => h("default", "@amphi/pipeline-components-manager", [0]),
-        4810: () => b("default", "antd", [4, 5, 16, 4], (() => Promise.all([S.e(687), S.e(628)]).then((() => () => S(7687))))),
+        4810: () => v("default", "antd", [4, 5, 16, 4], (() => Promise.all([S.e(687), S.e(628)]).then((() => () => S(7687))))),
         7628: () => h("default", "react-dom", [1, 18, 2, 0])
     }, g = {
         345: [3345],
         628: [7628],
         792: [1527, 2473, 3254, 4810]
     }, y = {}, S.f.consumes = (e, r) => {
         S.o(g, e) && g[e].forEach((e => {
-            if (S.o(v, e)) return r.push(v[e]);
+            if (S.o(m, e)) return r.push(m[e]);
             if (!y[e]) {
                 var t = r => {
-                    v[e] = 0, S.m[e] = t => {
+                    m[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
                 };
                 y[e] = !0;
                 var n = r => {
-                    delete v[e], S.m[e] = t => {
+                    delete m[e], S.m[e] = t => {
                         throw delete S.c[e], r
                     }
                 };
                 try {
-                    var o = m[e]();
-                    o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
+                    var o = b[e]();
+                    o.then ? r.push(m[e] = o.then(t).catch(n)) : t(o)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         var e = {
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-core/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992897727272727%*

 * *Differences: {"'packages'": "{75: {'versionInfo': '3.14.2'}}"}*

```diff
@@ -450,15 +450,15 @@
             "name": "rc-util",
             "versionInfo": "5.41.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-virtual-list",
-            "versionInfo": "3.14.0"
+            "versionInfo": "3.14.2"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react",
             "versionInfo": "18.3.1"
         },
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702380952380952%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.3.5'"}*

```diff
@@ -47,19 +47,14 @@
         "lib/*.js.map",
         "lib/*.js",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.001fdc1b89863b0cb38e.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-manager",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundle": false,
                 "singleton": true
             }
@@ -99,9 +94,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.3"
+    "version": "0.3.5"
 }
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/142.acbbd4c680da3a899eb9.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/142.acbbd4c680da3a899eb9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/422.27a4f789109562c256e8.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/422.bbb456b73e63e5a1e7d4.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 422.27a4f789109562c256e8.js.LICENSE.txt */
+/*! For license information please see 422.bbb456b73e63e5a1e7d4.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_components_manager = self.webpackChunk_amphi_pipeline_components_manager || []).push([
     [422], {
         5422: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 Affix: () => Ko,
                 Alert: () => Ci,
@@ -14747,28 +14747,30 @@
                         n(e)
                     }), []);
                 return o.cloneElement(t, {
                     ref: r
                 })
             }
             const gm = "object" === ("undefined" == typeof navigator ? "undefined" : (0, p.A)(navigator)) && /Firefox/i.test(navigator.userAgent),
-                hm = function(e, t) {
-                    var n = (0, o.useRef)(!1),
-                        r = (0, o.useRef)(null),
-                        i = (0, o.useRef)({
+                hm = function(e, t, n, r) {
+                    var i = (0, o.useRef)(!1),
+                        a = (0, o.useRef)(null),
+                        l = (0, o.useRef)({
                             top: e,
-                            bottom: t
+                            bottom: t,
+                            left: n,
+                            right: r
                         });
-                    return i.current.top = e, i.current.bottom = t,
-                        function(e) {
-                            var t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1],
-                                o = e < 0 && i.current.top || e > 0 && i.current.bottom;
-                            return t && o ? (clearTimeout(r.current), n.current = !1) : o && !n.current || (clearTimeout(r.current), n.current = !0, r.current = setTimeout((function() {
-                                n.current = !1
-                            }), 50)), !n.current && o
+                    return l.current.top = e, l.current.bottom = t, l.current.left = n, l.current.right = r,
+                        function(e, t) {
+                            var n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2],
+                                o = e ? t < 0 && l.current.left || t > 0 && l.current.right : t < 0 && l.current.top || t > 0 && l.current.bottom;
+                            return n && o ? (clearTimeout(a.current), i.current = !1) : o && !i.current || (clearTimeout(a.current), i.current = !0, a.current = setTimeout((function() {
+                                i.current = !1
+                            }), 50)), !i.current && o
                         }
                 };
             const vm = function() {
                 function e() {
                     X(this, e), (0, Ee.A)(this, "maps", void 0), (0, Ee.A)(this, "id", 0), this.maps = Object.create(null)
                 }
                 return Y(e, [{
@@ -15143,142 +15145,151 @@
                         return wm(we.height, he)
                     }), [we.height, he]),
                     Me = he - c,
                     je = (0, o.useRef)(Me);
                 je.current = Me;
                 var Pe = U <= 0,
                     Re = U >= Me,
-                    Te = hm(Pe, Re),
-                    ze = function() {
+                    Te = ee <= 0,
+                    ze = ee >= $,
+                    He = hm(Pe, Re, Te, ze),
+                    Be = function() {
                         return {
                             x: W ? -ee : ee,
                             y: U
                         }
                     },
-                    He = (0, o.useRef)(ze()),
-                    Be = wn((function(e) {
+                    De = (0, o.useRef)(Be()),
+                    Le = wn((function(e) {
                         if (k) {
-                            var t = (0, d.A)((0, d.A)({}, ze()), e);
-                            He.current.x === t.x && He.current.y === t.y || (k(t), He.current = t)
+                            var t = (0, d.A)((0, d.A)({}, Be()), e);
+                            De.current.x === t.x && De.current.y === t.y || (k(t), De.current = t)
                         }
                     }));
 
-                function De(e, t) {
+                function Fe(e, t) {
                     var n = e;
                     t ? ((0, f.flushSync)((function() {
                         te(n)
-                    })), Be()) : ue(n)
+                    })), Le()) : ue(n)
                 }
-                var Le = function(e) {
+                var We = function(e) {
                         var t = e,
                             n = $ ? $ - we.width : 0;
                         return t = Math.max(t, 0), Math.min(t, n)
                     },
-                    Fe = wn((function(e, t) {
+                    _e = wn((function(e, t) {
                         t ? ((0, f.flushSync)((function() {
                             te((function(t) {
-                                return Le(t + (W ? -e : e))
+                                return We(t + (W ? -e : e))
                             }))
-                        })), Be()) : ue((function(t) {
+                        })), Le()) : ue((function(t) {
                             return t + e
                         }))
                     })),
-                    We = function(e, t, n, r, i) {
-                        var a = (0, o.useRef)(0),
-                            l = (0, o.useRef)(null),
-                            c = (0, o.useRef)(null),
-                            s = (0, o.useRef)(!1),
-                            u = hm(t, n),
-                            d = (0, o.useRef)(null),
-                            p = (0, o.useRef)(null);
+                    Ve = function(e, t, n, r, i, a, l) {
+                        var c = (0, o.useRef)(0),
+                            s = (0, o.useRef)(null),
+                            u = (0, o.useRef)(null),
+                            d = (0, o.useRef)(!1),
+                            p = hm(t, n, r, i),
+                            f = (0, o.useRef)(null),
+                            m = (0, o.useRef)(null);
                         return [function(t) {
                             if (e) {
-                                Ce.cancel(p.current), p.current = Ce((function() {
-                                    d.current = null
+                                Ce.cancel(m.current), m.current = Ce((function() {
+                                    f.current = null
                                 }), 2);
                                 var n = t.deltaX,
                                     o = t.deltaY,
-                                    f = t.shiftKey,
-                                    m = n,
+                                    r = t.shiftKey,
+                                    i = n,
                                     g = o;
-                                ("sx" === d.current || !d.current && f && o && !n) && (m = o, g = 0, d.current = "sx");
-                                var h = Math.abs(m),
+                                ("sx" === f.current || !f.current && r && o && !n) && (i = o, g = 0, f.current = "sx");
+                                var h = Math.abs(i),
                                     v = Math.abs(g);
-                                null === d.current && (d.current = r && h > v ? "x" : "y"), "y" === d.current ? function(e, t) {
-                                    Ce.cancel(l.current), a.current += t, c.current = t, u(t) || (gm || e.preventDefault(), l.current = Ce((function() {
-                                        var e = s.current ? 10 : 1;
-                                        i(a.current * e), a.current = 0
+                                null === f.current && (f.current = a && h > v ? "x" : "y"), "y" === f.current ? function(e, t) {
+                                    Ce.cancel(s.current), c.current += t, u.current = t, p(!1, t) || (gm || e.preventDefault(), s.current = Ce((function() {
+                                        var e = d.current ? 10 : 1;
+                                        l(c.current * e), c.current = 0
                                     })))
                                 }(t, g) : function(e, t) {
-                                    i(t, !0), gm || e.preventDefault()
-                                }(t, m)
+                                    l(t, !0), gm || e.preventDefault()
+                                }(t, i)
                             }
                         }, function(t) {
-                            e && (s.current = t.detail === c.current)
+                            e && (d.current = t.detail === u.current)
                         }]
-                    }(D, Pe, Re, !!$, Fe),
-                    _e = (0, ke.A)(We, 2),
-                    Ve = _e[0],
-                    Ke = _e[1];
+                    }(D, Pe, Re, Te, ze, !!$, _e),
+                    Ke = (0, ke.A)(Ve, 2),
+                    Xe = Ke[0],
+                    qe = Ke[1];
                 ! function(e, t, n) {
                     var r, i = (0, o.useRef)(!1),
                         a = (0, o.useRef)(0),
-                        l = (0, o.useRef)(null),
+                        l = (0, o.useRef)(0),
                         c = (0, o.useRef)(null),
-                        s = function(e) {
+                        s = (0, o.useRef)(null),
+                        u = function(e) {
                             if (i.current) {
-                                var t = Math.ceil(e.touches[0].pageY),
-                                    o = a.current - t;
-                                a.current = t, n(o) && e.preventDefault(), clearInterval(c.current), c.current = setInterval((function() {
-                                    (!n(o *= bm, !0) || Math.abs(o) <= .1) && clearInterval(c.current)
+                                var t = Math.ceil(e.touches[0].pageX),
+                                    o = Math.ceil(e.touches[0].pageY),
+                                    r = a.current - t,
+                                    c = l.current - o,
+                                    u = Math.abs(r) > Math.abs(c);
+                                u ? a.current = t : l.current = o, n(u, u ? r : c) && e.preventDefault(), clearInterval(s.current), s.current = setInterval((function() {
+                                    u ? r *= bm : c *= bm;
+                                    var e = Math.floor(u ? r : c);
+                                    (!n(u, e, !0) || Math.abs(e) <= .1) && clearInterval(s.current)
                                 }), 16)
                             }
                         },
-                        u = function() {
+                        d = function() {
                             i.current = !1, r()
                         },
-                        d = function(e) {
-                            r(), 1 !== e.touches.length || i.current || (i.current = !0, a.current = Math.ceil(e.touches[0].pageY), l.current = e.target, l.current.addEventListener("touchmove", s), l.current.addEventListener("touchend", u))
+                        p = function(e) {
+                            r(), 1 !== e.touches.length || i.current || (i.current = !0, a.current = Math.ceil(e.touches[0].pageX), l.current = Math.ceil(e.touches[0].pageY), c.current = e.target, c.current.addEventListener("touchmove", u), c.current.addEventListener("touchend", d))
                         };
                     r = function() {
-                        l.current && (l.current.removeEventListener("touchmove", s), l.current.removeEventListener("touchend", u))
+                        c.current && (c.current.removeEventListener("touchmove", u), c.current.removeEventListener("touchend", d))
                     }, it((function() {
-                        return e && t.current.addEventListener("touchstart", d),
+                        return e && t.current.addEventListener("touchstart", p),
                             function() {
                                 var e;
-                                null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", d), r(), clearInterval(c.current)
+                                null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", p), r(), clearInterval(s.current)
                             }
                     }), [e])
-                }(D, K, (function(e, t) {
-                    return !Te(e, t) && (Ve({
+                }(D, K, (function(e, t, n) {
+                    return !He(e, t, n) && (Xe({
                         preventDefault: function() {},
-                        deltaY: e
+                        deltaX: e ? t : 0,
+                        deltaY: e ? 0 : t
                     }), !0)
                 })), it((function() {
                     function e(e) {
                         D && e.preventDefault()
                     }
                     var t = K.current;
-                    return t.addEventListener("wheel", Ve), t.addEventListener("DOMMouseScroll", Ke), t.addEventListener("MozMousePixelScroll", e),
+                    return t.addEventListener("wheel", Xe), t.addEventListener("DOMMouseScroll", qe), t.addEventListener("MozMousePixelScroll", e),
                         function() {
-                            t.removeEventListener("wheel", Ve), t.removeEventListener("DOMMouseScroll", Ke), t.removeEventListener("MozMousePixelScroll", e)
+                            t.removeEventListener("wheel", Xe), t.removeEventListener("DOMMouseScroll", qe), t.removeEventListener("MozMousePixelScroll", e)
                         }
                 }), [D]), it((function() {
                     if ($) {
-                        var e = Le(ee);
-                        te(e), Be({
+                        var e = We(ee);
+                        te(e), Le({
                             x: e
                         })
                     }
                 }), [we.width, $]);
-                var Xe = function() {
+                var Ge = function() {
                         var e, t;
                         null === (e = Oe.current) || void 0 === e || e.delayHidden(), null === (t = Ae.current) || void 0 === t || t.delayHidden()
                     },
-                    qe = function(e, t, n, r, i, a, l, c) {
+                    Ye = function(e, t, n, r, i, a, l, c) {
                         var s = o.useRef(),
                             u = o.useState(null),
                             f = (0, ke.A)(u, 2),
                             m = f[0],
                             g = f[1];
                         return it((function() {
                                 if (m && m.times < 10) {
@@ -15346,31 +15357,31 @@
                                             originAlign: o
                                         })
                                     }
                                 } else c()
                             }
                     }(K, V, H, s, j, (function() {
                         return z(!0)
-                    }), ue, Xe);
+                    }), ue, Ge);
                 o.useImperativeHandle(t, (function() {
                     return {
                         nativeElement: q.current,
-                        getScrollInfo: ze,
+                        getScrollInfo: Be,
                         scrollTo: function(e) {
                             var t;
-                            (t = e) && "object" === (0, p.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && te(Le(e.left)), qe(e.top)) : qe(e)
+                            (t = e) && "object" === (0, p.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && te(We(e.left)), Ye(e.top)) : Ye(e)
                         }
                     }
                 })), it((function() {
                     if (O) {
                         var e = V.slice(ve, be + 1);
                         O(e, V)
                     }
                 }), [ve, be, V]);
-                var Ge = function(e, t, n, r) {
+                var Ue = function(e, t, n, r) {
                         var i = o.useMemo((function() {
                                 return [new Map, []]
                             }), [e, n.id, r]),
                             a = (0, ke.A)(i, 2),
                             l = a[0],
                             c = a[1];
                         return function(o) {
@@ -15387,24 +15398,24 @@
                                 }
                             return {
                                 top: c[a - 1] || 0,
                                 bottom: c[s]
                             }
                         }
                     }(V, j, H, s),
-                    Ye = null == I ? void 0 : I({
+                    Qe = null == I ? void 0 : I({
                         start: ve,
                         end: be,
                         virtual: F,
                         offsetX: ee,
                         offsetY: ye,
                         rtl: W,
-                        getSize: Ge
+                        getSize: Ue
                     }),
-                    Ue = function(e, t, n, r, i, a, l, c) {
+                    Ze = function(e, t, n, r, i, a, l, c) {
                         var s = c.getKey;
                         return e.slice(t, n + 1).map((function(e, n) {
                             var c = l(e, t + n, {
                                     style: {
                                         width: r
                                     },
                                     offsetX: i
@@ -15414,70 +15425,70 @@
                                 key: u,
                                 setRef: function(t) {
                                     return a(e, t)
                                 }
                             }, c)
                         }))
                     }(V, ve, be, $, ee, T, b, se),
-                    Qe = null;
-                c && (Qe = (0, d.A)((0, Ee.A)({}, m ? "height" : "maxHeight", c), km), D && (Qe.overflowY = "hidden", $ && (Qe.overflowX = "hidden"), re && (Qe.pointerEvents = "none")));
-                var Ze = {};
-                return W && (Ze.dir = "rtl"), o.createElement("div", (0, l.A)({
+                    Je = null;
+                c && (Je = (0, d.A)((0, Ee.A)({}, m ? "height" : "maxHeight", c), km), D && (Je.overflowY = "hidden", $ && (Je.overflowX = "hidden"), re && (Je.pointerEvents = "none")));
+                var et = {};
+                return W && (et.dir = "rtl"), o.createElement("div", (0, l.A)({
                     ref: q,
                     style: (0, d.A)((0, d.A)({}, g), {}, {
                         position: "relative"
                     }),
                     className: _
-                }, Ze, M), o.createElement(ce, {
+                }, et, M), o.createElement(ce, {
                     onResize: function(e) {
                         Se({
                             width: e.width || e.offsetWidth,
                             height: e.height || e.offsetHeight
                         })
                     }
                 }, o.createElement(S, {
                     className: "".concat(r, "-holder"),
-                    style: Qe,
+                    style: Je,
                     ref: K,
                     onScroll: function(e) {
                         var t = e.currentTarget.scrollTop;
-                        t !== U && ue(t), null == E || E(e), Be()
+                        t !== U && ue(t), null == E || E(e), Le()
                     },
-                    onMouseEnter: Xe
+                    onMouseEnter: Ge
                 }, o.createElement(fm, {
                     prefixCls: r,
                     height: he,
                     offsetX: ee,
                     offsetY: ye,
                     scrollWidth: $,
                     onInnerResize: z,
                     ref: X,
                     innerProps: A,
                     rtl: W,
-                    extra: Ye
-                }, Ue))), F && he > c && o.createElement(xm, {
+                    extra: Qe
+                }, Ze))), F && he > c && o.createElement(xm, {
                     ref: Oe,
                     prefixCls: r,
                     scrollOffset: U,
                     scrollRange: he,
                     rtl: W,
-                    onScroll: De,
+                    onScroll: Fe,
                     onStartMove: ae,
                     onStopMove: le,
                     spinSize: Ne,
                     containerSize: we.height,
                     style: null == N ? void 0 : N.verticalScrollBar,
                     thumbStyle: null == N ? void 0 : N.verticalScrollBarThumb
                 }), F && $ > we.width && o.createElement(xm, {
                     ref: Ae,
                     prefixCls: r,
                     scrollOffset: ee,
                     scrollRange: $,
                     rtl: W,
-                    onScroll: De,
+                    onScroll: Fe,
                     onStartMove: ae,
                     onStopMove: le,
                     spinSize: Ie,
                     containerSize: we.width,
                     horizontal: !0,
                     style: null == N ? void 0 : N.horizontalScrollBar,
                     thumbStyle: null == N ? void 0 : N.horizontalScrollBarThumb
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/422.27a4f789109562c256e8.js.LICENSE.txt` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/422.bbb456b73e63e5a1e7d4.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/841.6f47bec498543a801840.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/841.0203c999f04b4e256cd6.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 841.6f47bec498543a801840.js.LICENSE.txt */
+/*! For license information please see 841.0203c999f04b4e256cd6.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_components_manager = self.webpackChunk_amphi_pipeline_components_manager || []).push([
     [841], {
         1841: (e, t, n) => {
             e = n.nmd(e),
                 function() {
                     var e = function() {
                         return this
@@ -665,15 +665,15 @@
                         if ("function" == typeof n.require) return n.require(e)
                     }, t.setModuleLoader = function(e, n) {
                         t.dynamicModules[e] = n
                     };
                     var c = function() {
                         l.basePath || l.workerPath || l.modePath || l.themePath || Object.keys(l.$moduleUrls).length || (console.error("Unable to infer path to ace from script src,", "use ace.config.set('basePath', 'path') to enable dynamic loading of modes and themes", "or with webpack use ace/webpack-resolver"), c = function() {})
                     };
-                    t.version = "1.33.3"
+                    t.version = "1.34.0"
                 })), ace.define("ace/loader_build", ["require", "exports", "module", "ace/lib/fixoldbrowsers", "ace/config"], (function(e, t, i) {
                     "use strict";
                     e("./lib/fixoldbrowsers");
                     var o = e("./config");
                     o.setLoader((function(t, n) {
                         e([t], (function(e) {
                             n(null, e)
@@ -1139,16 +1139,17 @@
                         try {
                             var _ = document.activeElement === n
                         } catch (e) {}
                         this.setNumberOfExtraLines = function(e) {
                             R = Number.MAX_SAFE_INTEGER, T = Number.MIN_SAFE_INTEGER, E = e < 0 ? 0 : e
                         }, this.setAriaOptions = function(e) {
                             if (e.activeDescendant ? (n.setAttribute("aria-haspopup", "true"), n.setAttribute("aria-autocomplete", e.inline ? "both" : "list"), n.setAttribute("aria-activedescendant", e.activeDescendant)) : (n.setAttribute("aria-haspopup", "false"), n.setAttribute("aria-autocomplete", "both"), n.removeAttribute("aria-activedescendant")), e.role && n.setAttribute("role", e.role), e.setLabel && (n.setAttribute("aria-roledescription", r("text-input.aria-roledescription", "editor")), t.session)) {
-                                var i = t.session.selection.cursor.row;
-                                n.setAttribute("aria-label", r("text-input.aria-label", "Cursor at row $0", [i + 1]))
+                                var i = t.session.selection.cursor.row,
+                                    o = "";
+                                t.$textInputAriaLabel && (o += "".concat(t.$textInputAriaLabel, ", ")), o += r("text-input.aria-label", "Cursor at row $0", [i + 1]), n.setAttribute("aria-label", o)
                             }
                         }, this.setAriaOptions({
                             role: "textbox"
                         }), o.addListener(n, "blur", (function(e) {
                             x || (t.onBlur(e), _ = !1)
                         }), t), o.addListener(n, "focus", (function(e) {
                             if (!x) {
@@ -8745,14 +8746,20 @@
                                             this.isRowVisible(t) || this.scrollToLine(t, !0, !0), this.focus()
                                         }
                                     };
                                 e ? (this.renderer.enableKeyboardAccessibility = !0, this.renderer.keyboardFocusClassName = "ace_keyboard-focus", this.textInput.getElement().setAttribute("tabindex", -1), this.textInput.setNumberOfExtraLines(a.isWin ? 3 : 0), this.renderer.scroller.setAttribute("tabindex", 0), this.renderer.scroller.setAttribute("role", "group"), this.renderer.scroller.setAttribute("aria-roledescription", C("editor.scroller.aria-roledescription", "editor")), this.renderer.scroller.classList.add(this.renderer.keyboardFocusClassName), this.renderer.scroller.setAttribute("aria-label", C("editor.scroller.aria-label", "Editor content, press Enter to start editing, press Escape to exit")), this.renderer.scroller.addEventListener("keyup", i.bind(this)), this.commands.addCommand(n), this.renderer.$gutter.setAttribute("tabindex", 0), this.renderer.$gutter.setAttribute("aria-hidden", !1), this.renderer.$gutter.setAttribute("role", "group"), this.renderer.$gutter.setAttribute("aria-roledescription", C("editor.gutter.aria-roledescription", "editor")), this.renderer.$gutter.setAttribute("aria-label", C("editor.gutter.aria-label", "Editor gutter, press Enter to interact with controls using arrow keys, press Escape to exit")), this.renderer.$gutter.classList.add(this.renderer.keyboardFocusClassName), this.renderer.content.setAttribute("aria-hidden", !0), t || (t = new $(this)), t.addListener()) : (this.renderer.enableKeyboardAccessibility = !1, this.textInput.getElement().setAttribute("tabindex", 0), this.textInput.setNumberOfExtraLines(0), this.renderer.scroller.setAttribute("tabindex", -1), this.renderer.scroller.removeAttribute("role"), this.renderer.scroller.removeAttribute("aria-roledescription"), this.renderer.scroller.classList.remove(this.renderer.keyboardFocusClassName), this.renderer.scroller.removeAttribute("aria-label"), this.renderer.scroller.removeEventListener("keyup", i.bind(this)), this.commands.removeCommand(n), this.renderer.content.removeAttribute("aria-hidden"), this.renderer.$gutter.setAttribute("tabindex", -1), this.renderer.$gutter.setAttribute("aria-hidden", !0), this.renderer.$gutter.removeAttribute("role"), this.renderer.$gutter.removeAttribute("aria-roledescription"), this.renderer.$gutter.removeAttribute("aria-label"), this.renderer.$gutter.classList.remove(this.renderer.keyboardFocusClassName), t && t.removeListener())
                             },
                             initialValue: !1
                         },
+                        textInputAriaLabel: {
+                            set: function(e) {
+                                this.$textInputAriaLabel = e
+                            },
+                            initialValue: ""
+                        },
                         customScrollbar: "renderer",
                         hScrollBarAlwaysVisible: "renderer",
                         vScrollBarAlwaysVisible: "renderer",
                         highlightGutterLine: "renderer",
                         animatedScroll: "renderer",
                         showInvisibles: "renderer",
                         showPrintMargin: "renderer",
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/remoteEntry.001fdc1b89863b0cb38e.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/remoteEntry.5ec1e44c8f356f845b6f.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -53,34 +53,34 @@
         12: "e1b4412a18535c560cd1",
         85: "227e3aea03a3014cd80a",
         142: "acbbd4c680da3a899eb9",
         173: "254dd13d95daff6ca4b4",
         186: "e77a90422af9cbab4e47",
         271: "3095f6e27a6de7c0174d",
         345: "39215b57fd3910de833c",
-        422: "27a4f789109562c256e8",
+        422: "bbb456b73e63e5a1e7d4",
         432: "1d493bea1143efe37c80",
         454: "b60aaa09eed0e7e4a124",
         628: "f8b00c70c263432a40ab",
         725: "90ddd44d4e0f0fae78c2",
-        841: "6f47bec498543a801840"
+        841: "0203c999f04b4e256cd6"
     } [e] + ".js?v=" + {
         12: "e1b4412a18535c560cd1",
         85: "227e3aea03a3014cd80a",
         142: "acbbd4c680da3a899eb9",
         173: "254dd13d95daff6ca4b4",
         186: "e77a90422af9cbab4e47",
         271: "3095f6e27a6de7c0174d",
         345: "39215b57fd3910de833c",
-        422: "27a4f789109562c256e8",
+        422: "bbb456b73e63e5a1e7d4",
         432: "1d493bea1143efe37c80",
         454: "b60aaa09eed0e7e4a124",
         628: "f8b00c70c263432a40ab",
         725: "90ddd44d4e0f0fae78c2",
-        841: "6f47bec498543a801840"
+        841: "0203c999f04b4e256cd6"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -132,15 +132,15 @@
                         (!d || !d.loaded && (!a != !d.eager ? a : i > d.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (d("@amphi/pipeline-components-manager", "0.3.3", (() => Promise.all([S.e(173), S.e(725), S.e(345), S.e(628), S.e(142)]).then((() => () => S(8142))))), d("ace-builds", "1.33.3", (() => S.e(841).then((() => () => S(1841))))), d("antd", "5.16.4", (() => Promise.all([S.e(422), S.e(173), S.e(345), S.e(628)]).then((() => () => S(5422))))), d("react-ace", "11.0.1", (() => Promise.all([S.e(271), S.e(345), S.e(186)]).then((() => () => S(6271))))), d("react-dnd-html5-backend", "16.0.1", (() => S.e(454).then((() => () => S(6454))))), d("react-dnd", "16.0.1", (() => Promise.all([S.e(12), S.e(345), S.e(85)]).then((() => () => S(4631)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@amphi/pipeline-components-manager", "0.3.4", (() => Promise.all([S.e(173), S.e(725), S.e(345), S.e(628), S.e(142)]).then((() => () => S(8142))))), d("ace-builds", "1.34.0", (() => S.e(841).then((() => () => S(1841))))), d("antd", "5.16.4", (() => Promise.all([S.e(422), S.e(173), S.e(345), S.e(628)]).then((() => () => S(5422))))), d("react-ace", "11.0.1", (() => Promise.all([S.e(271), S.e(345), S.e(186)]).then((() => () => S(6271))))), d("react-dnd-html5-backend", "16.0.1", (() => S.e(454).then((() => () => S(6454))))), d("react-dnd", "16.0.1", (() => Promise.all([S.e(12), S.e(345), S.e(85)]).then((() => () => S(4631)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-components-manager/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986979166666667%*

 * *Differences: {"'packages'": "{20: {'versionInfo': '1.34.0'}, 80: {'versionInfo': '3.14.2'}}"}*

```diff
@@ -120,15 +120,15 @@
             "name": "@reactflow/core",
             "versionInfo": "11.7.2"
         },
         {
             "extractedText": "Copyright (c) 2010, Ajax.org B.V.\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n    * Redistributions of source code must retain the above copyright\n      notice, this list of conditions and the following disclaimer.\n    * Redistributions in binary form must reproduce the above copyright\n      notice, this list of conditions and the following disclaimer in the\n      documentation and/or other materials provided with the distribution.\n    * Neither the name of Ajax.org B.V. nor the\n      names of its contributors may be used to endorse or promote products\n      derived from this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\" AND\nANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED\nWARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL AJAX.ORG B.V. BE LIABLE FOR ANY\nDIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES\n(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;\nLOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND\nON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT\n(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS\nSOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "ace-builds",
-            "versionInfo": "1.33.3"
+            "versionInfo": "1.34.0"
         },
         {
             "extractedText": "MIT LICENSE\n\nCopyright (c) 2015-present Ant UED, https://xtech.antfin.com/\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "antd",
             "versionInfo": "5.16.4"
         },
@@ -480,15 +480,15 @@
             "name": "rc-util",
             "versionInfo": "5.41.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-virtual-list",
-            "versionInfo": "3.14.0"
+            "versionInfo": "3.14.2"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react",
             "versionInfo": "18.3.1"
         },
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/package.json` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702380952380952%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.3.5'"}*

```diff
@@ -45,19 +45,14 @@
         "lib/*.js.map",
         "lib/*.js",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.bfb171550404534afb06.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "../../amphi/pipeline-editor",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
                 "singleton": true
             },
@@ -103,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.3"
+    "version": "0.3.5"
 }
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt` & `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/412.23a82146827c21626eae.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/412.23a82146827c21626eae.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/735.711b3b299b885104b862.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/735.59d5dbc617bf0dc8cc9f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 735.711b3b299b885104b862.js.LICENSE.txt */
+/*! For license information please see 735.59d5dbc617bf0dc8cc9f.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_editor = self.webpackChunk_amphi_pipeline_editor || []).push([
     [735], {
         1735: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 Affix: () => Wr,
                 Alert: () => Ta,
@@ -15600,28 +15600,30 @@
                         n(e)
                     }), []);
                 return o.cloneElement(t, {
                     ref: r
                 })
             }
             const kg = "object" === ("undefined" == typeof navigator ? "undefined" : b(navigator)) && /Firefox/i.test(navigator.userAgent),
-                Og = function(e, t) {
-                    var n = (0, o.useRef)(!1),
-                        r = (0, o.useRef)(null),
-                        i = (0, o.useRef)({
+                Og = function(e, t, n, r) {
+                    var i = (0, o.useRef)(!1),
+                        a = (0, o.useRef)(null),
+                        l = (0, o.useRef)({
                             top: e,
-                            bottom: t
+                            bottom: t,
+                            left: n,
+                            right: r
                         });
-                    return i.current.top = e, i.current.bottom = t,
-                        function(e) {
-                            var t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1],
-                                o = e < 0 && i.current.top || e > 0 && i.current.bottom;
-                            return t && o ? (clearTimeout(r.current), n.current = !1) : o && !n.current || (clearTimeout(r.current), n.current = !0, r.current = setTimeout((function() {
-                                n.current = !1
-                            }), 50)), !n.current && o
+                    return l.current.top = e, l.current.bottom = t, l.current.left = n, l.current.right = r,
+                        function(e, t) {
+                            var n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2],
+                                o = e ? t < 0 && l.current.left || t > 0 && l.current.right : t < 0 && l.current.top || t > 0 && l.current.bottom;
+                            return n && o ? (clearTimeout(a.current), i.current = !1) : o && !i.current || (clearTimeout(a.current), i.current = !0, a.current = setTimeout((function() {
+                                i.current = !1
+                            }), 50)), !i.current && o
                         }
                 };
             const Ig = function() {
                 function e() {
                     ne(this, e), C(this, "maps", void 0), C(this, "id", 0), this.maps = Object.create(null)
                 }
                 return re(e, [{
@@ -15984,141 +15986,150 @@
                         return Tg(be.height, fe)
                     }), [be.height, fe]),
                     Se = fe - c,
                     Ee = (0, o.useRef)(Se);
                 Ee.current = Se;
                 var ke = U <= 0,
                     Oe = U >= Se,
-                    Ie = Og(ke, Oe),
-                    Me = function() {
+                    Ie = J <= 0,
+                    Me = J >= y,
+                    je = Og(ke, Oe, Ie, Me),
+                    Pe = function() {
                         return {
                             x: _ ? -J : J,
                             y: U
                         }
                     },
-                    je = (0, o.useRef)(Me()),
-                    Pe = Vn((function(e) {
+                    Re = (0, o.useRef)(Pe()),
+                    Te = Vn((function(e) {
                         if (O) {
-                            var t = $($({}, Me()), e);
-                            je.current.x === t.x && je.current.y === t.y || (O(t), je.current = t)
+                            var t = $($({}, Pe()), e);
+                            Re.current.x === t.x && Re.current.y === t.y || (O(t), Re.current = t)
                         }
                     }));
 
-                function Re(e, t) {
+                function ze(e, t) {
                     var n = e;
                     t ? ((0, w.flushSync)((function() {
                         ee(n)
-                    })), Pe()) : le(n)
+                    })), Te()) : le(n)
                 }
-                var Te = function(e) {
+                var Be = function(e) {
                         var t = e,
                             n = y ? y - be.width : 0;
                         return t = Math.max(t, 0), Math.min(t, n)
                     },
-                    ze = Vn((function(e, t) {
+                    De = Vn((function(e, t) {
                         t ? ((0, w.flushSync)((function() {
                             ee((function(t) {
-                                return Te(t + (_ ? -e : e))
+                                return Be(t + (_ ? -e : e))
                             }))
-                        })), Pe()) : le((function(t) {
+                        })), Te()) : le((function(t) {
                             return t + e
                         }))
                     })),
-                    Be = He(function(e, t, n, r, i) {
-                        var a = (0, o.useRef)(0),
-                            l = (0, o.useRef)(null),
-                            c = (0, o.useRef)(null),
-                            s = (0, o.useRef)(!1),
-                            u = Og(t, n),
-                            d = (0, o.useRef)(null),
-                            f = (0, o.useRef)(null);
+                    Le = He(function(e, t, n, r, i, a, l) {
+                        var c = (0, o.useRef)(0),
+                            s = (0, o.useRef)(null),
+                            u = (0, o.useRef)(null),
+                            d = (0, o.useRef)(!1),
+                            f = Og(t, n, r, i),
+                            p = (0, o.useRef)(null),
+                            m = (0, o.useRef)(null);
                         return [function(t) {
                             if (e) {
-                                Ne.cancel(f.current), f.current = Ne((function() {
-                                    d.current = null
+                                Ne.cancel(m.current), m.current = Ne((function() {
+                                    p.current = null
                                 }), 2);
                                 var n = t.deltaX,
                                     o = t.deltaY,
-                                    p = t.shiftKey,
-                                    m = n,
+                                    r = t.shiftKey,
+                                    i = n,
                                     g = o;
-                                ("sx" === d.current || !d.current && p && o && !n) && (m = o, g = 0, d.current = "sx");
-                                var h = Math.abs(m),
+                                ("sx" === p.current || !p.current && r && o && !n) && (i = o, g = 0, p.current = "sx");
+                                var h = Math.abs(i),
                                     v = Math.abs(g);
-                                null === d.current && (d.current = r && h > v ? "x" : "y"), "y" === d.current ? function(e, t) {
-                                    Ne.cancel(l.current), a.current += t, c.current = t, u(t) || (kg || e.preventDefault(), l.current = Ne((function() {
-                                        var e = s.current ? 10 : 1;
-                                        i(a.current * e), a.current = 0
+                                null === p.current && (p.current = a && h > v ? "x" : "y"), "y" === p.current ? function(e, t) {
+                                    Ne.cancel(s.current), c.current += t, u.current = t, f(!1, t) || (kg || e.preventDefault(), s.current = Ne((function() {
+                                        var e = d.current ? 10 : 1;
+                                        l(c.current * e), c.current = 0
                                     })))
                                 }(t, g) : function(e, t) {
-                                    i(t, !0), kg || e.preventDefault()
-                                }(t, m)
+                                    l(t, !0), kg || e.preventDefault()
+                                }(t, i)
                             }
                         }, function(t) {
-                            e && (s.current = t.detail === c.current)
+                            e && (d.current = t.detail === u.current)
                         }]
-                    }(A, ke, Oe, !!y, ze), 2),
-                    De = Be[0],
-                    Le = Be[1];
+                    }(A, ke, Oe, Ie, Me, !!y, De), 2),
+                    Ae = Le[0],
+                    Fe = Le[1];
                 ! function(e, t, n) {
                     var r, i = (0, o.useRef)(!1),
                         a = (0, o.useRef)(0),
-                        l = (0, o.useRef)(null),
+                        l = (0, o.useRef)(0),
                         c = (0, o.useRef)(null),
-                        s = function(e) {
+                        s = (0, o.useRef)(null),
+                        u = function(e) {
                             if (i.current) {
-                                var t = Math.ceil(e.touches[0].pageY),
-                                    o = a.current - t;
-                                a.current = t, n(o) && e.preventDefault(), clearInterval(c.current), c.current = setInterval((function() {
-                                    (!n(o *= Ng, !0) || Math.abs(o) <= .1) && clearInterval(c.current)
+                                var t = Math.ceil(e.touches[0].pageX),
+                                    o = Math.ceil(e.touches[0].pageY),
+                                    r = a.current - t,
+                                    c = l.current - o,
+                                    u = Math.abs(r) > Math.abs(c);
+                                u ? a.current = t : l.current = o, n(u, u ? r : c) && e.preventDefault(), clearInterval(s.current), s.current = setInterval((function() {
+                                    u ? r *= Ng : c *= Ng;
+                                    var e = Math.floor(u ? r : c);
+                                    (!n(u, e, !0) || Math.abs(e) <= .1) && clearInterval(s.current)
                                 }), 16)
                             }
                         },
-                        u = function() {
+                        d = function() {
                             i.current = !1, r()
                         },
-                        d = function(e) {
-                            r(), 1 !== e.touches.length || i.current || (i.current = !0, a.current = Math.ceil(e.touches[0].pageY), l.current = e.target, l.current.addEventListener("touchmove", s), l.current.addEventListener("touchend", u))
+                        f = function(e) {
+                            r(), 1 !== e.touches.length || i.current || (i.current = !0, a.current = Math.ceil(e.touches[0].pageX), l.current = Math.ceil(e.touches[0].pageY), c.current = e.target, c.current.addEventListener("touchmove", u), c.current.addEventListener("touchend", d))
                         };
                     r = function() {
-                        l.current && (l.current.removeEventListener("touchmove", s), l.current.removeEventListener("touchend", u))
+                        c.current && (c.current.removeEventListener("touchmove", u), c.current.removeEventListener("touchend", d))
                     }, kt((function() {
-                        return e && t.current.addEventListener("touchstart", d),
+                        return e && t.current.addEventListener("touchstart", f),
                             function() {
                                 var e;
-                                null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", d), r(), clearInterval(c.current)
+                                null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", f), r(), clearInterval(s.current)
                             }
                     }), [e])
-                }(A, q, (function(e, t) {
-                    return !Ie(e, t) && (De({
+                }(A, q, (function(e, t, n) {
+                    return !je(e, t, n) && (Ae({
                         preventDefault: function() {},
-                        deltaY: e
+                        deltaX: e ? t : 0,
+                        deltaY: e ? 0 : t
                     }), !0)
                 })), kt((function() {
                     function e(e) {
                         A && e.preventDefault()
                     }
                     var t = q.current;
-                    return t.addEventListener("wheel", De), t.addEventListener("DOMMouseScroll", Le), t.addEventListener("MozMousePixelScroll", e),
+                    return t.addEventListener("wheel", Ae), t.addEventListener("DOMMouseScroll", Fe), t.addEventListener("MozMousePixelScroll", e),
                         function() {
-                            t.removeEventListener("wheel", De), t.removeEventListener("DOMMouseScroll", Le), t.removeEventListener("MozMousePixelScroll", e)
+                            t.removeEventListener("wheel", Ae), t.removeEventListener("DOMMouseScroll", Fe), t.removeEventListener("MozMousePixelScroll", e)
                         }
                 }), [A]), kt((function() {
                     if (y) {
-                        var e = Te(J);
-                        ee(e), Pe({
+                        var e = Be(J);
+                        ee(e), Te({
                             x: e
                         })
                     }
                 }), [be.width, y]);
-                var Ae = function() {
+                var We = function() {
                         var e, t;
                         null === (e = Ce.current) || void 0 === e || e.delayHidden(), null === (t = xe.current) || void 0 === t || t.delayHidden()
                     },
-                    Fe = function(e, t, n, r, i, a, l, c) {
+                    _e = function(e, t, n, r, i, a, l, c) {
                         var s = o.useRef(),
                             u = He(o.useState(null), 2),
                             d = u[0],
                             f = u[1];
                         return kt((function() {
                                 if (d && d.times < 10) {
                                     if (!e.current) return void f((function(e) {
@@ -16185,31 +16196,31 @@
                                             originAlign: o
                                         })
                                     }
                                 } else c()
                             }
                     }(q, K, D, s, R, (function() {
                         return B(!0)
-                    }), le, Ae);
+                    }), le, We);
                 o.useImperativeHandle(t, (function() {
                     return {
                         nativeElement: G.current,
-                        getScrollInfo: Me,
+                        getScrollInfo: Pe,
                         scrollTo: function(e) {
                             var t;
-                            (t = e) && "object" === b(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && ee(Te(e.left)), Fe(e.top)) : Fe(e)
+                            (t = e) && "object" === b(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && ee(Be(e.left)), _e(e.top)) : _e(e)
                         }
                     }
                 })), kt((function() {
                     if (I) {
                         var e = K.slice(pe, me + 1);
                         I(e, K)
                     }
                 }), [pe, me, K]);
-                var We = function(e, t, n, r) {
+                var Ve = function(e, t, n, r) {
                         var i = He(o.useMemo((function() {
                                 return [new Map, []]
                             }), [e, n.id, r]), 2),
                             a = i[0],
                             l = i[1];
                         return function(o) {
                             var i = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : o,
@@ -16225,24 +16236,24 @@
                                 }
                             return {
                                 top: l[c - 1] || 0,
                                 bottom: l[s]
                             }
                         }
                     }(K, R, D, s),
-                    _e = null == M ? void 0 : M({
+                    Ke = null == M ? void 0 : M({
                         start: pe,
                         end: me,
                         virtual: W,
                         offsetX: J,
                         offsetY: ge,
                         rtl: _,
-                        getSize: We
+                        getSize: Ve
                     }),
-                    Ve = function(e, t, n, r, i, a, l, c) {
+                    qe = function(e, t, n, r, i, a, l, c) {
                         var s = c.getKey;
                         return e.slice(t, n + 1).map((function(e, n) {
                             var c = l(e, t + n, {
                                     style: {
                                         width: r
                                     },
                                     offsetX: i
@@ -16252,70 +16263,70 @@
                                 key: u,
                                 setRef: function(t) {
                                     return a(e, t)
                                 }
                             }, c)
                         }))
                     }(K, pe, me, y, J, H, m, ae),
-                    Ke = null;
-                c && (Ke = $(C({}, d ? "height" : "maxHeight", c), Bg), A && (Ke.overflowY = "hidden", y && (Ke.overflowX = "hidden"), ne && (Ke.pointerEvents = "none")));
-                var qe = {};
-                return _ && (qe.dir = "rtl"), o.createElement("div", l({
+                    Xe = null;
+                c && (Xe = $(C({}, d ? "height" : "maxHeight", c), Bg), A && (Xe.overflowY = "hidden", y && (Xe.overflowX = "hidden"), ne && (Xe.pointerEvents = "none")));
+                var Ge = {};
+                return _ && (Ge.dir = "rtl"), o.createElement("div", l({
                     ref: G,
                     style: $($({}, f), {}, {
                         position: "relative"
                     }),
                     className: V
-                }, qe, P), o.createElement(ve, {
+                }, Ge, P), o.createElement(ve, {
                     onResize: function(e) {
                         ye({
                             width: e.width || e.offsetWidth,
                             height: e.height || e.offsetHeight
                         })
                     }
                 }, o.createElement(S, {
                     className: "".concat(r, "-holder"),
-                    style: Ke,
+                    style: Xe,
                     ref: q,
                     onScroll: function(e) {
                         var t = e.currentTarget.scrollTop;
-                        t !== U && le(t), null == E || E(e), Pe()
+                        t !== U && le(t), null == E || E(e), Te()
                     },
-                    onMouseEnter: Ae
+                    onMouseEnter: We
                 }, o.createElement(Sg, {
                     prefixCls: r,
                     height: fe,
                     offsetX: J,
                     offsetY: ge,
                     scrollWidth: y,
                     onInnerResize: B,
                     ref: X,
                     innerProps: N,
                     rtl: _,
-                    extra: _e
-                }, Ve))), W && fe > c && o.createElement(Pg, {
+                    extra: Ke
+                }, qe))), W && fe > c && o.createElement(Pg, {
                     ref: Ce,
                     prefixCls: r,
                     scrollOffset: U,
                     scrollRange: fe,
                     rtl: _,
-                    onScroll: Re,
+                    onScroll: ze,
                     onStartMove: re,
                     onStopMove: ie,
                     spinSize: we,
                     containerSize: be.height,
                     style: null == j ? void 0 : j.verticalScrollBar,
                     thumbStyle: null == j ? void 0 : j.verticalScrollBarThumb
                 }), W && y > be.width && o.createElement(Pg, {
                     ref: xe,
                     prefixCls: r,
                     scrollOffset: J,
                     scrollRange: y,
                     rtl: _,
-                    onScroll: Re,
+                    onScroll: ze,
                     onStartMove: re,
                     onStopMove: ie,
                     spinSize: $e,
                     containerSize: be.width,
                     horizontal: !0,
                     style: null == j ? void 0 : j.horizontalScrollBar,
                     thumbStyle: null == j ? void 0 : j.horizontalScrollBarThumb
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/735.711b3b299b885104b862.js.LICENSE.txt` & `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/735.59d5dbc617bf0dc8cc9f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/remoteEntry.bfb171550404534afb06.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/remoteEntry.54de67c179f201c5e11a.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -49,23 +49,23 @@
     }, _.f = {}, _.e = e => Promise.all(Object.keys(_.f).reduce(((r, t) => (_.f[t](e, r), r)), [])), _.u = e => e + "." + {
         285: "f1fef15430d9554bfba0",
         345: "4aa5390d29af88207b53",
         412: "23a82146827c21626eae",
         550: "025783cb8476390cbadc",
         628: "d05f56a756fb73f1c255",
         631: "20cdac1e84cf987a8781",
-        735: "711b3b299b885104b862"
+        735: "59d5dbc617bf0dc8cc9f"
     } [e] + ".js?v=" + {
         285: "f1fef15430d9554bfba0",
         345: "4aa5390d29af88207b53",
         412: "23a82146827c21626eae",
         550: "025783cb8476390cbadc",
         628: "d05f56a756fb73f1c255",
         631: "20cdac1e84cf987a8781",
-        735: "711b3b299b885104b862"
+        735: "59d5dbc617bf0dc8cc9f"
     } [e], _.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -117,15 +117,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@amphi/pipeline-editor", "0.3.3", (() => Promise.all([_.e(345), _.e(550), _.e(412)]).then((() => () => _(8412))))), l("antd", "5.16.4", (() => Promise.all([_.e(735), _.e(628), _.e(345)]).then((() => () => _(1735))))), l("reactflow", "11.9.4", (() => Promise.all([_.e(285), _.e(628), _.e(345)]).then((() => () => _(1285)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@amphi/pipeline-editor", "0.3.4", (() => Promise.all([_.e(345), _.e(550), _.e(412)]).then((() => () => _(8412))))), l("antd", "5.16.4", (() => Promise.all([_.e(735), _.e(628), _.e(345)]).then((() => () => _(1735))))), l("reactflow", "11.9.4", (() => Promise.all([_.e(285), _.e(628), _.e(345)]).then((() => () => _(1285)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         _.g.importScripts && (e = _.g.location + "");
         var r = _.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-editor/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992816091954023%*

 * *Differences: {"'packages'": "{75: {'versionInfo': '3.14.2'}}"}*

```diff
@@ -450,15 +450,15 @@
             "name": "rc-util",
             "versionInfo": "5.41.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-virtual-list",
-            "versionInfo": "3.14.0"
+            "versionInfo": "3.14.2"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react-is",
             "versionInfo": "18.3.1"
         },
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/package.json` & `jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8727182539682539%*

 * *Differences: {"'description'": "'Amphi Metadata Panel'",*

 * * "'devDependencies'": "{'reactflow': '11.7.2', delete: ['@types/react-dom', 'react']}",*

 * * "'jupyterlab'": "{'outputDir': '../../amphi/pipeline-metadata-panel', '_build': {'load': "*

 * *                 "'static/remoteEntry.da6df8ad6b7fdf2715dc.js'}}",*

 * * "'name'": "'@amphi/pipeline-metadata-panel'",*

 * * "'version'": "'0.3.4'",*

 * * 'delete': "['resolutions']"}*

```diff
@@ -21,27 +21,26 @@
         "@lumino/datagrid": "^2.0.0",
         "@lumino/disposable": "^2.0.0",
         "@lumino/signaling": "^2.0.0",
         "@lumino/widgets": "^2.0.0",
         "react": "^18.2.0",
         "wildcard-match": "^5.1.2"
     },
-    "description": "Amphi Pipeline Log Console",
+    "description": "Amphi Metadata Panel",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
-        "@types/react-dom": "^18.2.25",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
-        "react": "^18.2.0",
+        "reactflow": "11.7.2",
         "rimraf": "^3.0.2",
         "typescript": "~5.0.4",
         "yarn-deduplicate": "^6.0.2"
     },
     "directories": {
         "lib": "lib/"
     },
@@ -52,39 +51,36 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.871deda2d395cf3ebdb5.js",
+            "load": "static/remoteEntry.da6df8ad6b7fdf2715dc.js",
             "style": "./style"
         },
         "extension": true,
-        "outputDir": "../../amphi/pipeline-log-console",
+        "outputDir": "../../amphi/pipeline-metadata-panel",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
                 "singleton": true
             }
         }
     },
     "license": "Elastic License 2.0",
     "main": "lib/index.js",
-    "name": "@amphi/pipeline-log-console",
+    "name": "@amphi/pipeline-metadata-panel",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/amphi-ai/jupyterlab-amphi.git"
     },
-    "resolutions": {
-        "@amphi/pipeline-editor": "file:./../pipeline-editor"
-    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --build --verbose",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib && jlpm run clean:labextension",
@@ -99,9 +95,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.3"
+    "version": "0.3.4"
 }
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/595.853e8b63deafdcf653a9.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/595.7fd40f4a8673fc24185a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 595.853e8b63deafdcf653a9.js.LICENSE.txt */
+/*! For license information please see 595.7fd40f4a8673fc24185a.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_log_console = self.webpackChunk_amphi_pipeline_log_console || []).push([
     [595], {
         588: (e, t, n) => {
             "use strict";
             n.d(t, {
                 z1: () => C,
                 cM: () => b,
@@ -11444,28 +11444,30 @@
                         n(e)
                     }), []);
                 return r.cloneElement(t, {
                     ref: o
                 })
             }
             const Xe = "object" === ("undefined" == typeof navigator ? "undefined" : (0, S.A)(navigator)) && /Firefox/i.test(navigator.userAgent),
-                Ge = function(e, t) {
-                    var n = (0, r.useRef)(!1),
-                        o = (0, r.useRef)(null),
-                        i = (0, r.useRef)({
+                Ge = function(e, t, n, o) {
+                    var i = (0, r.useRef)(!1),
+                        a = (0, r.useRef)(null),
+                        l = (0, r.useRef)({
                             top: e,
-                            bottom: t
+                            bottom: t,
+                            left: n,
+                            right: o
                         });
-                    return i.current.top = e, i.current.bottom = t,
-                        function(e) {
-                            var t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1],
-                                r = e < 0 && i.current.top || e > 0 && i.current.bottom;
-                            return t && r ? (clearTimeout(o.current), n.current = !1) : r && !n.current || (clearTimeout(o.current), n.current = !0, o.current = setTimeout((function() {
-                                n.current = !1
-                            }), 50)), !n.current && r
+                    return l.current.top = e, l.current.bottom = t, l.current.left = n, l.current.right = o,
+                        function(e, t) {
+                            var n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2],
+                                r = e ? t < 0 && l.current.left || t > 0 && l.current.right : t < 0 && l.current.top || t > 0 && l.current.bottom;
+                            return n && r ? (clearTimeout(a.current), i.current = !1) : r && !i.current || (clearTimeout(a.current), i.current = !0, a.current = setTimeout((function() {
+                                i.current = !1
+                            }), 50)), !i.current && r
                         }
                 };
             var Ue = n(8299),
                 Ye = n(5139),
                 Qe = n(4743);
             const Ze = function() {
                 function e() {
@@ -11843,142 +11845,151 @@
                         return ot(ke.height, xe)
                     }), [ke.height, xe]),
                     Pe = xe - a,
                     ze = (0, r.useRef)(Pe);
                 ze.current = Pe;
                 var je = te <= 0,
                     Te = te >= Pe,
-                    Be = Ge(je, Te),
-                    De = function() {
+                    Be = ie <= 0,
+                    De = ie >= x,
+                    Fe = Ge(je, Te, Be, De),
+                    He = function() {
                         return {
                             x: q ? -ie : ie,
                             y: te
                         }
                     },
-                    Fe = (0, r.useRef)(De()),
-                    He = (0, T._q)((function(e) {
+                    Le = (0, r.useRef)(He()),
+                    _e = (0, T._q)((function(e) {
                         if ($) {
-                            var t = (0, E.A)((0, E.A)({}, De()), e);
-                            Fe.current.x === t.x && Fe.current.y === t.y || ($(t), Fe.current = t)
+                            var t = (0, E.A)((0, E.A)({}, He()), e);
+                            Le.current.x === t.x && Le.current.y === t.y || ($(t), Le.current = t)
                         }
                     }));
 
-                function Le(e, t) {
+                function Ke(e, t) {
                     var n = e;
                     t ? ((0, d.flushSync)((function() {
                         ae(n)
-                    })), He()) : me(n)
+                    })), _e()) : me(n)
                 }
-                var _e = function(e) {
+                var We = function(e) {
                         var t = e,
                             n = x ? x - ke.width : 0;
                         return t = Math.max(t, 0), Math.min(t, n)
                     },
-                    Ke = (0, T._q)((function(e, t) {
+                    Ye = (0, T._q)((function(e, t) {
                         t ? ((0, d.flushSync)((function() {
                             ae((function(t) {
-                                return _e(t + (q ? -e : e))
+                                return We(t + (q ? -e : e))
                             }))
-                        })), He()) : me((function(t) {
+                        })), _e()) : me((function(t) {
                             return t + e
                         }))
                     })),
-                    We = function(e, t, n, o, i) {
-                        var a = (0, r.useRef)(0),
-                            l = (0, r.useRef)(null),
-                            c = (0, r.useRef)(null),
-                            s = (0, r.useRef)(!1),
-                            u = Ge(t, n),
-                            d = (0, r.useRef)(null),
-                            f = (0, r.useRef)(null);
+                    Qe = function(e, t, n, o, i, a, l) {
+                        var c = (0, r.useRef)(0),
+                            s = (0, r.useRef)(null),
+                            u = (0, r.useRef)(null),
+                            d = (0, r.useRef)(!1),
+                            f = Ge(t, n, o, i),
+                            p = (0, r.useRef)(null),
+                            m = (0, r.useRef)(null);
                         return [function(t) {
                             if (e) {
-                                Re.A.cancel(f.current), f.current = (0, Re.A)((function() {
-                                    d.current = null
+                                Re.A.cancel(m.current), m.current = (0, Re.A)((function() {
+                                    p.current = null
                                 }), 2);
                                 var n = t.deltaX,
                                     r = t.deltaY,
-                                    p = t.shiftKey,
-                                    m = n,
+                                    o = t.shiftKey,
+                                    i = n,
                                     g = r;
-                                ("sx" === d.current || !d.current && p && r && !n) && (m = r, g = 0, d.current = "sx");
-                                var h = Math.abs(m),
+                                ("sx" === p.current || !p.current && o && r && !n) && (i = r, g = 0, p.current = "sx");
+                                var h = Math.abs(i),
                                     v = Math.abs(g);
-                                null === d.current && (d.current = o && h > v ? "x" : "y"), "y" === d.current ? function(e, t) {
-                                    Re.A.cancel(l.current), a.current += t, c.current = t, u(t) || (Xe || e.preventDefault(), l.current = (0, Re.A)((function() {
-                                        var e = s.current ? 10 : 1;
-                                        i(a.current * e), a.current = 0
+                                null === p.current && (p.current = a && h > v ? "x" : "y"), "y" === p.current ? function(e, t) {
+                                    Re.A.cancel(s.current), c.current += t, u.current = t, f(!1, t) || (Xe || e.preventDefault(), s.current = (0, Re.A)((function() {
+                                        var e = d.current ? 10 : 1;
+                                        l(c.current * e), c.current = 0
                                     })))
                                 }(t, g) : function(e, t) {
-                                    i(t, !0), Xe || e.preventDefault()
-                                }(t, m)
+                                    l(t, !0), Xe || e.preventDefault()
+                                }(t, i)
                             }
                         }, function(t) {
-                            e && (s.current = t.detail === c.current)
+                            e && (d.current = t.detail === u.current)
                         }]
-                    }(K, je, Te, !!x, Ke),
-                    Ye = (0, l.A)(We, 2),
-                    Qe = Ye[0],
-                    et = Ye[1];
+                    }(K, je, Te, Be, De, !!x, Ye),
+                    et = (0, l.A)(Qe, 2),
+                    tt = et[0],
+                    rt = et[1];
                 ! function(e, t, n) {
                     var o, i = (0, r.useRef)(!1),
                         a = (0, r.useRef)(0),
-                        l = (0, r.useRef)(null),
+                        l = (0, r.useRef)(0),
                         c = (0, r.useRef)(null),
-                        u = function(e) {
+                        u = (0, r.useRef)(null),
+                        d = function(e) {
                             if (i.current) {
-                                var t = Math.ceil(e.touches[0].pageY),
-                                    r = a.current - t;
-                                a.current = t, n(r) && e.preventDefault(), clearInterval(c.current), c.current = setInterval((function() {
-                                    (!n(r *= Je, !0) || Math.abs(r) <= .1) && clearInterval(c.current)
+                                var t = Math.ceil(e.touches[0].pageX),
+                                    r = Math.ceil(e.touches[0].pageY),
+                                    o = a.current - t,
+                                    c = l.current - r,
+                                    s = Math.abs(o) > Math.abs(c);
+                                s ? a.current = t : l.current = r, n(s, s ? o : c) && e.preventDefault(), clearInterval(u.current), u.current = setInterval((function() {
+                                    s ? o *= Je : c *= Je;
+                                    var e = Math.floor(s ? o : c);
+                                    (!n(s, e, !0) || Math.abs(e) <= .1) && clearInterval(u.current)
                                 }), 16)
                             }
                         },
-                        d = function() {
+                        f = function() {
                             i.current = !1, o()
                         },
-                        f = function(e) {
-                            o(), 1 !== e.touches.length || i.current || (i.current = !0, a.current = Math.ceil(e.touches[0].pageY), l.current = e.target, l.current.addEventListener("touchmove", u), l.current.addEventListener("touchend", d))
+                        p = function(e) {
+                            o(), 1 !== e.touches.length || i.current || (i.current = !0, a.current = Math.ceil(e.touches[0].pageX), l.current = Math.ceil(e.touches[0].pageY), c.current = e.target, c.current.addEventListener("touchmove", d), c.current.addEventListener("touchend", f))
                         };
                     o = function() {
-                        l.current && (l.current.removeEventListener("touchmove", u), l.current.removeEventListener("touchend", d))
+                        c.current && (c.current.removeEventListener("touchmove", d), c.current.removeEventListener("touchend", f))
                     }, (0, s.A)((function() {
-                        return e && t.current.addEventListener("touchstart", f),
+                        return e && t.current.addEventListener("touchstart", p),
                             function() {
                                 var e;
-                                null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", f), o(), clearInterval(c.current)
+                                null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", p), o(), clearInterval(u.current)
                             }
                     }), [e])
-                }(K, Y, (function(e, t) {
-                    return !Be(e, t) && (Qe({
+                }(K, Y, (function(e, t, n) {
+                    return !Fe(e, t, n) && (tt({
                         preventDefault: function() {},
-                        deltaY: e
+                        deltaX: e ? t : 0,
+                        deltaY: e ? 0 : t
                     }), !0)
                 })), (0, s.A)((function() {
                     function e(e) {
                         K && e.preventDefault()
                     }
                     var t = Y.current;
-                    return t.addEventListener("wheel", Qe), t.addEventListener("DOMMouseScroll", et), t.addEventListener("MozMousePixelScroll", e),
+                    return t.addEventListener("wheel", tt), t.addEventListener("DOMMouseScroll", rt), t.addEventListener("MozMousePixelScroll", e),
                         function() {
-                            t.removeEventListener("wheel", Qe), t.removeEventListener("DOMMouseScroll", et), t.removeEventListener("MozMousePixelScroll", e)
+                            t.removeEventListener("wheel", tt), t.removeEventListener("DOMMouseScroll", rt), t.removeEventListener("MozMousePixelScroll", e)
                         }
                 }), [K]), (0, s.A)((function() {
                     if (x) {
-                        var e = _e(ie);
-                        ae(e), He({
+                        var e = We(ie);
+                        ae(e), _e({
                             x: e
                         })
                     }
                 }), [ke.width, x]);
-                var tt = function() {
+                var ct = function() {
                         var e, t;
                         null === (e = Oe.current) || void 0 === e || e.delayHidden(), null === (t = Ie.current) || void 0 === t || t.delayHidden()
                     },
-                    rt = function(e, t, n, o, i, a, c, u) {
+                    st = function(e, t, n, o, i, a, c, u) {
                         var d = r.useRef(),
                             f = r.useState(null),
                             p = (0, l.A)(f, 2),
                             m = p[0],
                             g = p[1];
                         return (0, s.A)((function() {
                                 if (m && m.times < 10) {
@@ -12046,31 +12057,31 @@
                                             originAlign: r
                                         })
                                     }
                                 } else u()
                             }
                     }(Y, U, H, c, z, (function() {
                         return F(!0)
-                    }), me, tt);
+                    }), me, ct);
                 r.useImperativeHandle(t, (function() {
                     return {
                         nativeElement: Z.current,
-                        getScrollInfo: De,
+                        getScrollInfo: He,
                         scrollTo: function(e) {
                             var t;
-                            (t = e) && "object" === (0, S.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && ae(_e(e.left)), rt(e.top)) : rt(e)
+                            (t = e) && "object" === (0, S.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && ae(We(e.left)), st(e.top)) : st(e)
                         }
                     }
                 })), (0, s.A)((function() {
                     if (I) {
                         var e = U.slice(we, Ae + 1);
                         I(e, U)
                     }
                 }), [we, Ae, U]);
-                var ct = function(e, t, n, o) {
+                var ut = function(e, t, n, o) {
                         var i = r.useMemo((function() {
                                 return [new Map, []]
                             }), [e, n.id, o]),
                             a = (0, l.A)(i, 2),
                             c = a[0],
                             s = a[1];
                         return function(r) {
@@ -12087,24 +12098,24 @@
                                 }
                             return {
                                 top: s[a - 1] || 0,
                                 bottom: s[l]
                             }
                         }
                     }(U, z, H, c),
-                    st = null == M ? void 0 : M({
+                    dt = null == M ? void 0 : M({
                         start: we,
                         end: Ae,
                         virtual: V,
                         offsetX: ie,
                         offsetY: Ce,
                         rtl: q,
-                        getSize: ct
+                        getSize: ut
                     }),
-                    ut = function(e, t, n, o, i, a, l, c) {
+                    ft = function(e, t, n, o, i, a, l, c) {
                         var s = c.getKey;
                         return e.slice(t, n + 1).map((function(e, n) {
                             var c = l(e, t + n, {
                                     style: {
                                         width: o
                                     },
                                     offsetX: i
@@ -12114,70 +12125,70 @@
                                 key: u,
                                 setRef: function(t) {
                                     return a(e, t)
                                 }
                             }, c)
                         }))
                     }(U, we, Ae, x, ie, D, h, pe),
-                    dt = null;
-                a && (dt = (0, E.A)((0, k.A)({}, f ? "height" : "maxHeight", a), lt), K && (dt.overflowY = "hidden", x && (dt.overflowX = "hidden"), se && (dt.pointerEvents = "none")));
-                var ft = {};
-                return q && (ft.dir = "rtl"), r.createElement("div", (0, g.A)({
+                    pt = null;
+                a && (pt = (0, E.A)((0, k.A)({}, f ? "height" : "maxHeight", a), lt), K && (pt.overflowY = "hidden", x && (pt.overflowX = "hidden"), se && (pt.pointerEvents = "none")));
+                var mt = {};
+                return q && (mt.dir = "rtl"), r.createElement("div", (0, g.A)({
                     ref: Z,
                     style: (0, E.A)((0, E.A)({}, p), {}, {
                         position: "relative"
                     }),
                     className: G
-                }, ft, P), r.createElement(X.A, {
+                }, mt, P), r.createElement(X.A, {
                     onResize: function(e) {
                         $e({
                             width: e.width || e.offsetWidth,
                             height: e.height || e.offsetHeight
                         })
                     }
                 }, r.createElement(A, {
                     className: "".concat(o, "-holder"),
-                    style: dt,
+                    style: pt,
                     ref: Y,
                     onScroll: function(e) {
                         var t = e.currentTarget.scrollTop;
-                        t !== te && me(t), null == C || C(e), He()
+                        t !== te && me(t), null == C || C(e), _e()
                     },
-                    onMouseEnter: tt
+                    onMouseEnter: ct
                 }, r.createElement(Ve, {
                     prefixCls: o,
                     height: xe,
                     offsetX: ie,
                     offsetY: Ce,
                     scrollWidth: x,
                     onInnerResize: F,
                     ref: Q,
                     innerProps: N,
                     rtl: q,
-                    extra: st
-                }, ut))), V && xe > a && r.createElement(nt, {
+                    extra: dt
+                }, ft))), V && xe > a && r.createElement(nt, {
                     ref: Oe,
                     prefixCls: o,
                     scrollOffset: te,
                     scrollRange: xe,
                     rtl: q,
-                    onScroll: Le,
+                    onScroll: Ke,
                     onStartMove: de,
                     onStopMove: fe,
                     spinSize: Me,
                     containerSize: ke.height,
                     style: null == R ? void 0 : R.verticalScrollBar,
                     thumbStyle: null == R ? void 0 : R.verticalScrollBarThumb
                 }), V && x > ke.width && r.createElement(nt, {
                     ref: Ie,
                     prefixCls: o,
                     scrollOffset: ie,
                     scrollRange: x,
                     rtl: q,
-                    onScroll: Le,
+                    onScroll: Ke,
                     onStartMove: de,
                     onStopMove: fe,
                     spinSize: Ne,
                     containerSize: ke.width,
                     horizontal: !0,
                     style: null == R ? void 0 : R.horizontalScrollBar,
                     thumbStyle: null == R ? void 0 : R.horizontalScrollBarThumb
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/595.853e8b63deafdcf653a9.js.LICENSE.txt` & `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/595.7fd40f4a8673fc24185a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/684.06766aa445a023bc4adf.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/684.06766aa445a023bc4adf.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/remoteEntry.871deda2d395cf3ebdb5.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/remoteEntry.432f146e752b80daa98d.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, l, u, f, s, p, d, c, h, v, m, g = {
+    var e, r, t, n, o, i, a, l, u, s, p, f, d, c, h, v, m, g = {
             8383: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(595), t.e(684)]).then((() => () => t(684))),
                         "./extension": () => Promise.all([t.e(595), t.e(684)]).then((() => () => t(684))),
                         "./style": () => t.e(432).then((() => () => t(1432)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -44,50 +44,50 @@
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
         432: "75a351a33d4e17e2f8f8",
-        595: "853e8b63deafdcf653a9",
+        595: "7fd40f4a8673fc24185a",
         684: "06766aa445a023bc4adf"
     } [e] + ".js?v=" + {
         432: "75a351a33d4e17e2f8f8",
-        595: "853e8b63deafdcf653a9",
+        595: "7fd40f4a8673fc24185a",
         684: "06766aa445a023bc4adf"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-log-console:", y.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
             var a, l;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        a = s;
+                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
+                    var p = u[s];
+                    if (p.getAttribute("src") == t || p.getAttribute("data-webpack") == r + o) {
+                        a = p;
                         break
                     }
                 }
             a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, y.nc && a.setAttribute("nonce", y.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
-            var p = (r, n) => {
+            var f = (r, n) => {
                     a.onerror = a.onload = null, clearTimeout(d);
                     var o = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(p.bind(null, void 0, {
+                d = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
-            a.onerror = p.bind(null, a.onerror), a.onload = p.bind(null, a.onload), l && document.head.appendChild(a)
+            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), l && document.head.appendChild(a)
         }
     }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -108,15 +108,15 @@
                     var o = i[e] = i[e] || {},
                         l = o[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : a > l.from)) && (o[r] = {
                         get: () => Promise.all([y.e(595), y.e(684)]).then((() => () => y(684))),
                         from: a,
                         eager: !1
                     })
-                })("@amphi/pipeline-log-console", "0.3.3"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@amphi/pipeline-log-console", "0.3.4"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -166,33 +166,33 @@
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var a = 0, l = 1, u = !0;; l++, a++) {
-                var f, s, p = l < e.length ? (typeof e[l])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(f = r[a]))[0])) return !u || ("u" == p ? l > n && !o : "" == p != o);
-                if ("u" == s) {
-                    if (!u || "u" != p) return !1
+                var s, p, f = l < e.length ? (typeof e[l])[0] : "";
+                if (a >= r.length || "o" == (p = (typeof(s = r[a]))[0])) return !u || ("u" == f ? l > n && !o : "" == f != o);
+                if ("u" == p) {
+                    if (!u || "u" != f) return !1
                 } else if (u)
-                    if (p == s)
+                    if (f == p)
                         if (l <= n) {
-                            if (f != e[l]) return !1
+                            if (s != e[l]) return !1
                         } else {
-                            if (o ? f > e[l] : f < e[l]) return !1;
-                            f != e[l] && (u = !1)
+                            if (o ? s > e[l] : s < e[l]) return !1;
+                            s != e[l] && (u = !1)
                         }
-                else if ("s" != p && "n" != p) {
+                else if ("s" != f && "n" != f) {
                     if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || s < p != o) return !1;
+                    if (l <= n || p < f != o) return !1;
                     u = !1
-                } else "s" != p && "n" != p && (u = !1, l--)
+                } else "s" != f && "n" != f && (u = !1, l--)
             }
         }
         var d = [],
             c = d.pop.bind(d);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
             d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
@@ -201,23 +201,23 @@
     }, a = (e, r) => {
         var t = y.S[e];
         if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = l(e, t);
-        return i(n, o) || s(u(e, t, o, n)), p(e[t][o])
-    }, s = e => {
+        return i(n, o) || p(u(e, t, o, n)), f(e[t][o])
+    }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+    }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
         var i = y.I(r);
         return i && i.then ? i.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
-    })(((e, r, t, n) => (a(e, t), f(r, 0, t, n)))), c = {}, h = {
+    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), c = {}, h = {
         1527: () => d("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
         3345: () => d("default", "react", [1, 18, 2, 0]),
         4236: () => d("default", "@jupyterlab/rendermime", [1, 4, 2, 0]),
         4602: () => d("default", "@lumino/signaling", [1, 2, 0, 0]),
         5256: () => d("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         5881: () => d("default", "@amphi/pipeline-editor", [0]),
         5923: () => d("default", "@jupyterlab/apputils", [1, 4, 3, 0]),
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-log-console/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984756097560976%*

 * *Differences: {"'packages'": "{33: {'versionInfo': '3.14.2'}}"}*

```diff
@@ -198,15 +198,15 @@
             "name": "rc-util",
             "versionInfo": "5.41.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-virtual-list",
-            "versionInfo": "3.14.0"
+            "versionInfo": "3.14.2"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react-dom",
             "versionInfo": "18.3.1"
         },
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/package.json` & `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8727182539682539%*

 * *Differences: {"'description'": "'Amphi Pipeline Log Console'",*

 * * "'devDependencies'": "{'@types/react-dom': '^18.2.25', 'react': '^18.2.0', delete: ['reactflow']}",*

 * * "'jupyterlab'": "{'outputDir': '../../amphi/pipeline-log-console', '_build': {'load': "*

 * *                 "'static/remoteEntry.432f146e752b80daa98d.js'}}",*

 * * "'name'": "'@amphi/pipeline-log-console'",*

 * * "'resolutions'": "OrderedDict([('@amphi/pipeline-editor', 'file:./../pipeline-editor')])",*

 * * "'version'": "'0.3.4'"}*

```diff
@@ -21,26 +21,27 @@
         "@lumino/datagrid": "^2.0.0",
         "@lumino/disposable": "^2.0.0",
         "@lumino/signaling": "^2.0.0",
         "@lumino/widgets": "^2.0.0",
         "react": "^18.2.0",
         "wildcard-match": "^5.1.2"
     },
-    "description": "Amphi Metadata Panel",
+    "description": "Amphi Pipeline Log Console",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
+        "@types/react-dom": "^18.2.25",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
-        "reactflow": "11.7.2",
+        "react": "^18.2.0",
         "rimraf": "^3.0.2",
         "typescript": "~5.0.4",
         "yarn-deduplicate": "^6.0.2"
     },
     "directories": {
         "lib": "lib/"
     },
@@ -51,36 +52,39 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9bc842b6cc0c70b4b0c3.js",
+            "load": "static/remoteEntry.432f146e752b80daa98d.js",
             "style": "./style"
         },
         "extension": true,
-        "outputDir": "../../amphi/pipeline-metadata-panel",
+        "outputDir": "../../amphi/pipeline-log-console",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
                 "singleton": true
             }
         }
     },
     "license": "Elastic License 2.0",
     "main": "lib/index.js",
-    "name": "@amphi/pipeline-metadata-panel",
+    "name": "@amphi/pipeline-log-console",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/amphi-ai/jupyterlab-amphi.git"
     },
+    "resolutions": {
+        "@amphi/pipeline-editor": "file:./../pipeline-editor"
+    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --build --verbose",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib && jlpm run clean:labextension",
@@ -95,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.3"
+    "version": "0.3.4"
 }
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/732.1ea6cff032a5ee2821e8.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/732.1ea6cff032a5ee2821e8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/remoteEntry.9bc842b6cc0c70b4b0c3.js` & `jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/remoteEntry.da6df8ad6b7fdf2715dc.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,15 @@
                     var a = i[e] = i[e] || {},
                         l = a[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : o > l.from)) && (a[r] = {
                         get: () => y.e(732).then((() => () => y(732))),
                         from: o,
                         eager: !1
                     })
-                })("@amphi/pipeline-metadata-panel", "0.3.3"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@amphi/pipeline-metadata-panel", "0.3.4"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_amphi-0.3.4/amphi/pipeline-metadata-panel/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/package.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8783619929453262%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/apputils': '^4.1.9', '@amphi/pipeline-components-manager': "*

 * *                   "'file:./../pipeline-components-manager', '@jupyterlab/docmanager-extension': "*

 * *                   "'^4.1.5', '@jupyterlab/filebrowser': '^4.1.5', '@jupyterlab/launcher': "*

 * *                   "'^4.1.5', '@jupyterlab/logconsole': '^4.1.5', '@jupyterlab/mainmenu': "*

 * *                   "'^4.1.5', '@jupyterlab/services': '~7.1.5', '@jupyterlab/settingregistry': "*

 * *                   "'^4.1.5', '@jupy […]*

```diff
@@ -3,43 +3,41 @@
         "email": "tgourdel@amphi.ai",
         "name": "Thibaut Gourdel"
     },
     "bugs": {
         "url": "https://github.com/amphi-ai/jupyterlab-amphi/issues"
     },
     "dependencies": {
+        "@amphi/pipeline-components-manager": "file:./../pipeline-components-manager",
         "@jupyterlab/application": "^4.1.5",
-        "@jupyterlab/apputils": "^4.1.5",
-        "@lumino/widgets": "^2.0.0",
-        "@uiw/react-codemirror": "^4.22.0",
-        "ace-builds": "^1.33.1",
+        "@jupyterlab/apputils": "^4.1.9",
+        "@jupyterlab/docmanager-extension": "^4.1.5",
+        "@jupyterlab/filebrowser": "^4.1.5",
+        "@jupyterlab/launcher": "^4.1.5",
+        "@jupyterlab/logconsole": "^4.1.5",
+        "@jupyterlab/mainmenu": "^4.1.5",
+        "@jupyterlab/services": "~7.1.5",
+        "@jupyterlab/settingregistry": "^4.1.5",
+        "@jupyterlab/ui-components": "^4.1.5",
+        "@lumino/dragdrop": "^2.0.0",
+        "@tailwindcss/forms": "^0.5.7",
         "antd": "5.16.4",
-        "react-ace": "^11.0.1",
-        "react-dnd": "^16.0.1",
-        "react-dnd-html5-backend": "^16.0.1",
-        "react-dom": "^18.2.0",
-        "react-flow-renderer": "^10.3.17",
-        "react-mentions": "^4.4.10",
-        "react-select": "^5.8.0",
-        "styled-components": "^6.1.8"
+        "reactflow": "11.9.4",
+        "tailwindcss": "^3.4.1"
     },
-    "description": "Amphi Pipeline Components Manager",
+    "description": "Amphi Pipeline Editor",
     "devDependencies": {
         "@jupyterlab/builder": "^4.1.5",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "antd": "5.16.4",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "eslint-plugin-react": "^7.18.3",
+        "@types/json-schema": "^7.0.11",
+        "@types/node": "^20.7.0",
+        "@types/react": "^18.0.26",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "reactflow": "11.7.2",
-        "rimraf": "^3.0.2",
+        "prettier": "^3.0.0",
+        "react": "^18.2.0",
+        "rimraf": "^5.0.1",
         "typescript": "~5.2.2",
         "yarn-deduplicate": "^6.0.2"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
@@ -47,50 +45,61 @@
         "lib/*.js.map",
         "lib/*.js",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.54de67c179f201c5e11a.js",
+            "style": "./style"
+        },
         "extension": true,
-        "outputDir": "../../amphi/pipeline-components-manager",
+        "outputDir": "../../amphi/pipeline-editor",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
-                "bundle": false,
+                "bundled": false,
+                "singleton": true
+            },
+            "@amphi/pipeline-editor": {
+                "bundled": false,
                 "singleton": true
             }
         }
     },
     "license": "Elastic License 2.0",
     "main": "lib/index.js",
-    "name": "@amphi/pipeline-components-manager",
+    "name": "@amphi/pipeline-editor",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/amphi-ai/jupyterlab-amphi.git"
     },
     "resolutions": {
-        "@jupyterlab/rendermime-interfaces": "^3.8.9",
+        "@amphi/pipeline-components-manager": "file:./../pipeline-components-manager",
+        "@jupyterlab/rendermime-interfaces": "^4.1.5",
+        "@jupyterlab/services": "^7.1.5",
         "@lumino/widgets": "^2.0.0",
-        "@types/react": "^18.2.7",
-        "antd": "5.16.4"
+        "@types/react": "^18.2.7"
     },
     "scripts": {
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
+        "build": "npx tailwindcss -i ./style/canvas.css -o ./style/output.css && jlpm run build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --build --verbose",
-        "build:prod": "jlpm run build:lib && jlpm run build:labextension && jlpm install",
-        "clean": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf ../../amphi/pipeline-components-manager",
+        "build:prod": "npx tailwindcss -i ./style/canvas.css -o ./style/output.css && jlpm run build:lib && jlpm build:labextension && jlpm install",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension",
+        "clean:labextension": "rimraf ../../amphi/root",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
+        "dist": "cd ../../dist && npm pack ../packages/pipeline-editor",
+        "docs": "typedoc src",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
```

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/tsconfig.json` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/BrowseFileDialog.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/BrowseFileDialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/CodeGenerator.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/CodeGenerator.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/CustomHandle.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/CustomHandle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/DndProviderWrapper.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/DndProviderWrapper.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/PipelineComponent.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/PipelineComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/PipelineService.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/PipelineService.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/RequestService.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/RequestService.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/configUtils.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/configUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/connectionUtils.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/connectionUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/generatorUtils.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/generatorUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/icons.ts` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/index.ts` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/rendererUtils.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/rendererUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/InputRegular.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/InputRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/connectionSelector.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/connectionSelector.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/dataMapping.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/dataMapping.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/keyValueForm.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/keyValueForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectColumn.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectColumn.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectColumns.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectMultiple.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectMultiple.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectRegular.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/selectTokenization.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectTokenization.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/transferData.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/transferData.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/src/forms/valuesListForm.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/valuesListForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/settings-16.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/settings-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/settings-24.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/settings-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/trash-16.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/trash-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/trash-24.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/trash-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-components-manager/style/icons/x-square-16.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/x-square-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/package.json` & `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/package.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8422619047619048%*

 * *Differences: {"'author'": "{'email': ''}",*

 * * "'dependencies'": "{'@lumino/widgets': '^2.0.0', delete: ['@jupyterlab/apputils', "*

 * *                   "'@jupyterlab/docmanager-extension', '@jupyterlab/filebrowser', "*

 * *                   "'@jupyterlab/launcher', '@jupyterlab/logconsole', '@jupyterlab/mainmenu', "*

 * *                   "'@jupyterlab/services', '@jupyterlab/settingregistry', "*

 * *                   "'@jupyterlab/ui-components', '@lumino/dragdrop', '@tailwindcss/forms', "*

 * *                   "'tailwindcss']}",*

 * * "'descr […]*

```diff
@@ -1,100 +1,85 @@
 {
     "author": {
-        "email": "tgourdel@amphi.ai",
+        "email": "",
         "name": "Thibaut Gourdel"
     },
     "bugs": {
         "url": "https://github.com/amphi-ai/jupyterlab-amphi/issues"
     },
     "dependencies": {
         "@amphi/pipeline-components-manager": "file:./../pipeline-components-manager",
         "@jupyterlab/application": "^4.1.5",
-        "@jupyterlab/apputils": "^4.1.9",
-        "@jupyterlab/docmanager-extension": "^4.1.5",
-        "@jupyterlab/filebrowser": "^4.1.5",
-        "@jupyterlab/launcher": "^4.1.5",
-        "@jupyterlab/logconsole": "^4.1.5",
-        "@jupyterlab/mainmenu": "^4.1.5",
-        "@jupyterlab/services": "~7.1.5",
-        "@jupyterlab/settingregistry": "^4.1.5",
-        "@jupyterlab/ui-components": "^4.1.5",
-        "@lumino/dragdrop": "^2.0.0",
-        "@tailwindcss/forms": "^0.5.7",
+        "@lumino/widgets": "^2.0.0",
         "antd": "5.16.4",
-        "reactflow": "11.9.4",
-        "tailwindcss": "^3.4.1"
+        "reactflow": "11.9.4"
     },
-    "description": "Amphi Pipeline Editor",
+    "description": "Amphi Pipeline Core Components",
     "devDependencies": {
         "@jupyterlab/builder": "^4.1.5",
-        "@types/json-schema": "^7.0.11",
-        "@types/node": "^20.7.0",
-        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^4.8.1",
+        "@typescript-eslint/parser": "^4.8.1",
+        "eslint": "^7.14.0",
+        "eslint-config-prettier": "^6.15.0",
+        "eslint-plugin-prettier": "^3.1.4",
+        "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^3.0.0",
-        "react": "^18.2.0",
-        "rimraf": "^5.0.1",
-        "typescript": "~5.2.2",
+        "prettier": "^2.1.1",
+        "reactflow": "11.7.2",
+        "rimraf": "^3.0.2",
+        "typescript": "~5.0.4",
         "yarn-deduplicate": "^6.0.2"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/*.d.ts",
         "lib/*.js.map",
         "lib/*.js",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.f71216c42efa6af2ddcd.js",
+            "style": "./style"
+        },
         "extension": true,
-        "outputDir": "../../amphi/pipeline-editor",
+        "outputDir": "../../amphi/pipeline-components-core",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
                 "singleton": true
-            },
-            "@amphi/pipeline-editor": {
-                "bundled": false,
-                "singleton": true
             }
         }
     },
     "license": "Elastic License 2.0",
     "main": "lib/index.js",
-    "name": "@amphi/pipeline-editor",
+    "name": "@amphi/pipeline-components-core",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/amphi-ai/jupyterlab-amphi.git"
     },
-    "resolutions": {
-        "@amphi/pipeline-components-manager": "file:./../pipeline-components-manager",
-        "@jupyterlab/rendermime-interfaces": "^4.1.5",
-        "@jupyterlab/services": "^7.1.5",
-        "@lumino/widgets": "^2.0.0",
-        "@types/react": "^18.2.7"
-    },
     "scripts": {
-        "build": "npx tailwindcss -i ./style/canvas.css -o ./style/output.css && jlpm run build:lib && jlpm build:labextension:dev",
+        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --build --verbose",
-        "build:prod": "npx tailwindcss -i ./style/canvas.css -o ./style/output.css && jlpm run build:lib && jlpm build:labextension && jlpm install",
-        "clean": "jlpm clean:lib",
-        "clean:all": "jlpm clean:lib && jlpm clean:labextension",
-        "clean:labextension": "rimraf ../../amphi/root",
+        "build:prod": "jlpm run build:lib && jlpm run build:labextension",
+        "clean": "jlpm run clean:lib && jlpm run clean:labextension",
+        "clean:labextension": "rimraf ../../amphi/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "dist": "cd ../../dist && npm pack ../packages/pipeline-editor",
-        "docs": "typedoc src",
+        "eslint": "eslint . --ext .ts,.tsx --fix",
+        "eslint:check": "eslint . --ext .ts,.tsx",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
```

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/pipeline-16.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/pipeline-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/pipeline-24.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/pipeline-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/tsconfig.json` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/schema/plugin copy.json` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/schema/plugin copy.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/schema/plugin.json` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/Dropzone.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/Dropzone.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/PipelineEditorWidget.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/PipelineEditorWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/customEdge.tsx` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/customEdge.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/icons.ts` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/src/index.ts` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/index.ts`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
           try {
             // Create promise to track success or failure of the request
             const delegate = new PromiseDelegate<ReadonlyJSONValue>();
             const start = performance.now();
 
             Notification.promise(delegate.promise, {
               // Message when the task is pending
-              pending: { message: 'Running...', options: { autoClose: false } },
+              pending: { message: 'Running...', options: { autoClose: false }},
               // Message when the task finished successfully
               success: {
                 message: (result: any) => `Pipeline execution successful after ${result.delayInSeconds} seconds.`,
                 options: {
                   autoClose: 3000
                 }
               },
```

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/canvas.css` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/canvas.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/output.css` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/output.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/pipeline-category-icon.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/pipeline-category-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/react-icon.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/react-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/api-24.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/api-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/file-plus-24.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/file-plus-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/file-text-24.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/file-text-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/pipeline-brand-16.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/pipeline-brand-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/packages/pipeline-editor/style/icons/pipeline-brand-24.svg` & `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/pipeline-brand-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/LICENSE` & `jupyterlab_amphi-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/README.md` & `jupyterlab_amphi-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/pyproject.toml` & `jupyterlab_amphi-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.4/PKG-INFO` & `jupyterlab_amphi-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-amphi
-Version: 0.3.4
+Version: 0.3.5
 Dynamic: Keywords
 Summary: Amphi is a micro ETL for Jupyterlab.
 Project-URL: Homepage, https://amphi.ai
 Project-URL: Bug Tracker, https://github.com/amphi-ai/jupyterlab-amphi/issues
 Project-URL: Repository, https://github.com/amphi-ai/jupyterlab-amphi.git
 Author-email: Thibaut Gourdel <tgourdel@amphi.ai>
 License: Elastic License 2.0 \(ELv2\)
```


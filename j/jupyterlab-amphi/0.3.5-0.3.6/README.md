# Comparing `tmp/jupyterlab_amphi-0.3.5.tar.gz` & `tmp/jupyterlab_amphi-0.3.6.tar.gz`

## Comparing `jupyterlab_amphi-0.3.5.tar` & `jupyterlab_amphi-0.3.6.tar`

### file list

```diff
@@ -1,153 +1,153 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/.yarnrc.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/MANIFEST.in
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/install.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/lerna.json
--rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/output.json
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/package.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/setup.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/tsconfig.eslint.json
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/tsconfigbase.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/_version.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/package.json
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js
--rw-r--r--   0        0        0    22345 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js.LICENSE.txt
--rw-r--r--   0        0        0  1442297 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/687.3718223fe5543295ebcd.js
--rw-r--r--   0        0        0    35011 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/687.3718223fe5543295ebcd.js.LICENSE.txt
--rw-r--r--   0        0        0   542717 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt
--rw-r--r--   0        0        0   143367 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/792.7de2deb742ba9e036dda.js
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/remoteEntry.f71216c42efa6af2ddcd.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/style.js
--rw-r--r--   0        0        0   120113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/third-party-licenses.json
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/package.json
--rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
--rw-r--r--   0        0        0    56966 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/142.acbbd4c680da3a899eb9.js
--rw-r--r--   0        0        0    27269 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js.LICENSE.txt
--rw-r--r--   0        0        0    61091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js
--rw-r--r--   0        0        0  1438023 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/422.bbb456b73e63e5a1e7d4.js
--rw-r--r--   0        0        0    29737 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/422.bbb456b73e63e5a1e7d4.js.LICENSE.txt
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js
--rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
--rw-r--r--   0        0        0   150147 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt
--rw-r--r--   0        0        0   440126 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/841.0203c999f04b4e256cd6.js
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/841.0203c999f04b4e256cd6.js.LICENSE.txt
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
--rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/remoteEntry.5ec1e44c8f356f845b6f.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/style.js
--rw-r--r--   0        0        0   140477 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/third-party-licenses.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/package.json
--rw-r--r--   0        0        0   152553 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt
--rw-r--r--   0        0        0    33113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/412.23a82146827c21626eae.js
--rw-r--r--   0        0        0    27297 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/631.20cdac1e84cf987a8781.js
--rw-r--r--   0        0        0  1447990 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/735.59d5dbc617bf0dc8cc9f.js
--rw-r--r--   0        0        0    36421 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/735.59d5dbc617bf0dc8cc9f.js.LICENSE.txt
--rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/remoteEntry.54de67c179f201c5e11a.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/style.js
--rw-r--r--   0        0        0   118882 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/third-party-licenses.json
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/package.json
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js
--rw-r--r--   0        0        0   752340 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/595.7fd40f4a8673fc24185a.js
--rw-r--r--   0        0        0    13950 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/595.7fd40f4a8673fc24185a.js.LICENSE.txt
--rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/684.06766aa445a023bc4adf.js
--rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/remoteEntry.432f146e752b80daa98d.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/style.js
--rw-r--r--   0        0        0    64970 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/third-party-licenses.json
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/package.json
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js
--rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/732.1ea6cff032a5ee2821e8.js
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/remoteEntry.da6df8ad6b7fdf2715dc.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/third-party-licenses.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi_extension/_version.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/install.json
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/tsconfig.json
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
--rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/CodeGenerator.tsx
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/CustomHandle.tsx
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/DndProviderWrapper.tsx
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/PipelineComponent.tsx
--rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/PipelineService.tsx
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/RequestService.tsx
--rw-r--r--   0        0        0    20670 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/configUtils.tsx
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/connectionUtils.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/declarations.d.ts
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/generatorUtils.tsx
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/icons.ts
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/index.ts
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/rendererUtils.tsx
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/InputRegular.tsx
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/connectionSelector.tsx
--rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/dataMapping.tsx
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectColumn.tsx
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectColumns.tsx
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectRegular.tsx
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/transferData.tsx
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/base.css
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/index.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/crosshair-16.svg
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/minus-16.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/play-16.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/play-circle-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/plus-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/plus-24.svg
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/search-16.svg
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/search-24.svg
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/settings-16.svg
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/settings-24.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/trash-16.svg
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/trash-24.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/x-16.svg
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/x-square-16.svg
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/install.json
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/package.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/pipeline-16.svg
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/pipeline-24.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/tailwind.config.js
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/tsconfig.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/schema/extension.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/schema/plugin copy.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/schema/plugin.json
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/Dropzone.tsx
--rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/PipelineEditorWidget.tsx
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/customEdge.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/declarations.d.ts
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/icons.ts
--rw-r--r--   0        0        0    18171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/index.ts
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/canvas.css
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/index.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/index.js
--rw-r--r--   0        0        0    22125 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/output.css
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/pipeline-category-icon.svg
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/react-icon.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/tailwinds_preflight.css
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/api-24.svg
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/file-plus-24.svg
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/file-text-24.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/monitor-24.svg
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/.gitignore
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/README.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/.yarnrc.yml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/MANIFEST.in
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/install.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/lerna.json
+-rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/output.json
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/package.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/tsconfig.eslint.json
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/tsconfigbase.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/_version.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/package.json
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js
+-rw-r--r--   0        0        0    22345 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js.LICENSE.txt
+-rw-r--r--   0        0        0  1442297 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/687.3718223fe5543295ebcd.js
+-rw-r--r--   0        0        0    35011 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/687.3718223fe5543295ebcd.js.LICENSE.txt
+-rw-r--r--   0        0        0   542717 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt
+-rw-r--r--   0        0        0   143367 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/792.7de2deb742ba9e036dda.js
+-rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/remoteEntry.be309c73964f3370f798.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/style.js
+-rw-r--r--   0        0        0   120113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
+-rw-r--r--   0        0        0    56966 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/142.acbbd4c680da3a899eb9.js
+-rw-r--r--   0        0        0    27269 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js.LICENSE.txt
+-rw-r--r--   0        0        0    61091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js
+-rw-r--r--   0        0        0  1438023 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/422.bbb456b73e63e5a1e7d4.js
+-rw-r--r--   0        0        0    29737 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/422.bbb456b73e63e5a1e7d4.js.LICENSE.txt
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js
+-rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
+-rw-r--r--   0        0        0   150147 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt
+-rw-r--r--   0        0        0   440126 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/841.0203c999f04b4e256cd6.js
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/841.0203c999f04b4e256cd6.js.LICENSE.txt
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/remoteEntry.e8e175fb3bd1601a2ddf.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/style.js
+-rw-r--r--   0        0        0   140477 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-editor/package.json
+-rw-r--r--   0        0        0   152553 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt
+-rw-r--r--   0        0        0    33191 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/412.ddd9e2d00880716eff56.js
+-rw-r--r--   0        0        0    27297 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/631.20cdac1e84cf987a8781.js
+-rw-r--r--   0        0        0  1447990 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/735.59d5dbc617bf0dc8cc9f.js
+-rw-r--r--   0        0        0    36421 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/735.59d5dbc617bf0dc8cc9f.js.LICENSE.txt
+-rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/remoteEntry.4ff74fcef89bc3e36fe4.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/style.js
+-rw-r--r--   0        0        0   118882 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/package.json
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js
+-rw-r--r--   0        0        0   752340 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/595.7fd40f4a8673fc24185a.js
+-rw-r--r--   0        0        0    13950 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/595.7fd40f4a8673fc24185a.js.LICENSE.txt
+-rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/684.06766aa445a023bc4adf.js
+-rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/remoteEntry.7b90c2c5a47602453a70.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/style.js
+-rw-r--r--   0        0        0    64970 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-metadata-panel/package.json
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js
+-rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-metadata-panel/static/732.1ea6cff032a5ee2821e8.js
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-metadata-panel/static/remoteEntry.4ab9bad57a24f62bae72.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-metadata-panel/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi/pipeline-metadata-panel/static/third-party-licenses.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi_extension/_version.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/install.json
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/tsconfig.json
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
+-rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/CodeGenerator.tsx
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/CustomHandle.tsx
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/DndProviderWrapper.tsx
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/PipelineComponent.tsx
+-rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/PipelineService.tsx
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/RequestService.tsx
+-rw-r--r--   0        0        0    20670 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/configUtils.tsx
+-rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/connectionUtils.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/declarations.d.ts
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/generatorUtils.tsx
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/icons.ts
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/index.ts
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/rendererUtils.tsx
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/InputRegular.tsx
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/connectionSelector.tsx
+-rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/dataMapping.tsx
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/selectColumn.tsx
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/selectColumns.tsx
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/selectRegular.tsx
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/transferData.tsx
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/base.css
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/index.js
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/crosshair-16.svg
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/minus-16.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/play-16.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/play-circle-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/plus-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/plus-24.svg
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/search-16.svg
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/search-24.svg
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/settings-16.svg
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/settings-24.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/trash-16.svg
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/trash-24.svg
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/x-16.svg
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/x-square-16.svg
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/install.json
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/package.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/pipeline-16.svg
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/pipeline-24.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/tailwind.config.js
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/tsconfig.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/schema/extension.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/schema/plugin copy.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/schema/plugin.json
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/src/Dropzone.tsx
+-rw-r--r--   0        0        0    20868 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/src/PipelineEditorWidget.tsx
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/src/customEdge.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/src/declarations.d.ts
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/src/icons.ts
+-rw-r--r--   0        0        0    18171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/src/index.ts
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/canvas.css
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/index.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/index.js
+-rw-r--r--   0        0        0    22125 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/output.css
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/pipeline-category-icon.svg
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/react-icon.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/tailwinds_preflight.css
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/icons/api-24.svg
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/icons/file-plus-24.svg
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/icons/file-text-24.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/icons/monitor-24.svg
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/.gitignore
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/README.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.6/PKG-INFO
```

### Comparing `jupyterlab_amphi-0.3.5/output.json` & `jupyterlab_amphi-0.3.6/output.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/package.json` & `jupyterlab_amphi-0.3.6/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.3.6'"}*

```diff
@@ -66,15 +66,15 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.yaml}\"",
         "prettier:check": "jlpm prettier:base --check",
         "quickstart": "npm run setup:py && jlpm && jlpm deduplicate && jlpm clean:all && jlpm lint && jlpm build:prod && jlpm dist && jlpm docs && jlpm test",
         "setup:py": "python -m pip install -e \".[dev,lint,test,docs]\"",
         "test": "jlpm test:py",
         "test:py": "pytest"
     },
-    "version": "0.3.5",
+    "version": "0.3.6",
     "workspaces": {
         "packages": [
             "packages/pipeline-editor",
             "packages/pipeline-components-manager",
             "packages/pipeline-components-core",
             "packages/pipeline-console",
             "packages/pipeline-metadata-panel"
```

### Comparing `jupyterlab_amphi-0.3.5/tsconfigbase.json` & `jupyterlab_amphi-0.3.6/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/package.json` & `jupyterlab_amphi-0.3.6/amphi/pipeline-metadata-panel/package.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8869310897435897%*

 * *Differences: {"'author'": "{'email': 'tgourdel@amphi.ai'}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@amphi/pipeline-editor': "*

 * *                   "'file:./../pipeline-editor', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/console': '^4.0.0', '@jupyterlab/coreutils': '^6.0.0', "*

 * *                   "'@jupyterlab/notebook': '^4.0.0', '@jupyterlab/outputarea': '^4.0.0', "*

 * *                   "'@jupyterlab/rendermime': '^4.0.0', '@jupyterlab/services': '^7.0.0', "*

 * *                   " […]*

```diff
@@ -1,25 +1,37 @@
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
-        "@jupyterlab/application": "^4.1.5",
+        "@amphi/pipeline-editor": "file:./../pipeline-editor",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/console": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/outputarea": "^4.0.0",
+        "@jupyterlab/rendermime": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/ui-components": "^4.0.0",
+        "@lumino/coreutils": "^2.0.0",
+        "@lumino/datagrid": "^2.0.0",
+        "@lumino/disposable": "^2.0.0",
+        "@lumino/signaling": "^2.0.0",
         "@lumino/widgets": "^2.0.0",
-        "antd": "5.16.4",
-        "reactflow": "11.9.4"
+        "react": "^18.2.0",
+        "wildcard-match": "^5.1.2"
     },
-    "description": "Amphi Pipeline Core Components",
+    "description": "Amphi Metadata Panel",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.1.5",
+        "@jupyterlab/builder": "^4.0.0",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
@@ -39,53 +51,53 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f71216c42efa6af2ddcd.js",
+            "load": "static/remoteEntry.4ab9bad57a24f62bae72.js",
             "style": "./style"
         },
         "extension": true,
-        "outputDir": "../../amphi/pipeline-components-core",
+        "outputDir": "../../amphi/pipeline-metadata-panel",
         "sharedPackages": {
-            "@amphi/pipeline-components-manager": {
+            "@amphi/pipeline-editor": {
                 "bundled": false,
                 "singleton": true
             }
         }
     },
     "license": "Elastic License 2.0",
     "main": "lib/index.js",
-    "name": "@amphi/pipeline-components-core",
+    "name": "@amphi/pipeline-metadata-panel",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/amphi-ai/jupyterlab-amphi.git"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --build --verbose",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf ../../amphi/labextension",
+        "clean:labextension": "rimraf ../../amphi/pipeline-metadata-panel",
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
-    "version": "0.3.4"
+    "version": "0.3.5"
 }
```

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/687.3718223fe5543295ebcd.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/687.3718223fe5543295ebcd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/687.3718223fe5543295ebcd.js.LICENSE.txt` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/687.3718223fe5543295ebcd.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/792.7de2deb742ba9e036dda.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/792.7de2deb742ba9e036dda.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/remoteEntry.f71216c42efa6af2ddcd.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/remoteEntry.be309c73964f3370f798.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -117,15 +117,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@amphi/pipeline-components-core", "0.3.4", (() => Promise.all([S.e(518), S.e(345), S.e(792)]).then((() => () => S(5792))))), l("antd", "5.16.4", (() => Promise.all([S.e(687), S.e(518), S.e(628), S.e(345)]).then((() => () => S(7687))))), l("reactflow", "11.7.2", (() => Promise.all([S.e(713), S.e(628), S.e(345)]).then((() => () => S(5713)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@amphi/pipeline-components-core", "0.3.5", (() => Promise.all([S.e(518), S.e(345), S.e(792)]).then((() => () => S(5792))))), l("antd", "5.16.4", (() => Promise.all([S.e(687), S.e(518), S.e(628), S.e(345)]).then((() => () => S(7687))))), l("reactflow", "11.7.2", (() => Promise.all([S.e(713), S.e(628), S.e(345)]).then((() => () => S(5713)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-core/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e8e175fb3bd1601a2ddf.js'}}",*

 * * "'version'": "'0.3.5'"}*

```diff
@@ -49,15 +49,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.5ec1e44c8f356f845b6f.js",
+            "load": "static/remoteEntry.e8e175fb3bd1601a2ddf.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-manager",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundle": false,
@@ -99,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.4"
+    "version": "0.3.5"
 }
```

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/142.acbbd4c680da3a899eb9.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/142.acbbd4c680da3a899eb9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/173.254dd13d95daff6ca4b4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/422.bbb456b73e63e5a1e7d4.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/422.bbb456b73e63e5a1e7d4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/422.bbb456b73e63e5a1e7d4.js.LICENSE.txt` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/422.bbb456b73e63e5a1e7d4.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/841.0203c999f04b4e256cd6.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/841.0203c999f04b4e256cd6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/remoteEntry.5ec1e44c8f356f845b6f.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/remoteEntry.e8e175fb3bd1601a2ddf.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -132,15 +132,15 @@
                         (!d || !d.loaded && (!a != !d.eager ? a : i > d.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (d("@amphi/pipeline-components-manager", "0.3.4", (() => Promise.all([S.e(173), S.e(725), S.e(345), S.e(628), S.e(142)]).then((() => () => S(8142))))), d("ace-builds", "1.34.0", (() => S.e(841).then((() => () => S(1841))))), d("antd", "5.16.4", (() => Promise.all([S.e(422), S.e(173), S.e(345), S.e(628)]).then((() => () => S(5422))))), d("react-ace", "11.0.1", (() => Promise.all([S.e(271), S.e(345), S.e(186)]).then((() => () => S(6271))))), d("react-dnd-html5-backend", "16.0.1", (() => S.e(454).then((() => () => S(6454))))), d("react-dnd", "16.0.1", (() => Promise.all([S.e(12), S.e(345), S.e(85)]).then((() => () => S(4631)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@amphi/pipeline-components-manager", "0.3.5", (() => Promise.all([S.e(173), S.e(725), S.e(345), S.e(628), S.e(142)]).then((() => () => S(8142))))), d("ace-builds", "1.34.0", (() => S.e(841).then((() => () => S(1841))))), d("antd", "5.16.4", (() => Promise.all([S.e(422), S.e(173), S.e(345), S.e(628)]).then((() => () => S(5422))))), d("react-ace", "11.0.1", (() => Promise.all([S.e(271), S.e(345), S.e(186)]).then((() => () => S(6271))))), d("react-dnd-html5-backend", "16.0.1", (() => S.e(454).then((() => () => S(6454))))), d("react-dnd", "16.0.1", (() => Promise.all([S.e(12), S.e(345), S.e(85)]).then((() => () => S(4631)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-components-manager/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-manager/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/package.json` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702380952380952%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.3.6'"}*

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
-            "load": "static/remoteEntry.54de67c179f201c5e11a.js",
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
-    "version": "0.3.4"
+    "version": "0.3.6"
 }
```

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt` & `jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/412.23a82146827c21626eae.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/412.ddd9e2d00880716eff56.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -414,21 +414,26 @@
                             children: a
                         }
                     }));
                     return console.log(i), v().createElement("aside", {
                         className: t,
                         title: "Components"
                     }, v().createElement("div", {
-                        className: "description"
+                        className: "description",
+                        style: {
+                            textAlign: "center",
+                            fontWeight: "bold",
+                            marginBottom: "16px"
+                        }
                     }, v().createElement(m.extensionIcon.react, {
                         tag: "span",
                         width: "24px",
                         float: "left",
                         marginRight: "8px"
-                    }), "Drag and drop components."), v().createElement(H, {
+                    }), "Drag and drop components in the canvas"), v().createElement(H, {
                         selectable: !1,
                         multiple: !0,
                         blockNode: !0,
                         defaultExpandAll: !0,
                         treeData: i,
                         key: "palette-components"
                     }))
```

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/735.59d5dbc617bf0dc8cc9f.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/735.59d5dbc617bf0dc8cc9f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/735.59d5dbc617bf0dc8cc9f.js.LICENSE.txt` & `jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/735.59d5dbc617bf0dc8cc9f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/remoteEntry.54de67c179f201c5e11a.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/remoteEntry.4ff74fcef89bc3e36fe4.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, l, u, f, s, d, p, c, h, v, m, b, g, y, w, j, P, S, E = {
+    var e, r, t, a, n, o, i, l, u, f, d, s, p, c, h, v, m, b, g, y, w, j, P, S, E = {
             8535: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(345), t.e(550), t.e(412)]).then((() => () => t(8412))),
                         "./extension": () => Promise.all([t.e(345), t.e(550), t.e(412)]).then((() => () => t(8412))),
                         "./style": () => Promise.all([t.e(550), t.e(631)]).then((() => () => t(7631)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -45,23 +45,23 @@
         for (var t in r) _.o(r, t) && !_.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, _.f = {}, _.e = e => Promise.all(Object.keys(_.f).reduce(((r, t) => (_.f[t](e, r), r)), [])), _.u = e => e + "." + {
         285: "f1fef15430d9554bfba0",
         345: "4aa5390d29af88207b53",
-        412: "23a82146827c21626eae",
+        412: "ddd9e2d00880716eff56",
         550: "025783cb8476390cbadc",
         628: "d05f56a756fb73f1c255",
         631: "20cdac1e84cf987a8781",
         735: "59d5dbc617bf0dc8cc9f"
     } [e] + ".js?v=" + {
         285: "f1fef15430d9554bfba0",
         345: "4aa5390d29af88207b53",
-        412: "23a82146827c21626eae",
+        412: "ddd9e2d00880716eff56",
         550: "025783cb8476390cbadc",
         628: "d05f56a756fb73f1c255",
         631: "20cdac1e84cf987a8781",
         735: "59d5dbc617bf0dc8cc9f"
     } [e], _.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
@@ -71,31 +71,31 @@
         }
     }(), _.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-editor:", _.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, l;
             if (void 0 !== n)
                 for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
-                        i = s;
+                    var d = u[f];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
+                        i = d;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, _.nc && i.setAttribute("nonce", _.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var d = (r, a) => {
+            var s = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, _.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -117,15 +117,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@amphi/pipeline-editor", "0.3.4", (() => Promise.all([_.e(345), _.e(550), _.e(412)]).then((() => () => _(8412))))), l("antd", "5.16.4", (() => Promise.all([_.e(735), _.e(628), _.e(345)]).then((() => () => _(1735))))), l("reactflow", "11.9.4", (() => Promise.all([_.e(285), _.e(628), _.e(345)]).then((() => () => _(1285)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@amphi/pipeline-editor", "0.3.5", (() => Promise.all([_.e(345), _.e(550), _.e(412)]).then((() => () => _(8412))))), l("antd", "5.16.4", (() => Promise.all([_.e(735), _.e(628), _.e(345)]).then((() => () => _(1735))))), l("reactflow", "11.9.4", (() => Promise.all([_.e(285), _.e(628), _.e(345)]).then((() => () => _(1285)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         _.g.importScripts && (e = _.g.location + "");
         var r = _.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -175,33 +175,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > a && !n : "" == d != n);
-                if ("u" == s) {
-                    if (!u || "u" != d) return !1
+                var f, d, s = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !u || ("u" == s ? l > a && !n : "" == s != n);
+                if ("u" == d) {
+                    if (!u || "u" != s) return !1
                 } else if (u)
-                    if (d == s)
+                    if (s == d)
                         if (l <= a) {
                             if (f != e[l]) return !1
                         } else {
                             if (n ? f > e[l] : f < e[l]) return !1;
                             f != e[l] && (u = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != s && "n" != s) {
                     if (n || l <= a) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= a || s < d != n) return !1;
+                    if (l <= a || d < s != n) return !1;
                     u = !1
-                } else "s" != d && "n" != d && (u = !1, l--)
+                } else "s" != s && "n" != s && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
@@ -213,32 +213,32 @@
         return t
     }, l = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", s = (e, r, t, a) => {
+    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", d = (e, r, t, a) => {
         var n = u(e, t);
         return o(a, n) || c(f(e, t, n, a)), v(e[t][n])
-    }, d = (e, r, t) => {
+    }, s = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, p = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + n(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, h = (e, r, t, a) => {
         c(p(e, r, t, a))
     }, v = e => (e.loaded = 1, e.get()), b = (m = e => function(r, t, a, n) {
         var o = _.I(r);
         return o && o.then ? o.then(e.bind(e, r, _.S[r], t, a, n)) : e(r, _.S[r], t, a, n)
-    })(((e, r, t, a) => (i(e, t), v(d(r, t, a) || h(r, e, t, a) || l(r, t))))), g = m(((e, r, t, a) => (i(e, t), s(r, 0, t, a)))), y = m(((e, r, t, a, n) => {
-        var o = r && _.o(r, t) && d(r, t, a);
+    })(((e, r, t, a) => (i(e, t), v(s(r, t, a) || h(r, e, t, a) || l(r, t))))), g = m(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), y = m(((e, r, t, a, n) => {
+        var o = r && _.o(r, t) && s(r, t, a);
         return o ? v(o) : n()
     })), w = {}, j = {
         3345: () => g("default", "react", [1, 18, 2, 0]),
         1527: () => g("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
         2774: () => b("default", "@jupyterlab/docregistry", [1, 4, 2, 0]),
         2825: () => g("default", "@jupyterlab/settingregistry", [1, 4, 2, 0]),
         3254: () => g("default", "@amphi/pipeline-components-manager", [0]),
```

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-editor/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.6/amphi/pipeline-editor/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/package.json` & `jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.7b90c2c5a47602453a70.js'}}",*

 * * "'version'": "'0.3.5'"}*

```diff
@@ -52,15 +52,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.432f146e752b80daa98d.js",
+            "load": "static/remoteEntry.7b90c2c5a47602453a70.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-log-console",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -99,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.4"
+    "version": "0.3.5"
 }
```

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/595.7fd40f4a8673fc24185a.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/595.7fd40f4a8673fc24185a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/595.7fd40f4a8673fc24185a.js.LICENSE.txt` & `jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/595.7fd40f4a8673fc24185a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/684.06766aa445a023bc4adf.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/684.06766aa445a023bc4adf.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/remoteEntry.432f146e752b80daa98d.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/remoteEntry.7b90c2c5a47602453a70.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -108,15 +108,15 @@
                     var o = i[e] = i[e] || {},
                         l = o[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : a > l.from)) && (o[r] = {
                         get: () => Promise.all([y.e(595), y.e(684)]).then((() => () => y(684))),
                         from: a,
                         eager: !1
                     })
-                })("@amphi/pipeline-log-console", "0.3.4"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@amphi/pipeline-log-console", "0.3.5"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-log-console/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.6/amphi/pipeline-log-console/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/package.json` & `jupyterlab_amphi-0.3.6/amphi/pipeline-components-core/package.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8869310897435897%*

 * *Differences: {"'author'": "{'email': ''}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.1.5', '@amphi/pipeline-components-manager': "*

 * *                   "'file:./../pipeline-components-manager', 'antd': '5.16.4', 'reactflow': "*

 * *                   "'11.9.4', delete: ['@amphi/pipeline-editor', '@jupyterlab/apputils', "*

 * *                   "'@jupyterlab/console', '@jupyterlab/coreutils', '@jupyterlab/notebook', "*

 * *                   "'@jupyterlab/outputarea', '@jupyterlab/rendermime', '@jupyterlab/services', "*

 * *        […]*

```diff
@@ -1,37 +1,25 @@
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
-        "@amphi/pipeline-editor": "file:./../pipeline-editor",
-        "@jupyterlab/application": "^4.0.0",
-        "@jupyterlab/apputils": "^4.0.0",
-        "@jupyterlab/console": "^4.0.0",
-        "@jupyterlab/coreutils": "^6.0.0",
-        "@jupyterlab/notebook": "^4.0.0",
-        "@jupyterlab/outputarea": "^4.0.0",
-        "@jupyterlab/rendermime": "^4.0.0",
-        "@jupyterlab/services": "^7.0.0",
-        "@jupyterlab/ui-components": "^4.0.0",
-        "@lumino/coreutils": "^2.0.0",
-        "@lumino/datagrid": "^2.0.0",
-        "@lumino/disposable": "^2.0.0",
-        "@lumino/signaling": "^2.0.0",
+        "@amphi/pipeline-components-manager": "file:./../pipeline-components-manager",
+        "@jupyterlab/application": "^4.1.5",
         "@lumino/widgets": "^2.0.0",
-        "react": "^18.2.0",
-        "wildcard-match": "^5.1.2"
+        "antd": "5.16.4",
+        "reactflow": "11.9.4"
     },
-    "description": "Amphi Metadata Panel",
+    "description": "Amphi Pipeline Core Components",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/builder": "^4.1.5",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
@@ -51,53 +39,53 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.da6df8ad6b7fdf2715dc.js",
+            "load": "static/remoteEntry.be309c73964f3370f798.js",
             "style": "./style"
         },
         "extension": true,
-        "outputDir": "../../amphi/pipeline-metadata-panel",
+        "outputDir": "../../amphi/pipeline-components-core",
         "sharedPackages": {
-            "@amphi/pipeline-editor": {
+            "@amphi/pipeline-components-manager": {
                 "bundled": false,
                 "singleton": true
             }
         }
     },
     "license": "Elastic License 2.0",
     "main": "lib/index.js",
-    "name": "@amphi/pipeline-metadata-panel",
+    "name": "@amphi/pipeline-components-core",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/amphi-ai/jupyterlab-amphi.git"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --build --verbose",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf ../../amphi/pipeline-metadata-panel",
+        "clean:labextension": "rimraf ../../amphi/labextension",
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
-    "version": "0.3.4"
+    "version": "0.3.5"
 }
```

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/732.1ea6cff032a5ee2821e8.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-metadata-panel/static/732.1ea6cff032a5ee2821e8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/remoteEntry.da6df8ad6b7fdf2715dc.js` & `jupyterlab_amphi-0.3.6/amphi/pipeline-metadata-panel/static/remoteEntry.4ab9bad57a24f62bae72.js`

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
-                })("@amphi/pipeline-metadata-panel", "0.3.4"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@amphi/pipeline-metadata-panel", "0.3.5"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_amphi-0.3.5/amphi/pipeline-metadata-panel/static/third-party-licenses.json` & `jupyterlab_amphi-0.3.6/amphi/pipeline-metadata-panel/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.3.6'"}*

```diff
@@ -94,9 +94,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.5"
+    "version": "0.3.6"
 }
```

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/tsconfig.json` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/BrowseFileDialog.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/BrowseFileDialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/CodeGenerator.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/CodeGenerator.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/CustomHandle.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/CustomHandle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/DndProviderWrapper.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/DndProviderWrapper.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/PipelineComponent.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/PipelineComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/PipelineService.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/PipelineService.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/RequestService.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/RequestService.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/configUtils.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/configUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/connectionUtils.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/connectionUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/generatorUtils.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/generatorUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/icons.ts` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/index.ts` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/rendererUtils.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/rendererUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/InputRegular.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/InputRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/connectionSelector.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/connectionSelector.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/dataMapping.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/dataMapping.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/keyValueForm.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/keyValueForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectColumn.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/selectColumn.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectColumns.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/selectColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectMultiple.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/selectMultiple.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectRegular.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/selectRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/selectTokenization.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/selectTokenization.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/transferData.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/transferData.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/src/forms/valuesListForm.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/src/forms/valuesListForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/settings-16.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/settings-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/settings-24.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/settings-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/trash-16.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/trash-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/trash-24.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/trash-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-components-manager/style/icons/x-square-16.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-components-manager/style/icons/x-square-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/package.json` & `jupyterlab_amphi-0.3.6/amphi/pipeline-editor/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940476190476191%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.4ff74fcef89bc3e36fe4.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}"}*

```diff
@@ -45,14 +45,19 @@
         "lib/*.js.map",
         "lib/*.js",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.4ff74fcef89bc3e36fe4.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "../../amphi/pipeline-editor",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
                 "singleton": true
             },
```

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/pipeline-16.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/pipeline-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/pipeline-24.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/pipeline-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/tsconfig.json` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/schema/plugin copy.json` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/schema/plugin copy.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/schema/plugin.json` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/Dropzone.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/src/Dropzone.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/PipelineEditorWidget.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/src/PipelineEditorWidget.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -435,17 +435,17 @@
   // Output tree data (for debugging, you might want to console.log or use it directly in your components)
   console.log(treeData);
 
     return (
 
       <aside className={sidebarClass} title={'Components'}>
         
-        <div className="description">
+        <div className="description" style={{ textAlign: 'center', fontWeight: 'bold', marginBottom: '16px' }}>
           <extensionIcon.react tag="span" width="24px" float="left" marginRight="8px" />
-          Drag and drop components.
+          Drag and drop components in the canvas
         </div>
        
         <DirectoryTree
           selectable={false}
           multiple
           blockNode
           defaultExpandAll
```

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/customEdge.tsx` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/src/customEdge.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/icons.ts` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/src/index.ts` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/canvas.css` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/canvas.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/output.css` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/output.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/pipeline-category-icon.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/pipeline-category-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/react-icon.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/react-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/api-24.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/icons/api-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/file-plus-24.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/icons/file-plus-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/file-text-24.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/icons/file-text-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/pipeline-brand-16.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/icons/pipeline-brand-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/packages/pipeline-editor/style/icons/pipeline-brand-24.svg` & `jupyterlab_amphi-0.3.6/packages/pipeline-editor/style/icons/pipeline-brand-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/LICENSE` & `jupyterlab_amphi-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/README.md` & `jupyterlab_amphi-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/pyproject.toml` & `jupyterlab_amphi-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.5/PKG-INFO` & `jupyterlab_amphi-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-amphi
-Version: 0.3.5
+Version: 0.3.6
 Dynamic: Keywords
 Summary: Amphi is a micro ETL for Jupyterlab.
 Project-URL: Homepage, https://amphi.ai
 Project-URL: Bug Tracker, https://github.com/amphi-ai/jupyterlab-amphi/issues
 Project-URL: Repository, https://github.com/amphi-ai/jupyterlab-amphi.git
 Author-email: Thibaut Gourdel <tgourdel@amphi.ai>
 License: Elastic License 2.0 \(ELv2\)
```


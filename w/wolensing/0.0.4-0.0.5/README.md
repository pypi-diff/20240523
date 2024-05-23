# Comparing `tmp/wolensing-0.0.4.tar.gz` & `tmp/wolensing-0.0.5.tar.gz`

## Comparing `wolensing-0.0.4.tar` & `wolensing-0.0.5.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rwxr-xr-x   0        0        0     1063 2020-02-02 00:00:00.000000 wolensing-0.0.4/.readthedocs.yaml
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 wolensing-0.0.4/CITATION.cff
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 wolensing-0.0.4/requirements.txt
--rwxr-xr-x   0        0        0     1299 2020-02-02 00:00:00.000000 wolensing-0.0.4/.github/workflows/pytest.yaml
--rwxr-xr-x   0        0        0     2242 2020-02-02 00:00:00.000000 wolensing-0.0.4/.github/workflows/testPyPl.yml
--rwxr-xr-x   0        0        0      742 2020-02-02 00:00:00.000000 wolensing-0.0.4/.github/workflows/workflowsjoss.yml
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 wolensing-0.0.4/build/lib/wolensing/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.4/build/lib/wolensing/amplification_factor/__init__.py
--rwxr-xr-x   0        0        0    12018 2020-02-02 00:00:00.000000 wolensing-0.0.4/build/lib/wolensing/amplification_factor/amplification_factor.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.4/build/lib/wolensing/lensmodels/__init__.py
--rwxr-xr-x   0        0        0     1977 2020-02-02 00:00:00.000000 wolensing-0.0.4/build/lib/wolensing/lensmodels/hessian.py
--rwxr-xr-x   0        0        0     4989 2020-02-02 00:00:00.000000 wolensing-0.0.4/build/lib/wolensing/lensmodels/lens.py
--rwxr-xr-x   0        0        0     1867 2020-02-02 00:00:00.000000 wolensing-0.0.4/build/lib/wolensing/lensmodels/potential.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.4/build/lib/wolensing/plot/__init__.py
--rwxr-xr-x   0        0        0     2056 2020-02-02 00:00:00.000000 wolensing-0.0.4/build/lib/wolensing/plot/plot.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.4/build/lib/wolensing/utils/__init__.py
--rwxr-xr-x   0        0        0     5396 2020-02-02 00:00:00.000000 wolensing-0.0.4/build/lib/wolensing/utils/histogram.py
--rwxr-xr-x   0        0        0     4790 2020-02-02 00:00:00.000000 wolensing-0.0.4/build/lib/wolensing/utils/utils.py
--rwxr-xr-x   0        0        0      638 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/make.bat
--rwxr-xr-x   0        0        0       76 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/requirements.txt
--rwxr-xr-x   0        0        0     3752 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/doctrees/amplification_factor.doctree
--rwxr-xr-x   0        0        0   192916 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/doctrees/environment.pickle
--rwxr-xr-x   0        0        0     9500 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/doctrees/index.doctree
--rwxr-xr-x   0        0        0    54593 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/doctrees/lensmodels.doctree
--rwxr-xr-x   0        0        0     2826 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/doctrees/modules.doctree
--rwxr-xr-x   0        0        0    14678 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/doctrees/plot.doctree
--rwxr-xr-x   0        0        0    27145 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/doctrees/utils.doctree
--rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/.buildinfo
--rwxr-xr-x   0        0        0     5651 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/amplification_factor.html
--rwxr-xr-x   0        0        0     9715 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/genindex.html
--rwxr-xr-x   0        0        0     9425 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/index.html
--rwxr-xr-x   0        0        0    25707 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/lensmodels.html
--rwxr-xr-x   0        0        0     9423 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/modules.html
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/objects.inv
--rwxr-xr-x   0        0        0     8949 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/plot.html
--rwxr-xr-x   0        0        0     6621 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/py-modindex.html
--rwxr-xr-x   0        0        0     4108 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/search.html
--rwxr-xr-x   0        0        0     9043 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/searchindex.js
--rwxr-xr-x   0        0        0    12842 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/utils.html
--rwxr-xr-x   0        0        0     4106 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_modules/index.html
--rwxr-xr-x   0        0        0    56945 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_modules/amplification_factor/amplification_factor.html
--rwxr-xr-x   0        0        0    12221 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_modules/lensmodels/hessian.html
--rwxr-xr-x   0        0        0    30105 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_modules/lensmodels/lens.html
--rwxr-xr-x   0        0        0    12130 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_modules/lensmodels/potential.html
--rwxr-xr-x   0        0        0    11119 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_modules/plot/plot.html
--rwxr-xr-x   0        0        0    24149 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_modules/utils/histogram.html
--rwxr-xr-x   0        0        0      424 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_sources/amplification_factor.rst.txt
--rwxr-xr-x   0        0        0      491 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_sources/index.rst.txt
--rwxr-xr-x   0        0        0      602 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_sources/lensmodels.rst.txt
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_sources/modules.rst.txt
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_sources/plot.rst.txt
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_sources/utils.rst.txt
--rwxr-xr-x   0        0        0     4289 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rwxr-xr-x   0        0        0    15094 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/basic.css
--rwxr-xr-x   0        0        0     4472 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/doctools.js
--rwxr-xr-x   0        0        0      328 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/documentation_options.js
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/file.png
--rwxr-xr-x   0        0        0    89501 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/jquery.js
--rwxr-xr-x   0        0        0     4758 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/language_data.js
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/minus.png
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/plus.png
--rwxr-xr-x   0        0        0     4902 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/pygments.css
--rwxr-xr-x   0        0        0    18732 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/searchtools.js
--rwxr-xr-x   0        0        0     5123 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/sphinx_highlight.js
--rwxr-xr-x   0        0        0     3229 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/badge_only.css
--rwxr-xr-x   0        0        0   135314 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/theme.css
--rwxr-xr-x   0        0        0    87624 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rwxr-xr-x   0        0        0    67312 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rwxr-xr-x   0        0        0    86288 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rwxr-xr-x   0        0        0    66444 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rwxr-xr-x   0        0        0   165742 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rwxr-xr-x   0        0        0   444379 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rwxr-xr-x   0        0        0   165548 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rwxr-xr-x   0        0        0    98024 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rwxr-xr-x   0        0        0    77160 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rwxr-xr-x   0        0        0   323344 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rwxr-xr-x   0        0        0   193308 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rwxr-xr-x   0        0        0   309728 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-bold.woff
--rwxr-xr-x   0        0        0   184912 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-bold.woff2
--rwxr-xr-x   0        0        0   328412 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rwxr-xr-x   0        0        0   195704 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rwxr-xr-x   0        0        0   309192 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-normal.woff
--rwxr-xr-x   0        0        0   182708 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-normal.woff2
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/js/badge_only.js
--rwxr-xr-x   0        0        0     4370 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rwxr-xr-x   0        0        0     2734 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/js/html5shiv.min.js
--rwxr-xr-x   0        0        0     5023 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/build/html/_static/js/theme.js
--rwxr-xr-x   0        0        0      424 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/source/amplification_factor.rst
--rwxr-xr-x   0        0        0     2109 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/source/conf.py
--rwxr-xr-x   0        0        0      491 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/source/index.rst
--rwxr-xr-x   0        0        0      602 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/source/lensmodels.rst
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/source/modules.rst
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/source/plot.rst
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 wolensing-0.0.4/docs/source/utils.rst
--rwxr-xr-x   0        0        0     4838 2020-02-02 00:00:00.000000 wolensing-0.0.4/paper/paper.bib
--rwxr-xr-x   0        0        0     4783 2020-02-02 00:00:00.000000 wolensing-0.0.4/paper/paper.md
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.4/test/__init__.py
--rwxr-xr-x   0        0        0     3289 2020-02-02 00:00:00.000000 wolensing-0.0.4/test/amplification_factor_test.py
--rwxr-xr-x   0        0        0     2213 2020-02-02 00:00:00.000000 wolensing-0.0.4/test/conftest.py
--rwxr-xr-x   0        0        0   324975 2020-02-02 00:00:00.000000 wolensing-0.0.4/test/test_sis_F_tilde.txt
--rwxr-xr-x   0        0        0  1094040 2020-02-02 00:00:00.000000 wolensing-0.0.4/test/test_sis_Fws.txt
--rwxr-xr-x   0        0        0   324975 2020-02-02 00:00:00.000000 wolensing-0.0.4/test/test_sis_ts.txt
--rwxr-xr-x   0        0        0   506500 2020-02-02 00:00:00.000000 wolensing-0.0.4/test/test_sis_ws.txt
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/amplification_factor/__init__.py
--rwxr-xr-x   0        0        0    11862 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/amplification_factor/amplification_factor.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/lensmodels/__init__.py
--rwxr-xr-x   0        0        0     1961 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/lensmodels/hessian.py
--rwxr-xr-x   0        0        0     4989 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/lensmodels/lens.py
--rwxr-xr-x   0        0        0     1867 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/lensmodels/potential.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/plot/__init__.py
--rwxr-xr-x   0        0        0     2056 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/plot/plot.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/utils/__init__.py
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/utils/constants.py
--rwxr-xr-x   0        0        0     5396 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/utils/histogram.py
--rwxr-xr-x   0        0        0     5931 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing/utils/utils.py
--rwxr-xr-x   0        0        0     1991 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing.egg-info/PKG-INFO
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing.egg-info/SOURCES.txt
--rwxr-xr-x   0        0        0        1 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing.egg-info/dependency_links.txt
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing.egg-info/requires.txt
--rwxr-xr-x   0        0        0       10 2020-02-02 00:00:00.000000 wolensing-0.0.4/wolensing.egg-info/top_level.txt
--rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 wolensing-0.0.4/.gitignore
--rwxr-xr-x   0        0        0     1078 2020-02-02 00:00:00.000000 wolensing-0.0.4/LICENSE
--rwxr-xr-x   0        0        0     1118 2020-02-02 00:00:00.000000 wolensing-0.0.4/README.rst
--rwxr-xr-x   0        0        0      902 2020-02-02 00:00:00.000000 wolensing-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 wolensing-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wolensing-0.0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 wolensing-0.0.5/CITATION.cff
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wolensing-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 wolensing-0.0.5/.github/workflows/pytest.yaml
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 wolensing-0.0.5/.github/workflows/testPyPl.yml
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 wolensing-0.0.5/.github/workflows/workflowsjoss.yml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 wolensing-0.0.5/build/lib/wolensing/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.5/build/lib/wolensing/amplification_factor/__init__.py
+-rw-r--r--   0        0        0    12018 2020-02-02 00:00:00.000000 wolensing-0.0.5/build/lib/wolensing/amplification_factor/amplification_factor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.5/build/lib/wolensing/lensmodels/__init__.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 wolensing-0.0.5/build/lib/wolensing/lensmodels/hessian.py
+-rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 wolensing-0.0.5/build/lib/wolensing/lensmodels/lens.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 wolensing-0.0.5/build/lib/wolensing/lensmodels/potential.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.5/build/lib/wolensing/plot/__init__.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 wolensing-0.0.5/build/lib/wolensing/plot/plot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.5/build/lib/wolensing/utils/__init__.py
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 wolensing-0.0.5/build/lib/wolensing/utils/histogram.py
+-rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 wolensing-0.0.5/build/lib/wolensing/utils/utils.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/make.bat
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/requirements.txt
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/doctrees/amplification_factor.doctree
+-rw-r--r--   0        0        0   192916 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/doctrees/index.doctree
+-rw-r--r--   0        0        0    54593 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/doctrees/lensmodels.doctree
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/doctrees/modules.doctree
+-rw-r--r--   0        0        0    14678 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/doctrees/plot.doctree
+-rw-r--r--   0        0        0    27145 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/doctrees/utils.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/amplification_factor.html
+-rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     9425 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/index.html
+-rw-r--r--   0        0        0    25707 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/lensmodels.html
+-rw-r--r--   0        0        0     9423 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/modules.html
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     8949 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/plot.html
+-rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/search.html
+-rw-r--r--   0        0        0     9043 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    12842 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/utils.html
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_modules/index.html
+-rw-r--r--   0        0        0    56945 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_modules/amplification_factor/amplification_factor.html
+-rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_modules/lensmodels/hessian.html
+-rw-r--r--   0        0        0    30105 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_modules/lensmodels/lens.html
+-rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_modules/lensmodels/potential.html
+-rw-r--r--   0        0        0    11119 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_modules/plot/plot.html
+-rw-r--r--   0        0        0    24149 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_modules/utils/histogram.html
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_sources/amplification_factor.rst.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_sources/lensmodels.rst.txt
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_sources/plot.rst.txt
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_sources/utils.rst.txt
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/source/amplification_factor.rst
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/source/conf.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/source/index.rst
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/source/lensmodels.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/source/modules.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/source/plot.rst
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 wolensing-0.0.5/docs/source/utils.rst
+-rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 wolensing-0.0.5/paper/paper.bib
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 wolensing-0.0.5/paper/paper.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.5/test/__init__.py
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 wolensing-0.0.5/test/amplification_factor_test.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 wolensing-0.0.5/test/conftest.py
+-rw-r--r--   0        0        0   324975 2020-02-02 00:00:00.000000 wolensing-0.0.5/test/test_sis_F_tilde.txt
+-rw-r--r--   0        0        0  1094040 2020-02-02 00:00:00.000000 wolensing-0.0.5/test/test_sis_Fws.txt
+-rw-r--r--   0        0        0   324975 2020-02-02 00:00:00.000000 wolensing-0.0.5/test/test_sis_ts.txt
+-rw-r--r--   0        0        0   506500 2020-02-02 00:00:00.000000 wolensing-0.0.5/test/test_sis_ws.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/amplification_factor/__init__.py
+-rw-r--r--   0        0        0    12223 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/amplification_factor/amplification_factor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/lensmodels/__init__.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/lensmodels/hessian.py
+-rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/lensmodels/lens.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/lensmodels/potential.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/plot/__init__.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/plot/plot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/utils/__init__.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/utils/constants.py
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/utils/histogram.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing/utils/utils.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing.egg-info/requires.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 wolensing-0.0.5/wolensing.egg-info/top_level.txt
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wolensing-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 wolensing-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 wolensing-0.0.5/README.rst
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 wolensing-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 wolensing-0.0.5/PKG-INFO
```

### Comparing `wolensing-0.0.4/.readthedocs.yaml` & `wolensing-0.0.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/.github/workflows/pytest.yaml` & `wolensing-0.0.5/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/.github/workflows/testPyPl.yml` & `wolensing-0.0.5/.github/workflows/testPyPl.yml`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/.github/workflows/workflowsjoss.yml` & `wolensing-0.0.5/.github/workflows/workflowsjoss.yml`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/build/lib/wolensing/amplification_factor/amplification_factor.py` & `wolensing-0.0.5/build/lib/wolensing/amplification_factor/amplification_factor.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/build/lib/wolensing/lensmodels/hessian.py` & `wolensing-0.0.5/build/lib/wolensing/lensmodels/hessian.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/build/lib/wolensing/lensmodels/lens.py` & `wolensing-0.0.5/build/lib/wolensing/lensmodels/lens.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/build/lib/wolensing/lensmodels/potential.py` & `wolensing-0.0.5/build/lib/wolensing/lensmodels/potential.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/build/lib/wolensing/plot/plot.py` & `wolensing-0.0.5/build/lib/wolensing/plot/plot.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/build/lib/wolensing/utils/histogram.py` & `wolensing-0.0.5/build/lib/wolensing/utils/histogram.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/build/lib/wolensing/utils/utils.py` & `wolensing-0.0.5/build/lib/wolensing/utils/utils.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/Makefile` & `wolensing-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/make.bat` & `wolensing-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/doctrees/amplification_factor.doctree` & `wolensing-0.0.5/docs/build/doctrees/amplification_factor.doctree`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/doctrees/environment.pickle` & `wolensing-0.0.5/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/doctrees/index.doctree` & `wolensing-0.0.5/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/doctrees/lensmodels.doctree` & `wolensing-0.0.5/docs/build/doctrees/lensmodels.doctree`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/doctrees/modules.doctree` & `wolensing-0.0.5/docs/build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/doctrees/plot.doctree` & `wolensing-0.0.5/docs/build/doctrees/plot.doctree`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/doctrees/utils.doctree` & `wolensing-0.0.5/docs/build/doctrees/utils.doctree`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/amplification_factor.html` & `wolensing-0.0.5/docs/build/html/amplification_factor.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/genindex.html` & `wolensing-0.0.5/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/index.html` & `wolensing-0.0.5/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/lensmodels.html` & `wolensing-0.0.5/docs/build/html/lensmodels.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/modules.html` & `wolensing-0.0.5/docs/build/html/modules.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/objects.inv` & `wolensing-0.0.5/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/plot.html` & `wolensing-0.0.5/docs/build/html/plot.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/py-modindex.html` & `wolensing-0.0.5/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/search.html` & `wolensing-0.0.5/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/searchindex.js` & `wolensing-0.0.5/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/utils.html` & `wolensing-0.0.5/docs/build/html/utils.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_modules/index.html` & `wolensing-0.0.5/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_modules/amplification_factor/amplification_factor.html` & `wolensing-0.0.5/docs/build/html/_modules/amplification_factor/amplification_factor.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_modules/lensmodels/hessian.html` & `wolensing-0.0.5/docs/build/html/_modules/lensmodels/hessian.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_modules/lensmodels/lens.html` & `wolensing-0.0.5/docs/build/html/_modules/lensmodels/lens.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_modules/lensmodels/potential.html` & `wolensing-0.0.5/docs/build/html/_modules/lensmodels/potential.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_modules/plot/plot.html` & `wolensing-0.0.5/docs/build/html/_modules/plot/plot.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_modules/utils/histogram.html` & `wolensing-0.0.5/docs/build/html/_modules/utils/histogram.html`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_sources/lensmodels.rst.txt` & `wolensing-0.0.5/docs/build/html/_sources/lensmodels.rst.txt`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `wolensing-0.0.5/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/basic.css` & `wolensing-0.0.5/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/doctools.js` & `wolensing-0.0.5/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/jquery.js` & `wolensing-0.0.5/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/language_data.js` & `wolensing-0.0.5/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/pygments.css` & `wolensing-0.0.5/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/searchtools.js` & `wolensing-0.0.5/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/sphinx_highlight.js` & `wolensing-0.0.5/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/badge_only.css` & `wolensing-0.0.5/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/theme.css` & `wolensing-0.0.5/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-bold.woff` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-bold.woff2` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-normal.woff` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/css/fonts/lato-normal.woff2` & `wolensing-0.0.5/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/js/badge_only.js` & `wolensing-0.0.5/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `wolensing-0.0.5/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/js/html5shiv.min.js` & `wolensing-0.0.5/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/build/html/_static/js/theme.js` & `wolensing-0.0.5/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/source/conf.py` & `wolensing-0.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/docs/source/lensmodels.rst` & `wolensing-0.0.5/docs/source/lensmodels.rst`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/paper/paper.bib` & `wolensing-0.0.5/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/paper/paper.md` & `wolensing-0.0.5/paper/paper.md`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/test/amplification_factor_test.py` & `wolensing-0.0.5/test/amplification_factor_test.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/test/conftest.py` & `wolensing-0.0.5/test/conftest.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/test/test_sis_F_tilde.txt` & `wolensing-0.0.5/test/test_sis_F_tilde.txt`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/test/test_sis_Fws.txt` & `wolensing-0.0.5/test/test_sis_Fws.txt`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/test/test_sis_ts.txt` & `wolensing-0.0.5/test/test_sis_ts.txt`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/test/test_sis_ws.txt` & `wolensing-0.0.5/test/test_sis_ws.txt`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/wolensing/amplification_factor/amplification_factor.py` & `wolensing-0.0.5/wolensing/amplification_factor/amplification_factor.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,20 @@
         bincountfront = np.trim_zeros(bincount, 'b')
         fronttrimmed = len(bincount) - len(bincountback)
         backtrimmed = len(bincount) - len(bincountfront) + 1
         self._F_tilde = bincount[fronttrimmed:-backtrimmed] / (2 * np.pi * binwidth) / thetaE ** 2
         self._ts = bins[fronttrimmed:-backtrimmed] - bins[fronttrimmed]
         if binnumlength < len(self._ts):
             self._ts, self._F_tilde = self._ts[:binnumlength], self._F_tilde[:binnumlength]
+
+        import jax.numpy as jnp
+        if isinstance(self._ts, jnp.ndarray):
+            self._ts = np.array(self._ts)
+            self._F_tilde = np.array(self._F_tilde)
+
         return self._ts, self._F_tilde
 
     def fourier(self, freq_end=2000, type2=False):
         """
         Compute the amplification factor in frequency domain
 
         :param freq_end: higher end of the frequency series. Default to be 2000.
@@ -266,15 +272,15 @@
 
         if saveplot != None:
             plt.savefig(saveplot)
 
         plt.show()
         return ax 
 
-    def geometrical_optics(self, mus, tds, Img_ra, Img_dec, upper_lim = 3000):
+    def geometrical_optics(self, mus, tds, Img_ra, Img_dec, upper_lim = 3000, type2 = False):
         """
         :param mus: magnifications of images.
         :param tds: time delays of images.
         :param Img_ra: right ascension of images relative to the center of lens plane.
         :param Img_dec: declination of images relative to the center of lens plane.
         :param upper_lim: desired upper limit of freqeuncy range of geometrical optics.
         :return: frequency array and amplification factor F(f) of geometrical optics.
@@ -283,14 +289,19 @@
         fs_grid = fs[1]-fs[0]
         
         num_interp = int((upper_lim-fs[0])/fs_grid) 
         self._geofs = np.linspace(fs[0], upper_lim, num_interp)
         
         ns = Morse_indices(self._lens_model_list, Img_ra, Img_dec, self._kwargs_lens)
         self._geoFws = compute_geometrical(self._geofs, mus, tds, ns)
+
+        if type2:
+            index = np.argmin(tds)
+            overall_phase = np.exp(-1 * 2 * np.pi * 1j * (tds[index]) * fs)
+            self._geoFws *= overall_phase
         
         return self._geofs, self._geoFws
     
     def concatenate(self, transfreq = 1000):
         """
         :param transfreq: transitional frequency of wave optics to geometrical optics.
         :return: concatenated frequency array and amplification factor F(f).
```

### Comparing `wolensing-0.0.4/wolensing/lensmodels/hessian.py` & `wolensing-0.0.5/wolensing/lensmodels/hessian.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/wolensing/lensmodels/lens.py` & `wolensing-0.0.5/wolensing/lensmodels/lens.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/wolensing/lensmodels/potential.py` & `wolensing-0.0.5/wolensing/lensmodels/potential.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/wolensing/plot/plot.py` & `wolensing-0.0.5/wolensing/plot/plot.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/wolensing/utils/histogram.py` & `wolensing-0.0.5/wolensing/utils/histogram.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/wolensing/utils/utils.py` & `wolensing-0.0.5/wolensing/utils/utils.py`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/wolensing.egg-info/PKG-INFO` & `wolensing-0.0.5/wolensing.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/LICENSE` & `wolensing-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/README.rst` & `wolensing-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `wolensing-0.0.4/pyproject.toml` & `wolensing-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [project]
-version = "0.0.4"
+version = "0.0.5"
 name = "wolensing"
 authors = [
   { name="Simon Man-Chun Yeung, Mark Ho-Yeuk Cheung", email="yeungm@uwm.edu" },
 ]
 description = "A package for computing wave optics amplification factor."
 readme = "README.rst"
 requires-python = ">=3.6,<3.12"
```

### Comparing `wolensing-0.0.4/PKG-INFO` & `wolensing-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wolensing
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for computing wave optics amplification factor.
 Project-URL: Homepage, https://github.com/manchunyeung/wolensing
 Author-email: "Simon Man-Chun Yeung, Mark Ho-Yeuk Cheung" <yeungm@uwm.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/portrait-0.0.1b0.tar.gz` & `tmp/portrait-0.0.2b0.tar.gz`

## Comparing `portrait-0.0.1b0.tar` & `portrait-0.0.2b0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 portrait-0.0.1b0/CITATION.cff
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 portrait-0.0.1b0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 portrait-0.0.1b0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 portrait-0.0.1b0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 portrait-0.0.1b0/docs/Makefile
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 portrait-0.0.1b0/docs/acknowledgement.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 portrait-0.0.1b0/docs/api.rst
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 portrait-0.0.1b0/docs/conf.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 portrait-0.0.1b0/docs/index.md
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 portrait-0.0.1b0/docs/installation.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 portrait-0.0.1b0/docs/make.bat
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 portrait-0.0.1b0/docs/_static/style.css
--rw-r--r--   0        0        0    50947 2020-02-02 00:00:00.000000 portrait-0.0.1b0/docs/ipynb/coverage.ipynb
--rw-r--r--   0        0        0    23560 2020-02-02 00:00:00.000000 portrait-0.0.1b0/docs/ipynb/periodmatch.ipynb
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 portrait-0.0.1b0/portrait/__init__.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 portrait-0.0.1b0/portrait/main.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 portrait-0.0.1b0/tests/test_all.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 portrait-0.0.1b0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 portrait-0.0.1b0/LICENSE
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 portrait-0.0.1b0/README.md
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 portrait-0.0.1b0/pyproject.toml
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 portrait-0.0.1b0/PKG-INFO
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 portrait-0.0.2b0/.readthedocs.yaml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 portrait-0.0.2b0/CITATION.cff
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 portrait-0.0.2b0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 portrait-0.0.2b0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 portrait-0.0.2b0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 portrait-0.0.2b0/.vscode/settings.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 portrait-0.0.2b0/docs/Makefile
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 portrait-0.0.2b0/docs/acknowledgement.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 portrait-0.0.2b0/docs/api.rst
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 portrait-0.0.2b0/docs/conf.py
+-rw-r--r--   0        0        0    48046 2020-02-02 00:00:00.000000 portrait-0.0.2b0/docs/coverage.ipynb
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 portrait-0.0.2b0/docs/index.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 portrait-0.0.2b0/docs/installation.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 portrait-0.0.2b0/docs/make.bat
+-rw-r--r--   0        0        0    23560 2020-02-02 00:00:00.000000 portrait-0.0.2b0/docs/periodmatch.ipynb
+-rw-r--r--   0        0        0    53092 2020-02-02 00:00:00.000000 portrait-0.0.2b0/docs/tess.ipynb
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 portrait-0.0.2b0/portrait/__init__.py
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 portrait-0.0.2b0/portrait/core.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 portrait-0.0.2b0/tests/test_all.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 portrait-0.0.2b0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 portrait-0.0.2b0/LICENSE
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 portrait-0.0.2b0/README.md
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 portrait-0.0.2b0/pyproject.toml
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 portrait-0.0.2b0/PKG-INFO
```

### Comparing `portrait-0.0.1b0/CITATION.cff` & `portrait-0.0.2b0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `portrait-0.0.1b0/CODE_OF_CONDUCT.md` & `portrait-0.0.2b0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `portrait-0.0.1b0/CONTRIBUTING.md` & `portrait-0.0.2b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `portrait-0.0.1b0/.github/workflows/publish.yaml` & `portrait-0.0.2b0/.github/workflows/ci.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Build and publish
+name: Build, test and publish
 
 on:
   push:
     branches:
       - main
     tags:
       - "*"
@@ -26,21 +26,36 @@
           python -m pip install -U pip
           python -m pip install -U build
           python -m build .
       - uses: actions/upload-artifact@v4
         with:
           path: dist/*
 
+  test:
+    runs-on: ubuntu-latest
+    needs: [build]
+    steps:
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
+        with:
+          python-version: "3.10"
+      - name: Install dependencies
+        run: python -m pip install -U pip
+      - name: Install package and test dependencies
+        run: python -m pip install ".[dev]"
+      - name: Run tests
+        run: python -m pytest
+
   publish:
     environment:
       name: pypi
       url: https://pypi.org/p/portrait
     permissions:
       id-token: write
-    needs: [build]
+    needs: [test]
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/')
     steps:
       - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
```

### Comparing `portrait-0.0.1b0/docs/Makefile` & `portrait-0.0.2b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `portrait-0.0.1b0/docs/conf.py` & `portrait-0.0.2b0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,11 +70,9 @@
 ]
 
 templates_path = ["_templates"]
 nb_execution_mode = "cache"
 nb_execution_raise_on_error = True
 nb_execution_timeout = 60
 
-html_css_files = ["style.css"]
-
 autodoc_typehints = "signature"
 autoclass_content = "both"
```

### Comparing `portrait-0.0.1b0/docs/index.md` & `portrait-0.0.2b0/docs/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # portrait
 
 A Python package to compute and visualize observation metrics for periodic events. In Astronomy, *portrait* is useful to answer the following questions:
-- How much of an orbit with period $P$ has been observed given certain observation times? ([tutorial](ipynb/coverage))
-- What period $P$ matches with this list of events? ([tutorial](ipynb/periodmatch))
+- How much of an orbit with period $P$ has been observed given certain observation times? ([tutorial](coverage))
+- What period $P$ matches with this list of events? ([tutorial](periodmatch))
 - How a certain target must be observed to cover all orbits with periods lower than $P$ days? 
 
 ## Table of content
 ```{toctree}
 :maxdepth: 0
 :caption: Get started
 
@@ -14,16 +14,17 @@
 acknowledgement
 ```
 
 ```{toctree}
 :maxdepth: 0
 :caption: Tutorials
 
-ipynb/periodmatch
-ipynb/coverage
+periodmatch
+coverage
+tess
 ```
 
 ```{toctree}
 :maxdepth: 0
 :caption: Reference
 
 api.rst
```

### Comparing `portrait-0.0.1b0/docs/make.bat` & `portrait-0.0.2b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `portrait-0.0.1b0/docs/ipynb/periodmatch.ipynb` & `portrait-0.0.2b0/docs/periodmatch.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9939194775132275%*

 * *Differences: {"'cells'": "{3: {'execution_count': 1, 'source': {insert: [(4, 't0s = "*

 * *            "np.random.choice(np.arange(50) * true_period, size=6)\\n')], delete: [4]}}, 5: "*

 * *            "{'execution_count': 2}, 7: {'execution_count': 3, 'outputs': {1: {'data': "*

 * *            "{'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAAioAAAGwCAYAAACHJU4LAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjkuMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy80BEi2AAAACXBIWXMAAA9hAAAPYQGoP6dpAAA73UlEQVR4nO3deXhU5f3//9ckJCFAEmQJawAtoqCGHURQU […]*

```diff
@@ -24,15 +24,15 @@
                 "## Data simulation\n",
                 "\n",
                 "We simulate a list of times and only pick few of them to represent a sparse observation of a certain event (such as an exoplanet transit)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[46.892 34.552 17.276 51.828  8.638 24.68 ]\n"
@@ -40,15 +40,15 @@
                 }
             ],
             "source": [
                 "import numpy as np\n",
                 "\n",
                 "true_period = 1.23400\n",
                 "np.random.seed(42)\n",
-                "t0s = np.random.choice(np.arange(50)*true_period, size=6)\n",
+                "t0s = np.random.choice(np.arange(50) * true_period, size=6)\n",
                 "print(t0s)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -56,15 +56,15 @@
                 "## Finding optimal period\n",
                 "\n",
                 "We can then try to match these events with a range of periods"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from portrait import period_match\n",
                 "\n",
                 "periods = np.linspace(0.2, 5, 1000000)\n",
                 "\n",
@@ -76,28 +76,28 @@
             "metadata": {},
             "source": [
                 "And plot the results"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "true: 1.2340\n",
                         "found: 1.2340\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAioAAAGwCAYAAACHJU4LAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAAA73UlEQVR4nO3deXhU5f3//9ckJCFAEmQJawAtoqCGHURQUXFBpVJb9eePyvJR+8EGAREXbBW3GqzVDyhK1VpxQ7QqamXXChEru2GXTZCwBhGyQkJm5vsHMmaSSTL7uWfm+biuXFdm5sw57zln5pzX3Oee+9icTqdTAAAABoqzugAAAICaEFQAAICxCCoAAMBYBBUAAGAsggoAADAWQQUAABiLoAIAAIxVz+oCAuFwOLR//36lpKTIZrNZXQ4AAPCC0+lUUVGRWrdurbi42ttMIjqo7N+/XxkZGVaXAQAA/JCXl6e2bdvWOk1EB5WUlBRJp15oamqqxdUgmOx2uxYtWiRJuuqqqxQfH29xRQCAYCksLFRGRobrOF6biA4qp0/3pKamElSijN1uV4MGDSSd2r4EFQCIPt5026AzLQAAMBZBBQAAGIugAgAAjBXRfVQAAGaz2+06efKk1WUgzBISEoLWt5CgAgAIOqfTqYMHD+rYsWNWlwKLNG7cWC1btgx4nDOCCgAg6E6HlPT0dDVo0IBBOWOI0+lUaWmp8vPzJUmtWrUKaH4EFQBAUNntdldIadq0qdXlwALJycmSpPz8fKWnpwd0GojOtACAoDrdJ+X0WEiITae3f6B9lAgqAICQ4HRPbAvW9ieoAAAAY1keVPbt26ff//73atq0qZKTk3XBBRdo9erVVpcFAAAMYGlQOXr0qPr376+EhATNnz9fmzdv1rPPPqszzjjDyrIAAIhau3fvls1mU25ubkDzGThwoMaPHx+Ummpj6a9+nn76aWVkZOj111933XfmmWdaWNEvnE6nyiocqp9wqqey3eFUhcOhpHruPZdPnLQrMT5OcXG1n4s7Xm5XcmJwBr/xdpmRrtwuJVje5gcglgwcOFDdunXT1KlTrS4lZDIyMnTgwAE1a9bM6lK8Yulh4NNPP1WvXr100003KT09Xd27d9err75a4/RlZWUqLCx0+wuVrFlrde7DC/TDkRJJ0pAXlumCyYtUUlbhmqboxEmdP3mhfv3islrn9dn6/er8yAK9tmxXwHUVHD+pzo8s0G///t+A52WyH4vLdO/yOE3fFN1hDEBkcTqdqqioqHtCQ5WXlys+Pl4tW7ZUvXqRMUKJpUHl+++/14wZM3T22Wdr4cKFuuuuuzR27Fi98cYbHqfPzs5WWlqa6y8jIyNktc3bcFCS9M6KPZKkzQcKVW53aO2eo65pvtl5RBUOpzbuqz0wjX33W0nSE59tDriunG2H5XRK3+45FvC8TDZ/46n1v62AoAJEC7vdbsmft0aOHKmlS5dq2rRpstlsstlsmjlzpmw2m+bPn6+ePXsqKSlJy5Yt08iRIzV06FC3548fP14DBw503XY4HMrOztaZZ56p5ORkde3aVR988IFXtSxZskQ2m01z585VZmam6tevrwsvvFAbN250m27ZsmW6+OKLlZycrIyMDI0dO1YlJSWuxzt06KAnnnhCw4cPV2pqqv7whz94PPWzdOlS9enTR0lJSWrVqpUefPBBt0BWUlKi4cOHq1GjRmrVqpWeffZZr9droCyNUw6HQ7169dJTTz0lSerevbs2btyov//97xoxYkS16SdNmqQJEya4bhcWFoY0rAAAgsNut2vevHmWLPvaa6/1asCxadOmadu2bTr//PP1+OOPS5I2bdokSXrwwQf1t7/9TWeddZbX/Sizs7P19ttv6+9//7vOPvts5eTk6Pe//72aN2+uSy+91Kt53HfffZo2bZpatmyphx56SEOGDNG2bduUkJCgnTt36pprrtGTTz6pf/7znzp8+LDGjBmjMWPGuHWp+Nvf/qZHHnlEkydP9riMffv26dprr9XIkSP15ptv6rvvvtOdd96p+vXr69FHH3XVsXTpUn3yySdKT0/XQw89pLVr16pbt25evY5AWBpUWrVqpS5durjd17lzZ3344Ycep09KSlJSUlI4SgMAxJi0tDQlJiaqQYMGatmypSTpu+++kyQ9/vjjuvLKK72eV1lZmZ566il9/vnn6tevnyTprLPO0rJly/Tyyy97HVQmT57sWu4bb7yhtm3bas6cObr55puVnZ2tYcOGuTq0nn322Xr++ed16aWXasaMGapfv74k6fLLL9e9997rmufu3bvdlvHSSy8pIyND06dPl81m07nnnqv9+/frgQce0COPPKLS0lK99tprevvtt3XFFVe41RIOlgaV/v37a+vWrW73bdu2Te3bt7eoIgBAKMTHx+vaa6+1bNmB6tWrl0/T79ixQ6WlpdXCTXl5ubp37+71fE6HHElq0qSJzjnnHG3ZskWStG7dOq1fv17vvPOOaxqn0ymHw6Fdu3apc+fOXtW+ZcsW9evXz22Atv79+6u4uFh79+7V0aNHVV5err59+1arJRwsDSr33HOPLrroIj311FO6+eabtXLlSr3yyit65ZVXrCwLABACwQgMVmnYsKHb7bi4ODmdTrf7Kg8VX1xcLEmaO3eu2rRp4zZdsM4MFBcX63//9381duzYao+1a9fO9X/V2iONpUGld+/emjNnjiZNmqTHH39cZ555pqZOnaphw4ZZWRYAIEYlJiZ61QG3efPm1Tq25ubmKiEhQZLUpUsXJSUlac+ePV6f5vFk+fLlrtBx9OhRbdu2zdVS0qNHD23evFkdO3b0e/7SL10unE6nq1Xl66+/VkpKitq2basmTZooISFBK1asqFZLIK/NW5b/Nun666/X9ddfb3UZAACoQ4cOWrFihXbv3q1GjRrJ4XB4nO7yyy/XM888ozfffFP9+vXT22+/rY0bN7pO66SkpGjixIm655575HA4NGDAABUUFOjrr79Wamqqxx+MePL444+radOmatGihf70pz+pWbNmrl8bPfDAA7rwwgs1ZswY3XHHHWrYsKE2b96sxYsXa/r06V6/5j/+8Y+aOnWq7r77bo0ZM0Zbt27V5MmTNWHCBMXFxalRo0a6/fbbdd9996lp06ZKT0/Xn/70J8XFheeHwwynBQDAzyZOnKj4+Hh16dJFzZs31549ezxOd/XVV+vhhx/W/fffr969e6uoqEjDhw93m+aJJ57Qww8/rOzsbHXu3FnXXHON5s6d69PAplOmTNG4cePUs2dPHTx4UP/+97+VmJgoScrMzNTSpUu1bds2XXzxxerevbseeeQRtW7d2qfX3KZNG82bN08rV65U165dNXr0aN1+++3685//7JrmmWee0cUXX6whQ4Zo0KBBGjBggHr27OnTcvxleYsKAACm6NSpk7755hu3+0aOHOlx2scee0yPPfZYjfOy2WwaN26cxo0b53c9AwYMqHaKqbLevXtr0aJFNT5e9Rc+0qlWo6r9ay699FKtXLmyxvk0atRIb731lt566y3Xfffdd18tlQcPLSoAAMBYBBUAAMJs9OjRatSokce/0aNHW12eUTj1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pD179lQ79VNWVqaxY8cqPT1d9evX14ABA7Rq1Sq3WubNm6dOnTopOTlZl112mXbv3u32+A8//KAhQ4bojDPOUMOGDXXeeedp3rx5oVo1AIKEoAIgIG+88Ybq1aunlStXatq0aXruuef0j3/8Q5I0ZswYffPNN5o9e7bWr1+vm266Sddcc422b9/uen5paamefvpp/eMf/9CmTZuUnp5ebRn333+/PvzwQ73xxhtau3atOnbsqKuvvlo//fSTJCkvL0833nijhgwZotzcXN1xxx168MEH3eaRlZWlsrIy5eTkaMOGDXr66afVqFGjEK4ZAEHhBAA/XXrppc7OnTs7HQ6H674HHnjA2blzZ+cPP/zgjI+Pd+7bt8/tOVdccYVz0qRJTqfT6Xz99dedkpy5ublu04wYMcJ5ww03OJ1Op7O4uNiZkJDgfOedd1yPl5eXO1u3bu3861//6nQ6nc5JkyY5u3Tp4jaPBx54wCnJefToUafT6XRecMEFzkcffTQorxtA+NBHBUBALrzwQtlsNtftfv366dlnn9WGDRtkt9vVqVMnt+nLysrUtGlT1+3ExERlZmbWOP+dO3fq5MmT6t+/v+u+hIQE9enTR1u2bJEkbdmyRX379nV7Xr9+/dxujx07VnfddZcWLVqkQYMG6be//W2tywVgBoIKgJAoLi5WfHy81qxZo/j4eLfHKp9ySU5Odgs6oXLHHXfo6quv1ty5c7Vo0SJlZ2fr2Wef1d133x3yZQPwH31UAARkxYoVbreXL1+us88+W927d5fdbld+fr46duzo9teyZUuv5/+rX/1KiYmJ+vrrr133nTx5UqtWrVKXLl0kSZ07d9bKlSur1VFVRkaGRo8erY8++kj33nuvXn31VV9eKgALEFQABGTPnj2aMGGCtm7dqnfffVcvvPCCxo0bp06dOmnYsGEaPny4PvroI+3atUsrV65Udna25s6d6/X8GzZsqLvuukv33XefFixYoM2bN+vOO+9UaWmpbr/9dknS6NGjtX37dt13333aunWrZs2apZkzZ7rNZ/z48Vq4cKF27dqltWvX6ssvv1Tnzp2DuSoAhACnfgAEZPjw4Tp+/Lj69Omj+Ph4jRs3Tn/4wx8kSa+//rqefPJJ3Xvvvdq3b5+aNWumCy+8UNdff71Py5gyZYocDoduu+02FRUVqVevXlq4cKHOOOMMSVK7du304Ycf6p577tELL7ygPn366KmnntL//M//uOZht9uVlZWlvXv3KjU1Vddcc43+7//+L3grAkBI2JxOhn8E4J+BAweqW7dumjp1qtWlAIhSnPoBAADGIqgAAABjceoHAAAYixYVAABgLIIKAAAwFkEFAAAYi6ACAACMRVABAADGIqgAAABjEVQAAICxCCoAAMBY/w/5u8IbQF/rvAAAAABJRU5ErkJggg==",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAioAAAGwCAYAAACHJU4LAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjkuMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy80BEi2AAAACXBIWXMAAA9hAAAPYQGoP6dpAAA73UlEQVR4nO3deXhU5f3//9ckJCFAEmQJawAtoqCGHURQUXFBpVJb9eePyvJR+8EGAREXbBW3GqzVDyhK1VpxQ7QqamXXChEru2GXTZCwBhGyQkJm5vsHMmaSSTL7uWfm+biuXFdm5sw57zln5pzX3Oee+9icTqdTAAAABoqzugAAAICaEFQAAICxCCoAAMBYBBUAAGAsggoAADAWQQUAABiLoAIAAIxVz+oCAuFwOLR//36lpKTIZrNZXQ4AAPCC0+lUUVGRWrdurbi42ttMIjqo7N+/XxkZGVaXAQAA/JCXl6e2bdvWOk1EB5WUlBRJp15oamqqxdUgmOx2uxYtWiRJuuqqqxQfH29xRQCAYCksLFRGRobrOF6biA4qp0/3pKamElSijN1uV4MGDSSd2r4EFQCIPt5026AzLQAAMBZBBQAAGIugAgAAjBXRfVQAAGaz2+06efKk1WUgzBISEoLWt5CgAgAIOqfTqYMHD+rYsWNWlwKLNG7cWC1btgx4nDOCCgAg6E6HlPT0dDVo0IBBOWOI0+lUaWmp8vPzJUmtWrUKaH4EFQBAUNntdldIadq0qdXlwALJycmSpPz8fKWnpwd0GojOtACAoDrdJ+X0WEiITae3f6B9lAgqAICQ4HRPbAvW9ieoAAAAY1keVPbt26ff//73atq0qZKTk3XBBRdo9erVVpcFAAAMYGlQOXr0qPr376+EhATNnz9fmzdv1rPPPqszzjjDyrIAAIhau3fvls1mU25ubkDzGThwoMaPHx+Ummpj6a9+nn76aWVkZOj111933XfmmWdaWNEvnE6nyiocqp9wqqey3eFUhcOhpHruPZdPnLQrMT5OcXG1n4s7Xm5XcmJwBr/xdpmRrtwuJVje5gcglgwcOFDdunXT1KlTrS4lZDIyMnTgwAE1a9bM6lK8Yulh4NNPP1WvXr100003KT09Xd27d9err75a4/RlZWUqLCx0+wuVrFlrde7DC/TDkRJJ0pAXlumCyYtUUlbhmqboxEmdP3mhfv3islrn9dn6/er8yAK9tmxXwHUVHD+pzo8s0G///t+A52WyH4vLdO/yOE3fFN1hDEBkcTqdqqioqHtCQ5WXlys+Pl4tW7ZUvXqRMUKJpUHl+++/14wZM3T22Wdr4cKFuuuuuzR27Fi98cYbHqfPzs5WWlqa6y8jIyNktc3bcFCS9M6KPZKkzQcKVW53aO2eo65pvtl5RBUOpzbuqz0wjX33W0nSE59tDriunG2H5XRK3+45FvC8TDZ/46n1v62AoAJEC7vdbsmft0aOHKmlS5dq2rRpstlsstlsmjlzpmw2m+bPn6+ePXsqKSlJy5Yt08iRIzV06FC3548fP14DBw503XY4HMrOztaZZ56p5ORkde3aVR988IFXtSxZskQ2m01z585VZmam6tevrwsvvFAbN250m27ZsmW6+OKLlZycrIyMDI0dO1YlJSWuxzt06KAnnnhCw4cPV2pqqv7whz94PPWzdOlS9enTR0lJSWrVqpUefPBBt0BWUlKi4cOHq1GjRmrVqpWeffZZr9droCyNUw6HQ7169dJTTz0lSerevbs2btyov//97xoxYkS16SdNmqQJEya4bhcWFoY0rAAAgsNut2vevHmWLPvaa6/1asCxadOmadu2bTr//PP1+OOPS5I2bdokSXrwwQf1t7/9TWeddZbX/Sizs7P19ttv6+9//7vOPvts5eTk6Pe//72aN2+uSy+91Kt53HfffZo2bZpatmyphx56SEOGDNG2bduUkJCgnTt36pprrtGTTz6pf/7znzp8+LDGjBmjMWPGuHWp+Nvf/qZHHnlEkydP9riMffv26dprr9XIkSP15ptv6rvvvtOdd96p+vXr69FHH3XVsXTpUn3yySdKT0/XQw89pLVr16pbt25evY5AWBpUWrVqpS5durjd17lzZ3344Ycep09KSlJSUlI4SgMAxJi0tDQlJiaqQYMGatmypSTpu+++kyQ9/vjjuvLKK72eV1lZmZ566il9/vnn6tevnyTprLPO0rJly/Tyyy97HVQmT57sWu4bb7yhtm3bas6cObr55puVnZ2tYcOGuTq0nn322Xr++ed16aWXasaMGapfv74k6fLLL9e9997rmufu3bvdlvHSSy8pIyND06dPl81m07nnnqv9+/frgQce0COPPKLS0lK99tprevvtt3XFFVe41RIOlgaV/v37a+vWrW73bdu2Te3bt7eoIgBAKMTHx+vaa6+1bNmB6tWrl0/T79ixQ6WlpdXCTXl5ubp37+71fE6HHElq0qSJzjnnHG3ZskWStG7dOq1fv17vvPOOaxqn0ymHw6Fdu3apc+fOXtW+ZcsW9evXz22Atv79+6u4uFh79+7V0aNHVV5err59+1arJRwsDSr33HOPLrroIj311FO6+eabtXLlSr3yyit65ZVXrCwLABACwQgMVmnYsKHb7bi4ODmdTrf7Kg8VX1xcLEmaO3eu2rRp4zZdsM4MFBcX63//9381duzYao+1a9fO9X/V2iONpUGld+/emjNnjiZNmqTHH39cZ555pqZOnaphw4ZZWRYAIEYlJiZ61QG3efPm1Tq25ubmKiEhQZLUpUsXJSUlac+ePV6f5vFk+fLlrtBx9OhRbdu2zdVS0qNHD23evFkdO3b0e/7SL10unE6nq1Xl66+/VkpKitq2basmTZooISFBK1asqFZLIK/NW5b/Nun666/X9ddfb3UZAACoQ4cOWrFihXbv3q1GjRrJ4XB4nO7yyy/XM888ozfffFP9+vXT22+/rY0bN7pO66SkpGjixIm655575HA4NGDAABUUFOjrr79Wamqqxx+MePL444+radOmatGihf70pz+pWbNmrl8bPfDAA7rwwgs1ZswY3XHHHWrYsKE2b96sxYsXa/r06V6/5j/+8Y+aOnWq7r77bo0ZM0Zbt27V5MmTNWHCBMXFxalRo0a6/fbbdd9996lp06ZKT0/Xn/70J8XFheeHwwynBQDAzyZOnKj4+Hh16dJFzZs31549ezxOd/XVV+vhhx/W/fffr969e6uoqEjDhw93m+aJJ57Qww8/rOzsbHXu3FnXXHON5s6d69PAplOmTNG4cePUs2dPHTx4UP/+97+VmJgoScrMzNTSpUu1bds2XXzxxerevbseeeQRtW7d2qfX3KZNG82bN08rV65U165dNXr0aN1+++3685//7JrmmWee0cUXX6whQ4Zo0KBBGjBggHr27OnTcvxleYsKAACm6NSpk7755hu3+0aOHOlx2scee0yPPfZYjfOy2WwaN26cxo0b53c9AwYMqHaKqbLevXtr0aJFNT5e9Rc+0qlWo6r9ay699FKtXLmyxvk0atRIb731lt566y3Xfffdd18tlQcPLSoAAMBYBBUAAMJs9OjRatSokce/0aNHW12eUTj1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pD179lQ79VNWVqaxY8cqPT1d9evX14ABA7Rq1Sq3WubNm6dOnTopOTlZl112mXbv3u32+A8//KAhQ4bojDPOUMOGDXXeeedp3rx5oVo1AIKEoAIgIG+88Ybq1aunlStXatq0aXruuef0j3/8Q5I0ZswYffPNN5o9e7bWr1+vm266Sddcc422b9/uen5paamefvpp/eMf/9CmTZuUnp5ebRn333+/PvzwQ73xxhtau3atOnbsqKuvvlo//fSTJCkvL0833nijhgwZotzcXN1xxx168MEH3eaRlZWlsrIy5eTkaMOGDXr66afVqFGjEK4ZAEHhBAA/XXrppc7OnTs7HQ6H674HHnjA2blzZ+cPP/zgjI+Pd+7bt8/tOVdccYVz0qRJTqfT6Xz99dedkpy5ublu04wYMcJ5ww03OJ1Op7O4uNiZkJDgfOedd1yPl5eXO1u3bu3861//6nQ6nc5JkyY5u3Tp4jaPBx54wCnJefToUafT6XRecMEFzkcffTQorxtA+NBHBUBALrzwQtlsNtftfv366dlnn9WGDRtkt9vVqVMnt+nLysrUtGlT1+3ExERlZmbWOP+dO3fq5MmT6t+/v+u+hIQE9enTR1u2bJEkbdmyRX379nV7Xr9+/dxujx07VnfddZcWLVqkQYMG6be//W2tywVgBoIKgJAoLi5WfHy81qxZo/j4eLfHKp9ySU5Odgs6oXLHHXfo6quv1ty5c7Vo0SJlZ2fr2Wef1d133x3yZQPwH31UAARkxYoVbreXL1+us88+W927d5fdbld+fr46duzo9teyZUuv5/+rX/1KiYmJ+vrrr133nTx5UqtWrVKXLl0kSZ07d9bKlSur1VFVRkaGRo8erY8++kj33nuvXn31VV9eKgALEFQABGTPnj2aMGGCtm7dqnfffVcvvPCCxo0bp06dOmnYsGEaPny4PvroI+3atUsrV65Udna25s6d6/X8GzZsqLvuukv33XefFixYoM2bN+vOO+9UaWmpbr/9dknS6NGjtX37dt13333aunWrZs2apZkzZ7rNZ/z48Vq4cKF27dqltWvX6ssvv1Tnzp2DuSoAhACnfgAEZPjw4Tp+/Lj69Omj+Ph4jRs3Tn/4wx8kSa+//rqefPJJ3Xvvvdq3b5+aNWumCy+8UNdff71Py5gyZYocDoduu+02FRUVqVevXlq4cKHOOOMMSVK7du304Ycf6p577tELL7ygPn366KmnntL//M//uOZht9uVlZWlvXv3KjU1Vddcc43+7//+L3grAkBI2JxOhn8E4J+BAweqW7dumjp1qtWlAIhSnPoBAADGIqgAAABjceoHAAAYixYVAABgLIIKAAAwFkEFAAAYi6ACAACMRVABAADGIqgAAABjEVQAAICxCCoAAMBY/w/5u8IbQF/rvAAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -131,14 +131,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.16"
+            "version": "3.10.14"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `portrait-0.0.1b0/tests/test_all.py` & `portrait-0.0.2b0/tests/test_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     D = 20
     dt = 20 / 60 / 24
 
     times = np.hstack([np.arange(0, H / 24, dt) + i for i in np.arange(D)])
 
     P_max = 10
     periods = np.arange(0, P_max, 0.01)
-    _ = coverage(times, periods)
+    _ = coverage(times)(periods)
 
 
 def test_period_match():
     expected = 1.234
     np.random.seed(42)
     t0s = np.random.choice(np.arange(50) * expected, size=8)
     periods = np.linspace(0.2, 5, 1000000)
```

### Comparing `portrait-0.0.1b0/LICENSE` & `portrait-0.0.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `portrait-0.0.1b0/README.md` & `portrait-0.0.2b0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -12,10 +12,10 @@
       <img src="https://img.shields.io/badge/documentation-black.svg?style=flat" alt="documentation"/></a>
   </p>
 </p>
 
 A Python package to compute and visualize observation metrics for periodic events.
 
 In Astronomy, *portrait* is useful to answer the following questions:
-- How much of an orbit with period $P$ has been observed given certain observation times? ([tutorial](docs/ipynb/coverage))
-- What period $P$ matches with this list of events? ([tutorial](docs/ipynb/periodmatch))
+- How much of an orbit with period $P$ has been observed given certain observation times? ([tutorial](docs/coverage))
+- What period $P$ matches with this list of events? ([tutorial](docs/periodmatch))
 - How a certain target must be observed to cover all orbits with periods lower than $P$ days?
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # portrait
                     Observation metrics for periodic events
                        _[_g_i_t_h_u_b_][license]_[_d_o_c_u_m_e_n_t_a_t_i_o_n_]
 A Python package to compute and visualize observation metrics for periodic
 events. In Astronomy, *portrait* is useful to answer the following questions: -
 How much of an orbit with period $P$ has been observed given certain
-observation times? ([tutorial](docs/ipynb/coverage)) - What period $P$ matches
-with this list of events? ([tutorial](docs/ipynb/periodmatch)) - How a certain
-target must be observed to cover all orbits with periods lower than $P$ days?
+observation times? ([tutorial](docs/coverage)) - What period $P$ matches with
+this list of events? ([tutorial](docs/periodmatch)) - How a certain target must
+be observed to cover all orbits with periods lower than $P$ days?
```

### Comparing `portrait-0.0.1b0/pyproject.toml` & `portrait-0.0.2b0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "portrait"
-version = "0.0.1-beta"
+version = "0.0.2-beta"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "Lionel Garcia" }]
 description = "Compute and visualize observations phase coverage"
 readme = "README.md"
 keywords = ["jax", "astronomy", "image processing"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
 ]
-dependencies = ["numpy>=1.23.5"]
+dependencies = ["numpy>=1.23.5", "jax>=0.2.25", "jaxlib"]
 
 [project.optional-dependencies]
 dev = ["black", "isort", "pytest"]
 docs = [
   "sphinx",
   "docutils",
   "jupyterlab",
   "myst-parser",
   "twine",
   "sphinx-book-theme",
   "black",
   "myst-nb",
   "sphinx-copybutton",
+  "matplotlib",
+  "lightkurve",
 ]
```

### Comparing `portrait-0.0.1b0/PKG-INFO` & `portrait-0.0.2b0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.3
 Name: portrait
-Version: 0.0.1b0
+Version: 0.0.2b0
 Summary: Compute and visualize observations phase coverage
 Author: Lionel Garcia
 License-Expression: MIT
 License-File: LICENSE
 Keywords: astronomy,image processing,jax
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: jax>=0.2.25
+Requires-Dist: jaxlib
 Requires-Dist: numpy>=1.23.5
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: black; extra == 'docs'
 Requires-Dist: docutils; extra == 'docs'
 Requires-Dist: jupyterlab; extra == 'docs'
+Requires-Dist: lightkurve; extra == 'docs'
+Requires-Dist: matplotlib; extra == 'docs'
 Requires-Dist: myst-nb; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-book-theme; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: twine; extra == 'docs'
 Description-Content-Type: text/markdown
@@ -41,10 +45,10 @@
       <img src="https://img.shields.io/badge/documentation-black.svg?style=flat" alt="documentation"/></a>
   </p>
 </p>
 
 A Python package to compute and visualize observation metrics for periodic events.
 
 In Astronomy, *portrait* is useful to answer the following questions:
-- How much of an orbit with period $P$ has been observed given certain observation times? ([tutorial](docs/ipynb/coverage))
-- What period $P$ matches with this list of events? ([tutorial](docs/ipynb/periodmatch))
+- How much of an orbit with period $P$ has been observed given certain observation times? ([tutorial](docs/coverage))
+- What period $P$ matches with this list of events? ([tutorial](docs/periodmatch))
 - How a certain target must be observed to cover all orbits with periods lower than $P$ days?
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
-Metadata-Version: 2.3 Name: portrait Version: 0.0.1b0 Summary: Compute and
+Metadata-Version: 2.3 Name: portrait Version: 0.0.2b0 Summary: Compute and
 visualize observations phase coverage Author: Lionel Garcia License-Expression:
 MIT License-File: LICENSE Keywords: astronomy,image processing,jax Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
-Requires-Dist: numpy>=1.23.5 Provides-Extra: dev Requires-Dist: black; extra ==
-'dev' Requires-Dist: isort; extra == 'dev' Requires-Dist: pytest; extra ==
-'dev' Provides-Extra: docs Requires-Dist: black; extra == 'docs' Requires-Dist:
-docutils; extra == 'docs' Requires-Dist: jupyterlab; extra == 'docs' Requires-
-Dist: myst-nb; extra == 'docs' Requires-Dist: myst-parser; extra == 'docs'
-Requires-Dist: sphinx; extra == 'docs' Requires-Dist: sphinx-book-theme; extra
-== 'docs' Requires-Dist: sphinx-copybutton; extra == 'docs' Requires-Dist:
-twine; extra == 'docs' Description-Content-Type: text/markdown # portrait
+Requires-Dist: jax>=0.2.25 Requires-Dist: jaxlib Requires-Dist: numpy>=1.23.5
+Provides-Extra: dev Requires-Dist: black; extra == 'dev' Requires-Dist: isort;
+extra == 'dev' Requires-Dist: pytest; extra == 'dev' Provides-Extra: docs
+Requires-Dist: black; extra == 'docs' Requires-Dist: docutils; extra == 'docs'
+Requires-Dist: jupyterlab; extra == 'docs' Requires-Dist: lightkurve; extra ==
+'docs' Requires-Dist: matplotlib; extra == 'docs' Requires-Dist: myst-nb; extra
+== 'docs' Requires-Dist: myst-parser; extra == 'docs' Requires-Dist: sphinx;
+extra == 'docs' Requires-Dist: sphinx-book-theme; extra == 'docs' Requires-
+Dist: sphinx-copybutton; extra == 'docs' Requires-Dist: twine; extra == 'docs'
+Description-Content-Type: text/markdown # portrait
                     Observation metrics for periodic events
                        _[_g_i_t_h_u_b_][license]_[_d_o_c_u_m_e_n_t_a_t_i_o_n_]
 A Python package to compute and visualize observation metrics for periodic
 events. In Astronomy, *portrait* is useful to answer the following questions: -
 How much of an orbit with period $P$ has been observed given certain
-observation times? ([tutorial](docs/ipynb/coverage)) - What period $P$ matches
-with this list of events? ([tutorial](docs/ipynb/periodmatch)) - How a certain
-target must be observed to cover all orbits with periods lower than $P$ days?
+observation times? ([tutorial](docs/coverage)) - What period $P$ matches with
+this list of events? ([tutorial](docs/periodmatch)) - How a certain target must
+be observed to cover all orbits with periods lower than $P$ days?
```


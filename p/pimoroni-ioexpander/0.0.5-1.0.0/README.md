# Comparing `tmp/pimoroni_ioexpander-0.0.5.tar.gz` & `tmp/pimoroni_ioexpander-1.0.0.tar.gz`

## Comparing `pimoroni_ioexpander-0.0.5.tar` & `pimoroni_ioexpander-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/Makefile
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/README.md
--rw-r--r--   0        0        0    14545 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/REFERENCE.md
--rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/check.sh
--rwxr-xr-x   0        0        0     5533 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/install.sh
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/requirements-dev.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/tox.ini
--rwxr-xr-x   0        0        0     1060 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/uninstall.sh
--rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/docs/encoder.md
--rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/docs/motor.md
--rw-r--r--   0        0        0    17360 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/docs/servo.md
--rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/analog.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/basic-test-cycles.py
--rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/button.py
--rwxr-xr-x   0        0        0     1258 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/mics6814.py
--rwxr-xr-x   0        0        0     1295 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/pir.py
--rwxr-xr-x   0        0        0     1444 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/potentiometer.py
--rwxr-xr-x   0        0        0     1122 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/pwm.py
--rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/rgbled.py
--rwxr-xr-x   0        0        0     1559 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/rotary.py
--rwxr-xr-x   0        0        0      905 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/servo.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/superio-all-adc.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/superio-all-pwm.py
--rwxr-xr-x   0        0        0     1307 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/superio-pwm.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/weather.py
--rw-r--r--   0        0        0    47008 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/__init__.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/common.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/devices.py
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/encoder.py
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/ioe_regs.py
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/motor.py
--rw-r--r--   0        0        0    18674 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/servo.py
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/sioe_regs.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/tests/conftest.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/tests/test_io.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/tests/test_setup.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/tests/test_switch_counter.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/LICENSE
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    19376 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/Makefile
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/README.md
+-rw-r--r--   0        0        0    14545 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/REFERENCE.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/check.sh
+-rwxr-xr-x   0        0        0     9744 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/uninstall.sh
+-rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/docs/encoder.md
+-rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/docs/motor.md
+-rw-r--r--   0        0        0    17360 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/docs/servo.md
+-rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/analog.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/basic-test-cycles.py
+-rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/button.py
+-rwxr-xr-x   0        0        0     1258 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/mics6814.py
+-rwxr-xr-x   0        0        0     1295 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/pir.py
+-rwxr-xr-x   0        0        0     1444 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/potentiometer.py
+-rwxr-xr-x   0        0        0     1122 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/pwm.py
+-rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/rgbled.py
+-rwxr-xr-x   0        0        0     1559 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/rotary.py
+-rwxr-xr-x   0        0        0      905 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/servo.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/superio-all-adc.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/superio-all-pwm.py
+-rwxr-xr-x   0        0        0     1307 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/superio-pwm.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/examples/weather.py
+-rw-r--r--   0        0        0    46735 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/ioexpander/__init__.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/ioexpander/common.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/ioexpander/devices.py
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/ioexpander/encoder.py
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/ioexpander/ioe_regs.py
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/ioexpander/motor.py
+-rw-r--r--   0        0        0    18674 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/ioexpander/servo.py
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/ioexpander/sioe_regs.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/tests/test_io.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/tests/test_setup.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/tests/test_switch_counter.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    20113 2020-02-02 00:00:00.000000 pimoroni_ioexpander-1.0.0/PKG-INFO
```

### Comparing `pimoroni_ioexpander-0.0.5/Makefile` & `pimoroni_ioexpander-1.0.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -18,43 +18,49 @@
 	@echo "pytest:       run Python test fixtures"
 	@echo "clean:        clean Python build and dist directories"
 	@echo "build:        build Python distribution files"
 	@echo "testdeploy:   build and upload to test PyPi"
 	@echo "deploy:       build and upload to PyPi"
 	@echo "tag:          tag the repository with the current version\n"
 
+version:
+	@hatch version
+
 install:
 	./install.sh --unstable
 
 uninstall:
 	./uninstall.sh
 
 dev-deps:
 	python3 -m pip install -r requirements-dev.txt
-	sudo apt install dos2unix
+	sudo apt install dos2unix shellcheck
 
 check:
 	@bash check.sh
 
+shellcheck:
+	shellcheck *.sh
+
 qa:
 	tox -e qa
 
 pytest:
 	tox -e py
 
 nopost:
 	@bash check.sh --nopost
 
-tag:
+tag: version
 	git tag -a "v${LIBRARY_VERSION}" -m "Version ${LIBRARY_VERSION}"
 
 build: check
 	@hatch build
 
 clean:
 	-rm -r dist
 
 testdeploy: build
-	twine upload --repository-url https://test.pypi.org/legacy/ dist/*
+	twine upload --repository testpypi dist/*
 
 deploy: nopost build
 	twine upload dist/*
```

### Comparing `pimoroni_ioexpander-0.0.5/README.md` & `pimoroni_ioexpander-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # IO Expander
 
-[![Build Status](https://travis-ci.com/pimoroni/ioe-python.svg?branch=master)](https://travis-ci.com/pimoroni/ioe-python)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pimoroni/ioe-python/test.yml?branch=main)](https://github.com/pimoroni/ioe-python/actions/workflows/test.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pimoroni/ioe-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/ioe-python?branch=master)
 [![PyPi Package](https://img.shields.io/pypi/v/pimoroni-ioexpander.svg)](https://pypi.python.org/pypi/pimoroni-ioexpander)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pimoroni-ioexpander.svg)](https://pypi.python.org/pypi/pimoroni-ioexpander)
 
 IO Expander Breakout uses a Nuvoton MS51 microcontroller and I2C to give you 14 additional input/output pins to connect things up to. Eight of the pins are hooked up to an Analog to Digital Converter and six of the pins can be used as (up to 16-bit) PWM outputs.
 
 This library is also used to power our other Nuvoton-based boards and breakouts!
@@ -56,14 +56,18 @@
 
 Alternatively, you can enable the I2C interface by:
 * running `sudo raspi-config` and enabling the option under **Interfacing Options**.
 * opening the graphical **Raspberry Pi Configuration** application from the **Preferences** menu.
 
 You may need to reboot after enabling I2C for the change to take effect.
 
+## Note for Raspberry Pi 1
+
+The first version of the Raspberry Pi uses SMBus 0 instead of 1. The ioe-python library uses SMBus 1 by default.
+You can change the SMBus that is used by adding `smbus_id=0` to your calls to `io.IOE(...)`. If you want your code to run on multiple revisions of the Pi without having to change your code depending on the Raspberry Pi revision, you can make your code check the `Revision` part of `/proc/cpuinfo` and set the SMBus accordingly. Revisions `0002` and `0003` use SMBus 0. All others use SMBus 1.
 
 # Examples and Usage
 
 There are various examples to get you started with your IO Expander. With the library installed on your Raspberry Pi, these can be found in the `~/Pimoroni/pimoroni-ioexpander/examples` directory.
 
 To take IO Expander further, the full API is described in the [library reference](/REFERENCE.md), with additional feature specific information found in the [docs folder](/docs).
```

### Comparing `pimoroni_ioexpander-0.0.5/REFERENCE.md` & `pimoroni_ioexpander-1.0.0/REFERENCE.md`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/check.sh` & `pimoroni_ioexpander-1.0.0/check.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/bin/bash
 
 # This script handles some basic QA checks on the source
 
 NOPOST=$1
-LIBRARY_NAME=`hatch project metadata name`
-LIBRARY_VERSION=`hatch version | awk -F "." '{print $1"."$2"."$3}'`
-POST_VERSION=`hatch version | awk -F "." '{print substr($4,0,length($4))}'`
+LIBRARY_NAME=$(hatch project metadata name)
+LIBRARY_VERSION=$(hatch version | awk -F "." '{print $1"."$2"."$3}')
+POST_VERSION=$(hatch version | awk -F "." '{print substr($4,0,length($4))}')
+TERM=${TERM:="xterm-256color"}
 
 success() {
 	echo -e "$(tput setaf 2)$1$(tput sgr0)"
 }
 
 inform() {
 	echo -e "$(tput setaf 6)$1$(tput sgr0)"
@@ -24,57 +25,53 @@
 	case $K in
 	-p|--nopost)
 		NOPOST=true
 		shift
 		;;
 	*)
 		if [[ $1 == -* ]]; then
-			printf "Unrecognised option: $1\n";
+			printf "Unrecognised option: %s\n" "$1";
 			exit 1
 		fi
 		POSITIONAL_ARGS+=("$1")
 		shift
 	esac
 done
 
 inform "Checking $LIBRARY_NAME $LIBRARY_VERSION\n"
 
 inform "Checking for trailing whitespace..."
-grep -IUrn --color "[[:blank:]]$" --exclude-dir=dist --exclude-dir=.tox --exclude-dir=.git --exclude=PKG-INFO
-if [[ $? -eq 0 ]]; then
+if grep -IUrn --color "[[:blank:]]$" --exclude-dir=dist --exclude-dir=.tox --exclude-dir=.git --exclude=PKG-INFO; then
     warning "Trailing whitespace found!"
     exit 1
 else
     success "No trailing whitespace found."
 fi
 printf "\n"
 
 inform "Checking for DOS line-endings..."
-grep -lIUrn --color $'\r' --exclude-dir=dist --exclude-dir=.tox --exclude-dir=.git --exclude=Makefile
-if [[ $? -eq 0 ]]; then
+if grep -lIUrn --color $'\r' --exclude-dir=dist --exclude-dir=.tox --exclude-dir=.git --exclude=Makefile; then
     warning "DOS line-endings found!"
     exit 1
 else
     success "No DOS line-endings found."
 fi
 printf "\n"
 
 inform "Checking CHANGELOG.md..."
-cat CHANGELOG.md | grep ^${LIBRARY_VERSION} > /dev/null 2>&1
-if [[ $? -eq 1 ]]; then
+if ! grep "^${LIBRARY_VERSION}" CHANGELOG.md > /dev/null 2>&1; then
     warning "Changes missing for version ${LIBRARY_VERSION}! Please update CHANGELOG.md."
     exit 1
 else
     success "Changes found for version ${LIBRARY_VERSION}."
 fi
 printf "\n"
 
 inform "Checking for git tag ${LIBRARY_VERSION}..."
-git tag -l | grep -E "${LIBRARY_VERSION}$"
-if [[ $? -eq 1 ]]; then
+if ! git tag -l | grep -E "${LIBRARY_VERSION}$"; then
     warning "Missing git tag for version ${LIBRARY_VERSION}"
 fi
 printf "\n"
 
 if [[ $NOPOST ]]; then
     inform "Checking for .postN on library version..."
     if [[ "$POST_VERSION" != "" ]]; then
```

### Comparing `pimoroni_ioexpander-0.0.5/uninstall.sh` & `pimoroni_ioexpander-1.0.0/uninstall.sh`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 #!/bin/bash
 
 FORCE=false
-LIBRARY_NAME=`grep -m 1 name pyproject.toml | awk -F" = " '{print substr($2,2,length($2)-2)}'`
+LIBRARY_NAME=$(grep -m 1 name pyproject.toml | awk -F" = " '{print substr($2,2,length($2)-2)}')
 RESOURCES_DIR=$HOME/Pimoroni/$LIBRARY_NAME
-PYTHON="/usr/bin/python3"
+PYTHON="python"
+
+
+venv_check() {
+	PYTHON_BIN=$(which $PYTHON)
+	if [[ $VIRTUAL_ENV == "" ]] || [[ $PYTHON_BIN != $VIRTUAL_ENV* ]]; then
+		printf "This script should be run in a virtual Python environment.\n"
+		exit 1
+	fi
+}
 
 user_check() {
-	if [ $(id -u) -eq 0 ]; then
-		printf "Script should not be run as root. Try './install.sh'\n"
+	if [ "$(id -u)" -eq 0 ]; then
+		printf "Script should not be run as root. Try './uninstall.sh'\n"
 		exit 1
 	fi
 }
 
 confirm() {
 	if $FORCE; then
 		true
@@ -42,21 +51,22 @@
 	echo -e "$(tput setaf 6)$1$(tput sgr0)"
 }
 
 warning() {
 	echo -e "$(tput setaf 1)$1$(tput sgr0)"
 }
 
-printf "$LIBRARY_NAME Python Library: Uninstaller\n\n"
+printf "%s Python Library: Uninstaller\n\n" "$LIBRARY_NAME"
 
 user_check
+venv_check
 
 printf "Uninstalling for Python 3...\n"
-$PYTHON -m pip uninstall $LIBRARY_NAME
+$PYTHON -m pip uninstall "$LIBRARY_NAME"
 
-if [ -d $RESOURCES_DIR ]; then
+if [ -d "$RESOURCES_DIR" ]; then
 	if confirm "Would you like to delete $RESOURCES_DIR?"; then
-		rm -r $RESOURCES_DIR
+		rm -r "$RESOURCES_DIR"
 	fi
 fi
 
 printf "Done!\n"
```

### Comparing `pimoroni_ioexpander-0.0.5/docs/encoder.md` & `pimoroni_ioexpander-1.0.0/docs/encoder.md`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/docs/motor.md` & `pimoroni_ioexpander-1.0.0/docs/motor.md`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/docs/servo.md` & `pimoroni_ioexpander-1.0.0/docs/servo.md`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/examples/analog.py` & `pimoroni_ioexpander-1.0.0/examples/analog.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/examples/button.py` & `pimoroni_ioexpander-1.0.0/examples/button.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/examples/mics6814.py` & `pimoroni_ioexpander-1.0.0/examples/mics6814.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/examples/pir.py` & `pimoroni_ioexpander-1.0.0/examples/pir.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/examples/potentiometer.py` & `pimoroni_ioexpander-1.0.0/examples/potentiometer.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/examples/pwm.py` & `pimoroni_ioexpander-1.0.0/examples/pwm.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/examples/rgbled.py` & `pimoroni_ioexpander-1.0.0/examples/rgbled.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/examples/rotary.py` & `pimoroni_ioexpander-1.0.0/examples/rotary.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/examples/servo.py` & `pimoroni_ioexpander-1.0.0/examples/servo.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/examples/superio-all-pwm.py` & `pimoroni_ioexpander-1.0.0/examples/superio-all-pwm.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/examples/superio-pwm.py` & `pimoroni_ioexpander-1.0.0/examples/superio-pwm.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/examples/weather.py` & `pimoroni_ioexpander-1.0.0/examples/weather.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/ioexpander/__init__.py` & `pimoroni_ioexpander-1.0.0/ioexpander/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 
 from smbus2 import SMBus, i2c_msg
 
 from . import ioe_regs, sioe_regs
 
-__version__ = '0.0.5'
+__version__ = "1.0.0"
 
 
 # These values encode our desired pin function: IO, ADC, PWM
 # alongside the GPIO MODE for that port and pin (section 8.1)
 # the 5th bit additionally encodes the default output state
 PIN_MODE_IO = 0b00000   # General IO mode, IE: not ADC or PWM
 PIN_MODE_QB = 0b00000   # Output, Quasi-Bidirectional mode
@@ -163,33 +163,34 @@
     def __init__(
         self,
         i2c_addr,
         interrupt_timeout=1.0,
         interrupt_pin=None,
         interrupt_pull_up=False,
         gpio=None,
+        smbus_id=1,
         skip_chip_id_check=False,
         perform_reset=False
     ):
         self._i2c_addr = i2c_addr
-        self._i2c_dev = SMBus(1)
+        self._i2c_dev = SMBus(smbus_id)
         self._debug = False
         self._vref = 3.3
         self._adc_enabled = False
         self._timeout = interrupt_timeout
         self._interrupt_pin = interrupt_pin
         self._gpio = gpio
         self._encoder_offset = [0, 0, 0, 0]
         self._encoder_last = [0, 0, 0, 0]
 
         # Check the chip ID first, before setting up any GPIO
         if not skip_chip_id_check:
             chip_id = self.get_chip_id()
             if chip_id != self._chip_id:
-                raise RuntimeError("Chip ID invalid: {:04x} expected: {:04x}.".format(chip_id, self._chip_id))
+                raise RuntimeError(f"Chip ID invalid: {chip_id:04x} expected: {self._chip_id:04x}.")
 
         # Reset the chip if requested, to put it into a known state
         if perform_reset:
             self.reset()
 
         # Set up the interrupt pin on the Pi, and enable the chip's output
         if self._interrupt_pin is not None:
@@ -235,90 +236,90 @@
     def i2c_write8(self, reg, value):
         """Write a single (8bit) register to the device."""
         msg_w = i2c_msg.write(self._i2c_addr, [reg, value])
         self._i2c_dev.i2c_rdwr(msg_w)
 
     def i2c_write16(self, reg_l, reg_h, value):
         """Write two (8+8bit) registers to the device, as a single write if they are consecutive."""
-        val_l = value & 0xff
-        val_h = (value >> 8) & 0xff
+        val_l = value & 0xFF
+        val_h = (value >> 8) & 0xFF
         if reg_h == reg_l + 1:
             msg_w = i2c_msg.write(self._i2c_addr, [reg_l, val_l, val_h])
             self._i2c_dev.i2c_rdwr(msg_w)
         else:
             msg_wl = i2c_msg.write(self._i2c_addr, [reg_l, val_l])
             msg_wh = i2c_msg.write(self._i2c_addr, [reg_h, val_h])
             self._i2c_dev.i2c_rdwr(msg_wl, msg_wh)
 
     def get_pin(self, pin):
         """Get a pin definition from its index."""
         if pin < 1 or pin > len(self._pins):
-            raise ValueError("Pin should be in range 1-{}.".format(len(self._pins)))
+            raise ValueError(f"Pin should be in range 1-{len(self._pins)}.")
 
         return self._pins[pin - 1]
 
     def setup_switch_counter(self, pin, mode=IN_PU):
         """Enable switch counting on a pin."""
         io_pin = self.get_pin(pin)
 
         if io_pin.port not in (0, 1):
-            raise ValueError("Pin {} does not support switch counting.".format(pin))
+            raise ValueError(f"Pin {pin} does not support switch counting.")
 
         if mode not in [IN, IN_PU]:
             raise ValueError("Pin mode should be one of IN or IN_PU")
 
         self.set_mode(pin, mode, schmitt_trigger=True)
 
         sw_reg = [self.REG_SWITCH_EN_P0, self.REG_SWITCH_EN_P1][io_pin.port]
         self.set_bit(sw_reg, io_pin.pin)
 
     def read_switch_counter(self, pin):
         """Read the switch count value on a pin."""
         io_pin = self.get_pin(pin)
 
         if io_pin.port not in (0, 1):
-            raise ValueError("Pin {} does not support switch counting.".format(pin))
+            raise ValueError(f"Pin {pin} does not support switch counting.")
 
         sw_reg = [self.REG_SWITCH_P00, self.REG_SWITCH_P10][io_pin.port] + io_pin.pin
 
         value = self.i2c_read8(sw_reg)
 
         # The switch counter is 7-bit
         # The most significant bit encodes the current GPIO state
-        return value & 0x7f, value & 0x80 == 0x80
+        return value & 0x7F, value & 0x80 == 0x80
 
     def clear_switch_counter(self, pin):
         """Clear the switch count value on a pin to 0."""
         io_pin = self.get_pin(pin)
 
         if io_pin.port not in (0, 1):
-            raise ValueError("Pin {} does not support switch counting.".format(pin))
+            raise ValueError(f"Pin {pin} does not support switch counting.")
 
         sw_reg = [self.REG_SWITCH_P00, self.REG_SWITCH_P10][io_pin.port] + io_pin.pin
 
         self.i2c_write8(sw_reg, 0)
 
     def setup_rotary_encoder(self, channel, pin_a, pin_b, pin_c=None, count_microsteps=False):
         """Set up a rotary encoder."""
         if channel < 1 or channel > 4:
             raise ValueError("Channel should be in range 1-4.")
         channel -= 1
 
         enc_channel_a = self.get_pin(pin_a).enc_channel
         enc_channel_b = self.get_pin(pin_b).enc_channel
         if enc_channel_a is None:
-            raise ValueError("Pin {} does not support an encoder.".format(pin_a))
+            raise ValueError(f"Pin {pin_a} does not support an encoder.")
         if enc_channel_b is None:
-            raise ValueError("Pin {} does not support an encoder.".format(pin_b))
+            raise ValueError(f"Pin {pin_b} does not support an encoder.")
 
         self.set_mode(pin_a, PIN_MODE_PU, schmitt_trigger=True)
         self.set_mode(pin_b, PIN_MODE_PU, schmitt_trigger=True)
         if pin_c is not None:
             if pin_c < 1 or pin_c > len(self._pins):
-                raise ValueError("Pin C should be in range 1-{}, or None.".format(len(self._pins)))
+                raise ValueError(f"Pin C should be in range 1-{len(self._pins)}, or None.")
             self.set_mode(pin_c, PIN_MODE_OD)
             self.output(pin_c, 0)
 
         self.i2c_write8(
             [self.REG_ENC_1_CFG, self.REG_ENC_2_CFG, self.REG_ENC_3_CFG, self.REG_ENC_4_CFG][channel],
             enc_channel_a | (enc_channel_b << 4),
         )
@@ -475,20 +476,20 @@
         while self._check_reset() != 0x78:
             time.sleep(0.001)
             if time.time() - t_start >= self._timeout:
                 raise RuntimeError("Timed out waiting for Reset!")
 
     def get_pwm_module(self, pin):
         if pin < 1 or pin > len(self._pins):
-            raise ValueError("Pin should be in range 1-{}.".format(len(self._pins)))
+            raise ValueError(f"Pin should be in range 1-{len(self._pins)}.")
 
         io_pin = self._pins[pin - 1]
         if PIN_MODE_PWM not in io_pin.type:
             io_mode = (PIN_MODE_PWM >> 2) & 0b11
-            raise ValueError("Pin {} does not support {}!".format(pin, MODE_NAMES[io_mode]))
+            raise ValueError(f"Pin {pin} does not support {MODE_NAMES[io_mode]}!")
 
         if isinstance(io_pin, DUAL_PWM_PIN) and io_pin.is_using_alt():
             if io_pin.is_using_alt():
                 return io_pin.pwm_alt_module
         return io_pin.pwm_module
 
     def pwm_load(self, pwm_module=0, wait_for_load=True):
@@ -533,15 +534,15 @@
                 8: 0b011,
                 16: 0b100,
                 32: 0b101,
                 64: 0b110,
                 128: 0b111,
             }[divider]
         except KeyError:
-            raise ValueError("A clock divider of {}".format(divider))
+            raise ValueError(f"A clock divider of {divider}")
 
         # TODO: This currently sets GP, PWMTYP and FBINEN to 0
         # It might be desirable to make these available to the user
         # GP - Group mode enable (changes first three pairs of pAM to PWM01H and PWM01L)
         # PWMTYP - PWM type select: 0 edge-aligned, 1 center-aligned
         # FBINEN - Fault-break input enable
 
@@ -603,25 +604,20 @@
             return
 
         gpio_mode = mode & 0b11
         io_mode = (mode >> 2) & 0b11
         initial_state = mode >> 4
 
         if io_mode != PIN_MODE_IO and mode not in io_pin.type:
-            raise ValueError("Pin {} does not support {}!".format(pin, MODE_NAMES[io_mode]))
+            raise ValueError("Pin {pin} does not support {MODE_NAMES[io_mode]}!")
 
         io_pin.mode = mode
         if self._debug:
             print(
-                "Setting pin {pin} to mode {mode} {name}, state: {state}".format(
-                    pin=pin,
-                    mode=MODE_NAMES[io_mode],
-                    name=GPIO_NAMES[gpio_mode],
-                    state=STATE_NAMES[initial_state],
-                )
+               f"Setting pin {pin} to mode {MODE_NAMES[io_mode]} {GPIO_NAMES[gpio_mode]}, state: {STATE_NAMES[initial_state]}"
             )
 
         if mode == PIN_MODE_PWM:
             self.set_bit(self.get_pwm_regs(io_pin).piocon, io_pin.bit_iopwm)
             if isinstance(io_pin, DUAL_PWM_PIN) and io_pin.is_using_alt():
                 if io_pin.pwm_module == 0:  # Only module 0's outputs can be inverted
                     self.change_bit(self.REG_PNP, io_pin.bit_iopwm, invert)
@@ -676,23 +672,23 @@
         :param adc_timeout: Timeout (in seconds) for an ADC read (default 1.0)
 
         """
         io_pin = self.get_pin(pin)
 
         if io_pin.mode == PIN_MODE_ADC:
             if self._debug:
-                print("Reading ADC from pin {}".format(pin))
+                print(f"Reading ADC from pin {pin}")
 
             if io_pin.adc_channel > 8:
                 self.i2c_write8(self.REG_AINDIDS1, 1 << (io_pin.adc_channel - 8))
             else:
                 self.i2c_write8(self.REG_AINDIDS0, 1 << io_pin.adc_channel)
 
             con0value = self.i2c_read8(self.REG_ADCCON0)
-            con0value = con0value & ~0x0f
+            con0value = con0value & ~0x0F
             con0value = con0value | io_pin.adc_channel
 
             con0value = con0value & ~(1 << 7)   # ADCF - Clear the conversion complete flag
             con0value = con0value | (1 << 6)    # ADCS - Set the ADC conversion start flag
             self.i2c_write8(self.REG_ADCCON0, con0value)
 
             if adc_timeout is not None:
@@ -703,49 +699,49 @@
                     if time.time() - t_start >= adc_timeout:
                         raise RuntimeError("Timeout waiting for ADC conversion!")
 
             reading = self.i2c_read12(self.REG_ADCRL, self.REG_ADCRH)
             return (reading / 4095.0) * self._vref
         else:
             if self._debug:
-                print("Reading IO from pin {}".format(pin))
+                print(f"Reading IO from pin {pin}")
             pv = self.get_bit(self.get_pin_regs(io_pin).p, io_pin.pin)
 
             return HIGH if pv else LOW
 
     def output(self, pin, value, load=True, wait_for_load=True):
         """Write an IO pin state or PWM duty cycle.
 
         :param value: Either True/False for OUT, or a number between 0 and PWM period for PWM.
 
         """
         io_pin = self.get_pin(pin)
 
         if io_pin.mode == PIN_MODE_PWM:
             if self._debug:
-                print("Outputting PWM to pin: {pin}".format(pin=pin))
+                print(f"Outputting PWM to pin: {pin}")
 
             if isinstance(io_pin, DUAL_PWM_PIN) and io_pin.is_using_alt():
                 alt_regs = self.get_alt_pwm_regs(io_pin)
                 self.i2c_write16(alt_regs.pwml, alt_regs.pwmh, value)
                 if load:
                     self.pwm_load(io_pin.pwm_alt_module, wait_for_load)
             else:
                 regs = self.get_pwm_regs(io_pin)
                 self.i2c_write16(regs.pwml, regs.pwmh, value)
                 if load:
                     self.pwm_load(io_pin.pwm_module, wait_for_load)
         else:
             if value == LOW:
                 if self._debug:
-                    print("Outputting LOW to pin: {pin} (or HIGH if inverted)".format(pin=pin))
+                    print(f"Outputting LOW to pin: {pin} (or HIGH if inverted)")
                 self.change_bit(self.get_pin_regs(io_pin).p, io_pin.pin, io_pin.is_inverted())
             elif value == HIGH:
                 if self._debug:
-                    print("Outputting HIGH to pin: {pin} (or LOW if inverted)".format(pin=pin))
+                    print(f"Outputting HIGH to pin: {pin} (or LOW if inverted)")
                 self.change_bit(self.get_pin_regs(io_pin).p, io_pin.pin, not io_pin.is_inverted())
 
     def get_pwm_regs(self, pin):
         return PWMRegs(
             piocon=self._regs_piocon[pin.reg_iopwm],
             pwmcon0=self._regs_pwmcon0[pin.pwm_module],
             pwmcon1=self._regs_pwmcon1[pin.pwm_module],
@@ -769,15 +765,15 @@
             p=self._regs_p[pin.port],
             ps=self._regs_ps[pin.port],
             int_mask_p=self._regs_int_mask_p[pin.port],
         )
 
     def switch_pwm_to_alt(self, pin):
         if pin < 1 or pin > len(self._pins):
-            raise ValueError("Pin should be in range 1-{}.".format(len(self._pins)))
+            raise ValueError(f"Pin should be in range 1-{len(self._pins)}.")
 
         io_pin = self._pins[pin - 1]
 
         if not isinstance(io_pin, DUAL_PWM_PIN):
             raise ValueError("Pin does not have an alternate PWM.")
 
         auxr = self.i2c_read8(self._regs_auxr[io_pin.reg_auxr])
@@ -792,14 +788,15 @@
     def __init__(
         self,
         i2c_addr=None,
         interrupt_timeout=1.0,
         interrupt_pin=None,
         interrupt_pull_up=False,
         gpio=None,
+        smbus_id=1,
         skip_chip_id_check=False,
         perform_reset=False
     ):
         self._pins = [                                                                                            # Pin |  ADC   |  PWM   |  ENC  |
             PWM_PIN(port=1, pin=5, pwm_piocon=(1, 5), pwm_define=(0, 5), enc_channel=1),                          # 1   |        | [CH 5] | CH 1  |
             PWM_PIN(port=1, pin=0, pwm_piocon=(0, 2), pwm_define=(0, 2), enc_channel=2),                          # 2   |        | [CH 2] | CH 2  |
             PWM_PIN(port=1, pin=2, pwm_piocon=(0, 0), pwm_define=(0, 0), enc_channel=3),                          # 3   |        | [CH 0] | CH 3  |
@@ -839,15 +836,15 @@
         ]
 
         self._chip_id = self.CHIP_ID
 
         if i2c_addr is None:
             i2c_addr = self.I2C_ADDR
 
-        _IO.__init__(self, i2c_addr, interrupt_timeout, interrupt_pin, interrupt_pull_up, gpio, skip_chip_id_check, perform_reset)
+        _IO.__init__(self, i2c_addr, interrupt_timeout, interrupt_pin, interrupt_pull_up, gpio, smbus_id, skip_chip_id_check, perform_reset)
 
     def read_rotary_encoder(self, channel):
         """Read the step count from a rotary encoder."""
         if channel < 1 or channel > 4:
             raise ValueError("Channel should be in range 1-4.")
         channel -= 1
         last = self._encoder_last[channel]
@@ -987,15 +984,15 @@
                 16: 0b011,   # 102.4ms
                 32: 0b100,   # 204.8ms
                 64: 0b101,   # 409.6ms
                 128: 0b110,  # 819.2ms
                 256: 0b111,  # 1.638s
             }[divider]
         except KeyError:
-            raise ValueError("A clock divider of {}".format(divider))
+            raise ValueError(f"A clock divider of {divider}")
 
         wdt = self.i2c_read8(self.REG_WDCON)
         wdt = wdt & 0b11111000  # Clear the WDPS bits
         wdt = wdt | wdtdiv  # Set the new WDPS bits according to our divider
 
         self.i2c_write8(self.REG_WDCON, wdt)
```

### Comparing `pimoroni_ioexpander-0.0.5/ioexpander/common.py` & `pimoroni_ioexpander-1.0.0/ioexpander/common.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/ioexpander/devices.py` & `pimoroni_ioexpander-1.0.0/ioexpander/devices.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/ioexpander/encoder.py` & `pimoroni_ioexpander-1.0.0/ioexpander/encoder.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/ioexpander/ioe_regs.py` & `pimoroni_ioexpander-1.0.0/ioexpander/ioe_regs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 class REGS:
     I2C_ADDR = 0x18
     CHIP_ID = 0xE26A
     CHIP_VERSION = 2
 
-    REG_CHIP_ID_L = 0xfa
-    REG_CHIP_ID_H = 0xfb
-    REG_VERSION = 0xfc
+    REG_CHIP_ID_L = 0xFA
+    REG_CHIP_ID_H = 0xFB
+    REG_VERSION = 0xFC
 
     # Rotary encoder
     REG_ENC_EN = 0x04
     BIT_ENC_EN_1 = 0
     BIT_ENC_MICROSTEP_1 = 1
     BIT_ENC_EN_2 = 2
     BIT_ENC_MICROSTEP_2 = 3
@@ -48,160 +48,160 @@
     REG_DPH = 0x43      # Read only
     REG_RCTRIM0 = 0x44  # Read only
     REG_RCTRIM1 = 0x45  # Read only
     REG_RWK = 0x46
     REG_PCON = 0x47     # Read only
     REG_TCON = 0x48
     REG_TMOD = 0x49
-    REG_TL0 = 0x4a
-    REG_TL1 = 0x4b
-    REG_TH0 = 0x4c
-    REG_TH1 = 0x4d
-    REG_CKCON = 0x4e
-    REG_WKCON = 0x4f    # Read only
+    REG_TL0 = 0x4A
+    REG_TL1 = 0x4B
+    REG_TH0 = 0x4C
+    REG_TH1 = 0x4D
+    REG_CKCON = 0x4E
+    REG_WKCON = 0x4F    # Read only
     REG_P1 = 0x50       # protect_bits 3 6 # Bit addressing
     REG_SFRS = 0x51     # TA protected # Read only
     REG_CAPCON0 = 0x52
     REG_CAPCON1 = 0x53
     REG_CAPCON2 = 0x54
     REG_CKDIV = 0x55
     REG_CKSWT = 0x56    # TA protected # Read only
     REG_CKEN = 0x57     # TA protected # Read only
     REG_SCON = 0x58
     REG_SBUF = 0x59
-    REG_SBUF_1 = 0x5a
-    REG_EIE = 0x5b      # Read only
-    REG_EIE1 = 0x5c     # Read only
-    REG_CHPCON = 0x5f   # TA protected # Read only
+    REG_SBUF_1 = 0x5A
+    REG_EIE = 0x5B      # Read only
+    REG_EIE1 = 0x5C     # Read only
+    REG_CHPCON = 0x5F   # TA protected # Read only
     REG_P2 = 0x60       # Bit addressing
     REG_AUXR1 = 0x62
     REG_BODCON0 = 0x63  # TA protected
     REG_IAPTRG = 0x64   # TA protected # Read only
     REG_IAPUEN = 0x65   # TA protected # Read only
     REG_IAPAL = 0x66    # Read only
     REG_IAPAH = 0x67    # Read only
     REG_IE = 0x68       # Read only
     REG_SADDR = 0x69
-    REG_WDCON = 0x6a    # TA protected
-    REG_BODCON1 = 0x6b  # TA protected
-    REG_P3M1 = 0x6c
-    REG_P3S = 0xc0      # Page 1 # Reassigned from 0x6c to avoid collision
-    REG_P3M2 = 0x6d
-    REG_P3SR = 0xc1     # Page 1 # Reassigned from 0x6d to avoid collision
-    REG_IAPFD = 0x6e    # Read only
-    REG_IAPCN = 0x6f    # Read only
+    REG_WDCON = 0x6A    # TA protected
+    REG_BODCON1 = 0x6B  # TA protected
+    REG_P3M1 = 0x6C
+    REG_P3S = 0xC0      # Page 1 # Reassigned from 0x6c to avoid collision
+    REG_P3M2 = 0x6D
+    REG_P3SR = 0xC1     # Page 1 # Reassigned from 0x6d to avoid collision
+    REG_IAPFD = 0x6E    # Read only
+    REG_IAPCN = 0x6F    # Read only
     REG_P3 = 0x70       # Bit addressing
     REG_P0M1 = 0x71     # protect_bits  2
-    REG_P0S = 0xc2      # Page 1 # Reassigned from 0x71 to avoid collision
+    REG_P0S = 0xC2      # Page 1 # Reassigned from 0x71 to avoid collision
     REG_P0M2 = 0x72     # protect_bits  2
-    REG_P0SR = 0xc3     # Page 1 # Reassigned from 0x72 to avoid collision
+    REG_P0SR = 0xC3     # Page 1 # Reassigned from 0x72 to avoid collision
     REG_P1M1 = 0x73     # protect_bits  3 6
-    REG_P1S = 0xc4      # Page 1 # Reassigned from 0x73 to avoid collision
+    REG_P1S = 0xC4      # Page 1 # Reassigned from 0x73 to avoid collision
     REG_P1M2 = 0x74     # protect_bits  3 6
-    REG_P1SR = 0xc5     # Page 1 # Reassigned from 0x74 to avoid collision
+    REG_P1SR = 0xC5     # Page 1 # Reassigned from 0x74 to avoid collision
     REG_P2S = 0x75
     REG_IPH = 0x77      # Read only
-    REG_PWMINTC = 0xc6  # Page 1 # Read only # Reassigned from 0x77 to avoid collision
+    REG_PWMINTC = 0xC6  # Page 1 # Read only # Reassigned from 0x77 to avoid collision
     REG_IP = 0x78       # Read only
     REG_SADEN = 0x79
-    REG_SADEN_1 = 0x7a
-    REG_SADDR_1 = 0x7b
-    REG_I2DAT = 0x7c    # Read only
-    REG_I2STAT = 0x7d   # Read only
-    REG_I2CLK = 0x7e    # Read only
-    REG_I2TOC = 0x7f    # Read only
+    REG_SADEN_1 = 0x7A
+    REG_SADDR_1 = 0x7B
+    REG_I2DAT = 0x7C    # Read only
+    REG_I2STAT = 0x7D   # Read only
+    REG_I2CLK = 0x7E    # Read only
+    REG_I2TOC = 0x7F    # Read only
     REG_I2CON = 0x80    # Read only
     REG_I2ADDR = 0x81   # Read only
     REG_ADCRL = 0x82
     REG_ADCRH = 0x83
     REG_T3CON = 0x84
-    REG_PWM4H = 0xc7    # Page 1 # Reassigned from 0x84 to avoid collision
+    REG_PWM4H = 0xC7    # Page 1 # Reassigned from 0x84 to avoid collision
     REG_RL3 = 0x85
-    REG_PWM5H = 0xc8    # Page 1 # Reassigned from 0x85 to avoid collision
+    REG_PWM5H = 0xC8    # Page 1 # Reassigned from 0x85 to avoid collision
     REG_RH3 = 0x86
-    REG_PIOCON1 = 0xc9  # Page 1 # Reassigned from 0x86 to avoid collision
+    REG_PIOCON1 = 0xC9  # Page 1 # Reassigned from 0x86 to avoid collision
     REG_TA = 0x87       # Read only
     REG_T2CON = 0x88
     REG_T2MOD = 0x89
-    REG_RCMP2L = 0x8a
-    REG_RCMP2H = 0x8b
-    REG_TL2 = 0x8c
-    REG_PWM4L = 0xca    # Page 1 # Reassigned from 0x8c to avoid collision
-    REG_TH2 = 0x8d
-    REG_PWM5L = 0xcb    # Page 1 # Reassigned from 0x8d to avoid collision
-    REG_ADCMPL = 0x8e
-    REG_ADCMPH = 0x8f
+    REG_RCMP2L = 0x8A
+    REG_RCMP2H = 0x8B
+    REG_TL2 = 0x8C
+    REG_PWM4L = 0xCA    # Page 1 # Reassigned from 0x8c to avoid collision
+    REG_TH2 = 0x8D
+    REG_PWM5L = 0xCB    # Page 1 # Reassigned from 0x8d to avoid collision
+    REG_ADCMPL = 0x8E
+    REG_ADCMPH = 0x8F
     REG_PSW = 0x90      # Read only
     REG_PWMPH = 0x91
     REG_PWM0H = 0x92
     REG_PWM1H = 0x93
     REG_PWM2H = 0x94
     REG_PWM3H = 0x95
     REG_PNP = 0x96
     REG_FBD = 0x97
     REG_PWMCON0 = 0x98
     REG_PWMPL = 0x99
-    REG_PWM0L = 0x9a
-    REG_PWM1L = 0x9b
-    REG_PWM2L = 0x9c
-    REG_PWM3L = 0x9d
-    REG_PIOCON0 = 0x9e
-    REG_PWMCON1 = 0x9f
-    REG_ACC = 0xa0      # Read only
-    REG_ADCCON1 = 0xa1
-    REG_ADCCON2 = 0xa2
-    REG_ADCDLY = 0xa3
-    REG_C0L = 0xa4
-    REG_C0H = 0xa5
-    REG_C1L = 0xa6
-    REG_C1H = 0xa7
-    REG_ADCCON0 = 0xa8
-    REG_PICON = 0xa9    # Read only
-    REG_PINEN = 0xaa    # Read only
-    REG_PIPEN = 0xab    # Read only
-    REG_PIF = 0xac      # Read only
-    REG_C2L = 0xad
-    REG_C2H = 0xae
-    REG_EIP = 0xaf      # Read only
-    REG_B = 0xb0        # Read only
-    REG_CAPCON3 = 0xb1
-    REG_CAPCON4 = 0xb2
-    REG_SPCR = 0xb3
-    REG_SPCR2 = 0xcc    # Page 1 # Reassigned from 0xb3 to avoid collision
-    REG_SPSR = 0xb4
-    REG_SPDR = 0xb5
-    REG_AINDIDS0 = 0xb6
-    REG_AINDIDS1 = None # Added to have common code with SuperIO
-    REG_EIPH = 0xb7     # Read only
-    REG_SCON_1 = 0xb8
-    REG_PDTEN = 0xb9    # TA protected
-    REG_PDTCNT = 0xba   # TA protected
-    REG_PMEN = 0xbb
-    REG_PMD = 0xbc
-    REG_EIP1 = 0xbe     # Read only
-    REG_EIPH1 = 0xbf    # Read only
+    REG_PWM0L = 0x9A
+    REG_PWM1L = 0x9B
+    REG_PWM2L = 0x9C
+    REG_PWM3L = 0x9D
+    REG_PIOCON0 = 0x9E
+    REG_PWMCON1 = 0x9F
+    REG_ACC = 0xA0      # Read only
+    REG_ADCCON1 = 0xA1
+    REG_ADCCON2 = 0xA2
+    REG_ADCDLY = 0xA3
+    REG_C0L = 0xA4
+    REG_C0H = 0xA5
+    REG_C1L = 0xA6
+    REG_C1H = 0xA7
+    REG_ADCCON0 = 0xA8
+    REG_PICON = 0xA9    # Read only
+    REG_PINEN = 0xAA    # Read only
+    REG_PIPEN = 0xAB    # Read only
+    REG_PIF = 0xAC      # Read only
+    REG_C2L = 0xAD
+    REG_C2H = 0xAE
+    REG_EIP = 0xAF      # Read only
+    REG_B = 0xB0        # Read only
+    REG_CAPCON3 = 0xB1
+    REG_CAPCON4 = 0xB2
+    REG_SPCR = 0xB3
+    REG_SPCR2 = 0xCC    # Page 1 # Reassigned from 0xb3 to avoid collision
+    REG_SPSR = 0xB4
+    REG_SPDR = 0xB5
+    REG_AINDIDS0 = 0xB6
+    REG_AINDIDS1 = None  # Added to have common code with SuperIO
+    REG_EIPH = 0xB7     # Read only
+    REG_SCON_1 = 0xB8
+    REG_PDTEN = 0xB9    # TA protected
+    REG_PDTCNT = 0xBA   # TA protected
+    REG_PMEN = 0xBB
+    REG_PMD = 0xBC
+    REG_EIP1 = 0xBE     # Read only
+    REG_EIPH1 = 0xBF    # Read only
 
-    REG_USER_FLASH = 0xd0
-    REG_FLASH_PAGE = 0xf0
+    REG_USER_FLASH = 0xD0
+    REG_FLASH_PAGE = 0xF0
 
-    REG_INT = 0xf9
+    REG_INT = 0xF9
     MASK_INT_TRIG = 0x1
     MASK_INT_OUT = 0x2
     BIT_INT_TRIGD = 0
     BIT_INT_OUT_EN = 1
     BIT_INT_PIN_SWAP = 2  # 0 = P1.3, 1 = P0.0
 
     REG_INT_MASK_P0 = 0x00
     REG_INT_MASK_P1 = 0x01
     REG_INT_MASK_P3 = 0x03
 
-    REG_VERSION = 0xfc
-    REG_ADDR = 0xfd
+    REG_VERSION = 0xFC
+    REG_ADDR = 0xFD
 
-    REG_CTRL = 0xfe     # 0 = Sleep, 1 = Reset, 2 = Read Flash, 3 = Write Flash, 4 = Addr Unlock
+    REG_CTRL = 0xFE     # 0 = Sleep, 1 = Reset, 2 = Read Flash, 3 = Write Flash, 4 = Addr Unlock
     MASK_CTRL_SLEEP = 0x1
     MASK_CTRL_RESET = 0x2
     MASK_CTRL_FREAD = 0x4
     MASK_CTRL_FWRITE = 0x8
     MASK_CTRL_ADDRWR = 0x10
 
     # Special mode registers, use a bit-addressing scheme to avoid
```

### Comparing `pimoroni_ioexpander-0.0.5/ioexpander/motor.py` & `pimoroni_ioexpander-1.0.0/ioexpander/motor.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/ioexpander/servo.py` & `pimoroni_ioexpander-1.0.0/ioexpander/servo.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/ioexpander/sioe_regs.py` & `pimoroni_ioexpander-1.0.0/ioexpander/sioe_regs.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/tests/conftest.py` & `pimoroni_ioexpander-1.0.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
 import mock
 import pytest
 
 
-@pytest.fixture(scope='function', autouse=True)
+@pytest.fixture(scope="function", autouse=True)
 def cleanup():
     """This fixture removes modules under test from sys.modules.
 
     This ensures that each module is fully re-imported, along with
     the fixtures for each test function.
 
     """
@@ -16,23 +16,24 @@
     yield None
     try:
         del sys.modules["ioexpander"]
     except KeyError:
         pass
 
 
-@pytest.fixture(scope='function', autouse=False)
+@pytest.fixture(scope="function", autouse=False)
 def smbus2():
     """Mock smbus2 module."""
 
     smbus2 = mock.MagicMock()
     smbus2.i2c_msg.read().__iter__.return_value = [0b00000000]
-    sys.modules['smbus2'] = smbus2
+    sys.modules["smbus2"] = smbus2
     yield smbus2
-    del sys.modules['smbus2']
+    del sys.modules["smbus2"]
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def ioe():
     from ioexpander import IOE
+
     yield IOE(skip_chip_id_check=True)
     del sys.modules["ioexpander"]
```

### Comparing `pimoroni_ioexpander-0.0.5/tests/test_io.py` & `pimoroni_ioexpander-1.0.0/tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     assert ioe.get_mode(7) == PIN_MODE_ADC
 
     # Always return the high bit set, this pretends bit 7 of REG_ADCCON0 is set
     # and allows an "ADC read" to complete without a timeout exception.
     smbus2.i2c_msg.read().__iter__.return_value = [0b10000000, 0b10000000]
 
     result = ioe.input(7)
-    assert type(result) is float
+    assert isinstance(result, float)
 
     # (128 << 4) | 128 / 4095.0 * 3.3
     # round to 2dp to account for FLOATING POINT WEIRDNESS!
     assert round(result, 2) == 1.75
 
     ioe.set_adc_vref(5.0)
```

### Comparing `pimoroni_ioexpander-0.0.5/tests/test_setup.py` & `pimoroni_ioexpander-1.0.0/tests/test_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,11 +25,11 @@
     Using side_effect on i2c_msg returns the
     right values in sequence for our read8 calls:
 
     msg_r = i2c_msg.read(self._i2c_addr, 1)
     self._i2c_dev.i2c_rdwr(msg_r)
     return list(msg_r)[0]
     """
-    smbus2.i2c_msg.read.side_effect = [[0x6a, 0xe2]]
+    smbus2.i2c_msg.read.side_effect = [[0x6A, 0xE2]]
 
     ioe = IOE()
     del ioe
```

### Comparing `pimoroni_ioexpander-0.0.5/tests/test_switch_counter.py` & `pimoroni_ioexpander-1.0.0/tests/test_switch_counter.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/LICENSE` & `pimoroni_ioexpander-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.5/pyproject.toml` & `pimoroni_ioexpander-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -31,15 +31,17 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: System :: Hardware",
 ]
-dependencies = []
+dependencies = [
+    "smbus2>=0.4.0"
+]
 
 [project.urls]
 GitHub = "https://www.github.com/pimoroni/ioe-python"
 Homepage = "https://www.pimoroni.com"
 
 [tool.hatch.version]
 path = "ioexpander/__init__.py"
@@ -94,25 +96,28 @@
 ./build,\
 ./dist.\
 """
 
 [tool.isort]
 line_length = 220
 
+[tool.black]
+line-length = 220
+
 [tool.check-manifest]
 ignore = [
     '.stickler.yml',
     'boilerplate.md',
     'check.sh',
     'install.sh',
     'uninstall.sh',
     'Makefile',
     'tox.ini',
     'tests/*',
     'examples/*',
     '.coveragerc'
 ]
 
-[pimoroni]
-apt_packages = ["python3-rpi.gpio", "python3-smbus"]
+[tool.pimoroni]
+apt_packages = []
 configtxt = []
 commands = []
```

### Comparing `pimoroni_ioexpander-0.0.5/PKG-INFO` & `pimoroni_ioexpander-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pimoroni-ioexpander
-Version: 0.0.5
+Version: 1.0.0
 Summary: Python library for the Pimoroni IO Expander
 Project-URL: GitHub, https://www.github.com/pimoroni/ioe-python
 Project-URL: Homepage, https://www.pimoroni.com
 Author-email: Philip Howard <phil@pimoroni.com>
 Maintainer-email: Philip Howard <phil@pimoroni.com>, Christopher Parrott <chris@pimoroni.com>
 License: MIT License
         
@@ -40,19 +40,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Requires-Python: >=3.7
+Requires-Dist: smbus2>=0.4.0
 Description-Content-Type: text/markdown
 
 # IO Expander
 
-[![Build Status](https://travis-ci.com/pimoroni/ioe-python.svg?branch=master)](https://travis-ci.com/pimoroni/ioe-python)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pimoroni/ioe-python/test.yml?branch=main)](https://github.com/pimoroni/ioe-python/actions/workflows/test.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pimoroni/ioe-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/ioe-python?branch=master)
 [![PyPi Package](https://img.shields.io/pypi/v/pimoroni-ioexpander.svg)](https://pypi.python.org/pypi/pimoroni-ioexpander)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pimoroni-ioexpander.svg)](https://pypi.python.org/pypi/pimoroni-ioexpander)
 
 IO Expander Breakout uses a Nuvoton MS51 microcontroller and I2C to give you 14 additional input/output pins to connect things up to. Eight of the pins are hooked up to an Analog to Digital Converter and six of the pins can be used as (up to 16-bit) PWM outputs.
 
 This library is also used to power our other Nuvoton-based boards and breakouts!
@@ -104,14 +105,18 @@
 
 Alternatively, you can enable the I2C interface by:
 * running `sudo raspi-config` and enabling the option under **Interfacing Options**.
 * opening the graphical **Raspberry Pi Configuration** application from the **Preferences** menu.
 
 You may need to reboot after enabling I2C for the change to take effect.
 
+## Note for Raspberry Pi 1
+
+The first version of the Raspberry Pi uses SMBus 0 instead of 1. The ioe-python library uses SMBus 1 by default.
+You can change the SMBus that is used by adding `smbus_id=0` to your calls to `io.IOE(...)`. If you want your code to run on multiple revisions of the Pi without having to change your code depending on the Raspberry Pi revision, you can make your code check the `Revision` part of `/proc/cpuinfo` and set the SMBus accordingly. Revisions `0002` and `0003` use SMBus 0. All others use SMBus 1.
 
 # Examples and Usage
 
 There are various examples to get you started with your IO Expander. With the library installed on your Raspberry Pi, these can be found in the `~/Pimoroni/pimoroni-ioexpander/examples` directory.
 
 To take IO Expander further, the full API is described in the [library reference](/REFERENCE.md), with additional feature specific information found in the [docs folder](/docs).
 
@@ -534,14 +539,21 @@
 
 * `CLOCK_FREQ` = `24000000`
 * `MAX_PERIOD` = `(1 << 16) - 1`
 * `MAX_DIVIDER` = `(1 << 7)`
 
 # Changelog
 
+1.0.0
+-----
+
+* Add dependency on smbus2
+* Add support for alternate i2c bus number
+* Port to hatch/pyproject.toml
+
 0.0.5
 -----
 
 * Improved readme and documentation
 * Linting fixes
 
 0.0.4
```


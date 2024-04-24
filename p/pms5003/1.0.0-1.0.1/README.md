# Comparing `tmp/pms5003-1.0.0.tar.gz` & `tmp/pms5003-1.0.1.tar.gz`

## Comparing `pms5003-1.0.0.tar` & `pms5003-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pms5003-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 pms5003-1.0.0/Makefile
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pms5003-1.0.0/README.md
--rwxr-xr-x   0        0        0     2102 2020-02-02 00:00:00.000000 pms5003-1.0.0/check.sh
--rwxr-xr-x   0        0        0     6986 2020-02-02 00:00:00.000000 pms5003-1.0.0/install.sh
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pms5003-1.0.0/requirements-dev.txt
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 pms5003-1.0.0/tox.ini
--rwxr-xr-x   0        0        0     1268 2020-02-02 00:00:00.000000 pms5003-1.0.0/uninstall.sh
--rwxr-xr-x   0        0        0     1289 2020-02-02 00:00:00.000000 pms5003-1.0.0/examples/all.py
--rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 pms5003-1.0.0/examples/specific.py
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 pms5003-1.0.0/pms5003/__init__.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 pms5003-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pms5003-1.0.0/tests/test_setup.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pms5003-1.0.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pms5003-1.0.0/LICENSE
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 pms5003-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 pms5003-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 pms5003-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 pms5003-1.0.1/Makefile
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 pms5003-1.0.1/README.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 pms5003-1.0.1/check.sh
+-rwxr-xr-x   0        0        0     9720 2020-02-02 00:00:00.000000 pms5003-1.0.1/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pms5003-1.0.1/requirements-dev.txt
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 pms5003-1.0.1/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 pms5003-1.0.1/uninstall.sh
+-rwxr-xr-x   0        0        0     1858 2020-02-02 00:00:00.000000 pms5003-1.0.1/examples/all.py
+-rwxr-xr-x   0        0        0     1955 2020-02-02 00:00:00.000000 pms5003-1.0.1/examples/specific.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 pms5003-1.0.1/pms5003/__init__.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 pms5003-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pms5003-1.0.1/tests/test_setup.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pms5003-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pms5003-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 pms5003-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 pms5003-1.0.1/PKG-INFO
```

### Comparing `pms5003-1.0.0/CHANGELOG.md` & `pms5003-1.0.1/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+1.0.1
+-----
+
+* Remove platform detection and default to Pi-compatible pins
+* Support passing in LineRequest and offset for custom pins (supported in gpiodevice>=0.0.4)
+
 1.0.0
 -----
 
 * Repackage to hatch/pyproject.toml
 * Port to gpiod/gpiodevice (away from RPi.GPIO)
 
 0.0.5
```

### Comparing `pms5003-1.0.0/Makefile` & `pms5003-1.0.1/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -26,19 +26,22 @@
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
```

### Comparing `pms5003-1.0.0/check.sh` & `pms5003-1.0.1/check.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/bin/bash
 
 # This script handles some basic QA checks on the source
 
 NOPOST=$1
-LIBRARY_NAME=`hatch project metadata name`
-LIBRARY_VERSION=`hatch version | awk -F "." '{print $1"."$2"."$3}'`
-POST_VERSION=`hatch version | awk -F "." '{print substr($4,0,length($4))}'`
+LIBRARY_NAME=$(hatch project metadata name)
+LIBRARY_VERSION=$(hatch version | awk -F "." '{print $1"."$2"."$3}')
+POST_VERSION=$(hatch version | awk -F "." '{print substr($4,0,length($4))}')
 TERM=${TERM:="xterm-256color"}
 
 success() {
 	echo -e "$(tput setaf 2)$1$(tput sgr0)"
 }
 
 inform() {
@@ -25,57 +25,53 @@
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

### Comparing `pms5003-1.0.0/install.sh` & `pms5003-1.0.1/install.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/bin/bash
-LIBRARY_NAME=`grep -m 1 name pyproject.toml | awk -F" = " '{print substr($2,2,length($2)-2)}'`
-CONFIG=/boot/config.txt
-DATESTAMP=`date "+%Y-%m-%d-%H-%M-%S"`
+LIBRARY_NAME=$(grep -m 1 name pyproject.toml | awk -F" = " '{print substr($2,2,length($2)-2)}')
+CONFIG_FILE=config.txt
+CONFIG_DIR="/boot/firmware"
+DATESTAMP=$(date "+%Y-%m-%d-%H-%M-%S")
 CONFIG_BACKUP=false
 APT_HAS_UPDATED=false
-RESOURCES_TOP_DIR=$HOME/Pimoroni
-VENV_BASH_SNIPPET=$RESOURCES_DIR/auto_venv.sh
-VENV_DIR=$HOME/.virtualenvs/pimoroni
-WD=`pwd`
+RESOURCES_TOP_DIR="$HOME/Pimoroni"
+VENV_BASH_SNIPPET="$RESOURCES_TOP_DIR/auto_venv.sh"
+VENV_DIR="$HOME/.virtualenvs/pimoroni"
 USAGE="./install.sh (--unstable)"
 POSITIONAL_ARGS=()
 FORCE=false
 UNSTABLE=false
 PYTHON="python"
+CMD_ERRORS=false
 
 
 user_check() {
-	if [ $(id -u) -eq 0 ]; then
-		printf "Script should not be run as root. Try './install.sh'\n"
-		exit 1
+	if [ "$(id -u)" -eq 0 ]; then
+		fatal "Script should not be run as root. Try './install.sh'\n"
 	fi
 }
 
 confirm() {
 	if $FORCE; then
 		true
 	else
@@ -31,117 +31,143 @@
 			true
 		else
 			false
 		fi
 	fi
 }
 
-prompt() {
-	read -r -p "$1 [y/N] " response < /dev/tty
-	if [[ $response =~ ^(yes|y|Y)$ ]]; then
-		true
-	else
-		false
-	fi
-}
-
 success() {
 	echo -e "$(tput setaf 2)$1$(tput sgr0)"
 }
 
 inform() {
 	echo -e "$(tput setaf 6)$1$(tput sgr0)"
 }
 
 warning() {
-	echo -e "$(tput setaf 1)$1$(tput sgr0)"
+	echo -e "$(tput setaf 1)⚠ WARNING:$(tput sgr0) $1"
+}
+
+fatal() {
+	echo -e "$(tput setaf 1)⚠ FATAL:$(tput sgr0) $1"
+	exit 1
+}
+
+find_config() {
+	if [ ! -f "$CONFIG_DIR/$CONFIG_FILE" ]; then
+		CONFIG_DIR="/boot"
+		if [ ! -f "$CONFIG_DIR/$CONFIG_FILE" ]; then
+			fatal "Could not find $CONFIG_FILE!"
+		fi
+	fi
+	inform "Using $CONFIG_FILE in $CONFIG_DIR"
 }
 
 venv_bash_snippet() {
-	if [ ! -f $VENV_BASH_SNIPPET ]; then
-		cat << EOF > $VENV_BASH_SNIPPET
-# Add `source $RESOURCES_DIR/auto_venv.sh` to your ~/.bashrc to activate
+	inform "Checking for $VENV_BASH_SNIPPET\n"
+	if [ ! -f "$VENV_BASH_SNIPPET" ]; then
+		inform "Creating $VENV_BASH_SNIPPET\n"
+		mkdir -p "$RESOURCES_TOP_DIR"
+		cat << EOF > "$VENV_BASH_SNIPPET"
+# Add "source $VENV_BASH_SNIPPET" to your ~/.bashrc to activate
 # the Pimoroni virtual environment automagically!
 VENV_DIR="$VENV_DIR"
 if [ ! -f \$VENV_DIR/bin/activate ]; then
   printf "Creating user Python environment in \$VENV_DIR, please wait...\n"
   mkdir -p \$VENV_DIR
   python3 -m venv --system-site-packages \$VENV_DIR
 fi
 printf " ↓ ↓ ↓ ↓   Hello, we've activated a Python venv for you. To exit, type \"deactivate\".\n"
 source \$VENV_DIR/bin/activate
 EOF
 	fi
 }
 
 venv_check() {
-	PYTHON_BIN=`which $PYTHON`
+	PYTHON_BIN=$(which "$PYTHON")
 	if [[ $VIRTUAL_ENV == "" ]] || [[ $PYTHON_BIN != $VIRTUAL_ENV* ]]; then
 		printf "This script should be run in a virtual Python environment.\n"
-		if confirm "Would you like us to create one for you?"; then
-			if [ ! -f $VENV_DIR/bin/activate ]; then
-				inform "Creating virtual Python environment in $VENV_DIR, please wait...\n"
-				mkdir -p $VENV_DIR
-				/usr/bin/python3 -m venv $VENV_DIR --system-site-packages
+		if confirm "Would you like us to create and/or use a default one?"; then
+			printf "\n"
+			if [ ! -f "$VENV_DIR/bin/activate" ]; then
+				inform "Creating a new virtual Python environment in $VENV_DIR, please wait...\n"
+				mkdir -p "$VENV_DIR"
+				/usr/bin/python3 -m venv "$VENV_DIR" --system-site-packages
 				venv_bash_snippet
+				# shellcheck disable=SC1091
+				source "$VENV_DIR/bin/activate"
 			else
-				inform "Found existing virtual Python environment in $VENV_DIR\n"
+				inform "Activating existing virtual Python environment in $VENV_DIR\n"
+				printf "source \"%s/bin/activate\"\n" "$VENV_DIR"
+				# shellcheck disable=SC1091
+				source "$VENV_DIR/bin/activate"
 			fi
-			inform "Activating virtual Python environment in $VENV_DIR..."
-			inform "source $VENV_DIR/bin/activate\n"
-			source $VENV_DIR/bin/activate
-
 		else
-			exit 1
+			printf "\n"
+			fatal "Please create and/or activate a virtual Python environment and try again!\n"
 		fi
 	fi
+	printf "\n"
+}
+
+check_for_error() {
+	if [ $? -ne 0 ]; then
+		CMD_ERRORS=true
+		warning "^^^ 😬 previous command did not exit cleanly!"
+	fi
 }
 
 function do_config_backup {
 	if [ ! $CONFIG_BACKUP == true ]; then
 		CONFIG_BACKUP=true
 		FILENAME="config.preinstall-$LIBRARY_NAME-$DATESTAMP.txt"
-		inform "Backing up $CONFIG to /boot/$FILENAME\n"
-		sudo cp $CONFIG /boot/$FILENAME
-		mkdir -p $RESOURCES_TOP_DIR/config-backups/
-		cp $CONFIG $RESOURCES_TOP_DIR/config-backups/$FILENAME
+		inform "Backing up $CONFIG_DIR/$CONFIG_FILE to $CONFIG_DIR/$FILENAME\n"
+		sudo cp "$CONFIG_DIR/$CONFIG_FILE" "$CONFIG_DIR/$FILENAME"
+		mkdir -p "$RESOURCES_TOP_DIR/config-backups/"
+		cp $CONFIG_DIR/$CONFIG_FILE "$RESOURCES_TOP_DIR/config-backups/$FILENAME"
 		if [ -f "$UNINSTALLER" ]; then
-			echo "cp $RESOURCES_TOP_DIR/config-backups/$FILENAME $CONFIG" >> $UNINSTALLER
+			echo "cp $RESOURCES_TOP_DIR/config-backups/$FILENAME $CONFIG_DIR/$CONFIG_FILE" >> "$UNINSTALLER"
 		fi
 	fi
 }
 
 function apt_pkg_install {
-	PACKAGES=()
+	PACKAGES_NEEDED=()
 	PACKAGES_IN=("$@")
+	# Check the list of packages and only run update/install if we need to
 	for ((i = 0; i < ${#PACKAGES_IN[@]}; i++)); do
 		PACKAGE="${PACKAGES_IN[$i]}"
 		if [ "$PACKAGE" == "" ]; then continue; fi
-		printf "Checking for $PACKAGE\n"
-		dpkg -L $PACKAGE > /dev/null 2>&1
+		printf "Checking for %s\n" "$PACKAGE"
+		dpkg -L "$PACKAGE" > /dev/null 2>&1
 		if [ "$?" == "1" ]; then
-			PACKAGES+=("$PACKAGE")
+			PACKAGES_NEEDED+=("$PACKAGE")
 		fi
 	done
-	PACKAGES="${PACKAGES[@]}"
+	PACKAGES="${PACKAGES_NEEDED[*]}"
 	if ! [ "$PACKAGES" == "" ]; then
-		echo "Installing missing packages: $PACKAGES"
+		printf "\n"
+		inform "Installing missing packages: $PACKAGES"
 		if [ ! $APT_HAS_UPDATED ]; then
 			sudo apt update
 			APT_HAS_UPDATED=true
 		fi
+		# shellcheck disable=SC2086
 		sudo apt install -y $PACKAGES
+		check_for_error
 		if [ -f "$UNINSTALLER" ]; then
-			echo "apt uninstall -y $PACKAGES" >> $UNINSTALLER
+			echo "apt uninstall -y $PACKAGES" >> "$UNINSTALLER"
 		fi
 	fi
 }
 
 function pip_pkg_install {
+	# A null Keyring prevents pip stalling in the background
 	PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring $PYTHON -m pip install --upgrade "$@"
+	check_for_error
 }
 
 while [[ $# -gt 0 ]]; do
 	K="$1"
 	case $K in
 	-u|--unstable)
 		UNSTABLE=true
@@ -154,141 +180,191 @@
 	-p|--python)
 		PYTHON=$2
 		shift
 		shift
 		;;
 	*)
 		if [[ $1 == -* ]]; then
-			printf "Unrecognised option: $1\n";
-			printf "Usage: $USAGE\n";
+			printf "Unrecognised option: %s\n" "$1";
+			printf "Usage: %s\n" "$USAGE";
 			exit 1
 		fi
 		POSITIONAL_ARGS+=("$1")
 		shift
 	esac
 done
 
+printf "Installing %s...\n\n" "$LIBRARY_NAME"
+
 user_check
 venv_check
 
-if [ ! -f `which $PYTHON` ]; then
-	printf "Python path $PYTHON not found!\n"
-	exit 1
+if [ ! -f "$(which "$PYTHON")" ]; then
+	fatal "Python path %s not found!\n" "$PYTHON"
 fi
 
-PYTHON_VER=`$PYTHON --version`
-
-printf "$LIBRARY_NAME Python Library: Installer\n\n"
+PYTHON_VER=$($PYTHON --version)
 
 inform "Checking Dependencies. Please wait..."
 
+# Install toml and try to read pyproject.toml into bash variables
+
 pip_pkg_install toml
 
-CONFIG_VARS=`$PYTHON - <<EOF
+CONFIG_VARS=$(
+	$PYTHON - <<EOF
 import toml
 config = toml.load("pyproject.toml")
+github_url = config['project']['urls']['GitHub']
 p = dict(config['tool']['pimoroni'])
 # Convert list config entries into bash arrays
 for k, v in p.items():
     v = "'\n\t'".join(v)
     p[k] = f"('{v}')"
+print(f'GITHUB_URL="{github_url}"')
 print("""
 APT_PACKAGES={apt_packages}
 SETUP_CMDS={commands}
 CONFIG_TXT={configtxt}
 """.format(**p))
-EOF`
+EOF
+)
 
+# shellcheck disable=SC2181 # Inlining the above command would be messy
 if [ $? -ne 0 ]; then
-	warning "Error parsing configuration...\n"
-	exit 1
+	# This is bad, this should not happen in production!
+	fatal "Error parsing configuration...\n"
 fi
 
-eval $CONFIG_VARS
+eval "$CONFIG_VARS"
 
 RESOURCES_DIR=$RESOURCES_TOP_DIR/$LIBRARY_NAME
 UNINSTALLER=$RESOURCES_DIR/uninstall.sh
 
-RES_DIR_OWNER=`stat -c "%U" $RESOURCES_TOP_DIR`
+RES_DIR_OWNER=$(stat -c "%U" "$RESOURCES_TOP_DIR")
 
+# Previous install.sh scripts were run as root with sudo, which caused
+# the ~/Pimoroni dir to be created with root ownership. Try and fix it.
 if [[ "$RES_DIR_OWNER" == "root" ]]; then
 	warning "\n\nFixing $RESOURCES_TOP_DIR permissions!\n\n"
-	sudo chown -R $USER:$USER $RESOURCES_TOP_DIR
+	sudo chown -R "$USER:$USER" "$RESOURCES_TOP_DIR"
 fi
 
-mkdir -p $RESOURCES_DIR
+mkdir -p "$RESOURCES_DIR"
 
-cat << EOF > $UNINSTALLER
+# Create a stub uninstaller file, we'll try to add the inverse of every
+# install command run to here, though it's not complete.
+cat << EOF > "$UNINSTALLER"
 printf "It's recommended you run these steps manually.\n"
 printf "If you want to run the full script, open it in\n"
 printf "an editor and remove 'exit 1' from below.\n"
 exit 1
 source $VIRTUAL_ENV/bin/activate
 EOF
 
-if $UNSTABLE; then
-	warning "Installing unstable library from source.\n\n"
-else
-	printf "Installing stable library from pypi.\n\n"
-fi
+printf "\n"
 
 inform "Installing for $PYTHON_VER...\n"
+
+# Install apt packages from pyproject.toml / tool.pimoroni.apt_packages
 apt_pkg_install "${APT_PACKAGES[@]}"
+
+printf "\n"
+
 if $UNSTABLE; then
+	warning "Installing unstable library from source.\n"
 	pip_pkg_install .
 else
-	pip_pkg_install $LIBRARY_NAME
+	inform "Installing stable library from pypi.\n"
+	pip_pkg_install "$LIBRARY_NAME"
 fi
+
+# shellcheck disable=SC2181 # One of two commands run, depending on --unstable flag
 if [ $? -eq 0 ]; then
 	success "Done!\n"
-	echo "$PYTHON -m pip uninstall $LIBRARY_NAME" >> $UNINSTALLER
+	echo "$PYTHON -m pip uninstall $LIBRARY_NAME" >> "$UNINSTALLER"
 fi
 
-cd $WD
+find_config
 
+printf "\n"
+
+# Run the setup commands from pyproject.toml / tool.pimoroni.commands
+
+inform "Running setup commands...\n"
 for ((i = 0; i < ${#SETUP_CMDS[@]}; i++)); do
 	CMD="${SETUP_CMDS[$i]}"
-	# Attempt to catch anything that touches /boot/config.txt and trigger a backup
-	if [[ "$CMD" == *"raspi-config"* ]] || [[ "$CMD" == *"$CONFIG"* ]] || [[ "$CMD" == *"\$CONFIG"* ]]; then
+	# Attempt to catch anything that touches config.txt and trigger a backup
+	if [[ "$CMD" == *"raspi-config"* ]] || [[ "$CMD" == *"$CONFIG_DIR/$CONFIG_FILE"* ]] || [[ "$CMD" == *"\$CONFIG_DIR/\$CONFIG_FILE"* ]]; then
 		do_config_backup
 	fi
-	eval $CMD
+	if [[ ! "$CMD" == printf* ]]; then
+		printf "Running: \"%s\"\n" "$CMD"
+	fi
+	eval "$CMD"
+	check_for_error
 done
 
+printf "\n"
+
+# Add the config.txt entries from pyproject.toml / tool.pimoroni.configtxt
+
 for ((i = 0; i < ${#CONFIG_TXT[@]}; i++)); do
 	CONFIG_LINE="${CONFIG_TXT[$i]}"
 	if ! [ "$CONFIG_LINE" == "" ]; then
 		do_config_backup
-		inform "Adding $CONFIG_LINE to $CONFIG\n"
-		sudo sed -i "s/^#$CONFIG_LINE/$CONFIG_LINE/" $CONFIG
-		if ! grep -q "^$CONFIG_LINE" $CONFIG; then
-			printf "$CONFIG_LINE\n" | sudo tee --append $CONFIG
+		inform "Adding $CONFIG_LINE to $CONFIG_DIR/$CONFIG_FILE"
+		sudo sed -i "s/^#$CONFIG_LINE/$CONFIG_LINE/" $CONFIG_DIR/$CONFIG_FILE
+		if ! grep -q "^$CONFIG_LINE" $CONFIG_DIR/$CONFIG_FILE; then
+			printf "%s \n" "$CONFIG_LINE" | sudo tee --append $CONFIG_DIR/$CONFIG_FILE
 		fi
 	fi
 done
 
+printf "\n"
+
+# Just a straight copy of the examples/ dir into ~/Pimoroni/board/examples
+
 if [ -d "examples" ]; then
 	if confirm "Would you like to copy examples to $RESOURCES_DIR?"; then
 		inform "Copying examples to $RESOURCES_DIR"
-		cp -r examples/ $RESOURCES_DIR
-		echo "rm -r $RESOURCES_DIR" >> $UNINSTALLER
+		cp -r examples/ "$RESOURCES_DIR"
+		echo "rm -r $RESOURCES_DIR" >> "$UNINSTALLER"
 		success "Done!"
 	fi
 fi
 
 printf "\n"
 
+# Use pdoc to generate basic documentation from the installed module
+
 if confirm "Would you like to generate documentation?"; then
+	inform "Installing pdoc. Please wait..."
 	pip_pkg_install pdoc
-	printf "Generating documentation.\n"
-	$PYTHON -m pdoc $LIBRARY_NAME -o $RESOURCES_DIR/docs > /dev/null
-	if [ $? -eq 0 ]; then
+	inform "Generating documentation.\n"
+	if $PYTHON -m pdoc "$LIBRARY_NAME" -o "$RESOURCES_DIR/docs" > /dev/null; then
 		inform "Documentation saved to $RESOURCES_DIR/docs"
 		success "Done!"
 	else
 		warning "Error: Failed to generate documentation."
 	fi
 fi
 
-success "\nAll done!"
-inform "If this is your first time installing you should reboot for hardware changes to take effect.\n"
-inform "Find uninstall steps in $UNINSTALLER\n"
+printf "\n"
+
+if [ "$CMD_ERRORS" = true ]; then
+	warning "One or more setup commands appear to have failed."
+	printf "This might prevent things from working properly.\n"
+	printf "Make sure your OS is up to date and try re-running this installer.\n"
+	printf "If things still don't work, report this or find help at %s.\n\n" "$GITHUB_URL"
+else
+	success "\nAll done!"
+fi
+
+printf "If this is your first time installing you should reboot for hardware changes to take effect.\n"
+printf "Find uninstall steps in %s\n\n" "$UNINSTALLER"
+
+if [ "$CMD_ERRORS" = true ]; then
+	exit 1
+else
+	exit 0
+fi
```

### Comparing `pms5003-1.0.0/uninstall.sh` & `pms5003-1.0.1/uninstall.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/bin/bash
 
 FORCE=false
-LIBRARY_NAME=`grep -m 1 name pyproject.toml | awk -F" = " '{print substr($2,2,length($2)-2)}'`
+LIBRARY_NAME=$(grep -m 1 name pyproject.toml | awk -F" = " '{print substr($2,2,length($2)-2)}')
 RESOURCES_DIR=$HOME/Pimoroni/$LIBRARY_NAME
 PYTHON="python"
 
 
 venv_check() {
-	PYTHON_BIN=`which $PYTHON`
+	PYTHON_BIN=$(which $PYTHON)
 	if [[ $VIRTUAL_ENV == "" ]] || [[ $PYTHON_BIN != $VIRTUAL_ENV* ]]; then
 		printf "This script should be run in a virtual Python environment.\n"
 		exit 1
 	fi
 }
 
 user_check() {
-	if [ $(id -u) -eq 0 ]; then
+	if [ "$(id -u)" -eq 0 ]; then
 		printf "Script should not be run as root. Try './uninstall.sh'\n"
 		exit 1
 	fi
 }
 
 confirm() {
 	if $FORCE; then
@@ -51,22 +51,22 @@
 	echo -e "$(tput setaf 6)$1$(tput sgr0)"
 }
 
 warning() {
 	echo -e "$(tput setaf 1)$1$(tput sgr0)"
 }
 
-printf "$LIBRARY_NAME Python Library: Uninstaller\n\n"
+printf "%s Python Library: Uninstaller\n\n" "$LIBRARY_NAME"
 
 user_check
 venv_check
 
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

### Comparing `pms5003-1.0.0/pms5003/__init__.py` & `pms5003-1.0.1/pms5003/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,21 @@
 import time
 
 import gpiod
 import gpiodevice
 import serial
 from gpiod.line import Direction, Value
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 
 PMS5003_SOF = bytearray(b"\x42\x4d")
 
 OUTL = gpiod.LineSettings(direction=Direction.OUTPUT, output_value=Value.INACTIVE)
 OUTH = gpiod.LineSettings(direction=Direction.OUTPUT, output_value=Value.ACTIVE)
-PLATFORMS = {
-    "Radxa ROCK 5B": {"enable": ("PIN_15", OUTH), "reset": ("PIN_13", OUTL)},
-    "Raspberry Pi 5": {"enable": ("PIN15", OUTH), "reset": ("PIN13", OUTL)},
-    "Raspberry Pi 4": {"enable": ("GPIO22", OUTH), "reset": ("GPIO27", OUTL)}
-}
 
 
 class ChecksumMismatchError(RuntimeError):
     pass
 
 
 class ReadTimeoutError(RuntimeError):
@@ -92,25 +87,22 @@
         )
 
     def __str__(self):
         return self.__repr__()
 
 
 class PMS5003:
-    def __init__(self, device="/dev/ttyAMA0", baudrate=9600, pin_enable=None, pin_reset=None):
+    def __init__(self, device="/dev/ttyAMA0", baudrate=9600, pin_enable="GPIO22", pin_reset="GPIO27"):
         self._serial = None
         self._device = device
         self._baudrate = baudrate
 
-        if pin_enable is not None and pin_reset is not None:
-            gpiodevice.friendly_errors = True
-            self._pin_enable = gpiodevice.get_pin(pin_enable, "PMS5003_en", OUTH)
-            self._pin_reset = gpiodevice.get_pin(pin_reset, "PMS5003_rst", OUTL)
-        else:
-            self._pin_enable, self._pin_reset = gpiodevice.get_pins_for_platform(PLATFORMS)
+        gpiodevice.friendly_errors = True
+        self._pin_enable = gpiodevice.get_pin(pin_enable, "PMS5003_en", OUTH)
+        self._pin_reset = gpiodevice.get_pin(pin_reset, "PMS5003_rst", OUTL)
 
         self.setup()
 
     def setup(self):
         if self._serial is not None:
             self._serial.close()
```

### Comparing `pms5003-1.0.0/tests/conftest.py` & `pms5003-1.0.1/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     del sys.modules['gpiod']
 
 
 @pytest.fixture(scope='function', autouse=False)
 def gpiodevice():
     gpiodevice = mock.Mock()
     gpiodevice.get_pins_for_platform.return_value = [(mock.Mock(), 0), (mock.Mock(), 0)]
+    gpiodevice.get_pin.return_value = (mock.Mock(), 0)
 
     sys.modules['gpiodevice'] = gpiodevice
     yield gpiodevice
     del sys.modules['gpiodevice']
 
 
 @pytest.fixture(scope='function', autouse=False)
```

### Comparing `pms5003-1.0.0/LICENSE` & `pms5003-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pms5003-1.0.0/pyproject.toml` & `pms5003-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: System :: Hardware",
 ]
 dependencies = [
     "gpiod",
-    "gpiodevice",
+    "gpiodevice>=0.0.4",
     "pyserial"
 ]
 
 [project.urls]
 GitHub = "https://www.github.com/pimoroni/pms5003-python"
 Homepage = "https://www.pimoroni.com"
 
@@ -113,8 +113,12 @@
     '.coveragerc',
     'requirements-dev.txt'
 ]
 
 [tool.pimoroni]
 apt_packages = []
 configtxt = []
-commands = []
+commands = [
+	"printf \"Setting up serial for PMS5003..\\n\"",
+	"sudo raspi-config nonint do_serial_cons 1",
+	"sudo raspi-config nonint do_serial_hw 0"
+]
```

### Comparing `pms5003-1.0.0/PKG-INFO` & `pms5003-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pms5003
-Version: 1.0.0
+Version: 1.0.1
 Summary: PMS5003 Particulate Sensor
 Project-URL: GitHub, https://www.github.com/pimoroni/pms5003-python
 Project-URL: Homepage, https://www.pimoroni.com
 Author-email: Philip Howard <phil@pimoroni.com>
 Maintainer-email: Philip Howard <phil@pimoroni.com>
 License: MIT License
         
@@ -41,54 +41,74 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Requires-Python: >=3.7
 Requires-Dist: gpiod
-Requires-Dist: gpiodevice
+Requires-Dist: gpiodevice>=0.0.4
 Requires-Dist: pyserial
 Description-Content-Type: text/markdown
 
 # PMS5003 Particulate Sensor
 
-[![Build Status](https://travis-ci.com/pimoroni/pms5003-python.svg?branch=master)](https://travis-ci.com/pimoroni/pms5003-python)
-[![Coverage Status](https://coveralls.io/repos/github/pimoroni/pms5003-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/pms5003-python?branch=master)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pimoroni/pms5003-python/test.yml?branch=main)](https://github.com/pimoroni/pms5003-python/actions/workflows/test.yml)
+[![Coverage Status](https://coveralls.io/repos/github/pimoroni/pms5003-python/badge.svg?branch=main)](https://coveralls.io/github/pimoroni/pms5003-python?branch=main)
 [![PyPi Package](https://img.shields.io/pypi/v/pms5003.svg)](https://pypi.python.org/pypi/pms5003)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pms5003.svg)](https://pypi.python.org/pypi/pms5003)
 
 # Installing
 
-Stable library from PyPi:
+**Note** The code in this repository supports both the Enviro+ and Enviro Mini boards. _The Enviro Mini board does not have the Gas sensor or the breakout for the PM sensor._
 
-* Just run `sudo pip install pms5003`
+![Enviro Plus pHAT](https://raw.githubusercontent.com/pimoroni/enviroplus-python/main/Enviro-Plus-pHAT.jpg)
+![Enviro Mini pHAT](https://raw.githubusercontent.com/pimoroni/enviroplus-python/main/Enviro-mini-pHAT.jpg)
 
-Latest/development library from GitHub:
+:warning: This library now supports Python 3 only, Python 2 is EOL - https://www.python.org/doc/sunset-python-2/
+
+## Install and configure dependencies from GitHub:
 
 * `git clone https://github.com/pimoroni/pms5003-python`
 * `cd pms5003-python`
-* `sudo ./install.sh`
-
-# Requirements
+* `./install.sh`
 
-The serial port on your Raspberry Pi must be enabled:
+**Note** Libraries will be installed in the "pimoroni" virtual environment, you will need to activate it to run examples:
 
 ```
-# Disable serial terminal over /dev/ttyAMA0
-sudo raspi-config nonint do_serial 1
-
-# Enable serial port
-raspi-config nonint set_config_var enable_uart 1 /boot/config.txt
+source ~/.virtualenvs/pimoroni/bin/activate
 ```
 
-And additionally be using a full UART (versus the default miniUART):
+**Note** Raspbian/Raspberry Pi OS Lite users may first need to install git: `sudo apt install git`
+
+## Or... Install from PyPi and configure manually:
+
+* `python3 -m venv --system-site-packages $HOME/.virtualenvs/pimoroni`
+* Run `python3 -m pip install pms5003`
+
+**Note** this will not perform any of the required configuration changes on your Pi, you may additionally need to:
 
-Add the line `dtoverlay=pi3-miniuart-bt` to your `/boot/config.txt`
+### Bookworm
+
+* Enable serial: `raspi-config nonint do_serial_hw 0`
+* Disable serial terminal: `raspi-config nonint do_serial_cons 1`
+* Add `dtoverlay=pi3-miniuart-bt` to your `/boot/config.txt`
+
+### Bullseye
+
+* Enable serial: `raspi-config nonint set_config_var enable_uart 1 /boot/config.txt`
+* Disable serial terminal: `sudo raspi-config nonint do_serial 1`
+* Add `dtoverlay=pi3-miniuart-bt` to your `/boot/config.txt`
+
+In both cases the last line will switch Bluetooth over to miniUART, see https://www.raspberrypi.org/documentation/configuration/uart.md for more details.
+
+1.0.1
+-----
 
-This will switch Bluetooth over to miniUART, see https://www.raspberrypi.org/documentation/configuration/uart.md for more details.
+* Remove platform detection and default to Pi-compatible pins
+* Support passing in LineRequest and offset for custom pins (supported in gpiodevice>=0.0.4)
 
 1.0.0
 -----
 
 * Repackage to hatch/pyproject.toml
 * Port to gpiod/gpiodevice (away from RPi.GPIO)
```


# Comparing `tmp/glean-1.9.1.tar.gz` & `tmp/glean-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/glean-1.9.1.tar", last modified: Wed Mar 29 17:43:52 2017, max compression
+gzip compressed data, was "dist/glean-1.9.2.tar", last modified: Thu Aug 10 19:53:07 2017, max compression
```

## Comparing `glean-1.9.1.tar` & `glean-1.9.2.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      837 2017-03-29 17:43:51.000000 glean-1.9.1/AUTHORS
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      377 2017-03-29 17:42:24.000000 glean-1.9.1/test-requirements.txt
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      539 2017-03-29 17:42:24.000000 glean-1.9.1/CONTRIBUTING.rst
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)    10142 2017-03-29 17:42:24.000000 glean-1.9.1/LICENSE
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     4604 2017-03-29 17:43:51.000000 glean-1.9.1/ChangeLog
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      318 2017-03-29 17:42:24.000000 glean-1.9.1/.testr.conf
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      105 2017-03-29 17:42:24.000000 glean-1.9.1/.coveragerc
--rwxrwxr-x   0 jenkins   (3000) jenkins   (3001)      781 2017-03-29 17:42:24.000000 glean-1.9.1/setup.py
--rwxrwxr-x   0 jenkins   (3000) jenkins   (3001)     1404 2017-03-29 17:42:24.000000 glean-1.9.1/rebuild-test-output.sh
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/init/
--rwxrwxr-x   0 jenkins   (3000) jenkins   (3001)      643 2017-03-29 17:42:24.000000 glean-1.9.1/glean/init/glean.init
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      120 2017-03-29 17:42:24.000000 glean-1.9.1/glean/init/glean-udev.rules
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:42:24.000000 glean-1.9.1/glean/init/__init__.py
--rwxrwxr-x   0 jenkins   (3000) jenkins   (3001)     1991 2017-03-29 17:42:24.000000 glean-1.9.1/glean/init/glean.sh
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      434 2017-03-29 17:42:24.000000 glean-1.9.1/glean/init/glean.conf
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      314 2017-03-29 17:42:24.000000 glean-1.9.1/glean/init/glean@.service
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      193 2017-03-29 17:42:24.000000 glean-1.9.1/glean/init/glean.openrc
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)    45199 2017-03-29 17:42:24.000000 glean-1.9.1/glean/cmd.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:42:24.000000 glean-1.9.1/glean/__init__.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      968 2017-03-29 17:42:24.000000 glean-1.9.1/glean/systemlock.py
--rwxrwxr-x   0 jenkins   (3000) jenkins   (3001)     4039 2017-03-29 17:42:24.000000 glean-1.9.1/glean/install.py
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/mnt/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/mnt/config/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/mnt/config/openstack/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     3189 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/vendor_data.json
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1951 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/network_data.json
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1034 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/meta_data.json
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/sys/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/sys/class/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/sys/class/net/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/sys/class/net/eth0/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/sys/class/net/eth0/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/sys/class/net/eth0/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/sys/class/net/eth0/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/sys/class/net/eth1/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/sys/class/net/eth1/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/sys/class/net/eth1/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax-iad/sys/class/net/eth1/addr_assign_type
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      269 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/README.rst
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/test/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2327 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/liberty.ubuntu.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      854 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax.debian.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1015 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax-iad.ubuntu.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      332 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/nokey.debian.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      555 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/hp.centos.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      555 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/nokey.fedora.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      716 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax-iad.redhat.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1015 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax-iad.debian.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      414 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/nokey.opensuse.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      354 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/hp.gentoo.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      414 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/hp.opensuse.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      332 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/nokey.ubuntu.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      555 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/nokey.redhat.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2714 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/liberty.fedora.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2714 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/liberty.centos.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      642 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax.gentoo.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      766 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax.opensuse.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2714 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/liberty.redhat.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2714 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/liberty.debian.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1766 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/liberty.gentoo.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      354 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/nokey.gentoo.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      555 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/nokey.centos.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      478 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax.keys.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      555 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/hp.fedora.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      555 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/hp.redhat.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      716 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax-iad.centos.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      716 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax-iad.fedora.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      906 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax.redhat.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      854 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax.ubuntu.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      478 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/liberty.keys.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      478 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/hp.keys.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      623 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax-iad.opensuse.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      906 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax.centos.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      332 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/hp.debian.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      332 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/hp.ubuntu.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2829 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/liberty.opensuse.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      519 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax-iad.gentoo.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      478 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax-iad.keys.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      906 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/rax.fedora.network.out
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/test/nokey.keys.out
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:51.000000 glean-1.9.1/glean/tests/fixtures/hp/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:51.000000 glean-1.9.1/glean/tests/fixtures/hp/mnt/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:51.000000 glean-1.9.1/glean/tests/fixtures/hp/mnt/config/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:51.000000 glean-1.9.1/glean/tests/fixtures/hp/mnt/config/openstack/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/hp/mnt/config/openstack/latest/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        4 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/mnt/config/openstack/latest/vendor_data.json
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1351 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/mnt/config/openstack/latest/meta_data.json
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:51.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:51.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:51.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth3/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth3/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth3/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth3/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth0/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth0/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth0/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth0/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth2/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth2/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth2/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth2/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth1/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth1/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth1/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/hp/sys/class/net/eth1/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:51.000000 glean-1.9.1/glean/tests/fixtures/liberty/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:51.000000 glean-1.9.1/glean/tests/fixtures/liberty/mnt/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:51.000000 glean-1.9.1/glean/tests/fixtures/liberty/mnt/config/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:51.000000 glean-1.9.1/glean/tests/fixtures/liberty/mnt/config/openstack/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/mnt/config/openstack/latest/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     5527 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/mnt/config/openstack/latest/network_info.json
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1163 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/mnt/config/openstack/latest/vendor_data.json
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1360 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/mnt/config/openstack/latest/meta_data.json
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth3/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth3/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth3/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth3/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth7/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth7/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth7/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth7/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth9/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth9/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth9/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth9/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth0/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth0/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth0/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth0/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth4/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth4/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth4/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth4/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth10/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth10/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth10/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth10/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth5/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth5/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth5/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth5/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth8/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth8/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth8/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth8/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth2/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth2/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth2/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth2/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth1/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth1/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth1/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth1/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth6/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth6/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth6/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/liberty/sys/class/net/eth6/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax/mnt/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax/mnt/config/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax/mnt/config/openstack/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax/mnt/config/openstack/latest/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2751 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/mnt/config/openstack/latest/vendor_data.json
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1390 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/mnt/config/openstack/latest/meta_data.json
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth3/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth3/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth3/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth3/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth0/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth0/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth0/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth0/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth2/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth2/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth2/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth2/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth1/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth1/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth1/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/rax/sys/class/net/eth1/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/nokey/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/nokey/mnt/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/nokey/mnt/config/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/nokey/mnt/config/openstack/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/nokey/mnt/config/openstack/latest/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        4 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/mnt/config/openstack/latest/vendor_data.json
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      911 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/mnt/config/openstack/latest/meta_data.json
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth3/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth3/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth3/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth3/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth0/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth0/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth0/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth0/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth2/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth2/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth2/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth2/addr_assign_type
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth1/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth1/carrier
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       18 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth1/address
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        2 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/fixtures/nokey/sys/class/net/eth1/addr_assign_type
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)    10427 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/test_glean.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:42:24.000000 glean-1.9.1/glean/tests/__init__.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1100 2017-03-29 17:42:24.000000 glean-1.9.1/glean/utils.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      816 2017-03-29 17:42:24.000000 glean-1.9.1/tox.ini
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     3450 2017-03-29 17:42:24.000000 glean-1.9.1/README.rst
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     4990 2017-03-29 17:43:52.000000 glean-1.9.1/PKG-INFO
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/glean.egg-info/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     4990 2017-03-29 17:43:51.000000 glean-1.9.1/glean.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        1 2017-03-29 17:43:49.000000 glean-1.9.1/glean.egg-info/not-zip-safe
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       46 2017-03-29 17:43:51.000000 glean-1.9.1/glean.egg-info/pbr.json
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     7926 2017-03-29 17:43:51.000000 glean-1.9.1/glean.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       77 2017-03-29 17:43:51.000000 glean-1.9.1/glean.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        6 2017-03-29 17:43:51.000000 glean-1.9.1/glean.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        1 2017-03-29 17:43:51.000000 glean-1.9.1/glean.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      925 2017-03-29 17:43:52.000000 glean-1.9.1/setup.cfg
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       93 2017-03-29 17:42:24.000000 glean-1.9.1/MANIFEST.in
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:51.000000 glean-1.9.1/doc/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-29 17:43:52.000000 glean-1.9.1/doc/source/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      328 2017-03-29 17:42:24.000000 glean-1.9.1/doc/source/index.rst
--rwxrwxr-x   0 jenkins   (3000) jenkins   (3001)     2453 2017-03-29 17:42:24.000000 glean-1.9.1/doc/source/conf.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       74 2017-03-29 17:42:24.000000 glean-1.9.1/doc/source/contributing.rst
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      134 2017-03-29 17:42:24.000000 glean-1.9.1/HACKING.rst
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       88 2017-03-29 17:42:24.000000 glean-1.9.1/.mailmap
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4779 2017-08-10 19:53:07.000000 glean-1.9.2/ChangeLog
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      105 2017-08-10 19:51:12.000000 glean-1.9.2/.coveragerc
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3450 2017-08-10 19:51:12.000000 glean-1.9.2/README.rst
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      816 2017-08-10 19:51:12.000000 glean-1.9.2/tox.ini
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2017-08-10 19:51:12.000000 glean-1.9.2/.testr.conf
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10142 2017-08-10 19:51:12.000000 glean-1.9.2/LICENSE
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)      781 2017-08-10 19:51:12.000000 glean-1.9.2/setup.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      134 2017-08-10 19:51:12.000000 glean-1.9.2/HACKING.rst
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       88 2017-08-10 19:51:12.000000 glean-1.9.2/.mailmap
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       93 2017-08-10 19:51:12.000000 glean-1.9.2/MANIFEST.in
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      377 2017-08-10 19:51:12.000000 glean-1.9.2/test-requirements.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4990 2017-08-10 19:53:07.000000 glean-1.9.2/PKG-INFO
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean.egg-info/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7926 2017-08-10 19:53:07.000000 glean-1.9.2/glean.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       46 2017-08-10 19:53:07.000000 glean-1.9.2/glean.egg-info/pbr.json
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2017-08-10 19:53:03.000000 glean-1.9.2/glean.egg-info/not-zip-safe
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4990 2017-08-10 19:53:07.000000 glean-1.9.2/glean.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2017-08-10 19:53:07.000000 glean-1.9.2/glean.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        6 2017-08-10 19:53:07.000000 glean-1.9.2/glean.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       77 2017-08-10 19:53:07.000000 glean-1.9.2/glean.egg-info/entry_points.txt
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/doc/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/doc/source/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      328 2017-08-10 19:51:12.000000 glean-1.9.2/doc/source/index.rst
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2453 2017-08-10 19:51:12.000000 glean-1.9.2/doc/source/conf.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       74 2017-08-10 19:51:12.000000 glean-1.9.2/doc/source/contributing.rst
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      874 2017-08-10 19:53:07.000000 glean-1.9.2/AUTHORS
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      539 2017-08-10 19:51:12.000000 glean-1.9.2/CONTRIBUTING.rst
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      968 2017-08-10 19:51:12.000000 glean-1.9.2/glean/systemlock.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10427 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/test_glean.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/__init__.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      269 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/README.rst
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth0/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth0/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth0/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth0/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth2/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth2/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth2/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth2/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth3/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth3/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth3/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth3/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth1/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth1/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth1/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/sys/class/net/eth1/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax/mnt/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax/mnt/config/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax/mnt/config/openstack/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax/mnt/config/openstack/latest/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2751 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/mnt/config/openstack/latest/vendor_data.json
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1390 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax/mnt/config/openstack/latest/meta_data.json
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/hp/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth0/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth0/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth0/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth0/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth2/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth2/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth2/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth2/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth3/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth3/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth3/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth3/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth1/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth1/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth1/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/sys/class/net/eth1/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/hp/mnt/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/hp/mnt/config/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/hp/mnt/config/openstack/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/hp/mnt/config/openstack/latest/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        4 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/mnt/config/openstack/latest/vendor_data.json
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/hp/mnt/config/openstack/latest/meta_data.json
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth7/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth7/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth7/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth7/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth0/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth0/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth0/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth0/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth4/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth4/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth4/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth4/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth8/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth8/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth8/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth8/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth2/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth2/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth2/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth2/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth9/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth9/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth9/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth9/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth10/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth10/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth10/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth10/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth5/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth5/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth5/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth5/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth3/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth3/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth3/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth3/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth1/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth1/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth1/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth1/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth6/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth6/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth6/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/sys/class/net/eth6/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/mnt/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/mnt/config/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/mnt/config/openstack/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/liberty/mnt/config/openstack/latest/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5527 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/mnt/config/openstack/latest/network_info.json
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1163 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/mnt/config/openstack/latest/vendor_data.json
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1360 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/liberty/mnt/config/openstack/latest/meta_data.json
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/nokey/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth0/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth0/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth0/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth0/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth2/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth2/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth2/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth2/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth3/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth3/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth3/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth3/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth1/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth1/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth1/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/sys/class/net/eth1/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/nokey/mnt/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/nokey/mnt/config/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/nokey/mnt/config/openstack/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/nokey/mnt/config/openstack/latest/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        4 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/mnt/config/openstack/latest/vendor_data.json
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      911 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/nokey/mnt/config/openstack/latest/meta_data.json
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/sys/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/sys/class/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/sys/class/net/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/sys/class/net/eth0/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/sys/class/net/eth0/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/sys/class/net/eth0/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/sys/class/net/eth0/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/sys/class/net/eth1/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/sys/class/net/eth1/addr_assign_type
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        2 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/sys/class/net/eth1/carrier
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       18 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/sys/class/net/eth1/address
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/mnt/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/mnt/config/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/mnt/config/openstack/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1951 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/network_data.json
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3189 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/vendor_data.json
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1034 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/meta_data.json
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/tests/fixtures/test/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      332 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/nokey.ubuntu.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1015 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax-iad.debian.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      478 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/liberty.keys.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2327 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/liberty.ubuntu.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      906 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax.centos.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      854 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax.debian.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      716 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax-iad.centos.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      716 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax-iad.fedora.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      854 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax.ubuntu.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      906 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax.fedora.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2714 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/liberty.fedora.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      478 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax-iad.keys.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2714 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/liberty.debian.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2714 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/liberty.centos.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      555 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/nokey.fedora.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      332 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/hp.ubuntu.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      332 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/nokey.debian.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      906 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax.redhat.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      414 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/hp.opensuse.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2714 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/liberty.redhat.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      478 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/hp.keys.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      555 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/nokey.centos.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      555 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/hp.redhat.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      555 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/hp.centos.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      414 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/nokey.opensuse.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2829 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/liberty.opensuse.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      354 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/hp.gentoo.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      555 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/hp.fedora.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      716 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax-iad.redhat.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      519 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax-iad.gentoo.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      478 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax.keys.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      555 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/nokey.redhat.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      766 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax.opensuse.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1766 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/liberty.gentoo.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      354 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/nokey.gentoo.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      623 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax-iad.opensuse.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/nokey.keys.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      642 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax.gentoo.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      332 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/hp.debian.network.out
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1015 2017-08-10 19:51:12.000000 glean-1.9.2/glean/tests/fixtures/test/rax-iad.ubuntu.network.out
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     4792 2017-08-10 19:51:12.000000 glean-1.9.2/glean/install.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:51:12.000000 glean-1.9.2/glean/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2017-08-10 19:51:12.000000 glean-1.9.2/glean/utils.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:53:07.000000 glean-1.9.2/glean/init/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      314 2017-08-10 19:51:12.000000 glean-1.9.2/glean/init/glean@.service
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      120 2017-08-10 19:51:12.000000 glean-1.9.2/glean/init/glean-udev.rules
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2316 2017-08-10 19:51:12.000000 glean-1.9.2/glean/init/glean.sh
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)      643 2017-08-10 19:51:12.000000 glean-1.9.2/glean/init/glean.init
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2017-08-10 19:51:12.000000 glean-1.9.2/glean/init/glean.conf
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-10 19:51:12.000000 glean-1.9.2/glean/init/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      193 2017-08-10 19:51:12.000000 glean-1.9.2/glean/init/glean.openrc
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    45199 2017-08-10 19:51:12.000000 glean-1.9.2/glean/cmd.py
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     1404 2017-08-10 19:51:12.000000 glean-1.9.2/rebuild-test-output.sh
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      925 2017-08-10 19:53:07.000000 glean-1.9.2/setup.cfg
```

### Comparing `glean-1.9.1/AUTHORS` & `glean-1.9.2/AUTHORS`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 Ian Wienand <iwienand@redhat.com>
 John L. Villalovos <john.l.villalovos@intel.com>
 Julia Kreger <juliaashleykreger@gmail.com>
 Markos Chandras <mchandras@suse.de>
 Matt Mulsow <mamulsow@us.ibm.com>
 Matthew Mulsow <mamulsow@softlayer.com>
 Matthew Thode <mthode@mthode.org>
+Mohammed Naser <mnaser@vexxhost.com>
 Monty Taylor <mordred@inaugust.com>
 Paul Belanger <pabelanger@redhat.com>
 Ricardo Carrillo Cruz <ricardo.carrillo.cruz@gmail.com>
 Sam Betts <sam@code-smash.net>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
 Yolanda Robla <yolanda.robla-mota@hp.com>
 Yolanda Robla Mota <yroblamo@redhat.com>
```

### Comparing `glean-1.9.1/CONTRIBUTING.rst` & `glean-1.9.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/LICENSE` & `glean-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/ChangeLog` & `glean-1.9.2/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 CHANGES
 =======
 
+1.9.2
+-----
+
+* Add checks for uppercase config drive label
+* prevent overwrite of gentoo init script
+* Revise systemd determination to verify systemctl presence
+
 1.9.1
 -----
 
 * Revert "Enable network.service with systemd"
 
 1.9.0
 -----
 
-* Always define link_type in debian interfaces
+* Always define link\_type in debian interfaces
 * Remove support for py33/py26
 * Adjust the way we wait for interfaces to become available
 * Fix SUSE based network configuration
 
 1.8.0
 -----
 
@@ -25,31 +32,31 @@
 * Append to interface definition for multi-address
 * Refactor side-effect functions
 * Add selinux context manager for writing files
 * Patch glean.cmd.open for unit testing
 * Use mock patching for most functions
 * Ignore non permanenet addresses in udev too
 * Index networks using id, not links
-* Use OS_LOG_CAPTURE to get log output
+* Use OS\_LOG\_CAPTURE to get log output
 
 1.6.1
 -----
 
-* Skip interfaces not in sys_interfaces
+* Skip interfaces not in sys\_interfaces
 
 1.6.0
 -----
 
 * Remove After=network.target dependency cycle
 * Add check to skip bridge interfaces
 * Improve the support for checking vlan interfaces
 * Add logging around interface carrier detection
 * Remove discover from test-requirements
 * workaround for ubuntu 14.04 bonding issue
-* Added support for setting bond-lacp-rate and bond-xmit_hash_policy
+* Added support for setting bond-lacp-rate and bond-xmit\_hash\_policy
 * Explain vlan setup with interface names
 * Explain difference between config drive files
 * Use blkid to grab config drive fs type
 * Add coverage generated files to .gitignore
 * Use constant for mac addr permanent type
 * Ignore hacking rules
 * Remove mock of os.stat()
@@ -69,15 +76,15 @@
 * Fix hostname entries in glean
 * Allow glean to preserve existing keys for root
 
 1.5.0
 -----
 
 * Remove the manual start of network interfaces
-* Add link to documentation on network_info.json
+* Add link to documentation on network\_info.json
 * Stop confusing vim's tiny brain
 * enable glean in gentoo's init on install
 * Update glean to fix gentoo support
 * add gentoo support to glean
 * mask interfaces that shouldn't be configured by default
 * Fix bug in double configuring vlans on glean
 * Add some notes on the differences to cloud-init
@@ -93,23 +100,23 @@
 * Enable network.service with systemd
 * Make distro detection global
 * Fixup some logging issues
 * Update documentation and logging
 * Handle different paths to glean.sh
 * Basic logging
 * Dont pass os.path.exists through to host os
-* Fix missing .cfg on exist_debian_interface function check
+* Fix missing .cfg on exist\_debian\_interface function check
 * Run glean after networking service
-* Rename 'v' to 'network_info'
+* Rename 'v' to 'network\_info'
 * Fix creation of vlan interfaces in Debian/Ubuntu
 * Don't use --root for tmp lockfile
 * Start after local-filesystems
 * Add support for reading vlan information
 * Make ssh key output work with alternate roots
-* Change ignore-errors to ignore_errors
+* Change ignore-errors to ignore\_errors
 * Put a newline on key injected by Glean
 
 1.4.3
 -----
 
 * Fix FileExists exception handling for .ssh
 
@@ -151,21 +158,21 @@
 
 * Support setting hostname
 
 1.0.0
 -----
 
 * Use interfaces.d on debian distros
-* Overwrite .ssh/authorized_keys rather than append
+* Overwrite .ssh/authorized\_keys rather than append
 
 0.1.2
 -----
 
 * Remove all but latest openstack metadata files
-* Handle not having an ssh_key in config-drive
+* Handle not having an ssh\_key in config-drive
 
 0.1.1
 -----
 
 * Fix unittests for the fixture reparenting
 * Add lo back in to the debian files
 * Reparent the test fixtures
```

### Comparing `glean-1.9.1/setup.py` & `glean-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/rebuild-test-output.sh` & `glean-1.9.2/rebuild-test-output.sh`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/init/glean.init` & `glean-1.9.2/glean/init/glean.init`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/cmd.py` & `glean-1.9.2/glean/cmd.py`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/systemlock.py` & `glean-1.9.2/glean/systemlock.py`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/install.py` & `glean-1.9.2/glean/install.py`

 * *Files 20% similar despite different names*

```diff
@@ -92,15 +92,24 @@
         logging.basicConfig(level=logging.INFO)
 
     # needs to go first because gentoo can have systemd along side openrc
     if os.path.exists('/etc/gentoo-release'):
         log.info('installing openrc services')
         install('glean.openrc', '/etc/init.d/glean')
         subprocess.call(['rc-update', 'add', 'glean', 'boot'])
-    if os.path.exists('/usr/lib/systemd'):
+    # Needs to check for the presence of systemd and systemctl
+    # as apparently some packages may stage systemd init files
+    # when systemd is not present.
+    # We also cannot check the path for the init pid as the pid
+    # may be wrong as install is generally executed in a chroot
+    # with diskimage-builder.
+
+    if (os.path.exists('/usr/lib/systemd/system') and
+            (os.path.exists('/usr/bin/systemctl') or
+             os.path.exists('/bin/systemctl'))):
         p = _find_gleansh_path()
 
         log.info("Installing systemd services")
         log.info("glean.sh in %s" % p)
 
         install(
             'glean@.service',
@@ -110,14 +119,20 @@
         install(
             'glean-udev.rules',
             '/etc/udev/rules.d/99-glean.rules',
             mode='0644')
     elif os.path.exists('/etc/init'):
         log.info("Installing upstart services")
         install('glean.conf', '/etc/init/glean.conf')
+    elif os.path.exists('/etc/gentoo-release'):
+        # If installing on Gentoo and if systemd or upstart is not
+        # detected, then prevent the installation of sysv init scripts
+        # on Gentoo, which would overwrite the OpenRC init scripts as
+        # the sysv init script uses the same path.
+        pass
     else:
         log.info("Installing sysv services")
         install('glean.init', '/etc/init.d/glean')
         os.system('update-rc.d glean defaults')
 
 if __name__ == '__main__':
     main()
```

### Comparing `glean-1.9.1/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/vendor_data.json` & `glean-1.9.2/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/vendor_data.json`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/network_data.json` & `glean-1.9.2/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/network_data.json`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/meta_data.json` & `glean-1.9.2/glean/tests/fixtures/rax-iad/mnt/config/openstack/latest/meta_data.json`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/liberty.ubuntu.network.out` & `glean-1.9.2/glean/tests/fixtures/test/liberty.ubuntu.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax.debian.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax.debian.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax-iad.ubuntu.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax-iad.debian.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/hp.centos.network.out` & `glean-1.9.2/glean/tests/fixtures/test/nokey.fedora.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/nokey.fedora.network.out` & `glean-1.9.2/glean/tests/fixtures/test/nokey.centos.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax-iad.redhat.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax-iad.centos.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax-iad.debian.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax-iad.ubuntu.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/nokey.redhat.network.out` & `glean-1.9.2/glean/tests/fixtures/test/hp.redhat.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/liberty.fedora.network.out` & `glean-1.9.2/glean/tests/fixtures/test/liberty.fedora.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/liberty.centos.network.out` & `glean-1.9.2/glean/tests/fixtures/test/liberty.centos.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax.gentoo.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax.gentoo.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax.opensuse.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax.opensuse.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/liberty.redhat.network.out` & `glean-1.9.2/glean/tests/fixtures/test/liberty.redhat.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/liberty.debian.network.out` & `glean-1.9.2/glean/tests/fixtures/test/liberty.debian.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/liberty.gentoo.network.out` & `glean-1.9.2/glean/tests/fixtures/test/liberty.gentoo.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/nokey.centos.network.out` & `glean-1.9.2/glean/tests/fixtures/test/hp.centos.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/hp.fedora.network.out` & `glean-1.9.2/glean/tests/fixtures/test/hp.fedora.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/hp.redhat.network.out` & `glean-1.9.2/glean/tests/fixtures/test/nokey.redhat.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax-iad.centos.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax-iad.fedora.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax-iad.fedora.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax-iad.redhat.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax.redhat.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax.centos.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax.ubuntu.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax.ubuntu.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax-iad.opensuse.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax-iad.opensuse.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax.centos.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax.fedora.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/liberty.opensuse.network.out` & `glean-1.9.2/glean/tests/fixtures/test/liberty.opensuse.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax-iad.gentoo.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax-iad.gentoo.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/test/rax.fedora.network.out` & `glean-1.9.2/glean/tests/fixtures/test/rax.redhat.network.out`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/hp/mnt/config/openstack/latest/meta_data.json` & `glean-1.9.2/glean/tests/fixtures/hp/mnt/config/openstack/latest/meta_data.json`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/liberty/mnt/config/openstack/latest/network_info.json` & `glean-1.9.2/glean/tests/fixtures/liberty/mnt/config/openstack/latest/network_info.json`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/liberty/mnt/config/openstack/latest/vendor_data.json` & `glean-1.9.2/glean/tests/fixtures/liberty/mnt/config/openstack/latest/vendor_data.json`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/liberty/mnt/config/openstack/latest/meta_data.json` & `glean-1.9.2/glean/tests/fixtures/liberty/mnt/config/openstack/latest/meta_data.json`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/rax/mnt/config/openstack/latest/vendor_data.json` & `glean-1.9.2/glean/tests/fixtures/rax/mnt/config/openstack/latest/vendor_data.json`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/rax/mnt/config/openstack/latest/meta_data.json` & `glean-1.9.2/glean/tests/fixtures/rax/mnt/config/openstack/latest/meta_data.json`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/fixtures/nokey/mnt/config/openstack/latest/meta_data.json` & `glean-1.9.2/glean/tests/fixtures/nokey/mnt/config/openstack/latest/meta_data.json`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/tests/test_glean.py` & `glean-1.9.2/glean/tests/test_glean.py`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/glean/utils.py` & `glean-1.9.2/glean/utils.py`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/tox.ini` & `glean-1.9.2/tox.ini`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/README.rst` & `glean-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/PKG-INFO` & `glean-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: glean
-Version: 1.9.1
+Version: 1.9.2
 Summary: Simple program to write static config from config-drive
 Home-page: http://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: =====
         glean
```

### Comparing `glean-1.9.1/glean.egg-info/PKG-INFO` & `glean-1.9.2/glean.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: glean
-Version: 1.9.1
+Version: 1.9.2
 Summary: Simple program to write static config from config-drive
 Home-page: http://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: =====
         glean
```

### Comparing `glean-1.9.1/glean.egg-info/SOURCES.txt` & `glean-1.9.2/glean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/setup.cfg` & `glean-1.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `glean-1.9.1/doc/source/conf.py` & `glean-1.9.2/doc/source/conf.py`

 * *Files identical despite different names*


# Comparing `tmp/precli-0.5.0.tar.gz` & `tmp/precli-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precli-0.5.0.tar", last modified: Tue Apr 16 20:20:33 2024, max compression
+gzip compressed data, was "precli-0.5.1.tar", last modified: Tue Apr 23 16:52:26 2024, max compression
```

## Comparing `precli-0.5.0.tar` & `precli-0.5.1.tar`

### file list

```diff
@@ -1,723 +1,740 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.871334 precli-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.763329 precli-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 20:20:30.000000 precli-0.5.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-16 20:20:30.000000 precli-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.763329 precli-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 20:20:30.000000 precli-0.5.0/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-16 20:20:30.000000 precli-0.5.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-16 20:20:30.000000 precli-0.5.0/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-16 20:20:30.000000 precli-0.5.0/.github/workflows/unit-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-16 20:20:30.000000 precli-0.5.0/.github/workflows/upload-asset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-16 20:20:30.000000 precli-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 20:20:30.000000 precli-0.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 20:20:30.000000 precli-0.5.0/.stestr.conf
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-16 20:20:33.000000 precli-0.5.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-16 20:20:30.000000 precli-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    17468 2024-04-16 20:20:33.000000 precli-0.5.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-16 20:20:30.000000 precli-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-16 20:20:33.871334 precli-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-16 20:20:30.000000 precli-0.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-16 20:20:30.000000 precli-0.5.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.763329 precli-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-16 20:20:30.000000 precli-0.5.0/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-16 20:20:30.000000 precli-0.5.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.763329 precli-0.5.0/docs/man/
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-16 20:20:30.000000 precli-0.5.0/docs/man/precli.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 20:20:30.000000 precli-0.5.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.747328 precli-0.5.0/docs/rules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.747328 precli-0.5.0/docs/rules/go/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.763329 precli-0.5.0/docs/rules/go/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/go/stdlib/crypto-weak-cipher.md
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/go/stdlib/crypto-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/go/stdlib/crypto-weak-key.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.747328 precli-0.5.0/docs/rules/java/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.763329 precli-0.5.0/docs/rules/java/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/java/stdlib/java-security-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/java/stdlib/java-security-weak-key.md
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/java/stdlib/java-security-weak-random.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/java/stdlib/javax-crypto-weak-cipher.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.747328 precli-0.5.0/docs/rules/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.771329 precli-0.5.0/docs/rules/python/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/argparse-sensitive-info.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/assert.md
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/crypt-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/ftplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/ftplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/hashlib-improper-prng.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/hashlib-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/hmac-timing-attack.md
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/hmac-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/hmac-weak-key.md
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/http-server-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/http-url-secret.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/imaplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/imaplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/json-load.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/logging-insecure-listen-config.md
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/marshal-load.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/nntplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/nntplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/pickle-load.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/poplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/poplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/re-denial-of-service.md
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/secrets-weak-token.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/shelve-open.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/smtplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/smtplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/socket-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/socketserver-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/ssl-context-weak-key.md
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/ssl-create-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/ssl-insecure-tls-version.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/telnetlib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/tempfile-mktemp-race-condition.md
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules/python/stdlib/xmlrpc-server-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-04-16 20:20:30.000000 precli-0.5.0/docs/rules.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.771329 precli-0.5.0/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    47438 2024-04-16 20:20:30.000000 precli-0.5.0/logo/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-16 20:20:30.000000 precli-0.5.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.771329 precli-0.5.0/precli/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-16 20:20:30.000000 precli-0.5.0/precli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 20:20:30.000000 precli-0.5.0/precli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.771329 precli-0.5.0/precli/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/precli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-16 20:20:30.000000 precli-0.5.0/precli/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.775329 precli-0.5.0/precli/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/fix.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/linecache.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/redos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/suppression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/symtab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-16 20:20:30.000000 precli-0.5.0/precli/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.775329 precli-0.5.0/precli/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-16 20:20:30.000000 precli-0.5.0/precli/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-04-16 20:20:30.000000 precli-0.5.0/precli/parsers/go.py
--rw-r--r--   0 runner    (1001) docker     (127)    12793 2024-04-16 20:20:30.000000 precli-0.5.0/precli/parsers/java.py
--rw-r--r--   0 runner    (1001) docker     (127)    18881 2024-04-16 20:20:30.000000 precli-0.5.0/precli/parsers/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-16 20:20:30.000000 precli-0.5.0/precli/parsers/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.775329 precli-0.5.0/precli/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-16 20:20:30.000000 precli-0.5.0/precli/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-16 20:20:30.000000 precli-0.5.0/precli/renderers/detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-16 20:20:30.000000 precli-0.5.0/precli/renderers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-16 20:20:30.000000 precli-0.5.0/precli/renderers/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-16 20:20:30.000000 precli-0.5.0/precli/renderers/plain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.775329 precli-0.5.0/precli/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.775329 precli-0.5.0/precli/rules/go/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/go/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.779330 precli-0.5.0/precli/rules/go/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/go/stdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/go/stdlib/crypto_weak_cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/go/stdlib/crypto_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/go/stdlib/crypto_weak_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.779330 precli-0.5.0/precli/rules/java/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.779330 precli-0.5.0/precli/rules/java/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/java/stdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/java/stdlib/java_security_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/java/stdlib/java_security_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/java/stdlib/java_security_weak_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/java/stdlib/javax_crypto_weak_cipher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.779330 precli-0.5.0/precli/rules/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.787330 precli-0.5.0/precli/rules/python/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/argparse_sensitive_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/crypt_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/ftplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/ftplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/hashlib_improper_prng.py
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/hashlib_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/hmac_timing_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/hmac_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/hmac_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/http_server_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/http_url_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/imaplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/imaplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/json_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/logging_insecure_listen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/marshal_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/nntplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/nntplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/poplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/poplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/re_denial_of_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/secrets_weak_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/shelve_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/smtplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/smtplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/socket_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/socketserver_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/ssl_context_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/ssl_create_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/ssl_insecure_tls_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/telnetlib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-16 20:20:30.000000 precli-0.5.0/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.871334 precli-0.5.0/precli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-16 20:20:33.000000 precli-0.5.0/precli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    38543 2024-04-16 20:20:33.000000 precli-0.5.0/precli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:20:33.000000 precli-0.5.0/precli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-16 20:20:33.000000 precli-0.5.0/precli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:20:33.000000 precli-0.5.0/precli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 20:20:33.000000 precli-0.5.0/precli.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 20:20:33.000000 precli-0.5.0/precli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 20:20:33.000000 precli-0.5.0/precli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-16 20:20:30.000000 precli-0.5.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 20:20:30.000000 precli-0.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.787330 precli-0.5.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-04-16 20:20:30.000000 precli-0.5.0/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-16 20:20:33.871334 precli-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 20:20:30.000000 precli-0.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 20:20:30.000000 precli-0.5.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.787330 precli-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.787330 precli-0.5.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.787330 precli-0.5.0/tests/unit/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.787330 precli-0.5.0/tests/unit/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/core/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.787330 precli-0.5.0/tests/unit/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.791330 precli-0.5.0/tests/unit/parsers/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/expression_list_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/importlib_import_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_lowercase_rule.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_lowercase_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_multiline.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_multiple_comments.go
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_multiple_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_multiple_rules.go
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_multiple_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_preceding.go
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_preceding.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_spaced_rules.go
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_spaced_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_wrong_rule.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/examples/suppress_wrong_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/test_go.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/parsers/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.791330 precli-0.5.0/tests/unit/rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.791330 precli-0.5.0/tests/unit/rules/go/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.791330 precli-0.5.0/tests/unit/rules/go/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.791330 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.795330 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_aes.go
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_des.go
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_new.go
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_sum.go
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_new.go
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_sum.go
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_new.go
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_sum.go
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.795330 precli-0.5.0/tests/unit/rules/java/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.795330 precli-0.5.0/tests/unit/rules/java/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.795330 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.799331 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/JavaSecuritySecureRandomSHA1PRNG.java
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD2.java
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5.java
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5Property.java
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestSHA1.java
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestSHA256.java
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/SecureRandomDefault.java
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/SecureRandomSHA1PRNG.java
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/test_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/test_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/java_security/test_weak_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.799331 precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.799331 precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/Cipher3DESCBC.java
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC4.java
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/test_weak_cipher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.799331 precli-0.5.0/tests/unit/rules/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.799331 precli-0.5.0/tests/unit/rules/python/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.799331 precli-0.5.0/tests/unit/rules/python/stdlib/argparse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/argparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.799331 precli-0.5.0/tests/unit/rules/python/stdlib/argparse/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_default_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_store_true.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.803331 precli-0.5.0/tests/unit/rules/python/stdlib/assert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/assert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.803331 precli-0.5.0/tests/unit/rules/python/stdlib/assert/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/assert/examples/assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/assert/test_assert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.803331 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.803331 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_blowfish.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_blowfish.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.803331 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.807331 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftp_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login_single_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.807331 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.819331 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_pbkdf2_hmac.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_scrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_as_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_importlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_usedforsecurity_true.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_usedforsecurity_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_name_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha_usedforsecurity_false.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha_usedforsecurity_false.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.819331 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.835332 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha512_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class_hexdigest.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_compare_digest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.835332 precli-0.5.0/tests/unit/rules/python/stdlib/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.835332 precli-0.5.0/tests/unit/rules/python/stdlib/http/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/http/examples/http_server_http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/http/examples/http_server_threading_http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey_in_header.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/http/examples/http_url_secret_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/http/examples/http_url_secret_username.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/http/test_http_url_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.839332 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.839332 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login_cram_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.839332 precli-0.5.0/tests/unit/rules/python/stdlib/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.839332 precli-0.5.0/tests/unit/rules/python/stdlib/json/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/json/examples/json_jsondecoder_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/json/examples/json_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/json/examples/json_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/json/test_json_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.839332 precli-0.5.0/tests/unit/rules/python/stdlib/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.843332 precli-0.5.0/tests/unit/rules/python/stdlib/logging/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_empty_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none_port.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.843332 precli-0.5.0/tests/unit/rules/python/stdlib/marshal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/marshal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.843332 precli-0.5.0/tests/unit/rules/python/stdlib/marshal/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/marshal/examples/marshal_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/marshal/examples/marshal_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.843332 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.847333 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.847333 precli-0.5.0/tests/unit/rules/python/stdlib/pickle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/pickle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.847333 precli-0.5.0/tests/unit/rules/python/stdlib/pickle/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/pickle/examples/pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/pickle/examples/pickle_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/pickle/examples/pickle_unpickler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.847333 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.851333 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_apop.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_pass_.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_rpop.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.851333 precli-0.5.0/tests/unit/rules/python/stdlib/re/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.851333 precli-0.5.0/tests/unit/rules/python/stdlib/re/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/examples/re_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/examples/re_compile_good.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/examples/re_findall.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/examples/re_finditer.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/examples/re_fullmatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/examples/re_match.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/examples/re_search.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/examples/re_search_good.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/examples/re_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/examples/re_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/examples/re_subn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.851333 precli-0.5.0/tests/unit/rules/python/stdlib/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.851333 precli-0.5.0/tests/unit/rules/python/stdlib/secrets/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_default.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_size_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_urlsafe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.855333 precli-0.5.0/tests/unit/rules/python/stdlib/shelve/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/shelve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.855333 precli-0.5.0/tests/unit/rules/python/stdlib/shelve/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/shelve/examples/shelve_dbfilenameshelf.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/shelve/examples/shelve_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/shelve/examples/shelve_open_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.855333 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.855333 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.855333 precli-0.5.0/tests/unit/rules/python/stdlib/socket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.859333 precli-0.5.0/tests/unit/rules/python/stdlib/socket/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socket/examples/socket_create_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.859333 precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.859333 precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.859333 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.867334 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/create_default_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/create_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv23.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv11.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv12.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP256r1.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1tls13.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP512r1.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_default_context.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_ffdhe2048.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime192v1.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime256v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp160r2.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp256r1.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect163k1.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect571k1.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_default_param.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_param.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv23.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv11.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv12.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv23.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2_server_side_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv11.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.867334 precli-0.5.0/tests/unit/rules/python/stdlib/telnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/telnetlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.867334 precli-0.5.0/tests/unit/rules/python/stdlib/telnetlib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/telnetlib/examples/telnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.867334 precli-0.5.0/tests/unit/rules/python/stdlib/tempfile/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/tempfile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.867334 precli-0.5.0/tests/unit/rules/python/stdlib/tempfile/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_with_open_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_walrus_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.871334 precli-0.5.0/tests/unit/rules/python/stdlib/xmlrpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/xmlrpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:20:33.871334 precli-0.5.0/tests/unit/rules/python/stdlib/xmlrpc/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_doc_xml_rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_simple_xml_rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-16 20:20:30.000000 precli-0.5.0/tests/unit/rules/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-16 20:20:30.000000 precli-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.498411 precli-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.394411 precli-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 16:52:17.000000 precli-0.5.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-23 16:52:17.000000 precli-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.398411 precli-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-23 16:52:17.000000 precli-0.5.1/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-23 16:52:17.000000 precli-0.5.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-23 16:52:17.000000 precli-0.5.1/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-23 16:52:17.000000 precli-0.5.1/.github/workflows/unit-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-23 16:52:17.000000 precli-0.5.1/.github/workflows/upload-asset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-23 16:52:17.000000 precli-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-23 16:52:17.000000 precli-0.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 16:52:17.000000 precli-0.5.1/.stestr.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-23 16:52:26.000000 precli-0.5.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-23 16:52:17.000000 precli-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18011 2024-04-23 16:52:26.000000 precli-0.5.1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-23 16:52:17.000000 precli-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-23 16:52:26.498411 precli-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-23 16:52:17.000000 precli-0.5.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-23 16:52:17.000000 precli-0.5.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.398411 precli-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-23 16:52:17.000000 precli-0.5.1/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 16:52:17.000000 precli-0.5.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.398411 precli-0.5.1/docs/man/
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-23 16:52:17.000000 precli-0.5.1/docs/man/precli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 16:52:17.000000 precli-0.5.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.382411 precli-0.5.1/docs/rules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.382411 precli-0.5.1/docs/rules/go/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.398411 precli-0.5.1/docs/rules/go/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/go/stdlib/crypto-weak-cipher.md
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/go/stdlib/crypto-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/go/stdlib/crypto-weak-key.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.382411 precli-0.5.1/docs/rules/java/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.398411 precli-0.5.1/docs/rules/java/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/java/stdlib/java-net-insecure-cookie.md
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/java/stdlib/java-security-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/java/stdlib/java-security-weak-key.md
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/java/stdlib/java-security-weak-random.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/java/stdlib/javax-crypto-weak-cipher.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/java/stdlib/javax-servlet-http-insecure-cookie.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.382411 precli-0.5.1/docs/rules/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.406411 precli-0.5.1/docs/rules/python/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/argparse-sensitive-info.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/assert.md
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/crypt-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/ftplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/ftplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/hashlib-improper-prng.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/hashlib-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/hmac-timing-attack.md
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/hmac-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/hmac-weak-key.md
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/http-server-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/http-url-secret.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/imaplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/imaplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/json-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/logging-insecure-listen-config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/marshal-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/nntplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/nntplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/pickle-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/poplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/poplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/re-denial-of-service.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/secrets-weak-token.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/shelve-open.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/smtplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/smtplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/socket-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/socketserver-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/ssl-context-weak-key.md
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/ssl-create-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/ssl-insecure-tls-version.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/telnetlib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/tempfile-mktemp-race-condition.md
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules/python/stdlib/xmlrpc-server-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-23 16:52:17.000000 precli-0.5.1/docs/rules.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.406411 precli-0.5.1/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   179522 2024-04-23 16:52:17.000000 precli-0.5.1/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-23 16:52:17.000000 precli-0.5.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.406411 precli-0.5.1/precli/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-23 16:52:17.000000 precli-0.5.1/precli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 16:52:17.000000 precli-0.5.1/precli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.406411 precli-0.5.1/precli/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/precli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-23 16:52:17.000000 precli-0.5.1/precli/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.410411 precli-0.5.1/precli/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/linecache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/redos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/symtab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-23 16:52:17.000000 precli-0.5.1/precli/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.410411 precli-0.5.1/precli/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-23 16:52:17.000000 precli-0.5.1/precli/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-04-23 16:52:17.000000 precli-0.5.1/precli/parsers/go.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14094 2024-04-23 16:52:17.000000 precli-0.5.1/precli/parsers/java.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18869 2024-04-23 16:52:17.000000 precli-0.5.1/precli/parsers/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-23 16:52:17.000000 precli-0.5.1/precli/parsers/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.414411 precli-0.5.1/precli/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-23 16:52:17.000000 precli-0.5.1/precli/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-23 16:52:17.000000 precli-0.5.1/precli/renderers/detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-23 16:52:17.000000 precli-0.5.1/precli/renderers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-23 16:52:17.000000 precli-0.5.1/precli/renderers/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-23 16:52:17.000000 precli-0.5.1/precli/renderers/plain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.414411 precli-0.5.1/precli/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.414411 precli-0.5.1/precli/rules/go/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/go/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.414411 precli-0.5.1/precli/rules/go/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/go/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/go/stdlib/crypto_weak_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/go/stdlib/crypto_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/go/stdlib/crypto_weak_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.414411 precli-0.5.1/precli/rules/java/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.414411 precli-0.5.1/precli/rules/java/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/java/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/java/stdlib/java_net_insecure_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/java/stdlib/java_security_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/java/stdlib/java_security_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/java/stdlib/java_security_weak_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/java/stdlib/javax_crypto_weak_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/java/stdlib/javax_servlet_http_insecure_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.414411 precli-0.5.1/precli/rules/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.422411 precli-0.5.1/precli/rules/python/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/argparse_sensitive_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/crypt_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/ftplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/ftplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/hashlib_improper_prng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/hashlib_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/hmac_timing_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/hmac_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/hmac_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/http_server_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/http_url_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/imaplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/imaplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/json_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/logging_insecure_listen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/marshal_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/nntplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/nntplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/poplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/poplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/re_denial_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/secrets_weak_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/shelve_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/smtplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/smtplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/socket_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/socketserver_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/ssl_context_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/ssl_create_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/ssl_insecure_tls_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/telnetlib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-23 16:52:17.000000 precli-0.5.1/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.498411 precli-0.5.1/precli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-23 16:52:26.000000 precli-0.5.1/precli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39386 2024-04-23 16:52:26.000000 precli-0.5.1/precli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:52:26.000000 precli-0.5.1/precli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-23 16:52:26.000000 precli-0.5.1/precli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:52:26.000000 precli-0.5.1/precli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 16:52:26.000000 precli-0.5.1/precli.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-23 16:52:26.000000 precli-0.5.1/precli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 16:52:26.000000 precli-0.5.1/precli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-23 16:52:17.000000 precli-0.5.1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-23 16:52:17.000000 precli-0.5.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.422411 precli-0.5.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-04-23 16:52:17.000000 precli-0.5.1/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-23 16:52:26.502411 precli-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-23 16:52:17.000000 precli-0.5.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 16:52:17.000000 precli-0.5.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.422411 precli-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.422411 precli-0.5.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.422411 precli-0.5.1/tests/unit/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.422411 precli-0.5.1/tests/unit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/core/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.422411 precli-0.5.1/tests/unit/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.426411 precli-0.5.1/tests/unit/parsers/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/expression_list_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/expression_list_assignment_uneven.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/importlib_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_lowercase_rule.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_lowercase_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_multiline.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_multiple_comments.go
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_multiple_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_multiple_rules.go
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_multiple_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_preceding.go
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_preceding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_spaced_rules.go
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_spaced_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_wrong_rule.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/examples/suppress_wrong_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/parsers/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.426411 precli-0.5.1/tests/unit/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.426411 precli-0.5.1/tests/unit/rules/go/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.426411 precli-0.5.1/tests/unit/rules/go/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.426411 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.430411 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_aes.go
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_des.go
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_new.go
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_sum.go
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_new.go
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_sum.go
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_new.go
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_sum.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.430411 precli-0.5.1/tests/unit/rules/java/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.430411 precli-0.5.1/tests/unit/rules/java/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.430411 precli-0.5.1/tests/unit/rules/java/stdlib/java_net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.430411 precli-0.5.1/tests/unit/rules/java/stdlib/java_net/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_net/examples/HttpCookieSecureFalse.java
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_net/examples/HttpCookieSecureTrue.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_net/test_insecure_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.430411 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.434411 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/JavaSecuritySecureRandomSHA1PRNG.java
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD2.java
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5.java
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5Property.java
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestSHA1.java
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestSHA256.java
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/SecureRandomDefault.java
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/SecureRandomSHA1PRNG.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/test_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/test_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/java_security/test_weak_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.434411 precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.434411 precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/Cipher3DESCBC.java
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC4.java
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/test_weak_cipher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.434411 precli-0.5.1/tests/unit/rules/java/stdlib/javax_servlet_http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_servlet_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.434411 precli-0.5.1/tests/unit/rules/java/stdlib/javax_servlet_http/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_servlet_http/examples/CookieSecureFalse.java
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_servlet_http/examples/CookieSecureTrue.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/java/stdlib/javax_servlet_http/test_insecure_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.434411 precli-0.5.1/tests/unit/rules/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.434411 precli-0.5.1/tests/unit/rules/python/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.434411 precli-0.5.1/tests/unit/rules/python/stdlib/argparse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/argparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.438411 precli-0.5.1/tests/unit/rules/python/stdlib/argparse/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_default_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_store_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.438411 precli-0.5.1/tests/unit/rules/python/stdlib/assert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/assert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.438411 precli-0.5.1/tests/unit/rules/python/stdlib/assert/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/assert/examples/assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/assert/test_assert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.438411 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.438411 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.438411 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.442411 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftp_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login_single_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.442411 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.454411 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_pbkdf2_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_as_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_importlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_usedforsecurity_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_usedforsecurity_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_name_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha_usedforsecurity_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha_usedforsecurity_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.454411 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.466411 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha512_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class_hexdigest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_compare_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.466411 precli-0.5.1/tests/unit/rules/python/stdlib/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.470411 precli-0.5.1/tests/unit/rules/python/stdlib/http/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/http/examples/http_server_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/http/examples/http_server_threading_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey_in_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/http/examples/http_url_secret_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/http/examples/http_url_secret_username.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/http/test_http_url_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.470411 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.470411 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login_cram_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.470411 precli-0.5.1/tests/unit/rules/python/stdlib/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.470411 precli-0.5.1/tests/unit/rules/python/stdlib/json/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/json/examples/json_jsondecoder_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/json/examples/json_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/json/examples/json_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/json/test_json_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.474411 precli-0.5.1/tests/unit/rules/python/stdlib/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.474411 precli-0.5.1/tests/unit/rules/python/stdlib/logging/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_empty_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.474411 precli-0.5.1/tests/unit/rules/python/stdlib/marshal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/marshal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.474411 precli-0.5.1/tests/unit/rules/python/stdlib/marshal/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/marshal/examples/marshal_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/marshal/examples/marshal_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.474411 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.474411 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.478411 precli-0.5.1/tests/unit/rules/python/stdlib/pickle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/pickle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.478411 precli-0.5.1/tests/unit/rules/python/stdlib/pickle/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/pickle/examples/pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/pickle/examples/pickle_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/pickle/examples/pickle_unpickler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.478411 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.478411 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_apop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_pass_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_rpop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.478411 precli-0.5.1/tests/unit/rules/python/stdlib/re/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.482411 precli-0.5.1/tests/unit/rules/python/stdlib/re/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/examples/re_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/examples/re_compile_good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/examples/re_findall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/examples/re_finditer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/examples/re_fullmatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/examples/re_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/examples/re_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/examples/re_search_good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/examples/re_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/examples/re_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/examples/re_subn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.482411 precli-0.5.1/tests/unit/rules/python/stdlib/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.482411 precli-0.5.1/tests/unit/rules/python/stdlib/secrets/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_size_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_urlsafe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.482411 precli-0.5.1/tests/unit/rules/python/stdlib/shelve/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/shelve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.482411 precli-0.5.1/tests/unit/rules/python/stdlib/shelve/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/shelve/examples/shelve_dbfilenameshelf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/shelve/examples/shelve_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/shelve/examples/shelve_open_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.486411 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.486411 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.486411 precli-0.5.1/tests/unit/rules/python/stdlib/socket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.486411 precli-0.5.1/tests/unit/rules/python/stdlib/socket/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socket/examples/socket_create_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.486411 precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.490411 precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.490411 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.494411 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/create_default_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/create_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv23.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv12.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP256r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1tls13.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP512r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_default_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_ffdhe2048.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime192v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime256v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp160r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp256r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect163k1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect571k1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_default_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv23.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv11.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv23.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2_server_side_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.498411 precli-0.5.1/tests/unit/rules/python/stdlib/telnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/telnetlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.498411 precli-0.5.1/tests/unit/rules/python/stdlib/telnetlib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/telnetlib/examples/telnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.498411 precli-0.5.1/tests/unit/rules/python/stdlib/tempfile/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/tempfile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.498411 precli-0.5.1/tests/unit/rules/python/stdlib/tempfile/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_with_open_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_walrus_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.498411 precli-0.5.1/tests/unit/rules/python/stdlib/xmlrpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/xmlrpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:52:26.498411 precli-0.5.1/tests/unit/rules/python/stdlib/xmlrpc/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_doc_xml_rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_simple_xml_rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-23 16:52:17.000000 precli-0.5.1/tests/unit/rules/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-23 16:52:17.000000 precli-0.5.1/tox.ini
```

### Comparing `precli-0.5.0/.github/workflows/dependency-review.yml` & `precli-0.5.1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/.github/workflows/publish-to-pypi.yml` & `precli-0.5.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/.github/workflows/publish-to-test-pypi.yml` & `precli-0.5.1/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/.github/workflows/unit-test.yml` & `precli-0.5.1/.github/workflows/unit-test.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/.github/workflows/upload-asset.yml` & `precli-0.5.1/.github/workflows/upload-asset.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/.pre-commit-config.yaml` & `precli-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/CODE_OF_CONDUCT.md` & `precli-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/ChangeLog` & `precli-0.5.1/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 CHANGES
 =======
 
+0.5.1
+-----
+
+* Fix traceback raised on an expression list assignment (#439)
+* Correct the paths given in getting start examples (#438)
+* Trim trailing space in README (#437)
+* README example with wrong path (#436)
+* Simplify the README content (#435)
+* Create a nicer looking banner logo (#434)
+* Increase size of banner logo (#433)
+* Add Java rule for insecure java.net.HttpCookie (#432)
+* Fix broken link in rules table (#431)
+* Add rule to use of Cookie with secure flag false (#430)
+* Add Python requirement to install quick start (#428)
+
 0.5.0
 -----
 
 * Handle method calls with field access (#427)
 * Weak hash and weak random Java rules need to guard from none (#426)
 * Don't break codee with suggested fix (#425)
 * Add rule for detection of weak random algorithm in SecureRandom (#424)
```

### Comparing `precli-0.5.0/LICENSE` & `precli-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/PKG-INFO` & `precli-0.5.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precli
-Version: 0.5.0
+Version: 0.5.1
 Summary: Static analysis security tool command line
 Home-page: https://github.com/securesauce/precli
 Download-URL: https://pypi.org/project/precli/#files
 Author: Secure Sauce
 Project-URL: Release notes, https://github.com/securesauce/precli/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -42,56 +42,35 @@
 Precli is the core of the Precaution GitHub App and Action. It also serves as a command line interface to demonstate its functionality. It is designed to do static code analysis of source code with a number of rules covering the standard library for the corresponding programming language.
 
 If your needs go beyond the analysis of just the standard library, consider upgrading to Precaution Professional to get access to finding and fixing security vulnerabilities in third-party libraries. See https://www.securesauce.dev/ for more details.
 
 Quick Start
 -----------
 
-To install precli:
+To install precli (requires Python 3.12):
 
 .. code-block:: console
 
     pip install precli
 
 Run precli on a single test example:
 
 .. code-block:: console
 
-    precli tests/unit/rules/python/stdlib/examples/hmac_timing_attack.py
+    precli tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
 
-Run precli on a single test example, showing results in SARIF format:
+Example result:
 
 .. code-block:: console
 
-    precli tests/unit/rules/python/stdlib/examples/hmac_timing_attack.py --json
-
-Run precli on a single test example, showing results in plain format:
-
-.. code-block:: console
-
-    precli tests/unit/rules/python/stdlib/examples/hmac_timing_attack.py --plain
-
-Run precli on a single test example, showing results in markdown format:
-
-.. code-block:: console
-
-    precli tests/unit/rules/python/stdlib/examples/hmac_timing_attack.py --markdown
-
-Run precli against all the python test examples:
-
-.. code-block:: console
-
-    precli -r tests/unit/rules/python/stdlib/examples/
-
-Run precli against an entire GitHub repository:
-
-.. code-block:: console
-
-    precli -r https://github.com/securesauce/precli
-
-Run precli against an entire GitHub repository and output the results in markdown format to Gist.
-Note: this requires a GITHUB_TOKEN environment variable set to a valid GitHub token value:
-
-.. code-block:: console
-
-    precli -r https://github.com/securesauce/precli --markdown --gist
+    ⛔️ Error on line 18 in tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
+    PY005: Observable Timing Discrepancy
+    Comparing digests with the '==' operator is vulnerable to timing attacks.
+      17
+    ❱ 18 print(digest == received_digest)
+      19
+    Suggested fix: Use the 'hmac.compare_digest' function instead of the '==' operator to reduce the
+    vulnerability to timing attacks.
+      17
+    ❱ 18 print(hmac.compare_digest(digest, received_digest))
+      19
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `precli-0.5.0/SECURITY.md` & `precli-0.5.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/docs/getting-started.md` & `precli-0.5.1/docs/getting-started.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,39 +10,39 @@
 ```
 
 ## Usage
 
 Run precli on a single test example:
 
 ```
-precli tests/unit/rules/python/stdlib/examples/hmac_timing_attack.py
+precli tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
 ```
 
 Run precli on a single test example, showing results in SARIF format:
 
 ```
-precli tests/unit/rules/python/stdlib/examples/hmac_timing_attack.py --json
+precli tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py --json
 ```
 
 Run precli on a single test example, showing results in plain format:
 
 ```
-precli tests/unit/rules/python/stdlib/examples/hmac_timing_attack.py --plain
+precli tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py --plain
 ```
 
 Run precli on a single test example, showing results in markdown format:
 
 ```
-precli tests/unit/rules/python/stdlib/examples/hmac_timing_attack.py --markdown
+precli tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py --markdown
 ```
 
 Run precli against all the python test examples:
 
 ```
-precli -r tests/unit/rules/python/stdlib/examples/
+precli -r tests/unit/rules/python/
 ```
 
 Run precli against an entire GitHub repository:
 
 ```
 precli -r https://github.com/securesauce/precli
 ```
```

### Comparing `precli-0.5.0/docs/man/precli.rst` & `precli-0.5.1/docs/man/precli.rst`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/docs/rules.md` & `precli-0.5.1/docs/rules.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 | ID | Name | Description |
 |----|------|-------------|
 | JAV001 | [javax.crypto — weak cipher](rules/java/stdlib/javax-crypto-weak-cipher.md) | Use of a Broken or Risky Cryptographic Algorithm in `javax.crypto` Package |
 | JAV002 | [java.security — weak hash](rules/java/stdlib/java-security-weak-hash.md) | Reversible One Way Hash in `java.security` Package |
 | JAV003 | [java.security — weak key](rules/java/stdlib/java-security-weak-key.md) | Inadequate Encryption Strength Using Weak Keys in `java.security` Package |
 | JAV004 | [java.security — weak random](rules/java/stdlib/java-security-weak-random.md) | Use of Cryptographically Weak Pseudo-Random Number Generator `SHA1PRNG` |
+| JAV005 | [javax.servlet.http — insecure cookie](rules/java/stdlib/javax-servlet-http-insecure-cookie.md) | Sensitive Cookie in HTTPS Session Without 'Secure' Attribute |
+| JAV006 | [java.net — insecure cookie](rules/java/stdlib/java-net-insecure-cookie.md) | Sensitive Cookie in HTTPS Session Without 'Secure' Attribute |
 
 ## Python Standard Library
 
 | ID | Name | Description |
 |----|------|-------------|
 | PY001 | [assert](rules/python/stdlib/assert.md) | Improper Check Using `assert` Function |
 | PY002 | [crypt — weak hash](rules/python/stdlib/crypt-weak-hash.md) | Reversible One Way Hash in `crypt` Module |
```

### Comparing `precli-0.5.0/precli/cli/main.py` & `precli-0.5.1/precli/cli/main.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/argument.py` & `precli-0.5.1/precli/core/argument.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/artifact.py` & `precli-0.5.1/precli/core/artifact.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/call.py` & `precli-0.5.1/precli/core/call.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/comparison.py` & `precli-0.5.1/precli/core/comparison.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/config.py` & `precli-0.5.1/precli/core/config.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/fix.py` & `precli-0.5.1/precli/core/fix.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/kind.py` & `precli-0.5.1/precli/core/kind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/level.py` & `precli-0.5.1/precli/core/level.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/linecache.py` & `precli-0.5.1/precli/core/linecache.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/location.py` & `precli-0.5.1/precli/core/location.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/metrics.py` & `precli-0.5.1/precli/core/metrics.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/redos.py` & `precli-0.5.1/precli/core/redos.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/result.py` & `precli-0.5.1/precli/core/result.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/run.py` & `precli-0.5.1/precli/core/run.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/suppression.py` & `precli-0.5.1/precli/core/suppression.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/symtab.py` & `precli-0.5.1/precli/core/symtab.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/tool.py` & `precli-0.5.1/precli/core/tool.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/core/utils.py` & `precli-0.5.1/precli/core/utils.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/parsers/__init__.py` & `precli-0.5.1/precli/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/parsers/go.py` & `precli-0.5.1/precli/parsers/go.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/parsers/java.py` & `precli-0.5.1/precli/parsers/java.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,14 +132,15 @@
             and var_nodes[0].type
             in (
                 tokens.IDENTIFIER,
                 tokens.SCOPED_TYPE_IDENTIFIER,
             )
             and var_nodes[1].type
             in (
+                tokens.OBJECT_CREATION_EXPRESSION,
                 tokens.METHOD_INVOCATION,
                 tokens.ATTRIBUTE,
                 tokens.IDENTIFIER,
                 tokens.STRING_LITERAL,
                 tokens.CHARACTER_LITERAL,
                 tokens.DECIMAL_INTEGER_LITERAL,
                 tokens.HEX_INTEGER_LITERAL,
@@ -160,94 +161,107 @@
             )
 
             # This is to help full resolution of an attribute/call.
             # This results in two entries in the symtab for this assignment.
             self.current_symtab.put(left_hand, tokens.IDENTIFIER, right_hand)
 
             if var_nodes[1].type == tokens.METHOD_INVOCATION:
-                meth_invoke = var_nodes[1]
-                if (
-                    meth_invoke.children[1].type == "."
-                    and meth_invoke.children[2].type == tokens.IDENTIFIER
-                ):
-                    # (field_access | identifier) "." identifier argument_list
-                    obj_node = meth_invoke.children[0]
-                    method_node = meth_invoke.children[2]
-                else:
-                    # identifier argument_list
-                    obj_node = meth_invoke.children[0]
-                    method_node = meth_invoke.children[0]
-
-                arg_list_node = self.child_by_type(
-                    meth_invoke, tokens.ARGUMENT_LIST
-                )
-                call_args = self.get_func_args(arg_list_node)
-
-                call = Call(
-                    node=var_nodes[1],
-                    name=right_hand,
-                    name_qual=right_hand,
-                    # func_node=func_node, # no equivalent for Java
-                    var_node=obj_node,
-                    ident_node=method_node,
-                    arg_list_node=arg_list_node,
-                    args=call_args,
-                )
+                call = self.method_call(var_nodes[1], right_hand)
                 symbol = self.current_symtab.get(left_hand)
                 symbol.push_call(call)
 
         self.visit(nodes)
 
+    def visit_object_creation_expression(self, nodes: list[Node]):
+        if nodes[0].type != "new":
+            return
+
+        if nodes[1].type not in (
+            tokens.TYPE_IDENTIFIER,
+            tokens.SCOPED_TYPE_IDENTIFIER,
+        ):
+            return
+
+        # "new" (type_identifier | scoped_type_identifier) argument_list
+
+        cls_name = self.resolve(nodes[1])
+        if cls_name is None:
+            return
+        func_call_qual = cls_name
+
+        call = self.method_call(self.context["node"], func_call_qual)
+        self.analyze_node(tokens.OBJECT_CREATION_EXPRESSION, call=call)
+
+        self.visit(nodes)
+
     def visit_method_invocation(self, nodes: list[Node]):
-        meth_invoke = self.context["node"]
         if nodes[0].type not in (tokens.FIELD_ACCESS, tokens.IDENTIFIER):
             return
 
         if nodes[1].type == "." and nodes[2].type == tokens.IDENTIFIER:
             # (field_access | identifier) "." identifier argument_list
-            obj_node = nodes[0]
-            method_node = nodes[2]
-
-            obj_name = self.resolve(obj_node)
-            method = method_node.text.decode()
+            obj_name = self.resolve(nodes[0])
+            method = nodes[2].text.decode()
             if None in (obj_name, method):
                 return
-
             func_call_qual = ".".join([obj_name, method])
         else:
             # identifier argument_list
-            obj_node = nodes[0]
-            method_node = nodes[0]
-            method_name = self.resolve(method_node)
+            method_name = self.resolve(nodes[0])
             if method_name is None:
                 return
             func_call_qual = method_name
 
-        arg_list_node = self.child_by_type(meth_invoke, tokens.ARGUMENT_LIST)
+        call = self.method_call(self.context["node"], func_call_qual)
+        self.analyze_node(tokens.METHOD_INVOCATION, call=call)
+
+        symbol = self.current_symtab.get(call.var_node.text.decode())
+        if symbol is not None and symbol.type == tokens.IDENTIFIER:
+            symbol.push_call(call)
+
+        self.visit(nodes)
+
+    def method_call(self, node: Node, func_call_qual: str):
+        if (
+            node.children[1].type == "."
+            and node.children[2].type == tokens.IDENTIFIER
+        ):
+            # (field_access | identifier) "." identifier argument_list
+            func_node = None
+            obj_node = node.children[0]
+            method_node = node.children[2]
+        elif node.children[1].type in (
+            tokens.TYPE_IDENTIFIER,
+            tokens.SCOPED_TYPE_IDENTIFIER,
+        ):
+            # "new" (type_identifier | scoped_type_identifier) argument_list
+            func_node = node.children[1]
+            # TODO: get the obj_node and method_node from func_node
+            obj_node = None
+            method_node = None
+        else:
+            # identifier argument_list
+            func_node = None
+            obj_node = node.children[0]
+            method_node = node.children[0]
+
+        arg_list_node = self.child_by_type(node, tokens.ARGUMENT_LIST)
         call_args = self.get_func_args(arg_list_node)
 
-        call = Call(
-            node=meth_invoke,
+        return Call(
+            node=node,
             name=func_call_qual,
             name_qual=func_call_qual,
-            # func_node=func_node, # no equivalent for Java
+            func_node=func_node,
             var_node=obj_node,
             ident_node=method_node,
             arg_list_node=arg_list_node,
             args=call_args,
         )
 
-        self.analyze_node(tokens.METHOD_INVOCATION, call=call)
-
-        symbol = self.current_symtab.get(call.var_node.text.decode())
-        if symbol is not None and symbol.type == tokens.IDENTIFIER:
-            symbol.push_call(call)
-
-        self.visit(nodes)
-
     def get_func_args(self, node: Node) -> list:
         if node.type != tokens.ARGUMENT_LIST:
             return []
 
         args = []
         for child in node.named_children:
             args.append(self.resolve(child, default=child))
@@ -269,14 +283,35 @@
         """
         nodetext = node.text.decode()
         if isinstance(default, Node):
             default = default.text.decode()
 
         try:
             match node.type:
+                case tokens.OBJECT_CREATION_EXPRESSION:
+                    # "new" (type_identifier | scoped_type_identifier)
+                    # argument_list
+                    if node.children[0].type == "new" and node.children[
+                        1
+                    ].type in (
+                        tokens.TYPE_IDENTIFIER,
+                        tokens.SCOPED_TYPE_IDENTIFIER,
+                    ):
+                        nodetext = node.children[1].text.decode()
+                        if (
+                            node.children[1].type
+                            == tokens.SCOPED_TYPE_IDENTIFIER
+                        ):
+                            symbol = Symbol(
+                                nodetext, tokens.IDENTIFIER, nodetext
+                            )
+                        else:
+                            symbol = self.get_qual_name(node.children[1])
+                        if symbol is not None:
+                            value = self.join_symbol(nodetext, symbol)
                 case tokens.METHOD_INVOCATION:
                     if (
                         node.children[1].type == "."
                         and node.children[2].type == tokens.IDENTIFIER
                     ):
                         # (field_access | identifier) "." identifier
                         # argument_list
@@ -287,16 +322,15 @@
                         # identifier argument_list
                         nodetext = node.children[0].text.decode()
                     symbol = self.get_qual_name(node.children[0])
                     if symbol is not None:
                         value = self.join_symbol(nodetext, symbol)
                 case tokens.FIELD_ACCESS:
                     symbol = Symbol(nodetext, tokens.IDENTIFIER, nodetext)
-                    if symbol is not None:
-                        value = self.join_symbol(nodetext, symbol)
+                    value = self.join_symbol(nodetext, symbol)
                 case tokens.IDENTIFIER:
                     symbol = self.get_qual_name(node)
                     if symbol is not None:
                         value = self.join_symbol(nodetext, symbol)
                 case tokens.STRING_LITERAL:
                     value = nodetext
                 case tokens.CHARACTER_LITERAL:
```

### Comparing `precli-0.5.0/precli/parsers/python.py` & `precli-0.5.1/precli/parsers/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             self.current_symtab.put(left_hand, tokens.IDENTIFIER, right_hand)
 
             if nodes[2].type == tokens.CALL:
                 (call_args, call_kwargs) = self.get_func_args(
                     nodes[2].children[1]
                 )
 
-                if self.context["node"].children:
+                if nodes[2].children:
                     # (attribute | identifier) argument_list
                     func_node = nodes[2].children[0]
                     var_node = self._get_var_node(func_node)
                     ident_node = self._get_func_ident(func_node)
                     arg_list_node = nodes[2].children[1]
 
                 call = Call(
```

### Comparing `precli-0.5.0/precli/parsers/tokens.py` & `precli-0.5.1/precli/parsers/tokens.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 PACKAGE_IDENTIFIER = "package_identifier"
 BLANK_IDENTIFIER = "blank_identifier"
 ALIASED_IMPORT = "aliased_import"
 RELATIVE_IMPORT = "relative_import"
 WILDCARD_IMPORT = "wildcard_import"
 CALL = "call"
 CALL_EXPRESSION = "call_expression"
+OBJECT_CREATION_EXPRESSION = "object_creation_expression"
 METHOD_INVOCATION = "method_invocation"
 ARGUMENT_LIST = "argument_list"
 KEYWORD_ARGUMENT = "keyword_argument"
 ASSIGNMENT = "assignment"
 PATTERN_LIST = "pattern_list"
 EXPRESSION_LIST = "expression_list"
 TYPE_IDENTIFIER = "type_identifier"
```

### Comparing `precli-0.5.0/precli/renderers/__init__.py` & `precli-0.5.1/precli/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/renderers/detailed.py` & `precli-0.5.1/precli/renderers/detailed.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/renderers/json.py` & `precli-0.5.1/precli/renderers/json.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/renderers/markdown.py` & `precli-0.5.1/precli/renderers/markdown.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/renderers/plain.py` & `precli-0.5.1/precli/renderers/plain.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/__init__.py` & `precli-0.5.1/precli/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/go/stdlib/crypto_weak_cipher.py` & `precli-0.5.1/precli/rules/go/stdlib/crypto_weak_cipher.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/go/stdlib/crypto_weak_hash.py` & `precli-0.5.1/precli/rules/go/stdlib/crypto_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/go/stdlib/crypto_weak_key.py` & `precli-0.5.1/precli/rules/go/stdlib/crypto_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/java/stdlib/java_security_weak_hash.py` & `precli-0.5.1/precli/rules/java/stdlib/java_security_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/java/stdlib/java_security_weak_key.py` & `precli-0.5.1/precli/rules/java/stdlib/java_security_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/java/stdlib/java_security_weak_random.py` & `precli-0.5.1/precli/rules/java/stdlib/java_security_weak_random.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/java/stdlib/javax_crypto_weak_cipher.py` & `precli-0.5.1/precli/rules/java/stdlib/javax_crypto_weak_cipher.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/argparse_sensitive_info.py` & `precli-0.5.1/precli/rules/python/stdlib/argparse_sensitive_info.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/assert.py` & `precli-0.5.1/precli/rules/python/stdlib/assert.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/crypt_weak_hash.py` & `precli-0.5.1/precli/rules/python/stdlib/crypt_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/ftplib_cleartext.py` & `precli-0.5.1/precli/rules/python/stdlib/ftplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/ftplib_unverified_context.py` & `precli-0.5.1/precli/rules/python/stdlib/ftplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/hashlib_improper_prng.py` & `precli-0.5.1/precli/rules/python/stdlib/hashlib_improper_prng.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/hashlib_weak_hash.py` & `precli-0.5.1/precli/rules/python/stdlib/hashlib_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/hmac_timing_attack.py` & `precli-0.5.1/precli/rules/python/stdlib/hmac_timing_attack.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/hmac_weak_hash.py` & `precli-0.5.1/precli/rules/python/stdlib/hmac_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/hmac_weak_key.py` & `precli-0.5.1/precli/rules/python/stdlib/hmac_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/http_server_unrestricted_bind.py` & `precli-0.5.1/precli/rules/python/stdlib/http_server_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/http_url_secret.py` & `precli-0.5.1/precli/rules/python/stdlib/http_url_secret.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/imaplib_cleartext.py` & `precli-0.5.1/precli/rules/python/stdlib/imaplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/imaplib_unverified_context.py` & `precli-0.5.1/precli/rules/python/stdlib/imaplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/json_load.py` & `precli-0.5.1/precli/rules/python/stdlib/json_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/logging_insecure_listen_config.py` & `precli-0.5.1/precli/rules/python/stdlib/logging_insecure_listen_config.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/marshal_load.py` & `precli-0.5.1/precli/rules/python/stdlib/marshal_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/nntplib_cleartext.py` & `precli-0.5.1/precli/rules/python/stdlib/nntplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/nntplib_unverified_context.py` & `precli-0.5.1/precli/rules/python/stdlib/nntplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/pickle_load.py` & `precli-0.5.1/precli/rules/python/stdlib/pickle_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/poplib_cleartext.py` & `precli-0.5.1/precli/rules/python/stdlib/poplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/poplib_unverified_context.py` & `precli-0.5.1/precli/rules/python/stdlib/poplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/re_denial_of_service.py` & `precli-0.5.1/precli/rules/python/stdlib/re_denial_of_service.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/secrets_weak_token.py` & `precli-0.5.1/precli/rules/python/stdlib/secrets_weak_token.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/shelve_open.py` & `precli-0.5.1/precli/rules/python/stdlib/shelve_open.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/smtplib_cleartext.py` & `precli-0.5.1/precli/rules/python/stdlib/smtplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/smtplib_unverified_context.py` & `precli-0.5.1/precli/rules/python/stdlib/smtplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/socket_unrestricted_bind.py` & `precli-0.5.1/precli/rules/python/stdlib/socket_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/socketserver_unrestricted_bind.py` & `precli-0.5.1/precli/rules/python/stdlib/socketserver_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/ssl_context_weak_key.py` & `precli-0.5.1/precli/rules/python/stdlib/ssl_context_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/ssl_create_unverified_context.py` & `precli-0.5.1/precli/rules/python/stdlib/ssl_create_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/ssl_insecure_tls_version.py` & `precli-0.5.1/precli/rules/python/stdlib/ssl_insecure_tls_version.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/telnetlib_cleartext.py` & `precli-0.5.1/precli/rules/python/stdlib/telnetlib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py` & `precli-0.5.1/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py` & `precli-0.5.1/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/precli.egg-info/PKG-INFO` & `precli-0.5.1/precli.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precli
-Version: 0.5.0
+Version: 0.5.1
 Summary: Static analysis security tool command line
 Home-page: https://github.com/securesauce/precli
 Download-URL: https://pypi.org/project/precli/#files
 Author: Secure Sauce
 Project-URL: Release notes, https://github.com/securesauce/precli/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -42,56 +42,35 @@
 Precli is the core of the Precaution GitHub App and Action. It also serves as a command line interface to demonstate its functionality. It is designed to do static code analysis of source code with a number of rules covering the standard library for the corresponding programming language.
 
 If your needs go beyond the analysis of just the standard library, consider upgrading to Precaution Professional to get access to finding and fixing security vulnerabilities in third-party libraries. See https://www.securesauce.dev/ for more details.
 
 Quick Start
 -----------
 
-To install precli:
+To install precli (requires Python 3.12):
 
 .. code-block:: console
 
     pip install precli
 
 Run precli on a single test example:
 
 .. code-block:: console
 
-    precli tests/unit/rules/python/stdlib/examples/hmac_timing_attack.py
+    precli tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
 
-Run precli on a single test example, showing results in SARIF format:
+Example result:
 
 .. code-block:: console
 
-    precli tests/unit/rules/python/stdlib/examples/hmac_timing_attack.py --json
-
-Run precli on a single test example, showing results in plain format:
-
-.. code-block:: console
-
-    precli tests/unit/rules/python/stdlib/examples/hmac_timing_attack.py --plain
-
-Run precli on a single test example, showing results in markdown format:
-
-.. code-block:: console
-
-    precli tests/unit/rules/python/stdlib/examples/hmac_timing_attack.py --markdown
-
-Run precli against all the python test examples:
-
-.. code-block:: console
-
-    precli -r tests/unit/rules/python/stdlib/examples/
-
-Run precli against an entire GitHub repository:
-
-.. code-block:: console
-
-    precli -r https://github.com/securesauce/precli
-
-Run precli against an entire GitHub repository and output the results in markdown format to Gist.
-Note: this requires a GITHUB_TOKEN environment variable set to a valid GitHub token value:
-
-.. code-block:: console
-
-    precli -r https://github.com/securesauce/precli --markdown --gist
+    ⛔️ Error on line 18 in tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
+    PY005: Observable Timing Discrepancy
+    Comparing digests with the '==' operator is vulnerable to timing attacks.
+      17
+    ❱ 18 print(digest == received_digest)
+      19
+    Suggested fix: Use the 'hmac.compare_digest' function instead of the '==' operator to reduce the
+    vulnerability to timing attacks.
+      17
+    ❱ 18 print(hmac.compare_digest(digest, received_digest))
+      19
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `precli-0.5.0/precli.egg-info/SOURCES.txt` & `precli-0.5.1/precli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 docs/index.md
 docs/requirements.txt
 docs/rules.md
 docs/man/precli.rst
 docs/rules/go/stdlib/crypto-weak-cipher.md
 docs/rules/go/stdlib/crypto-weak-hash.md
 docs/rules/go/stdlib/crypto-weak-key.md
+docs/rules/java/stdlib/java-net-insecure-cookie.md
 docs/rules/java/stdlib/java-security-weak-hash.md
 docs/rules/java/stdlib/java-security-weak-key.md
 docs/rules/java/stdlib/java-security-weak-random.md
 docs/rules/java/stdlib/javax-crypto-weak-cipher.md
+docs/rules/java/stdlib/javax-servlet-http-insecure-cookie.md
 docs/rules/python/stdlib/argparse-sensitive-info.md
 docs/rules/python/stdlib/assert.md
 docs/rules/python/stdlib/crypt-weak-hash.md
 docs/rules/python/stdlib/ftplib-cleartext.md
 docs/rules/python/stdlib/ftplib-unverified-context.md
 docs/rules/python/stdlib/hashlib-improper-prng.md
 docs/rules/python/stdlib/hashlib-weak-hash.md
@@ -116,18 +118,20 @@
 precli/rules/go/__init__.py
 precli/rules/go/stdlib/__init__.py
 precli/rules/go/stdlib/crypto_weak_cipher.py
 precli/rules/go/stdlib/crypto_weak_hash.py
 precli/rules/go/stdlib/crypto_weak_key.py
 precli/rules/java/__init__.py
 precli/rules/java/stdlib/__init__.py
+precli/rules/java/stdlib/java_net_insecure_cookie.py
 precli/rules/java/stdlib/java_security_weak_hash.py
 precli/rules/java/stdlib/java_security_weak_key.py
 precli/rules/java/stdlib/java_security_weak_random.py
 precli/rules/java/stdlib/javax_crypto_weak_cipher.py
+precli/rules/java/stdlib/javax_servlet_http_insecure_cookie.py
 precli/rules/python/__init__.py
 precli/rules/python/stdlib/__init__.py
 precli/rules/python/stdlib/argparse_sensitive_info.py
 precli/rules/python/stdlib/assert.py
 precli/rules/python/stdlib/crypt_weak_hash.py
 precli/rules/python/stdlib/ftplib_cleartext.py
 precli/rules/python/stdlib/ftplib_unverified_context.py
@@ -167,14 +171,15 @@
 tests/unit/cli/__init__.py
 tests/unit/core/__init__.py
 tests/unit/core/test_python.py
 tests/unit/parsers/__init__.py
 tests/unit/parsers/test_go.py
 tests/unit/parsers/test_python.py
 tests/unit/parsers/examples/expression_list_assignment.py
+tests/unit/parsers/examples/expression_list_assignment_uneven.py
 tests/unit/parsers/examples/importlib_import_module.py
 tests/unit/parsers/examples/suppress.go
 tests/unit/parsers/examples/suppress.py
 tests/unit/parsers/examples/suppress_lowercase_rule.go
 tests/unit/parsers/examples/suppress_lowercase_rule.py
 tests/unit/parsers/examples/suppress_multiline.go
 tests/unit/parsers/examples/suppress_multiline.py
@@ -210,14 +215,18 @@
 tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go
 tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go
 tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go
 tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go
 tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go
 tests/unit/rules/java/__init__.py
 tests/unit/rules/java/stdlib/__init__.py
+tests/unit/rules/java/stdlib/java_net/__init__.py
+tests/unit/rules/java/stdlib/java_net/test_insecure_cookie.py
+tests/unit/rules/java/stdlib/java_net/examples/HttpCookieSecureFalse.java
+tests/unit/rules/java/stdlib/java_net/examples/HttpCookieSecureTrue.java
 tests/unit/rules/java/stdlib/java_security/__init__.py
 tests/unit/rules/java/stdlib/java_security/test_weak_hash.py
 tests/unit/rules/java/stdlib/java_security/test_weak_key.py
 tests/unit/rules/java/stdlib/java_security/test_weak_random.py
 tests/unit/rules/java/stdlib/java_security/examples/JavaSecuritySecureRandomSHA1PRNG.java
 tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java
 tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java
@@ -234,14 +243,18 @@
 tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java
 tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java
 tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java
 tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java
 tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java
 tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC4.java
 tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java
+tests/unit/rules/java/stdlib/javax_servlet_http/__init__.py
+tests/unit/rules/java/stdlib/javax_servlet_http/test_insecure_cookie.py
+tests/unit/rules/java/stdlib/javax_servlet_http/examples/CookieSecureFalse.java
+tests/unit/rules/java/stdlib/javax_servlet_http/examples/CookieSecureTrue.java
 tests/unit/rules/python/__init__.py
 tests/unit/rules/python/stdlib/__init__.py
 tests/unit/rules/python/stdlib/argparse/__init__.py
 tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py
 tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_api_key.py
 tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_default_action.py
 tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password.py
```

### Comparing `precli-0.5.0/precli.egg-info/entry_points.txt` & `precli-0.5.1/precli.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 GO003 = precli.rules.go.stdlib.crypto_weak_key:WeakKey
 
 [precli.rules.java]
 JAV001 = precli.rules.java.stdlib.javax_crypto_weak_cipher:WeakCipher
 JAV002 = precli.rules.java.stdlib.java_security_weak_hash:MessageDigestWeakHash
 JAV003 = precli.rules.java.stdlib.java_security_weak_key:KeyPairGeneratorWeakKey
 JAV004 = precli.rules.java.stdlib.java_security_weak_random:SecureRandomWeakRandom
+JAV005 = precli.rules.java.stdlib.javax_servlet_http_insecure_cookie:InsecureCookie
+JAV006 = precli.rules.java.stdlib.java_net_insecure_cookie:InsecureCookie
 
 [precli.rules.python]
 PY001 = precli.rules.python.stdlib.assert:Assert
 PY002 = precli.rules.python.stdlib.crypt_weak_hash:CryptWeakHash
 PY003 = precli.rules.python.stdlib.ftplib_cleartext:FtpCleartext
 PY004 = precli.rules.python.stdlib.hashlib_weak_hash:HashlibWeakHash
 PY005 = precli.rules.python.stdlib.hmac_timing_attack:HmacTimingAttack
```

### Comparing `precli-0.5.0/pylintrc` & `precli-0.5.1/pylintrc`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/setup.cfg` & `precli-0.5.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,18 @@
 	JAV001 = precli.rules.java.stdlib.javax_crypto_weak_cipher:WeakCipher
 	
 	JAV002 = precli.rules.java.stdlib.java_security_weak_hash:MessageDigestWeakHash
 	
 	JAV003 = precli.rules.java.stdlib.java_security_weak_key:KeyPairGeneratorWeakKey
 	
 	JAV004 = precli.rules.java.stdlib.java_security_weak_random:SecureRandomWeakRandom
+	
+	JAV005 = precli.rules.java.stdlib.javax_servlet_http_insecure_cookie:InsecureCookie
+	
+	JAV006 = precli.rules.java.stdlib.java_net_insecure_cookie:InsecureCookie
 precli.rules.python = 
 	PY001 = precli.rules.python.stdlib.assert:Assert
 	
 	PY002 = precli.rules.python.stdlib.crypt_weak_hash:CryptWeakHash
 	
 	PY003 = precli.rules.python.stdlib.ftplib_cleartext:FtpCleartext
```

### Comparing `precli-0.5.0/tests/unit/parsers/test_go.py` & `precli-0.5.1/tests/unit/parsers/test_go.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/parsers/test_python.py` & `precli-0.5.1/tests/unit/parsers/test_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,23 @@
     def test_expression_list_assignment(self):
         artifact = Artifact(
             os.path.join(self.base_path, "expression_list_assignment.py")
         )
         results = self.parser.parse(artifact)
         self.assertEqual(0, len(results))
 
+    def test_expression_list_assignment_uneven(self):
+        artifact = Artifact(
+            os.path.join(
+                self.base_path, "expression_list_assignment_uneven.py"
+            )
+        )
+        results = self.parser.parse(artifact)
+        self.assertEqual(0, len(results))
+
     def test_importlib_import_module(self):
         artifact = Artifact(
             os.path.join(self.base_path, "importlib_import_module.py")
         )
         results = self.parser.parse(artifact)
         self.assertEqual(0, len(results))
```

### Comparing `precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go` & `precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go` & `precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go` & `precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go` & `precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go` & `precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go` & `precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go` & `precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go` & `precli-0.5.1/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py` & `precli-0.5.1/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py` & `precli-0.5.1/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py` & `precli-0.5.1/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java` & `precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java` & `precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5Property.java` & `precli-0.5.1/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5Property.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/java_security/test_weak_hash.py` & `precli-0.5.1/tests/unit/rules/java/stdlib/java_security/test_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/java_security/test_weak_key.py` & `precli-0.5.1/tests/unit/rules/java/stdlib/java_security/test_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/java_security/test_weak_random.py` & `precli-0.5.1/tests/unit/rules/java/stdlib/java_security/test_weak_random.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/Cipher3DESCBC.java` & `precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/Cipher3DESCBC.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java` & `precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java` & `precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java` & `precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java` & `precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java` & `precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java` & `precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/java/stdlib/javax_crypto/test_weak_cipher.py` & `precli-0.5.1/tests/unit/rules/java/stdlib/javax_crypto/test_weak_cipher.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/assert/test_assert.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/assert/test_assert.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/http/test_http_url_secret.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/http/test_http_url_secret.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/json/test_json_load.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/json/test_json_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py` & `precli-0.5.1/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tests/unit/rules/test_case.py` & `precli-0.5.1/tests/unit/rules/test_case.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.0/tox.ini` & `precli-0.5.1/tox.ini`

 * *Files identical despite different names*


# Comparing `tmp/bowtie_json_schema-2024.4.4.tar.gz` & `tmp/bowtie_json_schema-2024.4.5.tar.gz`

## Comparing `bowtie_json_schema-2024.4.4.tar` & `bowtie_json_schema-2024.4.5.tar`

### file list

```diff
@@ -1,237 +1,245 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.gitpod.Dockerfile
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.gitpod.yml
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.prettierrc.json
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.readthedocs.yaml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/action.yml
--rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/noxfile.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/requirements.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/test-requirements.in
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/test-requirements.txt
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.devcontainer/devcontainer.json
--rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.pre-commit-hooks/check-dependabot
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.pre-commit-hooks/check-lintsonschema-schema
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/__main__.py
--rw-r--r--   0        0        0    49511 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/_cli.py
--rw-r--r--   0        0        0    11243 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/_commands.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/_containers.py
--rw-r--r--   0        0        0    21271 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/_core.py
--rw-r--r--   0        0        0    11162 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/_report.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/_suite.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/exceptions.py
--rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/hypothesis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/py.typed
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/models/dialect.json
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/models/group.json
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/models/implementation.json
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/models/registry.json
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/models/test.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/data/dialects.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/Makefile
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/cli.rst
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/conf.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/contributing.rst
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/github-actions.rst
--rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/implementers.rst
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/index.rst
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/motd.txt
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/requirements.in
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/requirements.txt
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/_static/bowtie_diagram_dark.svg
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/_static/bowtie_diagram_light.svg
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/_static/logo.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/index.html
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/package.json
--rw-r--r--   0        0        0   165892 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/tsconfig.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/vite.config.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/public/favicon.svg
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/DialectReportView.tsx
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/MainContainer.tsx
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/ReportDataHandler.tsx
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/global.css
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/index.tsx
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/assets/landscape-logo.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/CopyToClipboard.tsx
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/FilterSection.css
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/FilterSection.tsx
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/LoadingAnimation.tsx
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/NavBar.tsx
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/OtherImplementations.tsx
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CaseItem.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CaseResultSvg.test.tsx
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CaseResultSvg.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CasesSection.tsx
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Cases/SchemaDisplay.tsx
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/DragAndDrop/DragAndDrop.tsx
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Modals/DetailsButtonModal.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/RunInfo/RunInfoSection.tsx
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Summary/ImplementationRow.tsx
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Summary/SummarySection.tsx
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Summary/SummaryTable.tsx
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/context/BowtieVersionContext.tsx
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/context/ThemeContext.tsx
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/Badge.test.ts
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/Badge.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/Dialect.test.ts
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/Dialect.ts
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/Site.test.ts
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/Site.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/mapLanguage.ts
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/parseReportData.test.ts
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/hooks/useSearchParams.ts
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/.java-implementations-pmd-ruleset.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/clojure-json-schema/Dockerfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/clojure-json-schema/project.clj
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/cpp-valijson/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/cpp-valijson/.gitignore
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/cpp-valijson/Dockerfile
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/cpp-valijson/bowtie_valijson.cpp
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/cpp-valijson/compile_flags.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/.clang-format
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/Dockerfile
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/Program.cs
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-gojsonschema/Dockerfile
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-gojsonschema/bowtie_gojsonschema.go
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-gojsonschema/go.mod
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-gojsonschema/go.sum
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-jsonschema/Dockerfile
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-jsonschema/bowtie_jsonschema.go
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-jsonschema/go.mod
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-jsonschema/go.sum
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-json-schema/BowtieJsonSchema.java
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-json-schema/Dockerfile
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-json-schema/build.gradle
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-json-schema-validator/build.gradle
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-jsonschemafriend/Dockerfile
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-jsonschemafriend/build.gradle
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/.dockerignore
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/.editorconfig
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/Dockerfile
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/build.gradle.kts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/gradle.properties
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/justfile
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/settings.gradle.kts
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/gradle/libs.versions.toml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-ajv/Dockerfile
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-ajv/bowtie_ajv.js
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-ajv/package-lock.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-ajv/package.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-hyperjump/Dockerfile
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-hyperjump/bowtie_hyperjump.js
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-hyperjump/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-jsonschema/bowtie_jsonschema.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-jsonschema/package.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/.gitignore
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/bowtie_jsonschema.lua
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/json.lua
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/stylua.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/php-opis-json-schema/Dockerfile
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/php-opis-json-schema/bowtieJsonSchema.php
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/php-opis-json-schema/composer.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/python-fastjsonschema/Dockerfile
--rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/python-jschon/Dockerfile
--rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/python-jschon/bowtie_jschon.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/python-jsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/python-jsonschema/bowtie_jsonschema.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ruby-json_schemer/.rubocop.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ruby-json_schemer/Dockerfile
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ruby-json_schemer/Gemfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ruby-json_schemer/Gemfile.lock
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ruby-json_schemer/bowtie_json_schemer.rb
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-boon/Cargo.lock
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-boon/Cargo.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-boon/Dockerfile
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-boon/build.rs
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-boon/src/main.rs
--rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/Cargo.lock
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/Cargo.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/Dockerfile
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/build.rs
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/src/main.rs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/Dockerfile
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/Harness.scala
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/project/plugins.sbt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/Dockerfile
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/Harness.scala
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/project/plugins.sbt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ts-vscode-json-languageservice/Dockerfile
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ts-vscode-json-languageservice/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ts-vscode-json-languageservice/tsconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/conftest.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_cli.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_dialect.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_github.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_hypothesis.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_implementation.py
--rw-r--r--   0        0        0    64095 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_integration.py
--rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_report.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_schemas.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/group.json
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/test.json
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/LICENSE
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/README.rst
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/hatch_build.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/pyproject.toml
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/.gitpod.yml
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/.prettierrc.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/action.yml
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/noxfile.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/requirements.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/test-requirements.in
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/test-requirements.txt
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/.pre-commit-hooks/check-dependabot
+-rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/.pre-commit-hooks/check-lintsonschema-schema
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/__main__.py
+-rw-r--r--   0        0        0    49283 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/_cli.py
+-rw-r--r--   0        0        0    11243 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/_commands.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/_containers.py
+-rw-r--r--   0        0        0    21271 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/_core.py
+-rw-r--r--   0        0        0    11162 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/_report.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/_suite.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/exceptions.py
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/hypothesis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/py.typed
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/cli/info.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/cli/summary.json
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/models/dialect.json
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/bowtie/schemas/models/test.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/data/dialects.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/Makefile
+-rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/cli.rst
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/conf.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/contributing.rst
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/github-actions.rst
+-rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/implementers.rst
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/index.rst
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/motd.txt
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/requirements.in
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/requirements.txt
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/_static/bowtie_diagram_dark.svg
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/_static/bowtie_diagram_light.svg
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/docs/_static/logo.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/index.html
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/package.json
+-rw-r--r--   0        0        0   165892 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/tsconfig.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/vite.config.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/public/favicon.svg
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/DialectReportView.tsx
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/MainContainer.tsx
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/ReportDataHandler.tsx
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/global.css
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/index.tsx
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/assets/landscape-logo.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/CopyToClipboard.tsx
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/FilterSection.css
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/FilterSection.tsx
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/LoadingAnimation.tsx
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/NavBar.tsx
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/OtherImplementations.tsx
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/Cases/CaseItem.tsx
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/Cases/CaseResultSvg.test.tsx
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/Cases/CaseResultSvg.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/Cases/CasesSection.tsx
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/Cases/SchemaDisplay.tsx
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/DragAndDrop/DragAndDrop.tsx
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/Modals/DetailsButtonModal.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/RunInfo/RunInfoSection.tsx
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/Summary/ImplementationRow.tsx
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/Summary/SummarySection.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/components/Summary/SummaryTable.tsx
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/context/BowtieVersionContext.tsx
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/context/ThemeContext.tsx
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/data/Badge.test.ts
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/data/Badge.ts
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/data/Dialect.test.ts
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/data/Dialect.ts
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/data/Site.test.ts
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/data/Site.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/data/mapLanguage.ts
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/data/parseReportData.test.ts
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/frontend/src/hooks/useSearchParams.ts
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/.java-implementations-pmd-ruleset.xml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/clojure-json-schema/Dockerfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/clojure-json-schema/project.clj
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/cpp-valijson/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/cpp-valijson/.gitignore
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/cpp-valijson/Dockerfile
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/cpp-valijson/bowtie_valijson.cpp
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/cpp-valijson/compile_flags.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/dotnet-jsonschema-net/.clang-format
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/dotnet-jsonschema-net/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/dotnet-jsonschema-net/Dockerfile
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/dotnet-jsonschema-net/Program.cs
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/go-gojsonschema/Dockerfile
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/go-gojsonschema/bowtie_gojsonschema.go
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/go-gojsonschema/go.mod
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/go-gojsonschema/go.sum
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-json-schema/BowtieJsonSchema.java
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-json-schema/Dockerfile
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-json-schema/build.gradle
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-jsonschemafriend/Dockerfile
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-jsonschemafriend/build.gradle
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/.dockerignore
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/.editorconfig
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/Dockerfile
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/build.gradle.kts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/gradle.properties
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/justfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/settings.gradle.kts
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/gradle/libs.versions.toml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/js-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/js-jsonschema/bowtie_jsonschema.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/js-jsonschema/package.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/lua-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/lua-jsonschema/bowtie_jsonschema.lua
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/lua-jsonschema/stylua.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/php-opis-json-schema/Dockerfile
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/php-opis-json-schema/bowtieJsonSchema.php
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/php-opis-json-schema/composer.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/python-jschon/Dockerfile
+-rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/python-jschon/bowtie_jschon.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/python-jsonschema/bowtie_jsonschema.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/ruby-json_schemer/.rubocop.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/ruby-json_schemer/Dockerfile
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/ruby-json_schemer/Gemfile
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/ruby-json_schemer/Gemfile.lock
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/ruby-json_schemer/bowtie_json_schemer.rb
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/rust-boon/Cargo.lock
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/rust-boon/Cargo.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/rust-boon/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/rust-boon/build.rs
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/rust-boon/src/main.rs
+-rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/rust-jsonschema/build.rs
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/scala-mjs-validator/Dockerfile
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/scala-mjs-validator/Harness.scala
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/scala-mjs-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/scala-mjs-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/scala-mjs-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/scala-rc-circe-json-validator/Dockerfile
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/scala-rc-circe-json-validator/Harness.scala
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/scala-rc-circe-json-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/scala-rc-circe-json-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/scala-rc-circe-json-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/ts-vscode-json-languageservice/Dockerfile
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/ts-vscode-json-languageservice/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/implementations/ts-vscode-json-languageservice/tsconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/conftest.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/test_cli.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/test_dialect.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/test_github.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/test_hypothesis.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/test_implementation.py
+-rw-r--r--   0        0        0    65159 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/test_integration.py
+-rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/test_report.py
+-rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/test_schemas.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/models/test.json
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/LICENSE
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/README.rst
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/hatch_build.py
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/pyproject.toml
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.5/PKG-INFO
```

### Comparing `bowtie_json_schema-2024.4.4/.gitpod.yml` & `bowtie_json_schema-2024.4.5/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/.pre-commit-config.yaml` & `bowtie_json_schema-2024.4.5/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.7"
+    rev: "v0.4.1"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/python-jsonschema/check-jsonschema
     rev: 0.28.2
     hooks:
       - name: ensure bowtie's own schemas are valid
@@ -102,15 +102,15 @@
     rev: v0.20.0
     hooks:
       - name: stylua (lua implementations)
         id: stylua
         exclude: .*/json.lua
         args: ["--config-path", "implementations/lua-jsonschema/stylua.toml"]
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v18.1.3
+    rev: v18.1.4
     hooks:
       - name: clang-format (c/c++/c#/java implementations)
         id: clang-format
         types_or: [c++, c, c#, java, objective-c]
   - repo: https://github.com/dustinsand/pre-commit-jvm
     rev: v0.11.0
     hooks:
```

### Comparing `bowtie_json_schema-2024.4.4/CONTRIBUTING.rst` & `bowtie_json_schema-2024.4.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/action.yml` & `bowtie_json_schema-2024.4.5/action.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/noxfile.py` & `bowtie_json_schema-2024.4.5/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,25 @@
 REQUIREMENTS = dict(
     main=ROOT / "requirements.txt",
     docs=DOCS / "requirements.txt",
     tests=ROOT / "test-requirements.txt",
 )
 REQUIREMENTS_IN = [  # this is actually ordered, as files depend on each other
     (
-        ROOT / "pyproject.toml"
-        if path.absolute() == REQUIREMENTS["main"].absolute()
-        else path.parent / f"{path.stem}.in"
+        (
+            ROOT / "pyproject.toml"
+            if path.absolute() == REQUIREMENTS["main"].absolute()
+            else path.parent / f"{path.stem}.in"
+        ),
+        path,
     )
     for path in REQUIREMENTS.values()
 ]
 
 
-# aiohttp / aiodocker don't support 3.12
 SUPPORTED = ["pypy3.10", "3.11", "3.12"]
 LATEST = SUPPORTED[-1]
 
 nox.options.default_venv_backend = "uv|virtualenv"
 nox.options.sessions = []
 
 
@@ -364,16 +366,18 @@
     """
     if session.venv_backend == "uv":
         cmd = ["uv", "pip", "compile"]
     else:
         session.install("pip-tools")
         cmd = ["pip-compile", "--resolver", "backtracking", "--strip-extras"]
 
-    for each in REQUIREMENTS_IN:
-        session.run(*cmd, "-U", each.relative_to(ROOT))
+    for each, out in REQUIREMENTS_IN:
+        # otherwise output files end up with silly absolute path comments...
+        relative = each.relative_to(ROOT)
+        session.run(*cmd, "--upgrade", "--output-file", out, relative)
 
 
 @session(default=False, python=False)
 def ui(session):
     """
     Run a local development UI.
```

### Comparing `bowtie_json_schema-2024.4.4/requirements.txt` & `bowtie_json_schema-2024.4.5/test-requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,126 @@
-#
-# This file is autogenerated by pip-compile with Python 3.12
-# by the following command:
-#
-#    pip-compile --strip-extras pyproject.toml
-#
+# This file was autogenerated by uv via the following command:
+#    uv pip compile --output-file test-requirements.txt test-requirements.in
 aiodocker==0.21.0
-    # via bowtie-json-schema (pyproject.toml)
+    # via bowtie-json-schema
 aiohttp==3.9.5
     # via aiodocker
 aiosignal==1.3.1
     # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
-    #   bowtie-json-schema (pyproject.toml)
+    #   bowtie-json-schema
+    #   hypothesis
     #   jsonschema
     #   referencing
+bowtie-json-schema @ file:.#egg=bowtie-json-schema
 certifi==2024.2.2
     # via requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via rich-click
 cryptography==42.0.5
     # via pyjwt
 diagnostic==2.1.0
-    # via bowtie-json-schema (pyproject.toml)
-docutils==0.21.1
+    # via bowtie-json-schema
+docutils==0.21.2
     # via diagnostic
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
 github3-py==4.0.1
-    # via bowtie-json-schema (pyproject.toml)
+    # via bowtie-json-schema
+hypothesis==6.100.1
+icdiff==2.0.7
+    # via pytest-icdiff
 idna==3.7
     # via
     #   requests
     #   yarl
+iniconfig==2.0.0
+    # via pytest
 jsonschema==4.21.1
-    # via bowtie-json-schema (pyproject.toml)
+    # via bowtie-json-schema
 jsonschema-lexer==0.2.1
-    # via bowtie-json-schema (pyproject.toml)
+    # via bowtie-json-schema
 jsonschema-specifications==2023.12.1
     # via jsonschema
 markdown-it-py==3.0.0
     # via
     #   diagnostic
     #   rich
 mdurl==0.1.2
     # via markdown-it-py
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
+packaging==24.0
+    # via pytest
+pexpect==4.9.0
+pluggy==1.5.0
+    # via pytest
+pprintpp==0.4.0
+    # via pytest-icdiff
+ptyprocess==0.7.0
+    # via pexpect
 pycparser==2.22
     # via cffi
 pygments==2.17.2
     # via
     #   jsonschema-lexer
     #   rich
 pyjwt==2.8.0
     # via github3-py
+pytest==8.1.1
+    # via
+    #   pytest-asyncio
+    #   pytest-icdiff
+pytest-asyncio==0.21.1
+pytest-icdiff==0.9
 python-dateutil==2.9.0.post0
     # via github3-py
-referencing==0.34.0
+referencing==0.35.0
     # via
-    #   bowtie-json-schema (pyproject.toml)
+    #   bowtie-json-schema
     #   jsonschema
     #   jsonschema-specifications
     #   referencing-loaders
 referencing-loaders==2024.5.1
-    # via bowtie-json-schema (pyproject.toml)
+    # via bowtie-json-schema
 requests==2.31.0
     # via github3-py
 rich==13.7.1
     # via
-    #   bowtie-json-schema (pyproject.toml)
+    #   bowtie-json-schema
     #   diagnostic
     #   rich-click
-rich-click==1.8.0.dev6
-    # via bowtie-json-schema (pyproject.toml)
+rich-click==1.8.0.dev7
+    # via bowtie-json-schema
 rpds-py==0.18.0
     # via
-    #   bowtie-json-schema (pyproject.toml)
+    #   bowtie-json-schema
     #   jsonschema
     #   referencing
 six==1.16.0
     # via python-dateutil
+sortedcontainers==2.4.0
+    # via hypothesis
 structlog==24.1.0
-    # via bowtie-json-schema (pyproject.toml)
+    # via bowtie-json-schema
 typing-extensions==4.11.0
     # via
     #   aiodocker
     #   rich-click
 uritemplate==4.1.1
     # via github3-py
 url-py==0.10.0
-    # via bowtie-json-schema (pyproject.toml)
+    # via bowtie-json-schema
 urllib3==2.2.1
     # via requests
 yarl==1.9.4
     # via aiohttp
```

### Comparing `bowtie_json_schema-2024.4.4/.pre-commit-hooks/check-dependabot` & `bowtie_json_schema-2024.4.5/.pre-commit-hooks/check-dependabot`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/.pre-commit-hooks/check-lintsonschema-schema` & `bowtie_json_schema-2024.4.5/.pre-commit-hooks/check-lintsonschema-schema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/_cli.py` & `bowtie_json_schema-2024.4.5/bowtie/_cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -51,15 +51,16 @@
     from collections.abc import (
         AsyncIterator,
         Awaitable,
         Mapping,
         Sequence,
         Set,
     )
-    from typing import Any, TextIO
+    from os import PathLike
+    from typing import IO, Any, TextIO
 
     from click.decorators import FC
     from referencing.jsonschema import Schema, SchemaRegistry, SchemaResource
 
     from bowtie._commands import AnyTestResult, ImplementationId
     from bowtie._core import DialectRunner, ImplementationInfo, MakeValidator
 
@@ -70,33 +71,14 @@
 _EX_NOINPUT = getattr(os, "EX_NOINPUT", 1)
 
 STDERR = console.Console(stderr=True)
 
 
 IMAGE_REPOSITORY = "ghcr.io/bowtie-json-schema"
 
-FORMAT = click.option(
-    "--format",
-    "-f",
-    "format",
-    help="What format to use for the output",
-    default=lambda: "pretty" if sys.stdout.isatty() else "json",
-    show_default="pretty if stdout is a tty, otherwise JSON",
-    type=click.Choice(["json", "pretty", "markdown"]),
-)
-_F = Literal["json", "pretty", "markdown"]
-
-
-def option_group(name: str, *options: str, **kwargs: Any):
-    return OptionGroupDict(
-        name=name,
-        options=[f"--{option}" for option in options],
-        **kwargs,
-    )
-
 
 # rich-click's CommandGroupDict seems to be missing some covariance, as using a
 # regular dict here makes pyright complain.
 _COMMAND_GROUPS = dict(
     bowtie=[
         CommandGroupDict(
             name="Basic Commands",
@@ -109,141 +91,73 @@
         CommandGroupDict(
             name="Plumbing Commands",
             commands=["badges", "smoke"],
         ),
     ],
 )
 _OPTION_GROUPS = {
-    "bowtie validate": [
-        option_group(
-            "Required",
-            "implementation",
-        ),
-        option_group(
-            "Schema Behavior Options",
-            "dialect",
-            "set-schema",
-        ),
-        option_group(
-            "Validation Metadata Options",
-            "description",
-            "expect",
-        ),
-        option_group(
-            "Connection & Communication Options",
-            "read-timeout",
-            "validate-implementations",
-        ),
-        option_group("Help", "help"),
-    ],
-    "bowtie suite": [
-        option_group(
-            "Required",
-            "implementation",
-        ),
-        option_group(
-            "Test Run Options",
-            "fail-fast",
-            "filter",
-            "max-error",
-            "max-fail",
-        ),
-        option_group(
-            "Test Modification Options",
-            "set-schema",
-        ),
-        option_group(
-            "Connection & Communication Options",
-            "read-timeout",
-            "validate-implementations",
-        ),
-        option_group("Help", "help"),
-    ],
-    "bowtie info": [
-        option_group(
-            "Basic Options",
-            "implementation",
-            "format",
-        ),
-        option_group(
-            "Connection & Communication Options",
-            "read-timeout",
-        ),
-        option_group("Help", "help"),
-    ],
-    "bowtie smoke": [
-        option_group(
-            "Basic Options",
-            "implementation",
-            "quiet",
-            "format",
-        ),
-        option_group(
-            "Connection & Communication Options",
-            "read-timeout",
-        ),
-        option_group("Help", "help"),
-    ],
-    "bowtie filter-dialects": [
-        option_group(
-            "Required",
-            "implementation",
-        ),
-        option_group(
-            "Filters",
-            "dialect",
-            "latest",
-            "boolean-schemas",
-        ),
-        option_group(
-            "Connection & Communication Options",
-            "read-timeout",
-        ),
-        option_group("Help", "help"),
-    ],
-    "bowtie filter-implementations": [
-        option_group(
-            "Required",
-            "implementation",
-        ),
-        option_group(
-            "Filters",
-            "supports-dialect",
-            "language",
+    f"bowtie {command}": [
+        *[
+            OptionGroupDict(name=group, options=[f"--{o}" for o in options])
+            for group, options in groups
+        ],
+        OptionGroupDict(
+            name="Connection & Communication Options",
+            options=["--read-timeout", "--validate-implementations"],
         ),
-        option_group(
-            "Connection & Communication Options",
-            "read-timeout",
+        OptionGroupDict(name="Help", options=["--help"]),
+    ]
+    for command, groups in [
+        (
+            "validate",
+            [
+                ("Required", ["implementation"]),
+                ("Schema Behavior Options", ["dialect", "set-schema"]),
+                ("Validation Metadata Options", ["description", "expect"]),
+            ],
         ),
-        option_group("Help", "help"),
-    ],
-    "bowtie run": [
-        option_group(
-            "Required",
-            "implementation",
+        (
+            "suite",
+            [
+                ("Required", ["implementation"]),
+                (
+                    "Test Run Options",
+                    ["fail-fast", "filter", "max-error", "max-fail"],
+                ),
+                ("Test Modification Options", ["set-schema"]),
+            ],
         ),
-        option_group(
-            "Schema Behavior Options",
-            "dialect",
-            "set-schema",
+        ("info", [("Basic Options", ["implementation", "format"])]),
+        ("smoke", [("Basic Options", ["implementation", "quiet", "format"])]),
+        (
+            "filter-dialects",
+            [
+                ("Required", ["implementation"]),
+                ("Filters", ["dialect", "latest", "boolean-schemas"]),
+            ],
         ),
-        option_group(
-            "Test Run Options",
-            "fail-fast",
-            "filter",
-            "max-error",
-            "max-fail",
+        (
+            "filter-implementations",
+            [
+                ("Required", ["implementation"]),
+                ("Filters", ["supports-dialect", "language"]),
+            ],
         ),
-        option_group(
-            "Connection & Communication Options",
-            "read-timeout",
-            "validate-implementations",
+        (
+            "run",
+            [
+                ("Required", ["implementation"]),
+                ("Schema Behavior Options", ["dialect", "set-schema"]),
+                (
+                    "Test Run Options",
+                    ["fail-fast", "filter", "max-error", "max-fail"],
+                ),
+            ],
         ),
-        option_group("Help", "help"),
-    ],
+    ]
 }
 
 
 @click.rich_config(
     help_config=click.RichHelpConfiguration(
         command_groups=_COMMAND_GROUPS,
         option_groups=_OPTION_GROUPS,
@@ -488,16 +402,56 @@
                     return _EX_CONFIG
 
     for dir, dialects in supported_versions.items():
         badge = _report.supported_version_badge(dialects=dialects)
         dir.joinpath("supported_versions.json").write_text(json.dumps(badge))
 
 
+_F = Literal["json", "pretty", "markdown"]
+
+
+def format_option(fn: FC) -> FC:
+    def show_schema(
+        ctx: click.Context,
+        param: click.Parameter | None,
+        value: bool,
+    ) -> None:
+        if not value or ctx.resilient_parsing:
+            return
+        uri = f"tag:bowtie.report,2024:cli:{ctx.command.name}"
+        schema = bowtie_schemas_registry().contents(uri)
+        # FIXME: Syntax highlight? But rich appears to be doing some bizarre
+        #        line wrapping, even if I disable a bunch of random options
+        #        (crop, no_wrap, word_wrap in Syntax, ...) which fails the
+        #        integration tests.
+        click.echo(json.dumps(schema, indent=2))
+        ctx.exit()
+
+    return click.option(
+        "--format",
+        "-f",
+        "format",
+        help="What format to use for the output",
+        default=lambda: "pretty" if sys.stdout.isatty() else "json",
+        show_default="pretty if stdout is a tty, otherwise JSON",
+        type=click.Choice(["json", "pretty", "markdown"]),
+    )(
+        click.option(
+            "--schema",
+            callback=show_schema,
+            expose_value=False,
+            is_eager=True,
+            is_flag=True,
+            help="Show the JSON Schema for this command's JSON output.",
+        )(fn),
+    )
+
+
 @subcommand
-@FORMAT
+@format_option
 @click.option(
     "--show",
     "-s",
     default="validation",
     show_default=True,
     type=click.Choice(["failures", "validation"]),
     help=(
@@ -1089,14 +1043,27 @@
                 callback=disallow_fail_fast,
                 help=msg.format("error"),
             )(fn),
         ),
     )
 
 
+class JSON(click.File):
+
+    name = "JSON"
+
+    def convert(
+        self,
+        value: str | PathLike[str] | IO[Any],
+        param: click.Parameter | None,
+        ctx: click.Context | None,
+    ) -> Any:
+        return json.load(super().convert(value, param, ctx))
+
+
 @subcommand
 @IMPLEMENTATION
 @DIALECT
 @FILTER
 @fail_fast
 @SET_SCHEMA
 @TIMEOUT
@@ -1145,23 +1112,19 @@
     default="any",
     type=click.Choice(["valid", "invalid", "any"], case_sensitive=False),
     help=(
         "Expect the given input to be considered valid or invalid, "
         "or else (with 'any') to allow either result."
     ),
 )
-@click.argument(
-    "schema",
-    type=click.File(mode="rb"),
-    callback=lambda _, __, value: json.load(value),  # type: ignore[reportUnknownLambdaType]
-)
-@click.argument("instances", nargs=-1, type=click.File(mode="rb"))
+@click.argument("schema", type=JSON())
+@click.argument("instances", nargs=-1, type=JSON())
 def validate(
     schema: Any,
-    instances: Iterable[TextIO],
+    instances: Iterable[Any],
     expect: str,
     description: str,
     **kwargs: Any,
 ):
     """
     Validate instances under a schema across any supported implementation.
     """
@@ -1170,15 +1133,15 @@
 
     case = TestCase(
         description=description,
         schema=schema,
         tests=[
             Test(
                 description="",
-                instance=json.load(instance),
+                instance=instance,
                 valid=dict(valid=True, invalid=False, any=None)[expect],
             )
             for instance in instances
         ],
     )
     return asyncio.run(_run(fail_fast=False, **kwargs, cases=[case]))
 
@@ -1305,15 +1268,15 @@
     for dialect in sorted(matching, reverse=True):
         click.echo(dialect.uri)
         if latest:
             break
 
 
 @implementation_subcommand()  # type: ignore[reportArgumentType]
-@FORMAT
+@format_option
 async def info(
     start: Callable[[], AsyncIterator[Implementation]],
     format: _F,
 ):
     """
     Show information about a supported implementation.
     """
@@ -1365,15 +1328,15 @@
     # I have no idea why Click makes this so hard, but no combination of:
     #     type, default, is_flag, flag_value, nargs, ...
     # makes this work without doing it manually with callback.
     callback=lambda _, __, v: click.echo if not v else lambda *_, **__: None,  # type: ignore[reportUnknownLambdaType]
     is_flag=True,
     help="Don't print any output, just exit with nonzero status on failure.",
 )
-@FORMAT
+@format_option
 async def smoke(
     start: Callable[[], AsyncIterator[Implementation]],
     format: _F,
     echo: Callable[..., None],
 ) -> int:
     """
     Smoke test implementations for basic correctness against Bowtie's protocol.
```

### Comparing `bowtie_json_schema-2024.4.4/bowtie/_commands.py` & `bowtie_json_schema-2024.4.5/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/_containers.py` & `bowtie_json_schema-2024.4.5/bowtie/_containers.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/_core.py` & `bowtie_json_schema-2024.4.5/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/_report.py` & `bowtie_json_schema-2024.4.5/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/_suite.py` & `bowtie_json_schema-2024.4.5/bowtie/_suite.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/exceptions.py` & `bowtie_json_schema-2024.4.5/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/hypothesis.py` & `bowtie_json_schema-2024.4.5/bowtie/hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/schemas/io/v1.json` & `bowtie_json_schema-2024.4.5/bowtie/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.4.5/bowtie/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/run.json` & `bowtie_json_schema-2024.4.5/bowtie/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/start.json` & `bowtie_json_schema-2024.4.5/bowtie/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/schemas/models/dialect.json` & `bowtie_json_schema-2024.4.5/bowtie/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/schemas/models/group.json` & `bowtie_json_schema-2024.4.5/bowtie/schemas/models/group.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9352864583333333%*

 * *Differences: {"'$id'": "'tag:bowtie.report,2023:models:group'",*

 * * "'oneOf'": "{0: {'properties': {'children': {'items': {'$ref': "*

 * *            "'tag:bowtie.report,2023:models:test'}}}}}",*

 * * "'properties'": "{'registry': {'$ref': 'tag:bowtie.report,2023:models:registry'}}"}*

```diff
@@ -1,18 +1,18 @@
 {
-    "$id": "tag:bowtie.report,2023:ihop:group",
+    "$id": "tag:bowtie.report,2023:models:group",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "A collection of related, runnable tests, either individually or themselves in subgroups. Groups are used only for organizing test input and reporting -- they are not sent to harnesses when actually running tests, as there's no need for the harness to have to deal with any grouping structure.",
     "oneOf": [
         {
             "description": "a leaf test group (whose children are tests, and which therefore declares a schema for its children)",
             "properties": {
                 "children": {
                     "items": {
-                        "$ref": "tag:bowtie.report,2023:ihop:test"
+                        "$ref": "tag:bowtie.report,2023:models:test"
                     }
                 }
             },
             "required": [
                 "schema"
             ]
         },
@@ -43,15 +43,15 @@
             "type": "string"
         },
         "description": {
             "description": "A (human-readable) short description of this test group",
             "type": "string"
         },
         "registry": {
-            "$ref": "tag:bowtie.report,2023:ihop:registry",
+            "$ref": "tag:bowtie.report,2023:models:registry",
             "description": "A schema registry to be made available for all tests in this group."
         },
         "schema": {
             "$comment": "the URI used here is a sort of 'magic' URI set by Bowtie during runs, which will resolve to (effectively) the meta-schema for the current dialect being run by Bowtie. E.g. when running tests using the Draft 2020-12 dialect, the URI will resolve to the schema `{\"$ref\": \"https://json-schema.org/draft/2020-12/schema\"}`. This sort of dynamically set value is necessary, as schemas are supposed to be valid under the current dialect being spoken by Bowtie, but that's not known until runtime.",
             "$ref": "tag:bowtie.report,2023:ihop:__dialect__",
             "description": "A valid JSON Schema."
         }
```

### Comparing `bowtie_json_schema-2024.4.4/bowtie/schemas/models/implementation.json` & `bowtie_json_schema-2024.4.5/bowtie/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/bowtie/schemas/models/test.json` & `bowtie_json_schema-2024.4.5/bowtie/schemas/models/test.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'tag:bowtie.report,2023:models:test'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "tag:bowtie.report,2023:ihop:test",
+    "$id": "tag:bowtie.report,2023:models:test",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
     "description": "A single test case",
     "properties": {
         "comment": {
             "description": "Any additional comments about the test",
             "type": "string"
```

### Comparing `bowtie_json_schema-2024.4.4/data/dialects.json` & `bowtie_json_schema-2024.4.5/data/dialects.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/docs/Makefile` & `bowtie_json_schema-2024.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/docs/cli.rst` & `bowtie_json_schema-2024.4.5/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/docs/conf.py` & `bowtie_json_schema-2024.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/docs/contributing.rst` & `bowtie_json_schema-2024.4.5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/docs/github-actions.rst` & `bowtie_json_schema-2024.4.5/docs/github-actions.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/docs/implementers.rst` & `bowtie_json_schema-2024.4.5/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/docs/index.rst` & `bowtie_json_schema-2024.4.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/docs/motd.txt` & `bowtie_json_schema-2024.4.5/docs/motd.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/docs/requirements.txt` & `bowtie_json_schema-2024.4.5/docs/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-#
-# This file is autogenerated by pip-compile with Python 3.12
-# by the following command:
-#
-#    pip-compile --strip-extras docs/requirements.in
-#
+# This file was autogenerated by uv via the following command:
+#    uv pip compile --output-file docs/requirements.txt docs/requirements.in
 aiodocker==0.21.0
     # via bowtie-json-schema
-aiohttp==3.9.4
+aiohttp==3.9.5
     # via aiodocker
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
 attrs==23.2.0
     # via
@@ -18,44 +14,42 @@
     #   bowtie-json-schema
     #   jsonschema
     #   referencing
 babel==2.14.0
     # via sphinx
 beautifulsoup4==4.12.3
     # via furo
-file:.#egg=bowtie-json-schema
-    # via -r docs/requirements.in
+bowtie-json-schema @ file:.#egg=bowtie-json-schema
 certifi==2024.2.2
     # via requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   rich-click
     #   sphinx-click
 cryptography==42.0.5
     # via pyjwt
 diagnostic==2.1.0
     # via bowtie-json-schema
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   diagnostic
     #   sphinx
     #   sphinx-click
     #   sphinx-prompt
     #   sphinx-substitution-extensions
     #   sphinx-tabs
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
 furo==2024.1.29
-    # via -r docs/requirements.in
 github3-py==4.0.1
     # via bowtie-json-schema
 idna==3.7
     # via
     #   requests
     #   yarl
 imagesize==1.4.1
@@ -94,20 +88,19 @@
     #   jsonschema-lexer
     #   pygments-github-lexers
     #   rich
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
 pygments-github-lexers==0.0.5
-    # via -r docs/requirements.in
 pyjwt==2.8.0
     # via github3-py
 python-dateutil==2.9.0.post0
     # via github3-py
-referencing==0.34.0
+referencing==0.35.0
     # via
     #   bowtie-json-schema
     #   jsonschema
     #   jsonschema-specifications
     #   referencing-loaders
 referencing-loaders==2024.5.1
     # via bowtie-json-schema
@@ -116,79 +109,69 @@
     #   github3-py
     #   sphinx
 rich==13.7.1
     # via
     #   bowtie-json-schema
     #   diagnostic
     #   rich-click
-rich-click==1.8.0.dev6
+rich-click==1.8.0.dev7
     # via bowtie-json-schema
 rpds-py==0.18.0
     # via
     #   bowtie-json-schema
     #   jsonschema
     #   referencing
 six==1.16.0
     # via python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
-    #   -r docs/requirements.in
     #   furo
     #   sphinx-basic-ng
     #   sphinx-click
     #   sphinx-copybutton
     #   sphinx-json-schema-spec
     #   sphinx-prompt
     #   sphinx-substitution-extensions
     #   sphinx-tabs
     #   sphinxcontrib-spelling
     #   sphinxext-opengraph
 sphinx-basic-ng==1.0.0b2
     # via furo
 sphinx-click==5.1.0
-    # via -r docs/requirements.in
 sphinx-copybutton==0.5.2
-    # via -r docs/requirements.in
 sphinx-json-schema-spec==2024.1.1
-    # via -r docs/requirements.in
 sphinx-prompt==1.8.0
     # via sphinx-substitution-extensions
 sphinx-substitution-extensions==2024.2.25
-    # via -r docs/requirements.in
 sphinx-tabs==3.4.5
-    # via -r docs/requirements.in
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 sphinxcontrib-spelling==8.0.0
-    # via -r docs/requirements.in
 sphinxext-opengraph==0.9.1
-    # via -r docs/requirements.in
 structlog==24.1.0
     # via bowtie-json-schema
 typing-extensions==4.11.0
     # via
     #   aiodocker
     #   rich-click
 uritemplate==4.1.1
     # via github3-py
 url-py==0.10.0
-    # via
-    #   -r docs/requirements.in
-    #   bowtie-json-schema
+    # via bowtie-json-schema
 urllib3==2.2.1
     # via requests
 yarl==1.9.4
     # via aiohttp
```

### Comparing `bowtie_json_schema-2024.4.4/docs/_static/bowtie_diagram_dark.svg` & `bowtie_json_schema-2024.4.5/docs/_static/bowtie_diagram_dark.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/docs/_static/bowtie_diagram_light.svg` & `bowtie_json_schema-2024.4.5/docs/_static/bowtie_diagram_light.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/docs/_static/logo.svg` & `bowtie_json_schema-2024.4.5/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/package.json` & `bowtie_json_schema-2024.4.5/frontend/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9486842105263158%*

 * *Differences: {"'devDependencies'": "{'typescript': '^5.4.5'}", "'packageManager'": "'pnpm@9.0.4'"}*

```diff
@@ -23,15 +23,15 @@
         "eslint": "8.57.0",
         "eslint-plugin-react": "7.34.1",
         "eslint-plugin-react-hooks": "4.6.0",
         "jsdom": "^24.0.0",
         "react-test-renderer": "^18.2.0",
         "ts-loader": "^9.5.1",
         "ts-node": "^10.9.2",
-        "typescript": "^5.4.4",
+        "typescript": "^5.4.5",
         "vite": "^5.2.10",
         "vite-bundle-visualizer": "^1.1.0",
         "vitest": "^1.5.0"
     },
     "engines": {
         "node": ">=21.0.0"
     },
@@ -70,15 +70,15 @@
         "settings": {
             "react": {
                 "version": "18.2"
             }
         }
     },
     "name": "bowtie",
-    "packageManager": "pnpm@8.15.1",
+    "packageManager": "pnpm@9.0.4",
     "scripts": {
         "build": "tsc && vite build",
         "bundle-visualizer": "vite-bundle-visualizer",
         "lint": "eslint src --max-warnings 0",
         "preview": "vite preview",
         "start": "vite --no-clearScreen",
         "test": "vitest run",
```

### Comparing `bowtie_json_schema-2024.4.4/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2024.4.5/frontend/pnpm-lock.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -47,18 +47,18 @@
     specifier: ^18.0.7
     version: 18.0.7
   '@types/urijs':
     specifier: ^1.19.25
     version: 1.19.25
   '@typescript-eslint/eslint-plugin':
     specifier: ^7.0.0
-    version: 7.0.0(@typescript-eslint/parser@6.21.0)(eslint@8.57.0)(typescript@5.4.4)
+    version: 7.0.0(@typescript-eslint/parser@6.21.0)(eslint@8.57.0)(typescript@5.4.5)
   '@typescript-eslint/parser':
     specifier: ^6.21.0
-    version: 6.21.0(eslint@8.57.0)(typescript@5.4.4)
+    version: 6.21.0(eslint@8.57.0)(typescript@5.4.5)
   '@vitejs/plugin-react':
     specifier: ^4.2.1
     version: 4.2.1(vite@5.2.10)
   eslint:
     specifier: 8.57.0
     version: 8.57.0
   eslint-plugin-react:
@@ -71,21 +71,21 @@
     specifier: ^24.0.0
     version: 24.0.0
   react-test-renderer:
     specifier: ^18.2.0
     version: 18.2.0(react@18.2.0)
   ts-loader:
     specifier: ^9.5.1
-    version: 9.5.1(typescript@5.4.4)(webpack@5.89.0)
+    version: 9.5.1(typescript@5.4.5)(webpack@5.89.0)
   ts-node:
     specifier: ^10.9.2
-    version: 10.9.2(@types/node@20.11.5)(typescript@5.4.4)
+    version: 10.9.2(@types/node@20.11.5)(typescript@5.4.5)
   typescript:
-    specifier: ^5.4.4
-    version: 5.4.4
+    specifier: ^5.4.5
+    version: 5.4.5
   vite:
     specifier: ^5.2.10
     version: 5.2.10(@types/node@20.11.5)
   vite-bundle-visualizer:
     specifier: ^1.1.0
     version: 1.1.0
   vitest:
@@ -974,60 +974,60 @@
     resolution: {integrity: sha512-XOfUup9r3Y06nFAZh3WvO0rBU4OtlfPB/vgxpjg+NRdGU6CN6djdc6OEiH+PcqHCY6eFLo9Ista73uarf4gnBg==}
     dev: true
 
   /@types/warning@3.0.3:
     resolution: {integrity: sha512-D1XC7WK8K+zZEveUPY+cf4+kgauk8N4eHr/XIHXGlGYkHLud6hK9lYfZk1ry1TNh798cZUCgb6MqGEG8DkJt6Q==}
     dev: false
 
-  /@typescript-eslint/eslint-plugin@7.0.0(@typescript-eslint/parser@6.21.0)(eslint@8.57.0)(typescript@5.4.4):
+  /@typescript-eslint/eslint-plugin@7.0.0(@typescript-eslint/parser@6.21.0)(eslint@8.57.0)(typescript@5.4.5):
     resolution: {integrity: sha512-M72SJ0DkcQVmmsbqlzc6EJgb/3Oz2Wdm6AyESB4YkGgCxP8u5jt5jn4/OBMPK3HLOxcttZq5xbBBU7e2By4SZQ==}
     engines: {node: ^16.0.0 || >=18.0.0}
     peerDependencies:
       '@typescript-eslint/parser': ^6.0.0 || ^6.0.0-alpha
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
       '@eslint-community/regexpp': 4.10.0
-      '@typescript-eslint/parser': 6.21.0(eslint@8.57.0)(typescript@5.4.4)
+      '@typescript-eslint/parser': 6.21.0(eslint@8.57.0)(typescript@5.4.5)
       '@typescript-eslint/scope-manager': 7.0.0
-      '@typescript-eslint/type-utils': 7.0.0(eslint@8.57.0)(typescript@5.4.4)
-      '@typescript-eslint/utils': 7.0.0(eslint@8.57.0)(typescript@5.4.4)
+      '@typescript-eslint/type-utils': 7.0.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.0.0(eslint@8.57.0)(typescript@5.4.5)
       '@typescript-eslint/visitor-keys': 7.0.0
       debug: 4.3.4
       eslint: 8.57.0
       graphemer: 1.4.0
       ignore: 5.3.0
       natural-compare: 1.4.0
       semver: 7.5.4
-      ts-api-utils: 1.0.3(typescript@5.4.4)
-      typescript: 5.4.4
+      ts-api-utils: 1.0.3(typescript@5.4.5)
+      typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/parser@6.21.0(eslint@8.57.0)(typescript@5.4.4):
+  /@typescript-eslint/parser@6.21.0(eslint@8.57.0)(typescript@5.4.5):
     resolution: {integrity: sha512-tbsV1jPne5CkFQCgPBcDOt30ItF7aJoZL997JSF7MhGQqOeT3svWRYxiqlfA5RUdlHN6Fi+EI9bxqbdyAUZjYQ==}
     engines: {node: ^16.0.0 || >=18.0.0}
     peerDependencies:
       eslint: ^7.0.0 || ^8.0.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
       '@typescript-eslint/scope-manager': 6.21.0
       '@typescript-eslint/types': 6.21.0
-      '@typescript-eslint/typescript-estree': 6.21.0(typescript@5.4.4)
+      '@typescript-eslint/typescript-estree': 6.21.0(typescript@5.4.5)
       '@typescript-eslint/visitor-keys': 6.21.0
       debug: 4.3.4
       eslint: 8.57.0
-      typescript: 5.4.4
+      typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
   /@typescript-eslint/scope-manager@6.21.0:
     resolution: {integrity: sha512-OwLUIWZJry80O99zvqXVEioyniJMa+d2GrqpUTqi5/v5D5rOrppJVBPa0yKCblcigC0/aYAzxxqQ1B+DS2RYsg==}
     engines: {node: ^16.0.0 || >=18.0.0}
@@ -1040,45 +1040,45 @@
     resolution: {integrity: sha512-IxTStwhNDPO07CCrYuAqjuJ3Xf5MrMaNgbAZPxFXAUpAtwqFxiuItxUaVtP/SJQeCdJjwDGh9/lMOluAndkKeg==}
     engines: {node: ^16.0.0 || >=18.0.0}
     dependencies:
       '@typescript-eslint/types': 7.0.0
       '@typescript-eslint/visitor-keys': 7.0.0
     dev: true
 
-  /@typescript-eslint/type-utils@7.0.0(eslint@8.57.0)(typescript@5.4.4):
+  /@typescript-eslint/type-utils@7.0.0(eslint@8.57.0)(typescript@5.4.5):
     resolution: {integrity: sha512-FIM8HPxj1P2G7qfrpiXvbHeHypgo2mFpFGoh5I73ZlqmJOsloSa1x0ZyXCer43++P1doxCgNqIOLqmZR6SOT8g==}
     engines: {node: ^16.0.0 || >=18.0.0}
     peerDependencies:
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
-      '@typescript-eslint/typescript-estree': 7.0.0(typescript@5.4.4)
-      '@typescript-eslint/utils': 7.0.0(eslint@8.57.0)(typescript@5.4.4)
+      '@typescript-eslint/typescript-estree': 7.0.0(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.0.0(eslint@8.57.0)(typescript@5.4.5)
       debug: 4.3.4
       eslint: 8.57.0
-      ts-api-utils: 1.0.3(typescript@5.4.4)
-      typescript: 5.4.4
+      ts-api-utils: 1.0.3(typescript@5.4.5)
+      typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
   /@typescript-eslint/types@6.21.0:
     resolution: {integrity: sha512-1kFmZ1rOm5epu9NZEZm1kckCDGj5UJEf7P1kliH4LKu/RkwpsfqqGmY2OOcUs18lSlQBKLDYBOGxRVtrMN5lpg==}
     engines: {node: ^16.0.0 || >=18.0.0}
     dev: true
 
   /@typescript-eslint/types@7.0.0:
     resolution: {integrity: sha512-9ZIJDqagK1TTs4W9IyeB2sH/s1fFhN9958ycW8NRTg1vXGzzH5PQNzq6KbsbVGMT+oyyfa17DfchHDidcmf5cg==}
     engines: {node: ^16.0.0 || >=18.0.0}
     dev: true
 
-  /@typescript-eslint/typescript-estree@6.21.0(typescript@5.4.4):
+  /@typescript-eslint/typescript-estree@6.21.0(typescript@5.4.5):
     resolution: {integrity: sha512-6npJTkZcO+y2/kr+z0hc4HwNfrrP4kNYh57ek7yCNlrBjWQ1Y0OS7jiZTkgumrvkX5HkEKXFZkkdFNkaW2wmUQ==}
     engines: {node: ^16.0.0 || >=18.0.0}
     peerDependencies:
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
@@ -1086,21 +1086,21 @@
       '@typescript-eslint/types': 6.21.0
       '@typescript-eslint/visitor-keys': 6.21.0
       debug: 4.3.4
       globby: 11.1.0
       is-glob: 4.0.3
       minimatch: 9.0.3
       semver: 7.5.4
-      ts-api-utils: 1.0.3(typescript@5.4.4)
-      typescript: 5.4.4
+      ts-api-utils: 1.0.3(typescript@5.4.5)
+      typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/typescript-estree@7.0.0(typescript@5.4.4):
+  /@typescript-eslint/typescript-estree@7.0.0(typescript@5.4.5):
     resolution: {integrity: sha512-JzsOzhJJm74aQ3c9um/aDryHgSHfaX8SHFIu9x4Gpik/+qxLvxUylhTsO9abcNu39JIdhY2LgYrFxTii3IajLA==}
     engines: {node: ^16.0.0 || >=18.0.0}
     peerDependencies:
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
@@ -1108,32 +1108,32 @@
       '@typescript-eslint/types': 7.0.0
       '@typescript-eslint/visitor-keys': 7.0.0
       debug: 4.3.4
       globby: 11.1.0
       is-glob: 4.0.3
       minimatch: 9.0.3
       semver: 7.5.4
-      ts-api-utils: 1.0.3(typescript@5.4.4)
-      typescript: 5.4.4
+      ts-api-utils: 1.0.3(typescript@5.4.5)
+      typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/utils@7.0.0(eslint@8.57.0)(typescript@5.4.4):
+  /@typescript-eslint/utils@7.0.0(eslint@8.57.0)(typescript@5.4.5):
     resolution: {integrity: sha512-kuPZcPAdGcDBAyqDn/JVeJVhySvpkxzfXjJq1X1BFSTYo1TTuo4iyb937u457q4K0In84p6u2VHQGaFnv7VYqg==}
     engines: {node: ^16.0.0 || >=18.0.0}
     peerDependencies:
       eslint: ^8.56.0
     dependencies:
       '@eslint-community/eslint-utils': 4.4.0(eslint@8.57.0)
       '@types/json-schema': 7.0.15
       '@types/semver': 7.5.6
       '@typescript-eslint/scope-manager': 7.0.0
       '@typescript-eslint/types': 7.0.0
-      '@typescript-eslint/typescript-estree': 7.0.0(typescript@5.4.4)
+      '@typescript-eslint/typescript-estree': 7.0.0(typescript@5.4.5)
       eslint: 8.57.0
       semver: 7.5.4
     transitivePeerDependencies:
       - supports-color
       - typescript
     dev: true
 
@@ -4217,40 +4217,40 @@
   /tr46@5.0.0:
     resolution: {integrity: sha512-tk2G5R2KRwBd+ZN0zaEXpmzdKyOYksXwywulIX95MBODjSzMIuQnQ3m8JxgbhnL1LeVo7lqQKsYa1O3Htl7K5g==}
     engines: {node: '>=18'}
     dependencies:
       punycode: 2.3.1
     dev: true
 
-  /ts-api-utils@1.0.3(typescript@5.4.4):
+  /ts-api-utils@1.0.3(typescript@5.4.5):
     resolution: {integrity: sha512-wNMeqtMz5NtwpT/UZGY5alT+VoKdSsOOP/kqHFcUW1P/VRhH2wJ48+DN2WwUliNbQ976ETwDL0Ifd2VVvgonvg==}
     engines: {node: '>=16.13.0'}
     peerDependencies:
       typescript: '>=4.2.0'
     dependencies:
-      typescript: 5.4.4
+      typescript: 5.4.5
     dev: true
 
-  /ts-loader@9.5.1(typescript@5.4.4)(webpack@5.89.0):
+  /ts-loader@9.5.1(typescript@5.4.5)(webpack@5.89.0):
     resolution: {integrity: sha512-rNH3sK9kGZcH9dYzC7CewQm4NtxJTjSEVRJ2DyBZR7f8/wcta+iV44UPCXc5+nzDzivKtlzV6c9P4e+oFhDLYg==}
     engines: {node: '>=12.0.0'}
     peerDependencies:
       typescript: '*'
       webpack: ^5.0.0
     dependencies:
       chalk: 4.1.2
       enhanced-resolve: 5.15.0
       micromatch: 4.0.5
       semver: 7.5.4
       source-map: 0.7.4
-      typescript: 5.4.4
+      typescript: 5.4.5
       webpack: 5.89.0
     dev: true
 
-  /ts-node@10.9.2(@types/node@20.11.5)(typescript@5.4.4):
+  /ts-node@10.9.2(@types/node@20.11.5)(typescript@5.4.5):
     resolution: {integrity: sha512-f0FFpIdcHgn8zcPSbf1dRevwt047YMnaiJM3u2w2RewrB+fob/zePZcrOyQoLMMO7aBIddLcQIEK5dYjkLnGrQ==}
     hasBin: true
     peerDependencies:
       '@swc/core': '>=1.2.50'
       '@swc/wasm': '>=1.2.50'
       '@types/node': '*'
       typescript: '>=2.7'
@@ -4268,15 +4268,15 @@
       '@types/node': 20.11.5
       acorn: 8.11.3
       acorn-walk: 8.3.2
       arg: 4.1.3
       create-require: 1.1.1
       diff: 4.0.2
       make-error: 1.3.6
-      typescript: 5.4.4
+      typescript: 5.4.5
       v8-compile-cache-lib: 3.0.1
       yn: 3.1.1
     dev: true
 
   /tslib@2.6.2:
     resolution: {integrity: sha512-AEYxH93jGFPn/a2iVAwW87VuUIkR1FVUKB77NwMF7nBTDkDrrT/Hpt/IrCJ0QXhW27jTBDcf5ZY7w6RiqTMw2Q==}
     dev: false
@@ -4376,16 +4376,16 @@
       for-each: 0.3.3
       gopd: 1.0.1
       has-proto: 1.0.3
       is-typed-array: 1.1.13
       possible-typed-array-names: 1.0.0
     dev: true
 
-  /typescript@5.4.4:
-    resolution: {integrity: sha512-dGE2Vv8cpVvw28v8HCPqyb08EzbBURxDpuhJvTrusShUfGnhHBafDsLdS1EhhxyL6BJQE+2cT3dDPAv+MQ6oLw==}
+  /typescript@5.4.5:
+    resolution: {integrity: sha512-vcI4UpRgg81oIRUFwR0WSIHKt11nJ7SAVlYNIu+QpqeyXP+gpQJy/Z4+F0aGxSE4MqwjyXvW/TzgkLAx2AGHwQ==}
     engines: {node: '>=14.17'}
     hasBin: true
     dev: true
 
   /ufo@1.4.0:
     resolution: {integrity: sha512-Hhy+BhRBleFjpJ2vchUNN40qgkh0366FWJGqVLYBHev0vpHTrXSA0ryT+74UiW6KWsldNurQMKGqCm1M2zBciQ==}
     dev: true
```

### Comparing `bowtie_json_schema-2024.4.4/frontend/tsconfig.json` & `bowtie_json_schema-2024.4.5/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/public/favicon.svg` & `bowtie_json_schema-2024.4.5/frontend/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/DialectReportView.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/DialectReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/ReportDataHandler.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/ReportDataHandler.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/index.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/assets/landscape-logo.svg` & `bowtie_json_schema-2024.4.5/frontend/src/assets/landscape-logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/CopyToClipboard.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/CopyToClipboard.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/FilterSection.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/FilterSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/NavBar.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/NavBar.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/OtherImplementations.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/OtherImplementations.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CaseItem.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/Cases/CaseItem.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CaseResultSvg.test.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/Cases/CaseResultSvg.test.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CaseResultSvg.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/Cases/CaseResultSvg.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CasesSection.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/Cases/CasesSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/Cases/SchemaDisplay.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/Cases/SchemaDisplay.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/DragAndDrop/DragAndDrop.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/DragAndDrop/DragAndDrop.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/ImplementationReportView/DialectCompliance.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/ImplementationReportView/DialectCompliance.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/ImplementationReportView/EmbedBadges.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/ImplementationReportView/EmbedBadges.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/Modals/DetailsButtonModal.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/Modals/DetailsButtonModal.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/RunInfo/RunInfoSection.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/RunInfo/RunInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2024.4.5/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/Summary/ImplementationRow.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/Summary/ImplementationRow.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/Summary/SummarySection.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/Summary/SummarySection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/components/Summary/SummaryTable.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/components/Summary/SummaryTable.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/context/BowtieVersionContext.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/context/BowtieVersionContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/context/ThemeContext.tsx` & `bowtie_json_schema-2024.4.5/frontend/src/context/ThemeContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/data/Badge.test.ts` & `bowtie_json_schema-2024.4.5/frontend/src/data/Badge.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/data/Badge.ts` & `bowtie_json_schema-2024.4.5/frontend/src/data/Badge.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/data/Dialect.ts` & `bowtie_json_schema-2024.4.5/frontend/src/data/Dialect.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/data/Site.test.ts` & `bowtie_json_schema-2024.4.5/frontend/src/data/Site.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/data/parseReportData.test.ts` & `bowtie_json_schema-2024.4.5/frontend/src/data/parseReportData.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2024.4.5/frontend/src/data/parseReportData.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/.java-implementations-pmd-ruleset.xml` & `bowtie_json_schema-2024.4.5/implementations/.java-implementations-pmd-ruleset.xml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/clojure-json-schema/Dockerfile` & `bowtie_json_schema-2024.4.5/implementations/clojure-json-schema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj` & `bowtie_json_schema-2024.4.5/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/cpp-valijson/bowtie_valijson.cpp` & `bowtie_json_schema-2024.4.5/implementations/cpp-valijson/bowtie_valijson.cpp`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/.gitignore` & `bowtie_json_schema-2024.4.5/implementations/dotnet-jsonschema-net/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/Program.cs` & `bowtie_json_schema-2024.4.5/implementations/dotnet-jsonschema-net/Program.cs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/go-gojsonschema/bowtie_gojsonschema.go` & `bowtie_json_schema-2024.4.5/implementations/go-gojsonschema/bowtie_gojsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/go-gojsonschema/go.sum` & `bowtie_json_schema-2024.4.5/implementations/go-gojsonschema/go.sum`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/go-jsonschema/bowtie_jsonschema.go` & `bowtie_json_schema-2024.4.5/implementations/go-jsonschema/bowtie_jsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-json-schema/BowtieJsonSchema.java` & `bowtie_json_schema-2024.4.5/implementations/java-json-schema/BowtieJsonSchema.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-json-schema/build.gradle` & `bowtie_json_schema-2024.4.5/implementations/java-json-schema/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.4.5/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.4.5/implementations/java-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java` & `bowtie_json_schema-2024.4.5/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-jsonschemafriend/build.gradle` & `bowtie_json_schema-2024.4.5/implementations/java-jsonschemafriend/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/build.gradle.kts` & `bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/justfile` & `bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/justfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/gradle/libs.versions.toml` & `bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/gradle/libs.versions.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt` & `bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/Support.kt` & `bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/Support.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt` & `bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt` & `bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt` & `bowtie_json_schema-2024.4.5/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/js-ajv/bowtie_ajv.js` & `bowtie_json_schema-2024.4.5/implementations/js-ajv/bowtie_ajv.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/js-ajv/package-lock.json` & `bowtie_json_schema-2024.4.5/implementations/js-ajv/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/js-hyperjump/bowtie_hyperjump.js` & `bowtie_json_schema-2024.4.5/implementations/js-hyperjump/bowtie_hyperjump.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/js-jsonschema/bowtie_jsonschema.js` & `bowtie_json_schema-2024.4.5/implementations/js-jsonschema/bowtie_jsonschema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts` & `bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt` & `bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt` & `bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt` & `bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt` & `bowtie_json_schema-2024.4.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/Dockerfile` & `bowtie_json_schema-2024.4.5/implementations/lua-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/bowtie_jsonschema.lua` & `bowtie_json_schema-2024.4.5/implementations/lua-jsonschema/bowtie_jsonschema.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/json.lua` & `bowtie_json_schema-2024.4.5/implementations/lua-jsonschema/json.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/php-opis-json-schema/bowtieJsonSchema.php` & `bowtie_json_schema-2024.4.5/implementations/php-opis-json-schema/bowtieJsonSchema.php`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/python-fastjsonschema/bowtie_fastjsonschema.py` & `bowtie_json_schema-2024.4.5/implementations/python-fastjsonschema/bowtie_fastjsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/python-jschon/bowtie_jschon.py` & `bowtie_json_schema-2024.4.5/implementations/python-jschon/bowtie_jschon.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/python-jsonschema/bowtie_jsonschema.py` & `bowtie_json_schema-2024.4.5/implementations/python-jsonschema/bowtie_jsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/ruby-json_schemer/bowtie_json_schemer.rb` & `bowtie_json_schema-2024.4.5/implementations/ruby-json_schemer/bowtie_json_schemer.rb`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/rust-boon/Cargo.lock` & `bowtie_json_schema-2024.4.5/implementations/rust-boon/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/rust-boon/Dockerfile` & `bowtie_json_schema-2024.4.5/implementations/rust-boon/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/rust-boon/src/main.rs` & `bowtie_json_schema-2024.4.5/implementations/rust-boon/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/Cargo.lock` & `bowtie_json_schema-2024.4.5/implementations/rust-jsonschema/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/Dockerfile` & `bowtie_json_schema-2024.4.5/implementations/rust-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/src/main.rs` & `bowtie_json_schema-2024.4.5/implementations/rust-jsonschema/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/Harness.scala` & `bowtie_json_schema-2024.4.5/implementations/scala-mjs-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/build.sbt` & `bowtie_json_schema-2024.4.5/implementations/scala-mjs-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/Harness.scala` & `bowtie_json_schema-2024.4.5/implementations/scala-rc-circe-json-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/build.sbt` & `bowtie_json_schema-2024.4.5/implementations/scala-rc-circe-json-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts` & `bowtie_json_schema-2024.4.5/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/tests/test_github.py` & `bowtie_json_schema-2024.4.5/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/tests/test_hypothesis.py` & `bowtie_json_schema-2024.4.5/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/tests/test_integration.py` & `bowtie_json_schema-2024.4.5/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 import asyncio
 import json as _json
 import os
 import sys
 import tarfile
 
 from aiodocker.exceptions import DockerError
+from jsonschema import validate
 from markdown_it import MarkdownIt
 from markdown_it.tree import SyntaxTreeNode
 import pexpect
 import pytest
 import pytest_asyncio
 
+from bowtie._cli import bowtie_schemas_registry
 from bowtie._commands import ErroredTest, TestResult
 from bowtie._core import Dialect, Implementation, Test, TestCase
 from bowtie._report import EmptyReport, InvalidReport, Report
 
 Test.__test__ = TestCase.__test__ = TestResult.__test__ = (
     False  # frigging py.test
 )
@@ -27,14 +29,16 @@
 
 HERE = Path(__file__).parent
 FAUXMPLEMENTATIONS = HERE / "fauxmplementations"
 
 # Make believe we're wide for tests to avoid line breaks in rich-click.
 WIDE_TERMINAL_ENV = dict(os.environ, TERMINAL_WIDTH="512")
 
+REGISTRY = bowtie_schemas_registry()
+
 
 def tag(name: str):
     return f"bowtie-integration-tests/{name}"
 
 
 async def bowtie(*argv, stdin: str = "", exit_code=0, json=False):
     """
@@ -1018,24 +1022,29 @@
         <inline>
           <text>
         """.strip()
     ), stderr
 
 
 @pytest.mark.asyncio
+@pytest.mark.json
 async def test_smoke_json(envsonschema):
     jsonout, stderr = await bowtie(
         "smoke",
         "--format",
         "json",
         "-i",
         envsonschema,
         json=True,
         exit_code=-1,  # because indeed envsonschema gets answers wrong.
     )
+
+    schema, _ = await bowtie("smoke", "--schema")
+    validate(instance=jsonout, schema=_json.loads(schema), registry=REGISTRY)
+
     assert jsonout == [
         {
             "case": {
                 "description": "allow-everything",
                 "schema": {
                     "$schema": "https://json-schema.org/draft/2020-12/schema",
                 },
@@ -1265,23 +1274,29 @@
         """
         ).strip()
     )
     assert stderr == ""
 
 
 @pytest.mark.asyncio
+@pytest.mark.json
 async def test_info_json(envsonschema):
     stdout, stderr = await bowtie(
         "info",
         "--format",
         "json",
         "-i",
         envsonschema,
     )
-    assert _json.loads(stdout) == {
+    jsonout = _json.loads(stdout)
+
+    schema, _ = await bowtie("info", "--schema")
+    validate(instance=jsonout, schema=_json.loads(schema), registry=REGISTRY)
+
+    assert jsonout == {
         "name": "envsonschema",
         "language": "python",
         "homepage": "https://github.com/bowtie-json-schema/bowtie",
         "issues": "https://github.com/bowtie-json-schema/bowtie/issues",
         "source": "https://github.com/bowtie-json-schema/bowtie",
         "dialects": [
             "https://json-schema.org/draft/2020-12/schema",
@@ -1292,25 +1307,31 @@
             "http://json-schema.org/draft-03/schema#",
         ],
     }, stderr
     assert stderr == ""
 
 
 @pytest.mark.asyncio
+@pytest.mark.json
 async def test_info_json_multiple_implementations(envsonschema, links):
     stdout, stderr = await bowtie(
         "info",
         "--format",
         "json",
         "-i",
         envsonschema,
         "-i",
         links,
     )
-    assert _json.loads(stdout) == {
+    jsonout = _json.loads(stdout)
+
+    schema, _ = await bowtie("info", "--schema")
+    validate(instance=jsonout, schema=_json.loads(schema), registry=REGISTRY)
+
+    assert jsonout == {
         tag("envsonschema"): {
             "name": "envsonschema",
             "language": "python",
             "homepage": "https://github.com/bowtie-json-schema/bowtie",
             "issues": "https://github.com/bowtie-json-schema/bowtie/issues",
             "source": "https://github.com/bowtie-json-schema/bowtie",
             "dialects": [
@@ -1565,15 +1586,16 @@
         tmp_path / "b.json",
         exit_code=0,
     )
     assert stdout != ""  # the real assertion here is we succeed above
 
 
 @pytest.mark.asyncio
-async def test_summary_show_failures(envsonschema, tmp_path):
+@pytest.mark.json
+async def test_summary_show_failures_json(envsonschema, tmp_path):
     tmp_path.joinpath("schema.json").write_text("{}")
     tmp_path.joinpath("one.json").write_text("12")
     tmp_path.joinpath("two.json").write_text("37")
 
     validate_stdout, _ = await bowtie(
         "validate",
         "-i",
@@ -1590,21 +1612,25 @@
         "--format",
         "json",
         "--show",
         "failures",
         stdin=validate_stdout,
         json=True,
     )
-    assert stderr == ""
+
+    schema, _ = await bowtie("summary", "--schema")
+    validate(instance=jsonout, schema=_json.loads(schema), registry=REGISTRY)
+
     assert jsonout == [
         [
             tag("envsonschema"),
             dict(failed=2, skipped=0, errored=0),
         ],
     ]
+    assert stderr == ""
 
 
 @pytest.mark.asyncio
 async def test_summary_show_failures_markdown(envsonschema, tmp_path):
     tmp_path.joinpath("schema.json").write_text("{}")
     tmp_path.joinpath("one.json").write_text("12")
     tmp_path.joinpath("two.json").write_text("37")
@@ -1734,15 +1760,16 @@
         exit_code=-1,
     )
     assert stdout == ""
     assert stderr == ""
 
 
 @pytest.mark.asyncio
-async def test_summary_show_validation(envsonschema, always_valid):
+@pytest.mark.json
+async def test_summary_show_validation_json(envsonschema, always_valid):
     raw = """
         {"description":"one","schema":{"type": "integer"},"tests":[{"description":"valid:1","instance":12},{"description":"valid:0","instance":12.5}]}
         {"description":"two","schema":{"type": "string"},"tests":[{"description":"crash:1","instance":"{}"}]}
         {"description":"crash:1","schema":{"type": "number"},"tests":[{"description":"three","instance":"{}"}, {"description": "another", "instance": 37}]}
         {"description":"four","schema":{"type": "array"},"tests":[{"description":"skip:message=foo","instance":""}]}
         {"description":"skip:message=bar","schema":{"type": "boolean"},"tests":[{"description":"five","instance":""}]}
         {"description":"six","schema":{"type": "array"},"tests":[{"description":"error:message=boom","instance":""}, {"description":"valid:0", "instance":12}]}
@@ -1763,15 +1790,18 @@
         "--format",
         "json",
         "--show",
         "validation",
         stdin=run_stdout,
         json=True,
     )
-    assert stderr == ""
+
+    schema, _ = await bowtie("summary", "--schema")
+    validate(instance=jsonout, schema=_json.loads(schema), registry=REGISTRY)
+
     assert jsonout == [
         [
             {"type": "integer"},
             [
                 [
                     12,
                     {
@@ -1871,14 +1901,15 @@
                         tag("always_valid"): "valid",
                         tag("envsonschema"): "error",
                     },
                 ],
             ],
         ],
     ], run_stderr
+    assert stderr == ""
 
 
 @pytest.mark.asyncio
 async def test_badges(envsonschema, tmp_path):
     site = tmp_path / "site"
     site.mkdir()
 
@@ -1931,14 +1962,15 @@
     )
     assert stdout == ""
     assert stderr != ""
     assert not badges.is_dir()
 
 
 @pytest.mark.asyncio
+@pytest.mark.json
 async def test_run_with_registry(always_valid):
     raw = """
         {"description":"one","schema":{"type": "integer"}, "registry":{"urn:example:foo": "http://example.com"},"tests":[{"description":"valid:1","instance":12},{"description":"valid:0","instance":12.5}]}
     """  # noqa: E501
 
     run_stdout, run_stderr = await bowtie(
         "run",
@@ -1953,24 +1985,28 @@
         "--format",
         "json",
         "--show",
         "validation",
         stdin=run_stdout,
         json=True,
     )
-    assert stderr == ""
+
+    schema, _ = await bowtie("summary", "--schema")
+    validate(instance=jsonout, schema=_json.loads(schema), registry=REGISTRY)
+
     assert jsonout == [
         [
             {"type": "integer"},
             [
                 [12, {tag("always_valid"): "valid"}],
                 [12.5, {tag("always_valid"): "valid"}],
             ],
         ],
     ], run_stderr
+    assert stderr == ""
 
 
 @pytest.mark.asyncio
 async def test_no_such_image(tmp_path):
     stdout, stderr = await bowtie(
         "run",
         "-i",
```

### Comparing `bowtie_json_schema-2024.4.4/tests/test_report.py` & `bowtie_json_schema-2024.4.5/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/tests/test_schemas.py` & `bowtie_json_schema-2024.4.5/tests/test_schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                 "schema": {},
                 "children": [],
             },
         ),
     ],
 )
 def test_group(valid, instance):
-    got = errors("tag:bowtie.report,2023:ihop:group", instance)
+    got = errors("tag:bowtie.report,2023:models:group", instance)
     assert valid == (not got), got
 
 
 def test_root_schema():
     canonical_url = "tag:bowtie.report,2023:ihop"
     retrieved = REGISTRY.get_or_retrieve(canonical_url)
     assert retrieved.value.contents["$id"] == canonical_url
```

### Comparing `bowtie_json_schema-2024.4.4/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2024.4.5/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/v1.json` & `bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json` & `bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json` & `bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json` & `bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/group.json` & `bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/models/group.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9352864583333333%*

 * *Differences: {"'$id'": "'tag:bowtie.report,2023:models:group'",*

 * * "'oneOf'": "{0: {'properties': {'children': {'items': {'$ref': "*

 * *            "'tag:bowtie.report,2023:models:test'}}}}}",*

 * * "'properties'": "{'registry': {'$ref': 'tag:bowtie.report,2023:models:registry'}}"}*

```diff
@@ -1,18 +1,18 @@
 {
-    "$id": "tag:bowtie.report,2023:ihop:group",
+    "$id": "tag:bowtie.report,2023:models:group",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "A collection of related, runnable tests, either individually or themselves in subgroups. Groups are used only for organizing test input and reporting -- they are not sent to harnesses when actually running tests, as there's no need for the harness to have to deal with any grouping structure.",
     "oneOf": [
         {
             "description": "a leaf test group (whose children are tests, and which therefore declares a schema for its children)",
             "properties": {
                 "children": {
                     "items": {
-                        "$ref": "tag:bowtie.report,2023:ihop:test"
+                        "$ref": "tag:bowtie.report,2023:models:test"
                     }
                 }
             },
             "required": [
                 "schema"
             ]
         },
@@ -43,15 +43,15 @@
             "type": "string"
         },
         "description": {
             "description": "A (human-readable) short description of this test group",
             "type": "string"
         },
         "registry": {
-            "$ref": "tag:bowtie.report,2023:ihop:registry",
+            "$ref": "tag:bowtie.report,2023:models:registry",
             "description": "A schema registry to be made available for all tests in this group."
         },
         "schema": {
             "$comment": "the URI used here is a sort of 'magic' URI set by Bowtie during runs, which will resolve to (effectively) the meta-schema for the current dialect being run by Bowtie. E.g. when running tests using the Draft 2020-12 dialect, the URI will resolve to the schema `{\"$ref\": \"https://json-schema.org/draft/2020-12/schema\"}`. This sort of dynamically set value is necessary, as schemas are supposed to be valid under the current dialect being spoken by Bowtie, but that's not known until runtime.",
             "$ref": "tag:bowtie.report,2023:ihop:__dialect__",
             "description": "A valid JSON Schema."
         }
```

### Comparing `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json` & `bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/test.json` & `bowtie_json_schema-2024.4.5/tests/fauxmplementations/lintsonschema/schemas/models/test.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'tag:bowtie.report,2023:models:test'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "tag:bowtie.report,2023:ihop:test",
+    "$id": "tag:bowtie.report,2023:models:test",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
     "description": "A single test case",
     "properties": {
         "comment": {
             "description": "Any additional comments about the test",
             "type": "string"
```

### Comparing `bowtie_json_schema-2024.4.4/.gitignore` & `bowtie_json_schema-2024.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/LICENSE` & `bowtie_json_schema-2024.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/README.rst` & `bowtie_json_schema-2024.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/hatch_build.py` & `bowtie_json_schema-2024.4.5/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.4/pyproject.toml` & `bowtie_json_schema-2024.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,21 @@
 
 [tool.doc8]
 ignore = [
     "D000",  # see PyCQA/doc8#125
     "D001",  # one sentence per line, so max length doesn't make sense
 ]
 
+[tool.pytest.ini_options]
+addopts = ["--strict-markers"]
+xfail_strict = true
+markers = [
+    "json: Tests of Bowtie's JSON output",
+]
+
 [tool.pyright]
 reportUnnecessaryTypeIgnoreComment = true
 strict = ["**/*.py"]
 exclude = [
     "**/tests/__init__.py",
     "**/tests/test_*.py",
 ]
```

### Comparing `bowtie_json_schema-2024.4.4/PKG-INFO` & `bowtie_json_schema-2024.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bowtie-json-schema
-Version: 2024.4.4
+Version: 2024.4.5
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://docs.bowtie.report/
 Project-URL: Homepage, https://bowtie.report/
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author-email: Julian Berman <Julian+bowtie@GrayVines.com>
```


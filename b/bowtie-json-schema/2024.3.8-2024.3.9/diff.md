# Comparing `tmp/bowtie_json_schema-2024.3.8.tar.gz` & `tmp/bowtie_json_schema-2024.3.9.tar.gz`

## Comparing `bowtie_json_schema-2024.3.8.tar` & `bowtie_json_schema-2024.3.9.tar`

### file list

```diff
@@ -1,236 +1,236 @@
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/.gitpod.Dockerfile
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/.gitpod.yml
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/.prettierrc.json
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/.readthedocs.yaml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/action.yml
--rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/noxfile.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/requirements.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/test-requirements.in
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/test-requirements.txt
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/.devcontainer/.codespace.Dockerfile
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/.devcontainer/devcontainer.json
--rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/.pre-commit-hooks/check-dependabot
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/.pre-commit-hooks/check-lintsonschema-schema
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/__main__.py
--rw-r--r--   0        0        0    42528 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/_cli.py
--rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/_commands.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/_containers.py
--rw-r--r--   0        0        0    21220 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/_core.py
--rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/_report.py
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/_suite.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/exceptions.py
--rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/hypothesis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/py.typed
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/schemas/models/dialect.json
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/schemas/models/group.json
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/schemas/models/implementation.json
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/schemas/models/registry.json
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/bowtie/schemas/models/test.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/data/dialects.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/docs/Makefile
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/docs/cli.rst
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/docs/conf.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/docs/contributing.rst
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/docs/github-actions.rst
--rw-r--r--   0        0        0    36245 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/docs/implementers.rst
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/docs/index.rst
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/docs/motd.txt
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/docs/requirements.in
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/docs/requirements.txt
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/docs/_static/logo.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/index.html
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/package.json
--rw-r--r--   0        0        0   147209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/tsconfig.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/vite.config.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/public/favicon.svg
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/DialectReportView.tsx
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/MainContainer.tsx
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/ReportDataHandler.tsx
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/global.css
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/index.tsx
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/assets/landscape-logo.svg
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/CopyToClipboard.tsx
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/FilterSection.css
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/FilterSection.tsx
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/LoadingAnimation.tsx
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/NavBar.tsx
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/OtherImplementations.tsx
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/Cases/CaseItem.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/Cases/CaseResultSvg.test.tsx
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/Cases/CaseResultSvg.tsx
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/Cases/CasesSection.tsx
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/Cases/SchemaDisplay.tsx
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/DragAndDrop/DragAndDrop.tsx
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/Modals/DetailsButtonModal.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/RunInfo/RunInfoSection.tsx
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/Summary/ImplementationRow.tsx
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/Summary/SummarySection.tsx
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/components/Summary/SummaryTable.tsx
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/context/BowtieVersionContext.tsx
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/context/ThemeContext.tsx
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/data/Badge.test.ts
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/data/Badge.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/data/Dialect.test.ts
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/data/Dialect.ts
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/data/Site.test.ts
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/data/Site.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/data/mapLanguage.ts
--rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/data/parseReportData.test.ts
--rw-r--r--   0        0        0     8993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/frontend/src/hooks/useSearchParams.ts
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/.java-implementations-pmd-ruleset.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/clojure-json-schema/Dockerfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/clojure-json-schema/project.clj
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/cpp-valijson/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/cpp-valijson/.gitignore
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/cpp-valijson/Dockerfile
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/cpp-valijson/bowtie_valijson.cpp
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/cpp-valijson/compile_flags.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/dotnet-jsonschema-net/.clang-format
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/dotnet-jsonschema-net/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/dotnet-jsonschema-net/Dockerfile
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/dotnet-jsonschema-net/Program.cs
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/go-gojsonschema/Dockerfile
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/go-gojsonschema/bowtie_gojsonschema.go
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/go-gojsonschema/go.mod
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/go-gojsonschema/go.sum
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/go-jsonschema/Dockerfile
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/go-jsonschema/bowtie_jsonschema.go
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/go-jsonschema/go.mod
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/go-jsonschema/go.sum
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-json-schema/BowtieJsonSchema.java
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-json-schema/Dockerfile
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-json-schema/build.gradle
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-json-schema-validator/build.gradle
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-jsonschemafriend/Dockerfile
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-jsonschemafriend/build.gradle
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/.dockerignore
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/.editorconfig
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/Dockerfile
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/build.gradle.kts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/gradle.properties
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/justfile
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/settings.gradle.kts
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/gradle/libs.versions.toml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/js-ajv/Dockerfile
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/js-ajv/bowtie_ajv.js
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/js-ajv/package-lock.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/js-ajv/package.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/js-hyperjump/Dockerfile
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/js-hyperjump/bowtie_hyperjump.js
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/js-hyperjump/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/js-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/js-jsonschema/bowtie_jsonschema.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/js-jsonschema/package.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/.gitignore
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/lua-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/lua-jsonschema/bowtie_jsonschema.lua
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/lua-jsonschema/json.lua
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/lua-jsonschema/stylua.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/php-opis-json-schema/Dockerfile
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/php-opis-json-schema/bowtieJsonSchema.php
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/php-opis-json-schema/composer.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/python-fastjsonschema/Dockerfile
--rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/python-jschon/Dockerfile
--rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/python-jschon/bowtie_jschon.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/python-jsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/python-jsonschema/bowtie_jsonschema.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/ruby-json_schemer/.rubocop.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/ruby-json_schemer/Dockerfile
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/ruby-json_schemer/Gemfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/ruby-json_schemer/Gemfile.lock
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/ruby-json_schemer/bowtie_json_schemer.rb
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/rust-boon/Cargo.lock
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/rust-boon/Cargo.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/rust-boon/Dockerfile
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/rust-boon/build.rs
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/rust-boon/src/main.rs
--rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/rust-jsonschema/Cargo.lock
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/rust-jsonschema/Cargo.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/rust-jsonschema/Dockerfile
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/rust-jsonschema/build.rs
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/rust-jsonschema/src/main.rs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/scala-mjs-validator/Dockerfile
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/scala-mjs-validator/Harness.scala
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/scala-mjs-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/scala-mjs-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/scala-mjs-validator/project/plugins.sbt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/scala-rc-circe-json-validator/Dockerfile
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/scala-rc-circe-json-validator/Harness.scala
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/scala-rc-circe-json-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/scala-rc-circe-json-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/scala-rc-circe-json-validator/project/plugins.sbt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/ts-vscode-json-languageservice/Dockerfile
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/ts-vscode-json-languageservice/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/implementations/ts-vscode-json-languageservice/tsconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/conftest.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/test_cli.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/test_dialect.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/test_github.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/test_hypothesis.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/test_implementation.py
--rw-r--r--   0        0        0    62217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/test_integration.py
--rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/test_report.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/test_schemas.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/models/group.json
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/models/test.json
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/LICENSE
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/README.rst
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/hatch_build.py
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/pyproject.toml
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.8/PKG-INFO
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.gitpod.yml
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.prettierrc.json
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.readthedocs.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/action.yml
+-rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/noxfile.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/requirements.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/test-requirements.in
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/test-requirements.txt
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.devcontainer/.codespace.Dockerfile
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.pre-commit-hooks/check-dependabot
+-rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.pre-commit-hooks/check-lintsonschema-schema
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/__main__.py
+-rw-r--r--   0        0        0    42570 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/_cli.py
+-rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/_commands.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/_containers.py
+-rw-r--r--   0        0        0    21220 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/_core.py
+-rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/_report.py
+-rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/_suite.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/exceptions.py
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/hypothesis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/py.typed
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/models/dialect.json
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/models/group.json
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/models/implementation.json
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/models/registry.json
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/bowtie/schemas/models/test.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/data/dialects.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/Makefile
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/cli.rst
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/conf.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/contributing.rst
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/github-actions.rst
+-rw-r--r--   0        0        0    36245 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/implementers.rst
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/index.rst
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/motd.txt
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/requirements.in
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/requirements.txt
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/docs/_static/logo.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/index.html
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/package.json
+-rw-r--r--   0        0        0   152698 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/tsconfig.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/vite.config.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/public/favicon.svg
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/DialectReportView.tsx
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/MainContainer.tsx
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/ReportDataHandler.tsx
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/global.css
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/index.tsx
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/assets/landscape-logo.svg
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/CopyToClipboard.tsx
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/FilterSection.css
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/FilterSection.tsx
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/LoadingAnimation.tsx
+-rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/NavBar.tsx
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/OtherImplementations.tsx
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CaseItem.tsx
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CaseResultSvg.test.tsx
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CaseResultSvg.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CasesSection.tsx
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Cases/SchemaDisplay.tsx
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/DragAndDrop/DragAndDrop.tsx
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Modals/DetailsButtonModal.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/RunInfo/RunInfoSection.tsx
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Summary/ImplementationRow.tsx
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Summary/SummarySection.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/components/Summary/SummaryTable.tsx
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/context/BowtieVersionContext.tsx
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/context/ThemeContext.tsx
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/Badge.test.ts
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/Badge.ts
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/Dialect.test.ts
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/Dialect.ts
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/Site.test.ts
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/Site.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/mapLanguage.ts
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/parseReportData.test.ts
+-rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/frontend/src/hooks/useSearchParams.ts
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/.java-implementations-pmd-ruleset.xml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/clojure-json-schema/Dockerfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/clojure-json-schema/project.clj
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/cpp-valijson/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/cpp-valijson/.gitignore
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/cpp-valijson/Dockerfile
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/cpp-valijson/bowtie_valijson.cpp
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/cpp-valijson/compile_flags.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/.clang-format
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/Dockerfile
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/Program.cs
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-gojsonschema/Dockerfile
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-gojsonschema/bowtie_gojsonschema.go
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-gojsonschema/go.mod
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-gojsonschema/go.sum
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-json-schema/BowtieJsonSchema.java
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-json-schema/Dockerfile
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-json-schema/build.gradle
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-jsonschemafriend/Dockerfile
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-jsonschemafriend/build.gradle
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/.dockerignore
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/.editorconfig
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/Dockerfile
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/build.gradle.kts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/gradle.properties
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/justfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/settings.gradle.kts
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/gradle/libs.versions.toml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-jsonschema/bowtie_jsonschema.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/js-jsonschema/package.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/bowtie_jsonschema.lua
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/stylua.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/php-opis-json-schema/Dockerfile
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/php-opis-json-schema/bowtieJsonSchema.php
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/php-opis-json-schema/composer.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/python-jschon/Dockerfile
+-rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/python-jschon/bowtie_jschon.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/python-jsonschema/bowtie_jsonschema.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ruby-json_schemer/.rubocop.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ruby-json_schemer/Dockerfile
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ruby-json_schemer/Gemfile
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ruby-json_schemer/Gemfile.lock
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ruby-json_schemer/bowtie_json_schemer.rb
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-boon/Cargo.lock
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-boon/Cargo.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-boon/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-boon/build.rs
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-boon/src/main.rs
+-rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/build.rs
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/Dockerfile
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/Harness.scala
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/Dockerfile
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/Harness.scala
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ts-vscode-json-languageservice/Dockerfile
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ts-vscode-json-languageservice/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/implementations/ts-vscode-json-languageservice/tsconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/conftest.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_cli.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_dialect.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_github.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_hypothesis.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_implementation.py
+-rw-r--r--   0        0        0    62217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_integration.py
+-rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_report.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/test_schemas.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/group.json
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/test.json
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/LICENSE
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/README.rst
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/hatch_build.py
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.3.9/PKG-INFO
```

### Comparing `bowtie_json_schema-2024.3.8/.gitpod.yml` & `bowtie_json_schema-2024.3.9/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/.pre-commit-config.yaml` & `bowtie_json_schema-2024.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/CONTRIBUTING.rst` & `bowtie_json_schema-2024.3.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/action.yml` & `bowtie_json_schema-2024.3.9/action.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/noxfile.py` & `bowtie_json_schema-2024.3.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/requirements.txt` & `bowtie_json_schema-2024.3.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/test-requirements.txt` & `bowtie_json_schema-2024.3.9/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/.pre-commit-hooks/check-dependabot` & `bowtie_json_schema-2024.3.9/.pre-commit-hooks/check-dependabot`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/.pre-commit-hooks/check-lintsonschema-schema` & `bowtie_json_schema-2024.3.9/.pre-commit-hooks/check-lintsonschema-schema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/_cli.py` & `bowtie_json_schema-2024.3.9/bowtie/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -786,23 +786,25 @@
     callback=_disallow_max_fail,
     is_flag=True,
     default=False,
     help="Fail immediately after the first error or disagreement.",
 )
 MAX_FAIL = click.option(
     "--max-fail",
+    metavar="COUNT",
     type=click.IntRange(min=1),
     callback=_disallow_fail_fast,
-    help="Fail immediately if N tests fail in total across implementations",
+    help="Fail immediately if x tests fail in total across implementations",
 )
 MAX_ERROR = click.option(
     "--max-error",
+    metavar="COUNT",
     type=click.IntRange(min=1),
     callback=_disallow_fail_fast,
-    help="Fail immediately if N errors occur in total across implementations",
+    help="Fail immediately if x errors occur in total across implementations",
 )
 SET_SCHEMA = click.option(
     "--set-schema",
     "-S",
     "maybe_set_schema",
     # I have no idea why Click makes this so hard, but no combination of:
     #     type, default, is_flag, flag_value, nargs, ...
```

### Comparing `bowtie_json_schema-2024.3.8/bowtie/_commands.py` & `bowtie_json_schema-2024.3.9/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/_containers.py` & `bowtie_json_schema-2024.3.9/bowtie/_containers.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/_core.py` & `bowtie_json_schema-2024.3.9/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/_report.py` & `bowtie_json_schema-2024.3.9/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/_suite.py` & `bowtie_json_schema-2024.3.9/bowtie/_suite.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/exceptions.py` & `bowtie_json_schema-2024.3.9/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/hypothesis.py` & `bowtie_json_schema-2024.3.9/bowtie/hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/schemas/io/v1.json` & `bowtie_json_schema-2024.3.9/bowtie/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/schemas/io/commands/run.json` & `bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/schemas/io/commands/start.json` & `bowtie_json_schema-2024.3.9/bowtie/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/schemas/models/dialect.json` & `bowtie_json_schema-2024.3.9/bowtie/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/schemas/models/group.json` & `bowtie_json_schema-2024.3.9/bowtie/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/schemas/models/implementation.json` & `bowtie_json_schema-2024.3.9/bowtie/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/bowtie/schemas/models/test.json` & `bowtie_json_schema-2024.3.9/bowtie/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/data/dialects.json` & `bowtie_json_schema-2024.3.9/data/dialects.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/docs/Makefile` & `bowtie_json_schema-2024.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/docs/cli.rst` & `bowtie_json_schema-2024.3.9/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/docs/conf.py` & `bowtie_json_schema-2024.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/docs/contributing.rst` & `bowtie_json_schema-2024.3.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/docs/github-actions.rst` & `bowtie_json_schema-2024.3.9/docs/github-actions.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/docs/implementers.rst` & `bowtie_json_schema-2024.3.9/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/docs/index.rst` & `bowtie_json_schema-2024.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/docs/motd.txt` & `bowtie_json_schema-2024.3.9/docs/motd.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/docs/requirements.txt` & `bowtie_json_schema-2024.3.9/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/docs/_static/logo.svg` & `bowtie_json_schema-2024.3.9/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/package.json` & `bowtie_json_schema-2024.3.9/frontend/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9918128654970759%*

 * *Differences: {"'dependencies'": "{'react-syntax-highlighter': '^15.5.0'}",*

 * * "'devDependencies'": "{'@types/react-syntax-highlighter': '^15.5.11'}"}*

```diff
@@ -3,20 +3,22 @@
         "bootstrap": "^5.3.2",
         "dayjs": "^1.11.10",
         "react": "^18.2.0",
         "react-bootstrap": "^2.10.1",
         "react-bootstrap-icons": "^1.11.3",
         "react-dom": "^18.2.0",
         "react-router-dom": "^6.22.1",
+        "react-syntax-highlighter": "^15.5.0",
         "urijs": "^1.19.11"
     },
     "description": "The UI displays the outcomes generated by Bowtie, which serves as a meta-validator for the JSON Schema specification",
     "devDependencies": {
         "@types/react": "^18.2.56",
         "@types/react-dom": "^18.2.19",
+        "@types/react-syntax-highlighter": "^15.5.11",
         "@types/react-test-renderer": "^18.0.7",
         "@types/urijs": "^1.19.25",
         "@typescript-eslint/eslint-plugin": "^7.0.0",
         "@typescript-eslint/parser": "^6.21.0",
         "@vitejs/plugin-react": "^4.2.1",
         "eslint": "8.56.0",
         "eslint-plugin-react": "7.33.2",
```

### Comparing `bowtie_json_schema-2024.3.8/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2024.3.9/frontend/pnpm-lock.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -22,25 +22,31 @@
     version: 1.11.3(react@18.2.0)
   react-dom:
     specifier: ^18.2.0
     version: 18.2.0(react@18.2.0)
   react-router-dom:
     specifier: ^6.22.1
     version: 6.22.1(react-dom@18.2.0)(react@18.2.0)
+  react-syntax-highlighter:
+    specifier: ^15.5.0
+    version: 15.5.0(react@18.2.0)
   urijs:
     specifier: ^1.19.11
     version: 1.19.11
 
 devDependencies:
   '@types/react':
     specifier: ^18.2.56
     version: 18.2.56
   '@types/react-dom':
     specifier: ^18.2.19
     version: 18.2.19
+  '@types/react-syntax-highlighter':
+    specifier: ^15.5.11
+    version: 15.5.11
   '@types/react-test-renderer':
     specifier: ^18.0.7
     version: 18.0.7
   '@types/urijs':
     specifier: ^1.19.25
     version: 1.19.25
   '@typescript-eslint/eslint-plugin':
@@ -887,14 +893,20 @@
       '@types/json-schema': 7.0.15
     dev: true
 
   /@types/estree@1.0.5:
     resolution: {integrity: sha512-/kYRxGDLWzHOB7q+wtSUQlFrtcdUccpfy+X+9iMBpHK8QLLhx2wIPYuS5DYtR9Wa/YlZAbIovy7qVdB1Aq6Lyw==}
     dev: true
 
+  /@types/hast@2.3.10:
+    resolution: {integrity: sha512-McWspRw8xx8J9HurkVBfYj0xKoE25tOFlHGdx4MJ5xORQrMGZNqJhVQWaIbm6Oyla5kYOXtDiopzKRJzEOkwJw==}
+    dependencies:
+      '@types/unist': 2.0.10
+    dev: false
+
   /@types/json-schema@7.0.15:
     resolution: {integrity: sha512-5+fP8P8MFNC+AyZCDxrB2pkZFPGzqQWUzpSeuuVLvm8VMcorNYavBqoFcxK8bQz4Qsbn4oUEEem4wDLfcysGHA==}
     dev: true
 
   /@types/node@20.11.5:
     resolution: {integrity: sha512-g557vgQjUUfN76MZAN/dt1z3dzcUsimuysco0KeluHgrPdJXkP/XdAURgyO2W9fZWHRtRBiVKzKn8vyOAwlG+w==}
     dependencies:
@@ -906,14 +918,20 @@
 
   /@types/react-dom@18.2.19:
     resolution: {integrity: sha512-aZvQL6uUbIJpjZk4U8JZGbau9KDeAwMfmhyWorxgBkqDIEf6ROjRozcmPIicqsUwPUjbkDfHKgGee1Lq65APcA==}
     dependencies:
       '@types/react': 18.2.56
     dev: true
 
+  /@types/react-syntax-highlighter@15.5.11:
+    resolution: {integrity: sha512-ZqIJl+Pg8kD+47kxUjvrlElrraSUrYa4h0dauY/U/FTUuprSCqvUj+9PNQNQzVc6AJgIWUUxn87/gqsMHNbRjw==}
+    dependencies:
+      '@types/react': 18.2.56
+    dev: true
+
   /@types/react-test-renderer@18.0.7:
     resolution: {integrity: sha512-1+ANPOWc6rB3IkSnElhjv6VLlKg2dSv/OWClUyZimbLsQyBn8Js9Vtdsi3UICJ2rIQ3k2la06dkB+C92QfhKmg==}
     dependencies:
       '@types/react': 18.2.56
     dev: true
 
   /@types/react-transition-group@4.4.10:
@@ -932,14 +950,18 @@
   /@types/scheduler@0.16.8:
     resolution: {integrity: sha512-WZLiwShhwLRmeV6zH+GkbOFT6Z6VklCItrDioxUnv+u4Ll+8vKeFySoFyK/0ctcRpOmwAicELfmys1sDc/Rw+A==}
 
   /@types/semver@7.5.6:
     resolution: {integrity: sha512-dn1l8LaMea/IjDoHNd9J52uBbInB796CDffS6VdIxvqYCPSG0V0DzHp76GpaWnlhg88uYyPbXCDIowa86ybd5A==}
     dev: true
 
+  /@types/unist@2.0.10:
+    resolution: {integrity: sha512-IfYcSBWE3hLpBg8+X2SEa8LVkJdJEkT2Ese2aaLs3ptGdVtABxndrMaxuFlQ1qdFf9Q5rDvDpxI3WwgvKFAsQA==}
+    dev: false
+
   /@types/urijs@1.19.25:
     resolution: {integrity: sha512-XOfUup9r3Y06nFAZh3WvO0rBU4OtlfPB/vgxpjg+NRdGU6CN6djdc6OEiH+PcqHCY6eFLo9Ista73uarf4gnBg==}
     dev: true
 
   /@types/warning@3.0.3:
     resolution: {integrity: sha512-D1XC7WK8K+zZEveUPY+cf4+kgauk8N4eHr/XIHXGlGYkHLud6hK9lYfZk1ry1TNh798cZUCgb6MqGEG8DkJt6Q==}
     dev: false
@@ -1557,14 +1579,26 @@
     resolution: {integrity: sha512-oKnbhFyRIXpUuez8iBMmyEa4nbj4IOQyuhc/wy9kY7/WVPcwIO9VA668Pu8RkO7+0G76SLROeyw9CpQ061i4mA==}
     engines: {node: '>=10'}
     dependencies:
       ansi-styles: 4.3.0
       supports-color: 7.2.0
     dev: true
 
+  /character-entities-legacy@1.1.4:
+    resolution: {integrity: sha512-3Xnr+7ZFS1uxeiUDvV02wQ+QDbc55o97tIV5zHScSPJpcLm/r0DFPcoY3tYRp+VZukxuMeKgXYmsXQHO05zQeA==}
+    dev: false
+
+  /character-entities@1.2.4:
+    resolution: {integrity: sha512-iBMyeEHxfVnIakwOuDXpVkc54HijNgCyQB2w0VfGQThle6NXn50zU6V/u+LDhxHcDUPojn6Kpga3PTAD8W1bQw==}
+    dev: false
+
+  /character-reference-invalid@1.1.4:
+    resolution: {integrity: sha512-mKKUkUbhPpQlCOfIuZkvSEgktjPFIsZKRRbC6KWVEMvlzblj3i3asQv5ODsrwt0N3pHAEvjP8KTQPHkp0+6jOg==}
+    dev: false
+
   /check-error@1.0.3:
     resolution: {integrity: sha512-iKEoDYaRmd1mxM90a2OEfWhjsjPpYPuQ+lMYsoxB126+t8fw7ySEO48nmDg5COTjxDI65/Y2OWpeEHk3ZOe8zg==}
     dependencies:
       get-func-name: 2.0.2
     dev: true
 
   /chrome-trace-event@1.0.3:
@@ -1609,14 +1643,18 @@
   /combined-stream@1.0.8:
     resolution: {integrity: sha512-FQN4MRfuJeHf7cBbBMJFXhKSDq+2kAArBlmRBvcvFE5BB1HZKXtSFASDhdlz9zOYwxh8lDdnvmMOe/+5cdoEdg==}
     engines: {node: '>= 0.8'}
     dependencies:
       delayed-stream: 1.0.0
     dev: true
 
+  /comma-separated-tokens@1.0.8:
+    resolution: {integrity: sha512-GHuDRO12Sypu2cV70d1dkA2EUmXHgntrzbpvOB+Qy+49ypNfGgFQIC2fhhXbnyrJRynDCAARsT7Ou0M6hirpfw==}
+    dev: false
+
   /commander@2.20.3:
     resolution: {integrity: sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==}
     dev: true
 
   /concat-map@0.0.1:
     resolution: {integrity: sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==}
     dev: true
@@ -2108,14 +2146,20 @@
 
   /fastq@1.16.0:
     resolution: {integrity: sha512-ifCoaXsDrsdkWTtiNJX5uzHDsrck5TzfKKDcuFFTIrrc/BS076qgEIfoIy1VeZqViznfKiysPYTh/QeHtnIsYA==}
     dependencies:
       reusify: 1.0.4
     dev: true
 
+  /fault@1.0.4:
+    resolution: {integrity: sha512-CJ0HCB5tL5fYTEA7ToAq5+kTwd++Borf1/bifxd9iT70QcXr4MRrO3Llf8Ifs70q+SJcGHFtnIE/Nw6giCtECA==}
+    dependencies:
+      format: 0.2.2
+    dev: false
+
   /file-entry-cache@6.0.1:
     resolution: {integrity: sha512-7Gps/XWymbLk2QLYK4NzpMOrYjMhdIxXuIvy2QBsLE6ljuodKvdkWs/cpyJJ3CVIVpH0Oi1Hvg1ovbMzLdFBBg==}
     engines: {node: ^10.12.0 || >=12.0.0}
     dependencies:
       flat-cache: 3.2.0
     dev: true
 
@@ -2158,14 +2202,19 @@
     engines: {node: '>= 6'}
     dependencies:
       asynckit: 0.4.0
       combined-stream: 1.0.8
       mime-types: 2.1.35
     dev: true
 
+  /format@0.2.2:
+    resolution: {integrity: sha512-wzsgA6WOq+09wrU1tsJ09udeR/YZRaeArL9e1wPbFg3GG2yDnC2ldKpxs4xunpFF9DgqCqOIra3bc1HWrJ37Ww==}
+    engines: {node: '>=0.4.x'}
+    dev: false
+
   /fs.realpath@1.0.0:
     resolution: {integrity: sha512-OO0pH2lK6a0hZnAdau5ItzHPI6pUlvI7jMVnxUQRtw4owF2wk8lOSabtGDCTP4Ggrg2MbGnWO9X8K1t4+fGMDw==}
     dev: true
 
   /fsevents@2.3.3:
     resolution: {integrity: sha512-5xoDfX+fL7faATnagmWPpbFtwh/R77WmMMqqHGS65C3vvB0YHrgF+B1YmZ3441tMj5n63k0212XNoJwzlhffQw==}
     engines: {node: ^8.16.0 || ^10.6.0 || >=11.0.0}
@@ -2342,14 +2391,32 @@
   /hasown@2.0.0:
     resolution: {integrity: sha512-vUptKVTpIJhcczKBbgnS+RtcuYMB8+oNzPK2/Hp3hanz8JmpATdmmgLgSaadVREkDm+e2giHwY3ZRkyjSIDDFA==}
     engines: {node: '>= 0.4'}
     dependencies:
       function-bind: 1.1.2
     dev: true
 
+  /hast-util-parse-selector@2.2.5:
+    resolution: {integrity: sha512-7j6mrk/qqkSehsM92wQjdIgWM2/BW61u/53G6xmC8i1OmEdKLHbk419QKQUjz6LglWsfqoiHmyMRkP1BGjecNQ==}
+    dev: false
+
+  /hastscript@6.0.0:
+    resolution: {integrity: sha512-nDM6bvd7lIqDUiYEiu5Sl/+6ReP0BMk/2f4U/Rooccxkj0P5nm+acM5PrGJ/t5I8qPGiqZSE6hVAwZEdZIvP4w==}
+    dependencies:
+      '@types/hast': 2.3.10
+      comma-separated-tokens: 1.0.8
+      hast-util-parse-selector: 2.2.5
+      property-information: 5.6.0
+      space-separated-tokens: 1.1.5
+    dev: false
+
+  /highlight.js@10.7.3:
+    resolution: {integrity: sha512-tzcUFauisWKNHaRkN4Wjl/ZA07gENAjFl3J/c480dprkGTg5EQstgaNFqBfUqCq54kZRIEcreTsAgF/m2quD7A==}
+    dev: false
+
   /html-encoding-sniffer@4.0.0:
     resolution: {integrity: sha512-Y22oTqIU4uuPgEemfz7NDJz6OeKf12Lsu+QC+s3BVpda64lTiMYCyGwg5ki4vFxkMwQdeZDl2adZoqUgdFuTgQ==}
     engines: {node: '>=18'}
     dependencies:
       whatwg-encoding: 3.1.1
     dev: true
 
@@ -2439,14 +2506,25 @@
 
   /invariant@2.2.4:
     resolution: {integrity: sha512-phJfQVBuaJM5raOpJjSfkiD6BpbCE4Ns//LaXl6wGYtUBY83nWS6Rf9tXm2e8VaK60JEjYldbPif/A2B1C2gNA==}
     dependencies:
       loose-envify: 1.4.0
     dev: false
 
+  /is-alphabetical@1.0.4:
+    resolution: {integrity: sha512-DwzsA04LQ10FHTZuL0/grVDk4rFoVH1pjAToYwBrHSxcrBIGQuXrQMtD5U1b0U2XVgKZCTLLP8u2Qxqhy3l2Vg==}
+    dev: false
+
+  /is-alphanumerical@1.0.4:
+    resolution: {integrity: sha512-UzoZUr+XfVz3t3v4KyGEniVL9BDRoQtY7tOyrRybkVNjDFWyo1yhXNGrrBTQxp3ib9BLAWs7k2YKBQsFRkZG9A==}
+    dependencies:
+      is-alphabetical: 1.0.4
+      is-decimal: 1.0.4
+    dev: false
+
   /is-array-buffer@3.0.2:
     resolution: {integrity: sha512-y+FyyR/w8vfIRq4eQcM1EYgSTnmHXPqaF+IgzgraytCFq5Xh8lllDVmAZolPJiZttZLeFSINPYMaEJ7/vWUa1w==}
     dependencies:
       call-bind: 1.0.5
       get-intrinsic: 1.2.2
       is-typed-array: 1.1.12
     dev: true
@@ -2486,14 +2564,18 @@
   /is-date-object@1.0.5:
     resolution: {integrity: sha512-9YQaSxsAiSwcvS33MBk3wTCVnWK+HhF8VZR2jRxehM16QcVOdHqPn4VPHmRK4lSr38n9JriurInLcP90xsYNfQ==}
     engines: {node: '>= 0.4'}
     dependencies:
       has-tostringtag: 1.0.0
     dev: true
 
+  /is-decimal@1.0.4:
+    resolution: {integrity: sha512-RGdriMmQQvZ2aqaQq3awNA6dCGtKpiDFcOzrTWrDAT2MiWrKQVPmxLGHl7Y2nNu6led0kEyoX0enY0qXYsv9zw==}
+    dev: false
+
   /is-docker@2.2.1:
     resolution: {integrity: sha512-F+i2BKsFrH66iaUFc0woD8sLy8getkwTwtOBjvs56Cx4CgJDeKQeqfz8wAYiSb8JOprWhHH5p77PbmYCvvUuXQ==}
     engines: {node: '>=8'}
     hasBin: true
     dev: true
 
   /is-extglob@2.1.1:
@@ -2522,14 +2604,18 @@
   /is-glob@4.0.3:
     resolution: {integrity: sha512-xelSayHH36ZgE7ZWhli7pW34hNbNl8Ojv5KVmkJD4hBdD3th8Tfk9vYasLM+mXWOZhFkgZfxhLSnrwRr4elSSg==}
     engines: {node: '>=0.10.0'}
     dependencies:
       is-extglob: 2.1.1
     dev: true
 
+  /is-hexadecimal@1.0.4:
+    resolution: {integrity: sha512-gyPJuv83bHMpocVYoqof5VDiZveEoGoFL8m3BXNb2VW8Xs+rz9kqO8LOQ5DH6EsuvilT1ApazU0pyl+ytbPtlw==}
+    dev: false
+
   /is-map@2.0.2:
     resolution: {integrity: sha512-cOZFQQozTha1f4MxLFzlgKYPTyj26picdZTx82hbc/Xf4K/tZOOXSCkMvU4pKioRXGDLJRn0GM7Upe7kR721yg==}
     dev: true
 
   /is-negative-zero@2.0.2:
     resolution: {integrity: sha512-dqJvarLawXsFbNDeJW7zAz8ItJ9cd28YufuuFzh0G8pNHjJMnY08Dv7sYX2uF5UpQOwieAeOExEYAWWfu7ZZUA==}
     engines: {node: '>= 0.4'}
@@ -2789,14 +2875,21 @@
 
   /loupe@2.3.7:
     resolution: {integrity: sha512-zSMINGVYkdpYSOBmLi0D1Uo7JU9nVdQKrHxC8eYlV+9YKK9WePqAlL7lSlorG/U2Fw1w0hTBmaa/jrQ3UbPHtA==}
     dependencies:
       get-func-name: 2.0.2
     dev: true
 
+  /lowlight@1.20.0:
+    resolution: {integrity: sha512-8Ktj+prEb1RoCPkEOrPMYUN/nCggB7qAWe3a7OpMjWQkh3l2RD5wKRQ+o8Q8YuI9RG/xs95waaI/E6ym/7NsTw==}
+    dependencies:
+      fault: 1.0.4
+      highlight.js: 10.7.3
+    dev: false
+
   /lru-cache@5.1.1:
     resolution: {integrity: sha512-KpNARQA3Iwv+jTA0utUVVbrh+Jlrr1Fv0e56GGzAFOXN7dk/FviaDW8LHmK52DlcH4WP2n6gI8vN1aesBFgo9w==}
     dependencies:
       yallist: 3.1.1
     dev: true
 
   /lru-cache@6.0.0:
@@ -3021,14 +3114,25 @@
   /parent-module@1.0.1:
     resolution: {integrity: sha512-GQ2EWRpQV8/o+Aw8YqtfZZPfNRWZYkbidE9k5rpl/hC3vtHHBfGm2Ifi6qWV+coDGkrUKZAxE3Lot5kcsRlh+g==}
     engines: {node: '>=6'}
     dependencies:
       callsites: 3.1.0
     dev: true
 
+  /parse-entities@2.0.0:
+    resolution: {integrity: sha512-kkywGpCcRYhqQIchaWqZ875wzpS/bMKhz5HnN3p7wveJTkTtyAB/AlnS0f8DFSqYW1T82t6yEAkEcB+A1I3MbQ==}
+    dependencies:
+      character-entities: 1.2.4
+      character-entities-legacy: 1.1.4
+      character-reference-invalid: 1.1.4
+      is-alphanumerical: 1.0.4
+      is-decimal: 1.0.4
+      is-hexadecimal: 1.0.4
+    dev: false
+
   /parse5@7.1.2:
     resolution: {integrity: sha512-Czj1WaSVpaoj0wbhMzLmWD69anp2WH7FXMB9n1Sy8/ZFF9jolSQVMu1Ij5WIyGmcBmhk7EOndpO4mIpihVqAXw==}
     dependencies:
       entities: 4.5.0
     dev: true
 
   /path-exists@4.0.0:
@@ -3104,14 +3208,24 @@
     engines: {node: ^14.15.0 || ^16.10.0 || >=18.0.0}
     dependencies:
       '@jest/schemas': 29.6.3
       ansi-styles: 5.2.0
       react-is: 18.2.0
     dev: true
 
+  /prismjs@1.27.0:
+    resolution: {integrity: sha512-t13BGPUlFDR7wRB5kQDG4jjl7XeuH6jbJGt11JHPL96qwsEHNX2+68tFXqc1/k+/jALsbSWJKUOT/hcYAZ5LkA==}
+    engines: {node: '>=6'}
+    dev: false
+
+  /prismjs@1.29.0:
+    resolution: {integrity: sha512-Kx/1w86q/epKcmte75LNrEoT+lX8pBpavuAbvJWRXar7Hz8jrtF+e3vY751p0R8H9HdArwaCTNDDzHg/ScJK1Q==}
+    engines: {node: '>=6'}
+    dev: false
+
   /prop-types-extra@1.1.1(react@18.2.0):
     resolution: {integrity: sha512-59+AHNnHYCdiC+vMwY52WmvP5dM3QLeoumYuEyceQDi9aEhtwN9zIQ2ZNo25sMyXnbh32h+P1ezDsUpUH3JAew==}
     peerDependencies:
       react: '>=0.14.0'
     dependencies:
       react: 18.2.0
       react-is: 16.13.1
@@ -3121,14 +3235,20 @@
   /prop-types@15.8.1:
     resolution: {integrity: sha512-oj87CgZICdulUohogVAR7AjlC0327U4el4L6eAvOqCeudMDVU0NThNaV+b9Df4dXgSP1gXMTnPdhfe/2qDH5cg==}
     dependencies:
       loose-envify: 1.4.0
       object-assign: 4.1.1
       react-is: 16.13.1
 
+  /property-information@5.6.0:
+    resolution: {integrity: sha512-YUHSPk+A30YPv+0Qf8i9Mbfe/C0hdPXk1s1jPVToV8pk8BQtpw10ct89Eo7OWkutrwqvT0eicAxlOg3dOAu8JA==}
+    dependencies:
+      xtend: 4.0.2
+    dev: false
+
   /psl@1.9.0:
     resolution: {integrity: sha512-E/ZsdU4HLs/68gYzgGTkMicWTLPdAftJLfJFlLUAAKZGkStNU72sZjT66SnMDVOfOWY/YAoiD7Jxa9iHvngcag==}
     dev: true
 
   /punycode@2.3.1:
     resolution: {integrity: sha512-vYt7UD1U9Wg6138shLtLOvdAu+8DsC/ilFtEVHcH+wydcSpNE20AfSOduf6MkRFahL5FY7X1oU7nKVZFtfq8Fg==}
     engines: {node: '>=6'}
@@ -3239,14 +3359,27 @@
       react: ^16.0.0 || ^17.0.0 || ^18.0.0
     dependencies:
       object-assign: 4.1.1
       react: 18.2.0
       react-is: 18.2.0
     dev: true
 
+  /react-syntax-highlighter@15.5.0(react@18.2.0):
+    resolution: {integrity: sha512-+zq2myprEnQmH5yw6Gqc8lD55QHnpKaU8TOcFeC/Lg/MQSs8UknEA0JC4nTZGFAXC2J2Hyj/ijJ7NlabyPi2gg==}
+    peerDependencies:
+      react: '>= 0.14.0'
+    dependencies:
+      '@babel/runtime': 7.23.8
+      highlight.js: 10.7.3
+      lowlight: 1.20.0
+      prismjs: 1.29.0
+      react: 18.2.0
+      refractor: 3.6.0
+    dev: false
+
   /react-test-renderer@18.2.0(react@18.2.0):
     resolution: {integrity: sha512-JWD+aQ0lh2gvh4NM3bBM42Kx+XybOxCpgYK7F8ugAlpaTSnWsX+39Z4XkOykGZAHrjwwTZT3x3KxswVWxHPUqA==}
     peerDependencies:
       react: ^18.2.0
     dependencies:
       react: 18.2.0
       react-is: 18.2.0
@@ -3282,14 +3415,22 @@
       define-properties: 1.2.1
       es-abstract: 1.22.3
       get-intrinsic: 1.2.2
       globalthis: 1.0.3
       which-builtin-type: 1.1.3
     dev: true
 
+  /refractor@3.6.0:
+    resolution: {integrity: sha512-MY9W41IOWxxk31o+YvFCNyNzdkc9M20NoZK5vq6jkv4I/uh2zkWcfudj0Q1fovjUQJrNewS9NMzeTtqPf+n5EA==}
+    dependencies:
+      hastscript: 6.0.0
+      parse-entities: 2.0.0
+      prismjs: 1.27.0
+    dev: false
+
   /regenerator-runtime@0.14.1:
     resolution: {integrity: sha512-dYnhHh0nJoMfnkZs6GmmhFknAGRrLznOu5nc9ML+EJxGvrx6H7teuevqVqCuPcPK//3eDrrjQhehXVx9cnkGdw==}
     dev: false
 
   /regexp.prototype.flags@1.5.1:
     resolution: {integrity: sha512-sy6TXMN+hnP/wMy+ISxg3krXx7BAtWVO4UouuCN/ziM9UEne0euamVNafDfvC83bRNr95y0V5iijeDQFUNpvrg==}
     engines: {node: '>= 0.4'}
@@ -3522,14 +3663,18 @@
     dev: true
 
   /source-map@0.7.4:
     resolution: {integrity: sha512-l3BikUxvPOcn5E74dZiq5BGsTb5yEwhaTSzccU6t4sDOH8NWJCstKO5QT2CvtFoK6F0saL7p9xHAqHOlCPJygA==}
     engines: {node: '>= 8'}
     dev: true
 
+  /space-separated-tokens@1.1.5:
+    resolution: {integrity: sha512-q/JSVd1Lptzhf5bkYm4ob4iWPjx0KiRe3sRFBNrVqbJkFaBm5vbbowy1mymoPNLRa52+oadOhJ+K49wsSeSjTA==}
+    dev: false
+
   /stackback@0.0.2:
     resolution: {integrity: sha512-1XMJE5fQo1jGH6Y/7ebnwPOBEkIEnT4QF32d5R1+VXdXveM0IBMJt8zfaxX1P3QhVwrYe+576+jkANtSS2mBbw==}
     dev: true
 
   /std-env@3.7.0:
     resolution: {integrity: sha512-JPbdCEQLj1w5GilpiHAx3qJvFndqybBysA3qUOnznweH4QbNYUsW/ea8QzSrnh0vNsezMMw5bcVool8lM0gwzg==}
     dev: true
@@ -4237,14 +4382,19 @@
     engines: {node: '>=18'}
     dev: true
 
   /xmlchars@2.2.0:
     resolution: {integrity: sha512-JZnDKK8B0RCDw84FNdDAIpZK+JuJw+s7Lz8nksI7SIuU3UXJJslUthsi+uWBUYOwPFwW7W7PRLRfUKpxjtjFCw==}
     dev: true
 
+  /xtend@4.0.2:
+    resolution: {integrity: sha512-LKYU1iAXJXUgAXn9URjiu+MWhyUXHsvfp7mcuYm9dSUKK0/CjtrUwFAxD82/mCWbtLsGjFIad0wIsod4zrTAEQ==}
+    engines: {node: '>=0.4'}
+    dev: false
+
   /y18n@5.0.8:
     resolution: {integrity: sha512-0pfFzegeDWJHJIAmTLRP2DwHjdF5s7jo9tuztdQxAhINCdvS+3nGINqPd00AphqJR/0LhANUS6/+7SCb98YOfA==}
     engines: {node: '>=10'}
     dev: true
 
   /yallist@3.1.1:
     resolution: {integrity: sha512-a4UGQaWPH59mOXUYnAG2ewncQS4i4F43Tv3JoAM+s2VDAmS9NsK8GpDMLrCHPksFT7h3K6TOoUNn2pb7RoXx4g==}
```

### Comparing `bowtie_json_schema-2024.3.8/frontend/tsconfig.json` & `bowtie_json_schema-2024.3.9/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/public/favicon.svg` & `bowtie_json_schema-2024.3.9/frontend/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/DialectReportView.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/DialectReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/ReportDataHandler.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/ReportDataHandler.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/index.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/index.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -11,35 +11,33 @@
 import { ImplementationReportView } from "./components/ImplementationReportView/ImplementationReportView";
 import { MainContainer } from "./MainContainer";
 import { implementationMetadataURI } from "./data/Site";
 import {
   ImplementationData,
   ReportData,
   implementationFromData,
-  parseImplementationData,
+  prepareImplementationReport,
 } from "./data/parseReportData";
 
 const fetchReportData = async (dialect: Dialect) => {
   document.title = `Bowtie - ${dialect.prettyName}`;
   return dialect.fetchReport();
 };
 
-const fetchAllReportData = async (langImplementation: string) => {
+const fetchAllReportsData = async (langImplementation: string) => {
   document.title = `Bowtie - ${langImplementation}`;
-  const loaderData: Record<string, ReportData> = {};
+  const allReportsData = new Map<Dialect, ReportData>();
   const promises = [];
   for (const dialect of Dialect.known()) {
     promises.push(
-      dialect
-        .fetchReport()
-        .then((data) => (loaderData[dialect.shortName] = data)),
+      dialect.fetchReport().then((data) => allReportsData.set(dialect, data)),
     );
   }
   await Promise.all(promises);
-  return parseImplementationData(loaderData);
+  return prepareImplementationReport(allReportsData, langImplementation);
 };
 
 const fetchImplementationMetadata = async () => {
   const response = await fetch(implementationMetadataURI);
   const implementations = (await response.json()) as Record<
     string,
     ImplementationData
@@ -81,15 +79,15 @@
         path: "/local-report",
         Component: DragAndDrop,
       },
       {
         path: "/implementations/:langImplementation",
         Component: ImplementationReportView,
         loader: async ({ params }) =>
-          fetchAllReportData(params.langImplementation!),
+          fetchAllReportsData(params.langImplementation!),
       },
     ],
   },
 ]);
 
 document.addEventListener("DOMContentLoaded", () => {
   const root = createRoot(document.getElementById("root")!);
```

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/assets/landscape-logo.svg` & `bowtie_json_schema-2024.3.9/frontend/src/assets/landscape-logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/FilterSection.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/FilterSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/NavBar.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/NavBar.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/OtherImplementations.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/OtherImplementations.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/Cases/CaseItem.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CaseItem.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                   }
                 }}
               >
                 <td>
                   <p className="m-0">{test.description}</p>
                 </td>
                 {implementationsResults.map((implResult, i) => {
-                  const caseResults = implResult.cases.get(seq);
+                  const caseResults = implResult.caseResults.get(seq);
                   const result: CaseResult =
                     caseResults !== undefined
                       ? caseResults[index]
                       : { state: "errored" };
                   return <CaseResultSvg key={i} result={result} />;
                 })}
               </tr>
```

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/Cases/CaseResultSvg.test.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CaseResultSvg.test.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/Cases/CaseResultSvg.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CaseResultSvg.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/Cases/CasesSection.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/Cases/CasesSection.tsx`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import { ReportData } from "../../data/parseReportData";
 import CaseItem from "./CaseItem";
 
 const CasesSection = ({ reportData }: { reportData: ReportData }) => {
   const implementationsResults = Array.from(
     reportData.implementationsResults.values(),
   );
-  const implementations = implementationsResults.map(
-    (implResult) => reportData.runMetadata.implementations.get(implResult.id)!,
-  );
+  const implementations = Array.from(
+    reportData.implementationsResults.keys(),
+  ).map((id) => reportData.runMetadata.implementations.get(id)!);
 
   return (
     <Accordion id="cases">
       {Array.from(reportData.cases.entries()).map(([seq, caseData], index) => (
         <CaseItem
           key={index}
           seq={seq}
```

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/DragAndDrop/DragAndDrop.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/DragAndDrop/DragAndDrop.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/ImplementationReportView/DialectCompliance.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/ImplementationReportView/DialectCompliance.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import React from "react";
 import { Link } from "react-router-dom";
 import Card from "react-bootstrap/Card";
 import Image from "react-bootstrap/Image";
 import Table from "react-bootstrap/Table";
 
 import { complianceBadgeFor } from "../../data/Badge";
-import Dialect from "../../data/Dialect";
-import { ImplementationDialectCompliance } from "../../data/parseReportData";
+import { ImplementationReport } from "../../data/parseReportData";
 
 const DialectCompliance: React.FC<{
-  implementationDialectCompliance: ImplementationDialectCompliance;
-}> = ({ implementationDialectCompliance }) => {
-  const { implementation, dialectCompliance } = implementationDialectCompliance;
+  implementationReport: ImplementationReport;
+}> = ({ implementationReport }) => {
+  const { implementation, dialectCompliance } = implementationReport;
 
   return (
     <Card className="mx-auto mb-3 col-md-9">
       <Card.Header>Compliance</Card.Header>
       <Card.Body>
         <Table className="table-hover sm">
           <thead>
@@ -33,28 +32,26 @@
             <tr className="text-center">
               <th>Failed</th>
               <th>Skipped</th>
               <th>Errored</th>
             </tr>
           </thead>
           <tbody className="table-group-divider">
-            {Object.entries(dialectCompliance)
+            {Array.from(dialectCompliance.entries())
               .sort(
                 (a, b) =>
                   a[1].failedTests! +
                     a[1].erroredTests! +
                     a[1].skippedTests! -
                     b[1].failedTests! -
                     b[1].erroredTests! -
                     b[1].skippedTests! ||
-                  +Dialect.withName(b[0]).firstPublicationDate -
-                    +Dialect.withName(a[0]).firstPublicationDate,
+                  +b[0].firstPublicationDate - +a[0].firstPublicationDate,
               )
-              .map(([dialectName, result], index) => {
-                const dialect = Dialect.withName(dialectName);
+              .map(([dialect, result], index) => {
                 return (
                   <tr key={index}>
                     <td>{dialect.prettyName}</td>
                     <td className="text-center">{result.failedTests}</td>
                     <td className="text-center">{result.skippedTests}</td>
                     <td className="text-center">{result.erroredTests}</td>
                     <td>
```

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/ImplementationReportView/EmbedBadges.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/ImplementationReportView/EmbedBadges.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/Modals/DetailsButtonModal.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/Modals/DetailsButtonModal.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,26 @@
   show: boolean;
   handleClose: () => void;
   cases: Map<number, Case>;
   implementationResults: ImplementationResults;
   implementation: Implementation;
 }) => {
   const failedResults: JSX.Element[] = [];
-  Array.from(implementationResults.cases.entries()).forEach(
+  Array.from(implementationResults.caseResults.entries()).forEach(
     ([seq, results]) => {
       const caseData = cases.get(seq)!;
       for (let i = 0; i < results.length; i++) {
         const result = results[i];
         if (result.state === "successful") {
           continue;
         }
 
         let message;
         if (result.state === "skipped" || result.state === "errored") {
-          message = implementationResults.cases.get(seq)![i].message!;
+          message = implementationResults.caseResults.get(seq)![i].message!;
         } else if (result.valid) {
           message = "Unexpectedly valid";
         } else {
           message = "Unexpectedly invalid";
         }
         const borderClass =
           result.state === "skipped" ? "border-warning" : "border-danger";
```

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/RunInfo/RunInfoSection.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/RunInfo/RunInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2024.3.9/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/Summary/SummarySection.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/Summary/SummarySection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/components/Summary/SummaryTable.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/components/Summary/SummaryTable.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -55,31 +55,30 @@
             </div>
             unsuccessful
           </th>
           <th scope="col"></th>
         </tr>
       </thead>
       <tbody className="table-group-divider">
-        {Array.from(reportData.implementationsResults.values())
+        {Array.from(reportData.implementationsResults.entries())
           .sort(
-            (a, b) =>
-              a.failedTests +
-              a.erroredTests +
-              a.skippedTests -
-              b.failedTests -
-              b.erroredTests -
-              b.skippedTests,
+            ([, a], [, b]) =>
+              a.totals.failedTests! +
+              a.totals.erroredTests! +
+              a.totals.skippedTests! -
+              b.totals.failedTests! -
+              b.totals.erroredTests! -
+              b.totals.skippedTests!,
           )
-          .map((implResults, index) => (
+          .map(([id, implResults], index) => (
             <ImplementationRow
               cases={reportData.cases}
+              id={id}
+              implementation={reportData.runMetadata.implementations.get(id)!}
               implementationResults={implResults}
-              implementation={
-                reportData.runMetadata.implementations.get(implResults.id)!
-              }
               key={index}
               index={index}
             />
           ))}
       </tbody>
       <tfoot>
         <tr>
```

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/context/BowtieVersionContext.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/context/BowtieVersionContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/context/ThemeContext.tsx` & `bowtie_json_schema-2024.3.9/frontend/src/context/ThemeContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/data/Badge.test.ts` & `bowtie_json_schema-2024.3.9/frontend/src/data/Badge.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/data/Badge.ts` & `bowtie_json_schema-2024.3.9/frontend/src/data/Badge.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/data/Dialect.ts` & `bowtie_json_schema-2024.3.9/frontend/src/data/Dialect.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/data/Site.test.ts` & `bowtie_json_schema-2024.3.9/frontend/src/data/Site.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/data/parseReportData.test.ts` & `bowtie_json_schema-2024.3.9/frontend/src/data/parseReportData.test.ts`

 * *Files 2% similar despite different names*

```diff
@@ -85,21 +85,21 @@
         report.runMetadata.started,
         {},
       ),
       implementationsResults: new Map([
         [
           tag("envsonschema"),
           {
-            erroredCases: 0,
-            erroredTests: 0,
-            skippedTests: 0,
-            failedTests: 1,
-
-            id: tag("envsonschema"),
-            cases: new Map([[1, [{ state: "failed", valid: false }]]]),
+            totals: {
+              erroredCases: 0,
+              erroredTests: 0,
+              skippedTests: 0,
+              failedTests: 1,
+            },
+            caseResults: new Map([[1, [{ state: "failed", valid: false }]]]),
           },
         ],
       ]),
       cases: new Map([
         [
           1,
           {
@@ -217,21 +217,21 @@
         report.runMetadata.started,
         {},
       ),
       implementationsResults: new Map([
         [
           tag("envsonschema"),
           {
-            erroredCases: 0,
-            erroredTests: 0,
-            skippedTests: 0,
-            failedTests: 4,
-
-            id: tag("envsonschema"),
-            cases: new Map([
+            totals: {
+              erroredCases: 0,
+              erroredTests: 0,
+              skippedTests: 0,
+              failedTests: 4,
+            },
+            caseResults: new Map([
               [
                 1,
                 [
                   { state: "failed", valid: false },
                   { state: "failed", valid: false },
                   { state: "successful", valid: false },
                 ],
```

### Comparing `bowtie_json_schema-2024.3.8/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2024.3.9/frontend/src/data/parseReportData.ts`

 * *Files 5% similar despite different names*

```diff
@@ -67,20 +67,21 @@
   lines: Record<string, unknown>[],
 ): ReportData => {
   const runMetadata = RunMetadata.fromRecord(lines[0] as unknown as Header);
 
   const implementationsResultsMap = new Map<string, ImplementationResults>();
   for (const id of runMetadata.implementations.keys()) {
     implementationsResultsMap.set(id, {
-      id,
-      cases: new Map(),
-      erroredCases: 0,
-      skippedTests: 0,
-      failedTests: 0,
-      erroredTests: 0,
+      caseResults: new Map(),
+      totals: {
+        erroredCases: 0,
+        skippedTests: 0,
+        failedTests: 0,
+        erroredTests: 0,
+      },
     });
   }
 
   const caseMap = new Map<number, Case>();
   let didFailFast = false;
   for (const line of lines) {
     if (line.case) {
@@ -90,67 +91,67 @@
       const implementationResults = implementationsResultsMap.get(
         line.implementation as string,
       )!;
       if (line.caught !== undefined) {
         const context = line.context as Record<string, unknown>;
         const errorMessage: string = (context?.message ??
           context?.stderr) as string;
-        implementationResults.erroredCases++;
-        implementationResults.erroredTests += caseData.tests.length;
-        implementationResults.cases.set(
+        implementationResults.totals.erroredCases!++;
+        implementationResults.totals.erroredTests! += caseData.tests.length;
+        implementationResults.caseResults.set(
           line.seq as number,
           new Array<CaseResult>(caseData.tests.length).fill({
             state: "errored",
             message: errorMessage,
           }),
         );
       } else if (line.skipped) {
-        implementationResults.skippedTests += caseData.tests.length;
-        implementationResults.cases.set(
+        implementationResults.totals.skippedTests! += caseData.tests.length;
+        implementationResults.caseResults.set(
           line.seq as number,
           new Array<CaseResult>(caseData.tests.length).fill({
             state: "skipped",
             message: line.message as string,
           }),
         );
       } else if (line.implementation) {
         const caseResults: CaseResult[] = (
           line.results as Record<string, unknown>[]
         ).map((res, idx) => {
           if (res.errored) {
             const context = res.context as Record<string, unknown>;
             const errorMessage = context?.message ?? context?.stderr;
-            implementationResults.erroredTests++;
+            implementationResults.totals.erroredTests!++;
             return {
               state: "errored",
               message: errorMessage as string | undefined,
             };
           } else if (res.skipped) {
-            implementationResults.skippedTests++;
+            implementationResults.totals.skippedTests!++;
             return {
               state: "skipped",
               message: res.message as string | undefined,
             };
           } else {
             const successful = res.valid === caseData.tests[idx].valid;
             if (successful) {
               return {
                 state: "successful",
                 valid: res.valid as boolean | undefined,
               };
             } else {
-              implementationResults.failedTests++;
+              implementationResults.totals.failedTests!++;
               return {
                 state: "failed",
                 valid: res.valid as boolean | undefined,
               };
             }
           }
         });
-        implementationResults.cases.set(line.seq as number, caseResults);
+        implementationResults.caseResults.set(line.seq as number, caseResults);
       } else if (line.did_fail_fast !== undefined) {
         didFailFast = line.did_fail_fast as boolean;
       }
     }
   }
 
   return {
@@ -170,74 +171,82 @@
   data: ImplementationData,
 ): Implementation =>
   ({
     ...data,
     dialects: data.dialects.map((uri) => Dialect.forURI(uri)),
   }) as Implementation;
 
-export const parseImplementationData = (
-  loaderData: Record<string, ReportData>,
+/**
+ * Prepare a summarized implementation report for the
+ * passed implementation using all the dialect reports data
+ * that was fetched.
+ */
+export const prepareImplementationReport = (
+  allReportsData: Map<Dialect, ReportData>,
+  langImplementation: string,
 ) => {
-  const allImplementations: Record<string, ImplementationDialectCompliance> =
-    {};
-  const dialectCompliance: Record<string, Record<string, Partial<Totals>>> = {};
+  let implementationReport: ImplementationReport | null = null;
+  const dialectCompliance = new Map<Dialect, Partial<Totals>>();
+
+  // FIXME: This magic prefix is duplicated from the backend side,
+  //        and probably we can separate handling this in Implementation
+  //        class (when we have it).
+  const image = `ghcr.io/bowtie-json-schema/${langImplementation}`;
 
   for (const [
     dialect,
     { implementationsResults, runMetadata },
-  ] of Object.entries(loaderData)) {
-    dialectCompliance[dialect] = calculateImplementationTotal(
-      implementationsResults,
-    );
-
-    for (const [id, implementation] of runMetadata.implementations.entries()) {
-      if (!allImplementations[id]) {
-        allImplementations[id] = {
+  ] of allReportsData.entries()) {
+    const implementationResults = implementationsResults.get(image);
+
+    if (implementationResults) {
+      dialectCompliance.set(dialect, {
+        erroredTests: implementationResults.totals.erroredTests,
+        skippedTests: implementationResults.totals.skippedTests,
+        failedTests: implementationResults.totals.failedTests,
+      });
+
+      const implementation = runMetadata.implementations.get(image)!;
+
+      if (!implementationReport) {
+        implementationReport = {
           implementation,
-          dialectCompliance: {},
+          dialectCompliance,
+        };
+      } else {
+        implementationReport = {
+          implementation: Object.assign(
+            {},
+            implementationReport.implementation,
+            implementation,
+          ),
+          dialectCompliance: new Map([
+            ...implementationReport.dialectCompliance,
+            ...dialectCompliance,
+          ]),
         };
-      }
-      if (dialectCompliance[dialect][id]) {
-        allImplementations[id].dialectCompliance[dialect] =
-          dialectCompliance[dialect][id];
       }
     }
   }
 
-  return allImplementations;
-};
-
-const calculateImplementationTotal = (
-  implementationsResults: Map<string, ImplementationResults>,
-) => {
-  const implementationResult: Record<string, Partial<Totals>> = {};
-
-  Array.from(implementationsResults.entries()).forEach(([key, value]) => {
-    implementationResult[key] = {
-      erroredTests: value.erroredTests,
-      skippedTests: value.skippedTests,
-      failedTests: value.failedTests,
-    };
-  });
-
-  return implementationResult;
+  return implementationReport;
 };
 
 export const calculateTotals = (data: ReportData): Totals => {
   const totalTests = Array.from(data.cases.values()).reduce(
     (prev, curr) => prev + curr.tests.length,
     0,
   );
   return Array.from(data.implementationsResults.values()).reduce(
     (prev, curr) => ({
       totalTests,
-      erroredCases: prev.erroredCases + curr.erroredCases,
-      skippedTests: prev.skippedTests + curr.skippedTests,
-      failedTests: prev.failedTests + curr.failedTests,
-      erroredTests: prev.erroredTests + curr.erroredTests,
+      erroredCases: prev.erroredCases + curr.totals.erroredCases!,
+      skippedTests: prev.skippedTests + curr.totals.skippedTests!,
+      failedTests: prev.failedTests + curr.totals.failedTests!,
+      erroredTests: prev.erroredTests + curr.totals.erroredTests!,
     }),
     {
       totalTests: totalTests,
       erroredCases: 0,
       skippedTests: 0,
       failedTests: 0,
       erroredTests: 0,
@@ -269,20 +278,16 @@
   runMetadata: RunMetadata;
   cases: Map<number, Case>;
   implementationsResults: Map<string, ImplementationResults>;
   didFailFast: boolean;
 }
 
 export interface ImplementationResults {
-  id: string;
-  cases: Map<number, CaseResult[]>;
-  erroredCases: number;
-  skippedTests: number;
-  failedTests: number;
-  erroredTests: number;
+  caseResults: Map<number, CaseResult[]>;
+  totals: Partial<Totals>;
 }
 
 export interface CaseResult {
   state: "successful" | "failed" | "skipped" | "errored";
   valid?: boolean;
   message?: string;
 }
@@ -304,17 +309,17 @@
   os?: string;
   os_version?: string;
   language_version?: string;
 
   [k: string]: unknown;
 }
 
-export interface ImplementationDialectCompliance {
+export interface ImplementationReport {
   implementation: Implementation;
-  dialectCompliance: Record<string, Partial<Totals>>;
+  dialectCompliance: Map<Dialect, Partial<Totals>>;
 }
 
 export interface Case {
   description: string;
   comment?: string;
   schema: Record<string, unknown> | boolean;
   registry?: Record<string, unknown>;
```

### Comparing `bowtie_json_schema-2024.3.8/implementations/.java-implementations-pmd-ruleset.xml` & `bowtie_json_schema-2024.3.9/implementations/.java-implementations-pmd-ruleset.xml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/clojure-json-schema/Dockerfile` & `bowtie_json_schema-2024.3.9/implementations/clojure-json-schema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj` & `bowtie_json_schema-2024.3.9/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/cpp-valijson/bowtie_valijson.cpp` & `bowtie_json_schema-2024.3.9/implementations/cpp-valijson/bowtie_valijson.cpp`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/dotnet-jsonschema-net/.gitignore` & `bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/dotnet-jsonschema-net/Program.cs` & `bowtie_json_schema-2024.3.9/implementations/dotnet-jsonschema-net/Program.cs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/go-gojsonschema/bowtie_gojsonschema.go` & `bowtie_json_schema-2024.3.9/implementations/go-gojsonschema/bowtie_gojsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/go-gojsonschema/go.sum` & `bowtie_json_schema-2024.3.9/implementations/go-gojsonschema/go.sum`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/go-jsonschema/bowtie_jsonschema.go` & `bowtie_json_schema-2024.3.9/implementations/go-jsonschema/bowtie_jsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-json-schema/BowtieJsonSchema.java` & `bowtie_json_schema-2024.3.9/implementations/java-json-schema/BowtieJsonSchema.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-json-schema/build.gradle` & `bowtie_json_schema-2024.3.9/implementations/java-json-schema/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.3.9/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.3.9/implementations/java-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java` & `bowtie_json_schema-2024.3.9/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-jsonschemafriend/build.gradle` & `bowtie_json_schema-2024.3.9/implementations/java-jsonschemafriend/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/build.gradle.kts` & `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/justfile` & `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/justfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/gradle/libs.versions.toml` & `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/gradle/libs.versions.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt` & `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/Support.kt` & `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/Support.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt` & `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt` & `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt` & `bowtie_json_schema-2024.3.9/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/js-ajv/bowtie_ajv.js` & `bowtie_json_schema-2024.3.9/implementations/js-ajv/bowtie_ajv.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/js-ajv/package-lock.json` & `bowtie_json_schema-2024.3.9/implementations/js-ajv/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/js-hyperjump/bowtie_hyperjump.js` & `bowtie_json_schema-2024.3.9/implementations/js-hyperjump/bowtie_hyperjump.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/js-jsonschema/bowtie_jsonschema.js` & `bowtie_json_schema-2024.3.9/implementations/js-jsonschema/bowtie_jsonschema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts` & `bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt` & `bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt` & `bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt` & `bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt` & `bowtie_json_schema-2024.3.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/lua-jsonschema/Dockerfile` & `bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/lua-jsonschema/bowtie_jsonschema.lua` & `bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/bowtie_jsonschema.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/lua-jsonschema/json.lua` & `bowtie_json_schema-2024.3.9/implementations/lua-jsonschema/json.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/php-opis-json-schema/bowtieJsonSchema.php` & `bowtie_json_schema-2024.3.9/implementations/php-opis-json-schema/bowtieJsonSchema.php`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/python-fastjsonschema/bowtie_fastjsonschema.py` & `bowtie_json_schema-2024.3.9/implementations/python-fastjsonschema/bowtie_fastjsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/python-jschon/bowtie_jschon.py` & `bowtie_json_schema-2024.3.9/implementations/python-jschon/bowtie_jschon.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/python-jsonschema/bowtie_jsonschema.py` & `bowtie_json_schema-2024.3.9/implementations/python-jsonschema/bowtie_jsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/ruby-json_schemer/bowtie_json_schemer.rb` & `bowtie_json_schema-2024.3.9/implementations/ruby-json_schemer/bowtie_json_schemer.rb`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/rust-boon/Cargo.lock` & `bowtie_json_schema-2024.3.9/implementations/rust-boon/Cargo.lock`

 * *Files 15% similar despite different names*

```diff
@@ -62,14 +62,16 @@
 
 [[package]]
 name = "bowtie-rust-boon"
 version = "0.1.0"
 dependencies = [
  "boon",
  "cargo-lock",
+ "os_info",
+ "rustc_version_runtime",
  "serde_json",
 ]
 
 [[package]]
 name = "cargo-lock"
 version = "9.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -161,26 +163,43 @@
 [[package]]
 name = "libc"
 version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
+name = "log"
+version = "0.4.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
+
+[[package]]
 name = "memchr"
 version = "2.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
 
 [[package]]
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
+name = "os_info"
+version = "3.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae99c7fa6dd38c7cafe1ec085e804f8f555a2f8659b0dbe03f1f9963a9b51092"
+dependencies = [
+ "log",
+ "serde",
+ "windows-sys",
+]
+
+[[package]]
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
 name = "proc-macro2"
@@ -226,14 +245,33 @@
 [[package]]
 name = "regex-syntax"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
+name = "rustc_version"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
+dependencies = [
+ "semver",
+]
+
+[[package]]
+name = "rustc_version_runtime"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2dd18cd2bae1820af0b6ad5e54f4a51d0f3fcc53b05f845675074efcc7af071d"
+dependencies = [
+ "rustc_version",
+ "semver",
+]
+
+[[package]]
 name = "ryu"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b4b9743ed687d4b4bcedf9ff5eaa7398495ae14e61cba0a295704edbc7decde"
 
 [[package]]
 name = "semver"
@@ -262,17 +300,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -385,14 +423,80 @@
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+dependencies = [
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
+]
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+
+[[package]]
 name = "winnow"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
 dependencies = [
  "memchr",
 ]
```

### Comparing `bowtie_json_schema-2024.3.8/implementations/rust-boon/Dockerfile` & `bowtie_json_schema-2024.3.9/implementations/rust-boon/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/rust-boon/src/main.rs` & `bowtie_json_schema-2024.3.9/implementations/rust-boon/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/rust-jsonschema/Cargo.lock` & `bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -957,17 +957,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
```

### Comparing `bowtie_json_schema-2024.3.8/implementations/rust-jsonschema/Dockerfile` & `bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/rust-jsonschema/src/main.rs` & `bowtie_json_schema-2024.3.9/implementations/rust-jsonschema/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/scala-mjs-validator/Harness.scala` & `bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/scala-mjs-validator/build.sbt` & `bowtie_json_schema-2024.3.9/implementations/scala-mjs-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/scala-rc-circe-json-validator/Harness.scala` & `bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/scala-rc-circe-json-validator/build.sbt` & `bowtie_json_schema-2024.3.9/implementations/scala-rc-circe-json-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts` & `bowtie_json_schema-2024.3.9/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/test_cli.py` & `bowtie_json_schema-2024.3.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/test_github.py` & `bowtie_json_schema-2024.3.9/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/test_hypothesis.py` & `bowtie_json_schema-2024.3.9/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/test_integration.py` & `bowtie_json_schema-2024.3.9/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/test_report.py` & `bowtie_json_schema-2024.3.9/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/test_schemas.py` & `bowtie_json_schema-2024.3.9/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2024.3.9/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/io/v1.json` & `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json` & `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json` & `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json` & `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/models/group.json` & `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json` & `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/tests/fauxmplementations/lintsonschema/schemas/models/test.json` & `bowtie_json_schema-2024.3.9/tests/fauxmplementations/lintsonschema/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/.gitignore` & `bowtie_json_schema-2024.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/LICENSE` & `bowtie_json_schema-2024.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/README.rst` & `bowtie_json_schema-2024.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/hatch_build.py` & `bowtie_json_schema-2024.3.9/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/pyproject.toml` & `bowtie_json_schema-2024.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.3.8/PKG-INFO` & `bowtie_json_schema-2024.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bowtie-json-schema
-Version: 2024.3.8
+Version: 2024.3.9
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://docs.bowtie.report/
 Project-URL: Homepage, https://bowtie.report/
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author-email: Julian Berman <Julian+bowtie@GrayVines.com>
```


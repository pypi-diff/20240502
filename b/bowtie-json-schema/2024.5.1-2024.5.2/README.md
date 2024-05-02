# Comparing `tmp/bowtie_json_schema-2024.5.1.tar.gz` & `tmp/bowtie_json_schema-2024.5.2.tar.gz`

## Comparing `bowtie_json_schema-2024.5.1.tar` & `bowtie_json_schema-2024.5.2.tar`

### file list

```diff
@@ -1,248 +1,249 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/.gitpod.Dockerfile
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/.gitpod.yml
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/.prettierrc.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/.readthedocs.yaml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/action.yml
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/noxfile.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/requirements.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/test-requirements.in
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/test-requirements.txt
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/.devcontainer/devcontainer.json
--rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/.pre-commit-hooks/check-dependabot
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/.pre-commit-hooks/check-lintsonschema-schema
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/__main__.py
--rw-r--r--   0        0        0    49352 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/_cli.py
--rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/_commands.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/_containers.py
--rw-r--r--   0        0        0    22310 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/_core.py
--rw-r--r--   0        0        0    11276 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/_report.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/_suite.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/exceptions.py
--rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/hypothesis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/py.typed
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/report.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/cli/info.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/cli/smoke.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/cli/summary.json
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/models/dialect.json
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/bowtie/schemas/models/test.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/data/dialects.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/Makefile
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/cli.rst
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/conf.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/contributing.rst
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/github-actions.rst
--rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/implementers.rst
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/index.rst
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/motd.txt
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/requirements.in
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/requirements.txt
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/_static/bowtie_diagram_dark.svg
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/_static/bowtie_diagram_light.svg
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/docs/_static/logo.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/index.html
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/package.json
--rw-r--r--   0        0        0   163410 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/tsconfig.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/vite.config.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/public/favicon.svg
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/DialectReportView.tsx
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/MainContainer.tsx
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/ReportDataHandler.tsx
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/global.css
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/index.tsx
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/assets/landscape-logo.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/CopyToClipboard.tsx
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/FilterSection.css
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/FilterSection.tsx
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/LoadingAnimation.tsx
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/NavBar.tsx
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/OtherImplementations.tsx
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/Cases/CaseItem.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/Cases/CaseResultSvg.test.tsx
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/Cases/CaseResultSvg.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/Cases/CasesSection.tsx
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/Cases/SchemaDisplay.tsx
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/DragAndDrop/DragAndDrop.tsx
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/Modals/DetailsButtonModal.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/RunInfo/RunInfoSection.tsx
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/Summary/ImplementationRow.tsx
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/Summary/SummarySection.tsx
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/components/Summary/SummaryTable.tsx
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/context/BowtieVersionContext.tsx
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/context/ThemeContext.tsx
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/data/Badge.test.ts
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/data/Badge.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/data/Dialect.test.ts
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/data/Dialect.ts
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/data/Site.test.ts
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/data/Site.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/data/mapLanguage.ts
--rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/data/parseReportData.test.ts
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/frontend/src/hooks/useSearchParams.ts
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/.java-implementations-pmd-ruleset.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/clojure-json-schema/Dockerfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/clojure-json-schema/project.clj
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/cpp-valijson/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/cpp-valijson/.gitignore
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/cpp-valijson/Dockerfile
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/cpp-valijson/bowtie_valijson.cpp
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/cpp-valijson/compile_flags.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/dotnet-jsonschema-net/.clang-format
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/dotnet-jsonschema-net/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/dotnet-jsonschema-net/Dockerfile
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/dotnet-jsonschema-net/Program.cs
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/go-gojsonschema/Dockerfile
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/go-gojsonschema/bowtie_gojsonschema.go
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/go-gojsonschema/go.mod
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/go-gojsonschema/go.sum
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/go-jsonschema/Dockerfile
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/go-jsonschema/bowtie_jsonschema.go
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/go-jsonschema/go.mod
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/go-jsonschema/go.sum
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-json-schema/BowtieJsonSchema.java
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-json-schema/Dockerfile
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-json-schema/build.gradle
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-json-schema-validator/build.gradle
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-jsonschemafriend/Dockerfile
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-jsonschemafriend/build.gradle
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/.dockerignore
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/.editorconfig
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/Dockerfile
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/build.gradle.kts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/gradle.properties
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/justfile
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/settings.gradle.kts
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/gradle/libs.versions.toml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/js-ajv/Dockerfile
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/js-ajv/bowtie_ajv.js
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/js-ajv/package-lock.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/js-ajv/package.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/js-hyperjump/Dockerfile
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/js-hyperjump/bowtie_hyperjump.js
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/js-hyperjump/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/js-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/js-jsonschema/bowtie_jsonschema.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/js-jsonschema/package.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/.gitignore
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/lua-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/lua-jsonschema/bowtie_jsonschema.lua
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/lua-jsonschema/json.lua
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/lua-jsonschema/stylua.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/php-opis-json-schema/Dockerfile
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/php-opis-json-schema/bowtieJsonSchema.php
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/php-opis-json-schema/composer.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/python-fastjsonschema/Dockerfile
--rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/python-jschon/Dockerfile
--rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/python-jschon/bowtie_jschon.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/python-jsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/python-jsonschema/bowtie_jsonschema.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/ruby-json_schemer/.rubocop.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/ruby-json_schemer/Dockerfile
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/ruby-json_schemer/Gemfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/ruby-json_schemer/Gemfile.lock
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/ruby-json_schemer/bowtie_json_schemer.rb
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/rust-boon/Cargo.lock
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/rust-boon/Cargo.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/rust-boon/Dockerfile
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/rust-boon/build.rs
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/rust-boon/src/main.rs
--rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/rust-jsonschema/Cargo.lock
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/rust-jsonschema/Cargo.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/rust-jsonschema/Dockerfile
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/rust-jsonschema/build.rs
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/rust-jsonschema/src/main.rs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/scala-mjs-validator/Dockerfile
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/scala-mjs-validator/Harness.scala
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/scala-mjs-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/scala-mjs-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/scala-mjs-validator/project/plugins.sbt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/scala-rc-circe-json-validator/Dockerfile
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/scala-rc-circe-json-validator/Harness.scala
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/scala-rc-circe-json-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/scala-rc-circe-json-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/scala-rc-circe-json-validator/project/plugins.sbt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/ts-vscode-json-languageservice/Dockerfile
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/ts-vscode-json-languageservice/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/implementations/ts-vscode-json-languageservice/tsconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/conftest.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/test_cli.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/test_dialect.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/test_github.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/test_hypothesis.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/test_implementation.py
--rw-r--r--   0        0        0    65081 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/test_integration.py
--rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/test_report.py
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/test_schemas.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/report.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/models/test.json
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/LICENSE
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/README.rst
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/hatch_build.py
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/pyproject.toml
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.1/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/.gitpod.yml
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/.prettierrc.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/action.yml
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/noxfile.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/requirements.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/test-requirements.in
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/test-requirements.txt
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/.pre-commit-hooks/check-dependabot
+-rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/.pre-commit-hooks/check-lintsonschema-schema
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/__main__.py
+-rw-r--r--   0        0        0    49047 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/_cli.py
+-rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/_commands.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/_containers.py
+-rw-r--r--   0        0        0    22576 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/_core.py
+-rw-r--r--   0        0        0    11276 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/_report.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/_suite.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/exceptions.py
+-rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/hypothesis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/py.typed
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/report.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/cli/info.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/bowtie/schemas/models/test.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/data/dialects.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/Makefile
+-rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/cli.rst
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/conf.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/contributing.rst
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/github-actions.rst
+-rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/implementers.rst
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/index.rst
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/motd.txt
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/requirements.in
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/requirements.txt
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/_static/bowtie_diagram_dark.svg
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/_static/bowtie_diagram_light.svg
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/docs/_static/logo.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/index.html
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/package.json
+-rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/tsconfig.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/vite.config.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/public/favicon.svg
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/DialectReportView.tsx
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/MainContainer.tsx
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/ReportDataHandler.tsx
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/global.css
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/index.tsx
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/assets/landscape-logo.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/CopyToClipboard.tsx
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/FilterSection.css
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/FilterSection.tsx
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/LoadingAnimation.tsx
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/NavBar.tsx
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/OtherImplementations.tsx
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/Cases/CaseItem.tsx
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/Cases/CaseResultSvg.test.tsx
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/Cases/CaseResultSvg.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/Cases/CasesSection.tsx
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/Cases/SchemaDisplay.tsx
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/DragAndDrop/DragAndDrop.tsx
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/ImplementationReportView/EmbedBadges.css
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/Modals/DetailsButtonModal.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/RunInfo/RunInfoSection.tsx
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/Summary/ImplementationRow.tsx
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/Summary/SummarySection.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/components/Summary/SummaryTable.tsx
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/context/BowtieVersionContext.tsx
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/context/ThemeContext.tsx
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/data/Badge.test.ts
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/data/Badge.ts
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/data/Dialect.test.ts
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/data/Dialect.ts
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/data/Site.test.ts
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/data/Site.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/data/mapLanguage.ts
+-rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/data/parseReportData.test.ts
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/frontend/src/hooks/useSearchParams.ts
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/.java-implementations-pmd-ruleset.xml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/clojure-json-schema/Dockerfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/clojure-json-schema/project.clj
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/cpp-valijson/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/cpp-valijson/.gitignore
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/cpp-valijson/Dockerfile
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/cpp-valijson/bowtie_valijson.cpp
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/cpp-valijson/compile_flags.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/dotnet-jsonschema-net/.clang-format
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/dotnet-jsonschema-net/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/dotnet-jsonschema-net/Dockerfile
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/dotnet-jsonschema-net/Program.cs
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/go-gojsonschema/Dockerfile
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/go-gojsonschema/bowtie_gojsonschema.go
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/go-gojsonschema/go.mod
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/go-gojsonschema/go.sum
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-json-schema/BowtieJsonSchema.java
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-json-schema/Dockerfile
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-json-schema/build.gradle
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-jsonschemafriend/Dockerfile
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-jsonschemafriend/build.gradle
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/.dockerignore
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/.editorconfig
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/Dockerfile
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/build.gradle.kts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/gradle.properties
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/justfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/settings.gradle.kts
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/gradle/libs.versions.toml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/js-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/js-jsonschema/bowtie_jsonschema.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/js-jsonschema/package.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/lua-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/lua-jsonschema/bowtie_jsonschema.lua
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/lua-jsonschema/stylua.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/php-opis-json-schema/Dockerfile
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/php-opis-json-schema/bowtieJsonSchema.php
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/php-opis-json-schema/composer.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/python-jschon/Dockerfile
+-rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/python-jschon/bowtie_jschon.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/python-jsonschema/bowtie_jsonschema.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/ruby-json_schemer/.rubocop.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/ruby-json_schemer/Dockerfile
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/ruby-json_schemer/Gemfile
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/ruby-json_schemer/Gemfile.lock
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/ruby-json_schemer/bowtie_json_schemer.rb
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/rust-boon/Cargo.lock
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/rust-boon/Cargo.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/rust-boon/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/rust-boon/build.rs
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/rust-boon/src/main.rs
+-rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/rust-jsonschema/build.rs
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/scala-mjs-validator/Dockerfile
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/scala-mjs-validator/Harness.scala
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/scala-mjs-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/scala-mjs-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/scala-mjs-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/scala-rc-circe-json-validator/Dockerfile
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/scala-rc-circe-json-validator/Harness.scala
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/scala-rc-circe-json-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/scala-rc-circe-json-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/scala-rc-circe-json-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/ts-vscode-json-languageservice/Dockerfile
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/ts-vscode-json-languageservice/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/implementations/ts-vscode-json-languageservice/tsconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/conftest.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/test_cli.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/test_dialect.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/test_github.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/test_hypothesis.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/test_implementation.py
+-rw-r--r--   0        0        0    65083 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/test_integration.py
+-rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/test_report.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/test_schemas.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/report.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/models/test.json
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/LICENSE
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/README.rst
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/hatch_build.py
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.2/PKG-INFO
```

### Comparing `bowtie_json_schema-2024.5.1/.gitpod.yml` & `bowtie_json_schema-2024.5.2/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/.pre-commit-config.yaml` & `bowtie_json_schema-2024.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/CONTRIBUTING.rst` & `bowtie_json_schema-2024.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/action.yml` & `bowtie_json_schema-2024.5.2/action.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/noxfile.py` & `bowtie_json_schema-2024.5.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/requirements.txt` & `bowtie_json_schema-2024.5.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/test-requirements.txt` & `bowtie_json_schema-2024.5.2/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/.pre-commit-hooks/check-dependabot` & `bowtie_json_schema-2024.5.2/.pre-commit-hooks/check-dependabot`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/.pre-commit-hooks/check-lintsonschema-schema` & `bowtie_json_schema-2024.5.2/.pre-commit-hooks/check-lintsonschema-schema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/_cli.py` & `bowtie_json_schema-2024.5.2/bowtie/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable
 from contextlib import AsyncExitStack, asynccontextmanager
 from fnmatch import fnmatch
-from functools import cache, wraps
-from importlib.resources import files
+from functools import wraps
 from pathlib import Path
 from pprint import pformat
 from textwrap import dedent
 from typing import TYPE_CHECKING, Literal, ParamSpec, Protocol
 import asyncio
 import json
 import logging
@@ -19,36 +18,35 @@
 from attrs import asdict
 from click.shell_completion import CompletionItem
 from diagnostic import DiagnosticError
 from jsonschema_lexer import JSONSchemaLexer
 from pygments.lexers.data import (  # type: ignore[reportMissingTypeStubs]
     JsonLexer,
 )
-from referencing.jsonschema import EMPTY_REGISTRY
 from rich import box, console, panel
 from rich.syntax import Syntax
 from rich.table import Column, Table
 from rich.text import Text
 from rich_click.utils import CommandGroupDict, OptionGroupDict
 from url import URL, RelativeURLWithoutBase
-import referencing_loaders
 import rich_click as click
 import structlog
 import structlog.typing
 
 from bowtie import _containers, _report, _suite
 from bowtie._commands import SeqCase, Unsuccessful
 from bowtie._core import (
     Dialect,
     Example,
     Implementation,
     NoSuchImplementation,
     StartupFailed,
     Test,
     TestCase,
+    bowtie_schemas_registry,
 )
 from bowtie.exceptions import DialectError, ProtocolError, UnsupportedDialect
 
 if TYPE_CHECKING:
     from collections.abc import (
         AsyncIterator,
         Awaitable,
@@ -56,15 +54,15 @@
         Sequence,
         Set,
     )
     from os import PathLike
     from typing import IO, Any, TextIO
 
     from click.decorators import FC
-    from referencing.jsonschema import Schema, SchemaRegistry, SchemaResource
+    from referencing.jsonschema import Schema, SchemaResource
 
     from bowtie._commands import AnyTestResult, ImplementationId
     from bowtie._core import DialectRunner, ImplementationInfo, MakeValidator
 
 
 # Windows fallbacks...
 _EX_CONFIG = getattr(os, "EX_CONFIG", 1)
@@ -739,20 +737,14 @@
         final_content += f"### {idx+1}. Schema:\n {row_data[0]}\n\n"
         final_content += "### Results:"
         final_content += row_data[1]
 
     return final_content
 
 
-@cache
-def bowtie_schemas_registry() -> SchemaRegistry:
-    resources = referencing_loaders.from_traversable(files("bowtie.schemas"))
-    return EMPTY_REGISTRY.with_resources(resources).crawl()
-
-
 def make_validator(*more_schemas: SchemaResource):
     from jsonschema.validators import (
         validator_for,  # type: ignore[reportUnknownVariableType]
     )
 
     registry = more_schemas @ bowtie_schemas_registry()
```

### Comparing `bowtie_json_schema-2024.5.1/bowtie/_commands.py` & `bowtie_json_schema-2024.5.2/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/_containers.py` & `bowtie_json_schema-2024.5.2/bowtie/_containers.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/_core.py` & `bowtie_json_schema-2024.5.2/bowtie/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,19 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Protocol, TypeVar, cast
 from uuid import uuid4
 import json
 
 from attrs import asdict, evolve, field, frozen, mutable
 from diagnostic import DiagnosticError
-from referencing.jsonschema import (
-    EMPTY_REGISTRY,
-    Schema,
-    SchemaRegistry,
-    specification_with,
-)
+from referencing.jsonschema import EMPTY_REGISTRY, Schema, specification_with
 from rich.panel import Panel
 from rpds import HashTrieMap
 from url import URL
+import referencing_loaders
 
 from bowtie._commands import (
     START_V1,
     STOP,
     CaseErrored,
     Dialect as DialectCommand,
     SeqCase,
@@ -40,15 +36,15 @@
         Mapping,
         Sequence,
         Set,
     )
     from typing import Any, Self
 
     from referencing import Specification
-    from referencing.jsonschema import SchemaResource
+    from referencing.jsonschema import SchemaRegistry, SchemaResource
     from rich.console import Console, ConsoleOptions, RenderResult
 
     from bowtie._commands import (
         AnyCaseResult,
         Command,
         ImplementationId,
         Message,
@@ -138,22 +134,25 @@
     def serializable(self):
         return str(self.uri)
 
     def specification(self, **kwargs: Any) -> Specification[SchemaResource]:
         return specification_with(str(self.uri), **kwargs)
 
     def current_dialect_resource(self) -> SchemaResource:
+        referrer = bowtie_schemas_registry().contents(
+            "tag:bowtie.report,2024:ihop:schemaInCurrentDialect",
+        )
+
         # it's of course unimportant what dialect is used for this referencing
         # schema, what matters is that the target dialect is applied
         from referencing.jsonschema import DRAFT202012
 
         return DRAFT202012.create_resource(
             {
-                # Should match the magic value for `schema` in `schemas/io/`
-                "$id": "tag:bowtie.report,2023:ihop:__dialect__",
+                "$id": referrer["$ref"],  # type: ignore[reportIndexIssue]
                 "$ref": str(self.uri),
             },
         )
 
 
 @frozen
 class NoSuchImplementation(Exception):
@@ -762,7 +761,13 @@
                 k: v
                 for k, v in test.items()
                 if k != "valid" and (k != "comment" or v is not None)
             }
             for test in serializable.pop("tests")
         ]
         return serializable
+
+
+@cache
+def bowtie_schemas_registry() -> SchemaRegistry:
+    resources = referencing_loaders.from_traversable(files("bowtie.schemas"))
+    return EMPTY_REGISTRY.with_resources(resources).crawl()
```

### Comparing `bowtie_json_schema-2024.5.1/bowtie/_report.py` & `bowtie_json_schema-2024.5.2/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/_suite.py` & `bowtie_json_schema-2024.5.2/bowtie/_suite.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/exceptions.py` & `bowtie_json_schema-2024.5.2/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/hypothesis.py` & `bowtie_json_schema-2024.5.2/bowtie/hypothesis.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,37 +28,44 @@
     text,
     tuples,
     uuids,
 )
 from url import URL
 
 from bowtie import _commands
-from bowtie._cli import bowtie_schemas_registry
-from bowtie._core import Dialect, Example, ImplementationInfo, Test, TestCase
+from bowtie._core import (
+    Dialect,
+    Example,
+    ImplementationInfo,
+    Test,
+    TestCase,
+    bowtie_schemas_registry,
+)
 from bowtie._report import Report, RunMetadata
 
 
 def pattern_from(id):
     """
     Return a strategy which matches the pattern in the given schema.
     """
     return from_regex(bowtie_schemas_registry().contents(id)["pattern"])
 
 
 # FIXME: probably via hypothesis-jsonschema
-schemas = booleans() | dictionaries(
+object_schemas = dictionaries(
     keys=text(),
     values=recursive(
         none() | booleans() | floats() | text(printable),
         lambda children: lists(children)
         | dictionaries(text(printable), children),
         max_leaves=3,
     ),
     max_size=5,
 )
+schemas = booleans() | object_schemas
 
 seqs = uuids().map(lambda uuid: uuid.hex)
 implementation_names = pattern_from(
     "tag:bowtie.report,2024:models:implementation:name",
 )
 languages = pattern_from(
     "tag:bowtie.report,2024:models:implementation:language",
@@ -89,30 +96,30 @@
 known_dialects = sampled_from(sorted(Dialect.known()))
 
 
 @composite
 def implementation_infos(
     draw,
     names=implementation_names,
-    dialects=dialects(),
+    dialects=frozensets(known_dialects, min_size=1, max_size=4),
     languages=languages,
 ):
     """
     Generate an implementation (info).
     """
     name = draw(names)
     language = draw(languages)
     return ImplementationInfo(
         image=f"bowtie-hypothesis-generated/{language}/{name}",
         name=name,
         language=language,
         homepage=draw(urls().map(URL.parse)),
         issues=draw(urls().map(URL.parse)),
         source=draw(urls().map(URL.parse)),
-        dialects=draw(frozensets(dialects, min_size=1, max_size=4)),
+        dialects=draw(dialects),
     )
 
 
 def implementations(
     infos=implementation_infos(),
     min_size=1,
     max_size=5,
@@ -160,24 +167,24 @@
         valid=valid,
         comment=comment,
     )
 
 
 def test_cases(
     description=text(),
-    schema=schemas,
+    schemas=schemas,
     tests=lists(examples() | tests(), min_size=1, max_size=8),
 ):
     r"""
     Generate `TestCase`\ s.
     """
     return builds(
         TestCase,
         description=description,
-        schema=schema,
+        schema=schemas,
         tests=tests,
     )
 
 
 successful_tests = sampled_from(
     [
         _commands.TestResult.VALID,
@@ -257,14 +264,19 @@
             implementation=implementations,
             expected=lists(booleans() | none(), min_size=size, max_size=size),
             result=any_case_results(min_tests=size, max_tests=size),
         ),
     )
 
 
+# Evade the s h a d o w
+_implementations = implementations
+_test_cases = test_cases
+
+
 @composite
 def cases_and_results(
     draw,
     implementations=implementations(),
     responding=None,
     seqs=seqs,
     test_cases=test_cases(),
@@ -292,78 +304,70 @@
     seq_cases = draw(strategy)
 
     return seq_cases, [
         draw(
             seq_results(
                 seqs=just(seq_case.seq),
                 implementations=just(implementation.id),
+                min_tests=len(seq_case.case.tests),
+                max_tests=len(seq_case.case.tests),
             ),
         )
         for seq_case in seq_cases
         for implementation in draw(responding(seq_case))
     ]
 
 
-# Evade the s h a d o w
-_implementations = implementations
 _cases_and_results = cases_and_results
 
 
-def run_metadata(dialects=dialects(), implementations=None):
+@composite
+def run_metadata(draw, dialects=known_dialects, implementations=None):
     """
     Generate just a report's metadata.
     """
+    dialect = draw(dialects)
     if implementations is None:
-        implementations = _implementations(
-            infos=implementation_infos(dialects=dialects),
-        )
-    return builds(
-        RunMetadata,
-        dialect=dialects,
-        implementations=implementations,
-    )
-
-
-_run_metadata = run_metadata
+        with_dialect = frozensets(
+            dialects,
+            max_size=4,
+        ).map(lambda v: v | {dialect})
+        infos = implementation_infos(dialects=with_dialect)
+        implementations = _implementations(infos=infos)
+    return RunMetadata(dialect=dialect, implementations=draw(implementations))
 
 
 @composite
 def report_data(
     draw,
-    dialects=known_dialects,
-    implementations=None,
-    run_metadata=None,
+    run_metadata=run_metadata(),
     cases_and_results=None,
     fail_fast=booleans(),
 ):
     """
     Generate Bowtie report data (suitable for `Report.from_input`).
     """
-    if implementations is None:
-        if cases_and_results is not None:
-            raise ValueError(
-                "Providing cases+results without implementations can lead to "
-                "inconsistent reports.",
-            )
-        infos = implementation_infos(dialects=dialects)
-        implementations = _implementations(infos=infos)
-    impls = draw(implementations)
+    metadata = draw(run_metadata)
 
     if cases_and_results is None:
-        cases_and_results = _cases_and_results(implementations=just(impls))
+        cases = test_cases(
+            schemas=(
+                schemas
+                if metadata.dialect.has_boolean_schemas
+                else object_schemas
+            ),
+        )
+        cases_and_results = _cases_and_results(
+            test_cases=cases,
+            implementations=just(metadata.implementations),
+        )
 
     seq_cases, results = draw(cases_and_results)
-
-    if run_metadata is None:
-        run_metadata = _run_metadata(
-            dialects=dialects,
-            implementations=just(impls),
-        )
     return [  # FIXME: Combine with the logic in CaseReporter
-        draw(run_metadata).serializable(),
+        metadata.serializable(),
         *[seq_case.serializable() for seq_case in seq_cases],
         *[result.serializable() for result in results],
         {"did_fail_fast": draw(fail_fast)},
     ]
 
 
 def reports(**kwargs):
```

### Comparing `bowtie_json_schema-2024.5.1/bowtie/schemas/cli/info.json` & `bowtie_json_schema-2024.5.2/bowtie/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/schemas/cli/summary.json` & `bowtie_json_schema-2024.5.2/bowtie/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/schemas/io/v1.json` & `bowtie_json_schema-2024.5.2/bowtie/schemas/io/v1.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999652777777778%*

 * *Differences: {"'$defs'": "{'case': {'properties': {'schema': {'$id': "*

 * *            "'tag:bowtie.report,2024:ihop:schemaInCurrentDialect'}}}}"}*

```diff
@@ -18,14 +18,15 @@
                     "propertyNames": {
                         "format": "uri"
                     },
                     "type": "object"
                 },
                 "schema": {
                     "$comment": "the URI used here is a sort of 'magic' URI set by Bowtie during runs, which will resolve to (effectively) the meta-schema for the current dialect being run by Bowtie. E.g. when running tests using the Draft 2020-12 dialect, the URI will resolve to the schema `{\"$ref\": \"https://json-schema.org/draft/2020-12/schema\"}`. This sort of dynamically set value is necessary, as schemas are supposed to be valid under the current dialect being spoken by Bowtie, but that's not known until runtime.",
+                    "$id": "tag:bowtie.report,2024:ihop:schemaInCurrentDialect",
                     "$ref": "tag:bowtie.report,2023:ihop:__dialect__",
                     "description": "A valid JSON Schema."
                 },
                 "tests": {
                     "description": "A set of related tests all using the same schema",
                     "items": {
                         "$ref": "tag:bowtie.report,2023:models:test"
```

### Comparing `bowtie_json_schema-2024.5.1/bowtie/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.5.2/bowtie/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/schemas/io/commands/run.json` & `bowtie_json_schema-2024.5.2/bowtie/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/schemas/io/commands/start.json` & `bowtie_json_schema-2024.5.2/bowtie/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/schemas/models/dialect.json` & `bowtie_json_schema-2024.5.2/bowtie/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/schemas/models/group.json` & `bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/io/v1.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2%*

 * *Differences: {"'$defs'": "OrderedDict([('version', OrderedDict([('description', 'The current version of this "*

 * *            "protocol, to be incremented if changed'), ('$anchor', 'version'), ('type', "*

 * *            "'integer'), ('const', 1)])), ('command', OrderedDict([('type', 'object'), "*

 * *            "('required', ['cmd']), ('unevaluatedProperties', False), ('oneOf', "*

 * *            "[OrderedDict([('$ref', 'tag:bowtie.report,2023:ihop:command:start')]), "*

 * *            "OrderedDict([('$ref', 'tag:bowtie.report,2023:ihop:com […]*

```diff
@@ -1,65 +1,77 @@
 {
-    "$id": "tag:bowtie.report,2023:models:group",
-    "$schema": "https://json-schema.org/draft/2020-12/schema",
-    "description": "A collection of related, runnable tests, either individually or themselves in subgroups. Groups are used only for organizing test input and reporting -- they are not sent to harnesses when actually running tests, as there's no need for the harness to have to deal with any grouping structure.",
-    "oneOf": [
-        {
-            "description": "a leaf test group (whose children are tests, and which therefore declares a schema for its children)",
+    "$defs": {
+        "case": {
+            "$anchor": "case",
+            "additionalProperties": false,
+            "description": "An individual test case, consisting of a single schema and one or more instances to validate under it",
             "properties": {
-                "children": {
+                "comment": {
+                    "description": "Any additional comments about the test case",
+                    "type": "string"
+                },
+                "description": {
+                    "description": "A (human-readable) short description of this test case",
+                    "type": "string"
+                },
+                "registry": {
+                    "description": "A collection of schemas (with URIs) which tests may reference (via $ref) and expect to be retrievable. They should be registered in whatever mechanism is expected by the implementation.",
+                    "propertyNames": {
+                        "format": "uri"
+                    },
+                    "type": "object"
+                },
+                "schema": {
+                    "$comment": "the URI used here is a sort of 'magic' URI set by Bowtie during runs, which will resolve to (effectively) the meta-schema for the current dialect being run by Bowtie. E.g. when running tests using the Draft 2020-12 dialect, the URI will resolve to the schema `{\"$ref\": \"https://json-schema.org/draft/2020-12/schema\"}`. This sort of dynamically set value is necessary, as schemas are supposed to be valid under the current dialect being spoken by Bowtie, but that's not known until runtime.",
+                    "$id": "tag:bowtie.report,2024:ihop:schemaInCurrentDialect",
+                    "$ref": "tag:bowtie.report,2023:ihop:__dialect__",
+                    "description": "A valid JSON Schema."
+                },
+                "tests": {
+                    "description": "A set of related tests all using the same schema",
                     "items": {
                         "$ref": "tag:bowtie.report,2023:models:test"
-                    }
+                    },
+                    "minItems": 1,
+                    "type": "array"
                 }
             },
             "required": [
-                "schema"
-            ]
+                "description",
+                "schema",
+                "tests"
+            ],
+            "type": "object"
         },
-        {
-            "description": "an outer test group (whose children are further test groups)",
-            "not": {
-                "required": [
-                    "schema"
-                ]
-            },
-            "properties": {
-                "children": {
-                    "items": {
-                        "$ref": "#"
-                    }
+        "command": {
+            "oneOf": [
+                {
+                    "$ref": "tag:bowtie.report,2023:ihop:command:start"
+                },
+                {
+                    "$ref": "tag:bowtie.report,2023:ihop:command:dialect"
+                },
+                {
+                    "$ref": "tag:bowtie.report,2023:ihop:command:run"
+                },
+                {
+                    "$ref": "tag:bowtie.report,2023:ihop:command:stop"
                 }
-            }
-        }
-    ],
-    "properties": {
-        "children": {
-            "description": "A set of related children of this test group",
-            "minItems": 1,
-            "type": "array"
-        },
-        "comment": {
-            "description": "Any additional comments about the test group",
-            "type": "string"
-        },
-        "description": {
-            "description": "A (human-readable) short description of this test group",
-            "type": "string"
-        },
-        "registry": {
-            "$ref": "tag:bowtie.report,2023:models:registry",
-            "description": "A schema registry to be made available for all tests in this group."
+            ],
+            "required": [
+                "cmd"
+            ],
+            "type": "object",
+            "unevaluatedProperties": false
         },
-        "schema": {
-            "$comment": "the URI used here is a sort of 'magic' URI set by Bowtie during runs, which will resolve to (effectively) the meta-schema for the current dialect being run by Bowtie. E.g. when running tests using the Draft 2020-12 dialect, the URI will resolve to the schema `{\"$ref\": \"https://json-schema.org/draft/2020-12/schema\"}`. This sort of dynamically set value is necessary, as schemas are supposed to be valid under the current dialect being spoken by Bowtie, but that's not known until runtime.",
-            "$ref": "tag:bowtie.report,2023:ihop:__dialect__",
-            "description": "A valid JSON Schema."
+        "version": {
+            "$anchor": "version",
+            "const": 1,
+            "description": "The current version of this protocol, to be incremented if changed",
+            "type": "integer"
         }
     },
-    "required": [
-        "description",
-        "children"
-    ],
-    "type": "object",
-    "unevaluatedProperties": false
+    "$id": "tag:bowtie.report,2023:ihop",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
+    "description": "Input/output specification for Bowtie, a meta-validator for JSON Schema validator implementations",
+    "title": "Bowtie IO Protocol"
 }
```

### Comparing `bowtie_json_schema-2024.5.1/bowtie/schemas/models/implementation.json` & `bowtie_json_schema-2024.5.2/bowtie/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/bowtie/schemas/models/test.json` & `bowtie_json_schema-2024.5.2/bowtie/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/data/dialects.json` & `bowtie_json_schema-2024.5.2/data/dialects.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/docs/Makefile` & `bowtie_json_schema-2024.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/docs/cli.rst` & `bowtie_json_schema-2024.5.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/docs/conf.py` & `bowtie_json_schema-2024.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/docs/contributing.rst` & `bowtie_json_schema-2024.5.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/docs/github-actions.rst` & `bowtie_json_schema-2024.5.2/docs/github-actions.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/docs/implementers.rst` & `bowtie_json_schema-2024.5.2/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/docs/index.rst` & `bowtie_json_schema-2024.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/docs/motd.txt` & `bowtie_json_schema-2024.5.2/docs/motd.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/docs/requirements.txt` & `bowtie_json_schema-2024.5.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/docs/_static/bowtie_diagram_dark.svg` & `bowtie_json_schema-2024.5.2/docs/_static/bowtie_diagram_dark.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/docs/_static/bowtie_diagram_light.svg` & `bowtie_json_schema-2024.5.2/docs/_static/bowtie_diagram_light.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/docs/_static/logo.svg` & `bowtie_json_schema-2024.5.2/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/package.json` & `bowtie_json_schema-2024.5.2/frontend/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947368421052631%*

 * *Differences: {"'devDependencies'": "{'@typescript-eslint/eslint-plugin': '^7.8.0', '@typescript-eslint/parser': "*

 * *                      "'^7.8.0', 'vite': '^5.2.11', 'vitest': '^1.5.3'}"}*

```diff
@@ -13,28 +13,28 @@
     "description": "The UI displays the outcomes generated by Bowtie, which serves as a meta-validator for the JSON Schema specification",
     "devDependencies": {
         "@types/react": "^18.3.1",
         "@types/react-dom": "^18.3.0",
         "@types/react-syntax-highlighter": "^15.5.11",
         "@types/react-test-renderer": "^18.3.0",
         "@types/urijs": "^1.19.25",
-        "@typescript-eslint/eslint-plugin": "^7.7.1",
-        "@typescript-eslint/parser": "^7.7.1",
+        "@typescript-eslint/eslint-plugin": "^7.8.0",
+        "@typescript-eslint/parser": "^7.8.0",
         "@vitejs/plugin-react": "^4.2.1",
         "eslint": "8.57.0",
         "eslint-plugin-react": "7.34.1",
         "eslint-plugin-react-hooks": "4.6.2",
         "jsdom": "^24.0.0",
         "react-test-renderer": "^18.3.1",
         "ts-loader": "^9.5.1",
         "ts-node": "^10.9.2",
         "typescript": "^5.4.5",
-        "vite": "^5.2.10",
+        "vite": "^5.2.11",
         "vite-bundle-visualizer": "^1.1.0",
-        "vitest": "^1.5.2"
+        "vitest": "^1.5.3"
     },
     "engines": {
         "node": ">=21.0.0"
     },
     "eslintConfig": {
         "env": {
             "browser": true,
```

### Comparing `bowtie_json_schema-2024.5.1/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2024.5.2/frontend/pnpm-lock.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -48,22 +48,22 @@
       '@types/react-test-renderer':
         specifier: ^18.3.0
         version: 18.3.0
       '@types/urijs':
         specifier: ^1.19.25
         version: 1.19.25
       '@typescript-eslint/eslint-plugin':
-        specifier: ^7.7.1
-        version: 7.7.1(@typescript-eslint/parser@7.7.1(eslint@8.57.0)(typescript@5.4.5))(eslint@8.57.0)(typescript@5.4.5)
+        specifier: ^7.8.0
+        version: 7.8.0(@typescript-eslint/parser@7.8.0(eslint@8.57.0)(typescript@5.4.5))(eslint@8.57.0)(typescript@5.4.5)
       '@typescript-eslint/parser':
-        specifier: ^7.7.1
-        version: 7.7.1(eslint@8.57.0)(typescript@5.4.5)
+        specifier: ^7.8.0
+        version: 7.8.0(eslint@8.57.0)(typescript@5.4.5)
       '@vitejs/plugin-react':
         specifier: ^4.2.1
-        version: 4.2.1(vite@5.2.10(@types/node@20.11.5)(terser@5.27.0))
+        version: 4.2.1(vite@5.2.11(@types/node@20.11.5)(terser@5.27.0))
       eslint:
         specifier: 8.57.0
         version: 8.57.0
       eslint-plugin-react:
         specifier: 7.34.1
         version: 7.34.1(eslint@8.57.0)
       eslint-plugin-react-hooks:
@@ -81,22 +81,22 @@
       ts-node:
         specifier: ^10.9.2
         version: 10.9.2(@types/node@20.11.5)(typescript@5.4.5)
       typescript:
         specifier: ^5.4.5
         version: 5.4.5
       vite:
-        specifier: ^5.2.10
-        version: 5.2.10(@types/node@20.11.5)(terser@5.27.0)
+        specifier: ^5.2.11
+        version: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
       vite-bundle-visualizer:
         specifier: ^1.1.0
-        version: 1.1.0(rollup@4.17.1)
+        version: 1.1.0(rollup@4.17.2)
       vitest:
-        specifier: ^1.5.2
-        version: 1.5.2(@types/node@20.11.5)(jsdom@24.0.0)(terser@5.27.0)
+        specifier: ^1.5.3
+        version: 1.5.3(@types/node@20.11.5)(jsdom@24.0.0)(terser@5.27.0)
 
 packages:
 
   '@ampproject/remapping@2.3.0':
     resolution: {integrity: sha512-30iZtAPgz+LTIYoeivqYo853f02jBYSd5uGnGpkFV0M3xOt9aN73erkgYAmZU43x4VfqcnLxW9Kpg3R5LC4YYw==}
     engines: {node: '>=6.0.0'}
 
@@ -104,20 +104,20 @@
     resolution: {integrity: sha512-y5+tLQyV8pg3fsiln67BVLD1P13Eg4lh5RW9mF0zUuvLrv9uIQ4MCL+CRT+FTsBlBjcIan6PGsLcBN0m3ClUyQ==}
     engines: {node: '>=6.9.0'}
 
   '@babel/compat-data@7.24.4':
     resolution: {integrity: sha512-vg8Gih2MLK+kOkHJp4gBEIkyaIi00jgWot2D9QOmmfLC8jINSOzmCLta6Bvz/JSBCqnegV0L80jhxkol5GWNfQ==}
     engines: {node: '>=6.9.0'}
 
-  '@babel/core@7.24.4':
-    resolution: {integrity: sha512-MBVlMXP+kkl5394RBLSxxk/iLTeVGuXTV3cIDXavPpMMqnSnt6apKgan/U8O3USWZCWZT/TbgfEpKa4uMgN4Dg==}
+  '@babel/core@7.24.5':
+    resolution: {integrity: sha512-tVQRucExLQ02Boi4vdPp49svNGcfL2GhdTCT9aldhXgCJVAI21EtRfBettiuLUwce/7r6bFdgs6JFkcdTiFttA==}
     engines: {node: '>=6.9.0'}
 
-  '@babel/generator@7.24.4':
-    resolution: {integrity: sha512-Xd6+v6SnjWVx/nus+y0l1sxMOTOMBkyL4+BIdbALyatQnAe/SRVjANeDPSCYaX+i1iJmuGSKf3Z+E+V/va1Hvw==}
+  '@babel/generator@7.24.5':
+    resolution: {integrity: sha512-x32i4hEXvr+iI0NEoEfDKzlemF8AmtOP8CcrRaEcpzysWuoEb1KknpcvMsHKPONoKZiDuItklgWhB18xEhr9PA==}
     engines: {node: '>=6.9.0'}
 
   '@babel/helper-compilation-targets@7.23.6':
     resolution: {integrity: sha512-9JB548GZoQVmzrFgp8o7KxdgkTGm6xs9DW0o/Pim72UDjzr5ObUQ6ZzYPqA+g9OTS2bBQoctLJrky0RDCAWRgQ==}
     engines: {node: '>=6.9.0'}
 
   '@babel/helper-environment-visitor@7.22.20':
@@ -132,83 +132,83 @@
     resolution: {integrity: sha512-wGjk9QZVzvknA6yKIUURb8zY3grXCcOZt+/7Wcy8O2uctxhplmUPkOdlgoNhmdVee2c92JXbf1xpMtVNbfoxRw==}
     engines: {node: '>=6.9.0'}
 
   '@babel/helper-module-imports@7.24.3':
     resolution: {integrity: sha512-viKb0F9f2s0BCS22QSF308z/+1YWKV/76mwt61NBzS5izMzDPwdq1pTrzf+Li3npBWX9KdQbkeCt1jSAM7lZqg==}
     engines: {node: '>=6.9.0'}
 
-  '@babel/helper-module-transforms@7.23.3':
-    resolution: {integrity: sha512-7bBs4ED9OmswdfDzpz4MpWgSrV7FXlc3zIagvLFjS5H+Mk7Snr21vQ6QwrsoCGMfNC4e4LQPdoULEt4ykz0SRQ==}
+  '@babel/helper-module-transforms@7.24.5':
+    resolution: {integrity: sha512-9GxeY8c2d2mdQUP1Dye0ks3VDyIMS98kt/llQ2nUId8IsWqTF0l1LkSX0/uP7l7MCDrzXS009Hyhe2gzTiGW8A==}
     engines: {node: '>=6.9.0'}
     peerDependencies:
       '@babel/core': ^7.0.0
 
-  '@babel/helper-plugin-utils@7.24.0':
-    resolution: {integrity: sha512-9cUznXMG0+FxRuJfvL82QlTqIzhVW9sL0KjMPHhAOOvpQGL8QtdxnBKILjBqxlHyliz0yCa1G903ZXI/FuHy2w==}
+  '@babel/helper-plugin-utils@7.24.5':
+    resolution: {integrity: sha512-xjNLDopRzW2o6ba0gKbkZq5YWEBaK3PCyTOY1K2P/O07LGMhMqlMXPxwN4S5/RhWuCobT8z0jrlKGlYmeR1OhQ==}
     engines: {node: '>=6.9.0'}
 
-  '@babel/helper-simple-access@7.22.5':
-    resolution: {integrity: sha512-n0H99E/K+Bika3++WNL17POvo4rKWZ7lZEp1Q+fStVbUi8nxPQEBOlTmCOxW/0JsS56SKKQ+ojAe2pHKJHN35w==}
+  '@babel/helper-simple-access@7.24.5':
+    resolution: {integrity: sha512-uH3Hmf5q5n7n8mz7arjUlDOCbttY/DW4DYhE6FUsjKJ/oYC1kQQUvwEQWxRwUpX9qQKRXeqLwWxrqilMrf32sQ==}
     engines: {node: '>=6.9.0'}
 
-  '@babel/helper-split-export-declaration@7.22.6':
-    resolution: {integrity: sha512-AsUnxuLhRYsisFiaJwvp1QF+I3KjD5FOxut14q/GzovUe6orHLesW2C7d754kRm53h5gqrz6sFl6sxc4BVtE/g==}
+  '@babel/helper-split-export-declaration@7.24.5':
+    resolution: {integrity: sha512-5CHncttXohrHk8GWOFCcCl4oRD9fKosWlIRgWm4ql9VYioKm52Mk2xsmoohvm7f3JoiLSM5ZgJuRaf5QZZYd3Q==}
     engines: {node: '>=6.9.0'}
 
   '@babel/helper-string-parser@7.24.1':
     resolution: {integrity: sha512-2ofRCjnnA9y+wk8b9IAREroeUP02KHp431N2mhKniy2yKIDKpbrHv9eXwm8cBeWQYcJmzv5qKCu65P47eCF7CQ==}
     engines: {node: '>=6.9.0'}
 
-  '@babel/helper-validator-identifier@7.22.20':
-    resolution: {integrity: sha512-Y4OZ+ytlatR8AI+8KZfKuL5urKp7qey08ha31L8b3BwewJAoJamTzyvxPR/5D+KkdJCGPq/+8TukHBlY10FX9A==}
+  '@babel/helper-validator-identifier@7.24.5':
+    resolution: {integrity: sha512-3q93SSKX2TWCG30M2G2kwaKeTYgEUp5Snjuj8qm729SObL6nbtUldAi37qbxkD5gg3xnBio+f9nqpSepGZMvxA==}
     engines: {node: '>=6.9.0'}
 
   '@babel/helper-validator-option@7.23.5':
     resolution: {integrity: sha512-85ttAOMLsr53VgXkTbkx8oA6YTfT4q7/HzXSLEYmjcSTJPMPQtvq1BD79Byep5xMUYbGRzEpDsjUf3dyp54IKw==}
     engines: {node: '>=6.9.0'}
 
-  '@babel/helpers@7.24.4':
-    resolution: {integrity: sha512-FewdlZbSiwaVGlgT1DPANDuCHaDMiOo+D/IDYRFYjHOuv66xMSJ7fQwwODwRNAPkADIO/z1EoF/l2BCWlWABDw==}
+  '@babel/helpers@7.24.5':
+    resolution: {integrity: sha512-CiQmBMMpMQHwM5m01YnrM6imUG1ebgYJ+fAIW4FZe6m4qHTPaRHti+R8cggAwkdz4oXhtO4/K9JWlh+8hIfR2Q==}
     engines: {node: '>=6.9.0'}
 
-  '@babel/highlight@7.24.2':
-    resolution: {integrity: sha512-Yac1ao4flkTxTteCDZLEvdxg2fZfz1v8M4QpaGypq/WPDqg3ijHYbDfs+LG5hvzSoqaSZ9/Z9lKSP3CjZjv+pA==}
+  '@babel/highlight@7.24.5':
+    resolution: {integrity: sha512-8lLmua6AVh/8SLJRRVD6V8p73Hir9w5mJrhE+IPpILG31KKlI9iz5zmBYKcWPS59qSfgP9RaSBQSHHE81WKuEw==}
     engines: {node: '>=6.9.0'}
 
-  '@babel/parser@7.24.4':
-    resolution: {integrity: sha512-zTvEBcghmeBma9QIGunWevvBAp4/Qu9Bdq+2k0Ot4fVMD6v3dsC9WOcRSKk7tRRyBM/53yKMJko9xOatGQAwSg==}
+  '@babel/parser@7.24.5':
+    resolution: {integrity: sha512-EOv5IK8arwh3LI47dz1b0tKUb/1uhHAnHJOrjgtQMIpu1uXd9mlFrJg9IUgGUgZ41Ch0K8REPTYpO7B76b4vJg==}
     engines: {node: '>=6.0.0'}
     hasBin: true
 
-  '@babel/plugin-transform-react-jsx-self@7.24.1':
-    resolution: {integrity: sha512-kDJgnPujTmAZ/9q2CN4m2/lRsUUPDvsG3+tSHWUJIzMGTt5U/b/fwWd3RO3n+5mjLrsBrVa5eKFRVSQbi3dF1w==}
+  '@babel/plugin-transform-react-jsx-self@7.24.5':
+    resolution: {integrity: sha512-RtCJoUO2oYrYwFPtR1/jkoBEcFuI1ae9a9IMxeyAVa3a1Ap4AnxmyIKG2b2FaJKqkidw/0cxRbWN+HOs6ZWd1w==}
     engines: {node: '>=6.9.0'}
     peerDependencies:
       '@babel/core': ^7.0.0-0
 
   '@babel/plugin-transform-react-jsx-source@7.24.1':
     resolution: {integrity: sha512-1v202n7aUq4uXAieRTKcwPzNyphlCuqHHDcdSNc+vdhoTEZcFMh+L5yZuCmGaIO7bs1nJUNfHB89TZyoL48xNA==}
     engines: {node: '>=6.9.0'}
     peerDependencies:
       '@babel/core': ^7.0.0-0
 
-  '@babel/runtime@7.24.4':
-    resolution: {integrity: sha512-dkxf7+hn8mFBwKjs9bvBlArzLVxVbS8usaPUDd5p2a9JCL9tB8OaOVN1isD4+Xyk4ns89/xeOmbQvgdK7IIVdA==}
+  '@babel/runtime@7.24.5':
+    resolution: {integrity: sha512-Nms86NXrsaeU9vbBJKni6gXiEXZ4CVpYVzEjDH9Sb8vmZ3UljyA1GSOJl/6LGPO8EHLuSF9H+IxNXHPX8QHJ4g==}
     engines: {node: '>=6.9.0'}
 
   '@babel/template@7.24.0':
     resolution: {integrity: sha512-Bkf2q8lMB0AFpX0NFEqSbx1OkTHf0f+0j82mkw+ZpzBnkk7e9Ql0891vlfgi+kHwOk8tQjiQHpqh4LaSa0fKEA==}
     engines: {node: '>=6.9.0'}
 
-  '@babel/traverse@7.24.1':
-    resolution: {integrity: sha512-xuU6o9m68KeqZbQuDt2TcKSxUw/mrsvavlEqQ1leZ/B+C9tk6E4sRWy97WaXgvq5E+nU3cXMxv3WKOCanVMCmQ==}
+  '@babel/traverse@7.24.5':
+    resolution: {integrity: sha512-7aaBLeDQ4zYcUFDUD41lJc1fG8+5IU9DaNSJAgal866FGvmD5EbWQgnEC6kO1gGLsX0esNkfnJSndbTXA3r7UA==}
     engines: {node: '>=6.9.0'}
 
-  '@babel/types@7.24.0':
-    resolution: {integrity: sha512-+j7a5c253RfKh8iABBhywc8NSfP5LURe7Uh4qpsh6jc+aLJguvmIUBdjSdEMQv2bENrCR5MfRdjGo7vzS/ob7w==}
+  '@babel/types@7.24.5':
+    resolution: {integrity: sha512-6mQNsaLeXTw0nxYUYu+NSa4Hx4BlF1x1x8/PMFbiR+GBSr+2DkECc69b8hgy2frEodNcvPffeH8YfWd3LI6jhQ==}
     engines: {node: '>=6.9.0'}
 
   '@cspotcode/source-map-support@0.8.1':
     resolution: {integrity: sha512-IchNf6dN4tHoMFIn/7OE8LWZ19Y6q/67Bmf6vnGREv8RSbBVb9LPJxEcnwrcwX6ixSvaiGoomAUvu4YSxXrVgw==}
     engines: {node: '>=12'}
 
   '@esbuild/aix-ppc64@0.20.2':
@@ -417,16 +417,16 @@
   '@nodelib/fs.walk@1.2.8':
     resolution: {integrity: sha512-oGB+UxlgWcgQkgwo8GcEGwemoTFt3FIO9ababBmaGwXIoBKZ+GTy0pP185beGg7Llih/NSHSV2XAs1lnznocSg==}
     engines: {node: '>= 8'}
 
   '@popperjs/core@2.11.8':
     resolution: {integrity: sha512-P1st0aksCrn9sGZhp8GMYwBnQsbvAWsZAX44oXNNvLHGqAOcoVxmjZiohstwQ7SqKnbR47akdNi+uleWD8+g6A==}
 
-  '@react-aria/ssr@3.9.2':
-    resolution: {integrity: sha512-0gKkgDYdnq1w+ey8KzG9l+H5Z821qh9vVjztk55rUg71vTk/Eaebeir+WtzcLLwTjw3m/asIjx8Y59y1lJZhBw==}
+  '@react-aria/ssr@3.9.3':
+    resolution: {integrity: sha512-5bUZ93dmvHFcmfUcEN7qzYe8yQQ8JY+nHN6m9/iSDCQ/QmCiE0kWXYwhurjw5ch6I8WokQzx66xKIMHBAa4NNA==}
     engines: {node: '>= 12'}
     peerDependencies:
       react: ^16.8.0 || ^17.0.0-rc.1 || ^18.0.0
 
   '@remix-run/router@1.16.0':
     resolution: {integrity: sha512-Quz1KOffeEf/zwkCBM3kBtH4ZoZ+pT3xIXBG4PPW/XFtDP7EGhtTiC2+gpL9GnR7+Qdet5Oa6cYSvwKYg6kN9Q==}
     engines: {node: '>=14.0.0'}
@@ -438,91 +438,91 @@
 
   '@restart/ui@1.6.8':
     resolution: {integrity: sha512-6ndCv3oZ7r9vuP1Ok9KH55TM1/UkdBnP/fSraW0DFDMbPMzWKhVKeFAIEUCRCSdzayjZDcFYK6xbMlipN9dmMA==}
     peerDependencies:
       react: '>=16.14.0'
       react-dom: '>=16.14.0'
 
-  '@rollup/rollup-android-arm-eabi@4.17.1':
-    resolution: {integrity: sha512-P6Wg856Ou/DLpR+O0ZLneNmrv7QpqBg+hK4wE05ijbC/t349BRfMfx+UFj5Ha3fCFopIa6iSZlpdaB4agkWp2Q==}
+  '@rollup/rollup-android-arm-eabi@4.17.2':
+    resolution: {integrity: sha512-NM0jFxY8bB8QLkoKxIQeObCaDlJKewVlIEkuyYKm5An1tdVZ966w2+MPQ2l8LBZLjR+SgyV+nRkTIunzOYBMLQ==}
     cpu: [arm]
     os: [android]
 
-  '@rollup/rollup-android-arm64@4.17.1':
-    resolution: {integrity: sha512-piwZDjuW2WiHr05djVdUkrG5JbjnGbtx8BXQchYCMfib/nhjzWoiScelZ+s5IJI7lecrwSxHCzW026MWBL+oJQ==}
+  '@rollup/rollup-android-arm64@4.17.2':
+    resolution: {integrity: sha512-yeX/Usk7daNIVwkq2uGoq2BYJKZY1JfyLTaHO/jaiSwi/lsf8fTFoQW/n6IdAsx5tx+iotu2zCJwz8MxI6D/Bw==}
     cpu: [arm64]
     os: [android]
 
-  '@rollup/rollup-darwin-arm64@4.17.1':
-    resolution: {integrity: sha512-LsZXXIsN5Q460cKDT4Y+bzoPDhBmO5DTr7wP80d+2EnYlxSgkwdPfE3hbE+Fk8dtya+8092N9srjBTJ0di8RIA==}
+  '@rollup/rollup-darwin-arm64@4.17.2':
+    resolution: {integrity: sha512-kcMLpE6uCwls023+kknm71ug7MZOrtXo+y5p/tsg6jltpDtgQY1Eq5sGfHcQfb+lfuKwhBmEURDga9N0ol4YPw==}
     cpu: [arm64]
     os: [darwin]
 
-  '@rollup/rollup-darwin-x64@4.17.1':
-    resolution: {integrity: sha512-S7TYNQpWXB9APkxu/SLmYHezWwCoZRA9QLgrDeml+SR2A1LLPD2DBUdUlvmCF7FUpRMKvbeeWky+iizQj65Etw==}
+  '@rollup/rollup-darwin-x64@4.17.2':
+    resolution: {integrity: sha512-AtKwD0VEx0zWkL0ZjixEkp5tbNLzX+FCqGG1SvOu993HnSz4qDI6S4kGzubrEJAljpVkhRSlg5bzpV//E6ysTQ==}
     cpu: [x64]
     os: [darwin]
 
-  '@rollup/rollup-linux-arm-gnueabihf@4.17.1':
-    resolution: {integrity: sha512-Lq2JR5a5jsA5um2ZoLiXXEaOagnVyCpCW7xvlcqHC7y46tLwTEgUSTM3a2TfmmTMmdqv+jknUioWXlmxYxE9Yw==}
+  '@rollup/rollup-linux-arm-gnueabihf@4.17.2':
+    resolution: {integrity: sha512-3reX2fUHqN7sffBNqmEyMQVj/CKhIHZd4y631duy0hZqI8Qoqf6lTtmAKvJFYa6bhU95B1D0WgzHkmTg33In0A==}
     cpu: [arm]
     os: [linux]
 
-  '@rollup/rollup-linux-arm-musleabihf@4.17.1':
-    resolution: {integrity: sha512-9BfzwyPNV0IizQoR+5HTNBGkh1KXE8BqU0DBkqMngmyFW7BfuIZyMjQ0s6igJEiPSBvT3ZcnIFohZ19OqjhDPg==}
+  '@rollup/rollup-linux-arm-musleabihf@4.17.2':
+    resolution: {integrity: sha512-uSqpsp91mheRgw96xtyAGP9FW5ChctTFEoXP0r5FAzj/3ZRv3Uxjtc7taRQSaQM/q85KEKjKsZuiZM3GyUivRg==}
     cpu: [arm]
     os: [linux]
 
-  '@rollup/rollup-linux-arm64-gnu@4.17.1':
-    resolution: {integrity: sha512-e2uWaoxo/rtzA52OifrTSXTvJhAXb0XeRkz4CdHBK2KtxrFmuU/uNd544Ogkpu938BzEfvmWs8NZ8Axhw33FDw==}
+  '@rollup/rollup-linux-arm64-gnu@4.17.2':
+    resolution: {integrity: sha512-EMMPHkiCRtE8Wdk3Qhtciq6BndLtstqZIroHiiGzB3C5LDJmIZcSzVtLRbwuXuUft1Cnv+9fxuDtDxz3k3EW2A==}
     cpu: [arm64]
     os: [linux]
 
-  '@rollup/rollup-linux-arm64-musl@4.17.1':
-    resolution: {integrity: sha512-ekggix/Bc/d/60H1Mi4YeYb/7dbal1kEDZ6sIFVAE8pUSx7PiWeEh+NWbL7bGu0X68BBIkgF3ibRJe1oFTksQQ==}
+  '@rollup/rollup-linux-arm64-musl@4.17.2':
+    resolution: {integrity: sha512-NMPylUUZ1i0z/xJUIx6VUhISZDRT+uTWpBcjdv0/zkp7b/bQDF+NfnfdzuTiB1G6HTodgoFa93hp0O1xl+/UbA==}
     cpu: [arm64]
     os: [linux]
 
-  '@rollup/rollup-linux-powerpc64le-gnu@4.17.1':
-    resolution: {integrity: sha512-UGV0dUo/xCv4pkr/C8KY7XLFwBNnvladt8q+VmdKrw/3RUd3rD0TptwjisvE2TTnnlENtuY4/PZuoOYRiGp8Gw==}
+  '@rollup/rollup-linux-powerpc64le-gnu@4.17.2':
+    resolution: {integrity: sha512-T19My13y8uYXPw/L/k0JYaX1fJKFT/PWdXiHr8mTbXWxjVF1t+8Xl31DgBBvEKclw+1b00Chg0hxE2O7bTG7GQ==}
     cpu: [ppc64]
     os: [linux]
 
-  '@rollup/rollup-linux-riscv64-gnu@4.17.1':
-    resolution: {integrity: sha512-gEYmYYHaehdvX46mwXrU49vD6Euf1Bxhq9pPb82cbUU9UT2NV+RSckQ5tKWOnNXZixKsy8/cPGtiUWqzPuAcXQ==}
+  '@rollup/rollup-linux-riscv64-gnu@4.17.2':
+    resolution: {integrity: sha512-BOaNfthf3X3fOWAB+IJ9kxTgPmMqPPH5f5k2DcCsRrBIbWnaJCgX2ll77dV1TdSy9SaXTR5iDXRL8n7AnoP5cg==}
     cpu: [riscv64]
     os: [linux]
 
-  '@rollup/rollup-linux-s390x-gnu@4.17.1':
-    resolution: {integrity: sha512-xeae5pMAxHFp6yX5vajInG2toST5lsCTrckSRUFwNgzYqnUjNBcQyqk1bXUxX5yhjWFl2Mnz3F8vQjl+2FRIcw==}
+  '@rollup/rollup-linux-s390x-gnu@4.17.2':
+    resolution: {integrity: sha512-W0UP/x7bnn3xN2eYMql2T/+wpASLE5SjObXILTMPUBDB/Fg/FxC+gX4nvCfPBCbNhz51C+HcqQp2qQ4u25ok6g==}
     cpu: [s390x]
     os: [linux]
 
-  '@rollup/rollup-linux-x64-gnu@4.17.1':
-    resolution: {integrity: sha512-AsdnINQoDWfKpBzCPqQWxSPdAWzSgnYbrJYtn6W0H2E9It5bZss99PiLA8CgmDRfvKygt20UpZ3xkhFlIfX9zQ==}
+  '@rollup/rollup-linux-x64-gnu@4.17.2':
+    resolution: {integrity: sha512-Hy7pLwByUOuyaFC6mAr7m+oMC+V7qyifzs/nW2OJfC8H4hbCzOX07Ov0VFk/zP3kBsELWNFi7rJtgbKYsav9QQ==}
     cpu: [x64]
     os: [linux]
 
-  '@rollup/rollup-linux-x64-musl@4.17.1':
-    resolution: {integrity: sha512-KoB4fyKXTR+wYENkIG3fFF+5G6N4GFvzYx8Jax8BR4vmddtuqSb5oQmYu2Uu067vT/Fod7gxeQYKupm8gAcMSQ==}
+  '@rollup/rollup-linux-x64-musl@4.17.2':
+    resolution: {integrity: sha512-h1+yTWeYbRdAyJ/jMiVw0l6fOOm/0D1vNLui9iPuqgRGnXA0u21gAqOyB5iHjlM9MMfNOm9RHCQ7zLIzT0x11Q==}
     cpu: [x64]
     os: [linux]
 
-  '@rollup/rollup-win32-arm64-msvc@4.17.1':
-    resolution: {integrity: sha512-J0d3NVNf7wBL9t4blCNat+d0PYqAx8wOoY+/9Q5cujnafbX7BmtYk3XvzkqLmFECaWvXGLuHmKj/wrILUinmQg==}
+  '@rollup/rollup-win32-arm64-msvc@4.17.2':
+    resolution: {integrity: sha512-tmdtXMfKAjy5+IQsVtDiCfqbynAQE/TQRpWdVataHmhMb9DCoJxp9vLcCBjEQWMiUYxO1QprH/HbY9ragCEFLA==}
     cpu: [arm64]
     os: [win32]
 
-  '@rollup/rollup-win32-ia32-msvc@4.17.1':
-    resolution: {integrity: sha512-xjgkWUwlq7IbgJSIxvl516FJ2iuC/7ttjsAxSPpC9kkI5iQQFHKyEN5BjbhvJ/IXIZ3yIBcW5QDlWAyrA+TFag==}
+  '@rollup/rollup-win32-ia32-msvc@4.17.2':
+    resolution: {integrity: sha512-7II/QCSTAHuE5vdZaQEwJq2ZACkBpQDOmQsE6D6XUbnBHW8IAhm4eTufL6msLJorzrHDFv3CF8oCA/hSIRuZeQ==}
     cpu: [ia32]
     os: [win32]
 
-  '@rollup/rollup-win32-x64-msvc@4.17.1':
-    resolution: {integrity: sha512-0QbCkfk6cnnVKWqqlC0cUrrUMDMfu5ffvYMTUHf+qMN2uAb3MKP31LPcwiMXBNsvoFGs/kYdFOsuLmvppCopXA==}
+  '@rollup/rollup-win32-x64-msvc@4.17.2':
+    resolution: {integrity: sha512-TGGO7v7qOq4CYmSBVEYpI1Y5xDuCEnbVC5Vth8mOsW0gDSzxNrVERPc790IGHsrT2dQSimgMr9Ub3Y1Jci5/8w==}
     cpu: [x64]
     os: [win32]
 
   '@sinclair/typebox@0.27.8':
     resolution: {integrity: sha512-+Fj43pSMwJs4KRrH/938Uf+uAELIgVBmQzg/q1YG10djyfA3TnrU8N8XzqCh/okZdszqBQTZf96idMfE5lnwTA==}
 
   '@swc/helpers@0.5.11':
@@ -596,95 +596,95 @@
 
   '@types/urijs@1.19.25':
     resolution: {integrity: sha512-XOfUup9r3Y06nFAZh3WvO0rBU4OtlfPB/vgxpjg+NRdGU6CN6djdc6OEiH+PcqHCY6eFLo9Ista73uarf4gnBg==}
 
   '@types/warning@3.0.3':
     resolution: {integrity: sha512-D1XC7WK8K+zZEveUPY+cf4+kgauk8N4eHr/XIHXGlGYkHLud6hK9lYfZk1ry1TNh798cZUCgb6MqGEG8DkJt6Q==}
 
-  '@typescript-eslint/eslint-plugin@7.7.1':
-    resolution: {integrity: sha512-KwfdWXJBOviaBVhxO3p5TJiLpNuh2iyXyjmWN0f1nU87pwyvfS0EmjC6ukQVYVFJd/K1+0NWGPDXiyEyQorn0Q==}
+  '@typescript-eslint/eslint-plugin@7.8.0':
+    resolution: {integrity: sha512-gFTT+ezJmkwutUPmB0skOj3GZJtlEGnlssems4AjkVweUPGj7jRwwqg0Hhg7++kPGJqKtTYx+R05Ftww372aIg==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       '@typescript-eslint/parser': ^7.0.0
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
 
-  '@typescript-eslint/parser@7.7.1':
-    resolution: {integrity: sha512-vmPzBOOtz48F6JAGVS/kZYk4EkXao6iGrD838sp1w3NQQC0W8ry/q641KU4PrG7AKNAf56NOcR8GOpH8l9FPCw==}
+  '@typescript-eslint/parser@7.8.0':
+    resolution: {integrity: sha512-KgKQly1pv0l4ltcftP59uQZCi4HUYswCLbTqVZEJu7uLX8CTLyswqMLqLN+2QFz4jCptqWVV4SB7vdxcH2+0kQ==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
 
-  '@typescript-eslint/scope-manager@7.7.1':
-    resolution: {integrity: sha512-PytBif2SF+9SpEUKynYn5g1RHFddJUcyynGpztX3l/ik7KmZEv19WCMhUBkHXPU9es/VWGD3/zg3wg90+Dh2rA==}
+  '@typescript-eslint/scope-manager@7.8.0':
+    resolution: {integrity: sha512-viEmZ1LmwsGcnr85gIq+FCYI7nO90DVbE37/ll51hjv9aG+YZMb4WDE2fyWpUR4O/UrhGRpYXK/XajcGTk2B8g==}
     engines: {node: ^18.18.0 || >=20.0.0}
 
-  '@typescript-eslint/type-utils@7.7.1':
-    resolution: {integrity: sha512-ZksJLW3WF7o75zaBPScdW1Gbkwhd/lyeXGf1kQCxJaOeITscoSl0MjynVvCzuV5boUz/3fOI06Lz8La55mu29Q==}
+  '@typescript-eslint/type-utils@7.8.0':
+    resolution: {integrity: sha512-H70R3AefQDQpz9mGv13Uhi121FNMh+WEaRqcXTX09YEDky21km4dV1ZXJIp8QjXc4ZaVkXVdohvWDzbnbHDS+A==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
 
-  '@typescript-eslint/types@7.7.1':
-    resolution: {integrity: sha512-AmPmnGW1ZLTpWa+/2omPrPfR7BcbUU4oha5VIbSbS1a1Tv966bklvLNXxp3mrbc+P2j4MNOTfDffNsk4o0c6/w==}
+  '@typescript-eslint/types@7.8.0':
+    resolution: {integrity: sha512-wf0peJ+ZGlcH+2ZS23aJbOv+ztjeeP8uQ9GgwMJGVLx/Nj9CJt17GWgWWoSmoRVKAX2X+7fzEnAjxdvK2gqCLw==}
     engines: {node: ^18.18.0 || >=20.0.0}
 
-  '@typescript-eslint/typescript-estree@7.7.1':
-    resolution: {integrity: sha512-CXe0JHCXru8Fa36dteXqmH2YxngKJjkQLjxzoj6LYwzZ7qZvgsLSc+eqItCrqIop8Vl2UKoAi0StVWu97FQZIQ==}
+  '@typescript-eslint/typescript-estree@7.8.0':
+    resolution: {integrity: sha512-5pfUCOwK5yjPaJQNy44prjCwtr981dO8Qo9J9PwYXZ0MosgAbfEMB008dJ5sNo3+/BN6ytBPuSvXUg9SAqB0dg==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
 
-  '@typescript-eslint/utils@7.7.1':
-    resolution: {integrity: sha512-QUvBxPEaBXf41ZBbaidKICgVL8Hin0p6prQDu6bbetWo39BKbWJxRsErOzMNT1rXvTll+J7ChrbmMCXM9rsvOQ==}
+  '@typescript-eslint/utils@7.8.0':
+    resolution: {integrity: sha512-L0yFqOCflVqXxiZyXrDr80lnahQfSOfc9ELAAZ75sqicqp2i36kEZZGuUymHNFoYOqxRT05up760b4iGsl02nQ==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
 
-  '@typescript-eslint/visitor-keys@7.7.1':
-    resolution: {integrity: sha512-gBL3Eq25uADw1LQ9kVpf3hRM+DWzs0uZknHYK3hq4jcTPqVCClHGDnB6UUUV2SFeBeA4KWHWbbLqmbGcZ4FYbw==}
+  '@typescript-eslint/visitor-keys@7.8.0':
+    resolution: {integrity: sha512-q4/gibTNBQNA0lGyYQCmWRS5D15n8rXh4QjK3KV+MBPlTYHpfBUT3D3PaPR/HeNiI9W6R7FvlkcGhNyAoP+caA==}
     engines: {node: ^18.18.0 || >=20.0.0}
 
   '@ungap/structured-clone@1.2.0':
     resolution: {integrity: sha512-zuVdFrMJiuCDQUMCzQaD6KL28MjnqqN8XnAqiEq9PNm/hCPTSGfrXCOfwj1ow4LFb/tNymJPwsNbVePc1xFqrQ==}
 
   '@vitejs/plugin-react@4.2.1':
     resolution: {integrity: sha512-oojO9IDc4nCUUi8qIR11KoQm0XFFLIwsRBwHRR4d/88IWghn1y6ckz/bJ8GHDCsYEJee8mDzqtJxh15/cisJNQ==}
     engines: {node: ^14.18.0 || >=16.0.0}
     peerDependencies:
       vite: ^4.2.0 || ^5.0.0
 
-  '@vitest/expect@1.5.2':
-    resolution: {integrity: sha512-rf7MTD1WCoDlN3FfYJ9Llfp0PbdtOMZ3FIF0AVkDnKbp3oiMW1c8AmvRZBcqbAhDUAvF52e9zx4WQM1r3oraVA==}
+  '@vitest/expect@1.5.3':
+    resolution: {integrity: sha512-y+waPz31pOFr3rD7vWTbwiLe5+MgsMm40jTZbQE8p8/qXyBX3CQsIXRx9XK12IbY7q/t5a5aM/ckt33b4PxK2g==}
 
-  '@vitest/runner@1.5.2':
-    resolution: {integrity: sha512-7IJ7sJhMZrqx7HIEpv3WrMYcq8ZNz9L6alo81Y6f8hV5mIE6yVZsFoivLZmr0D777klm1ReqonE9LyChdcmw6g==}
+  '@vitest/runner@1.5.3':
+    resolution: {integrity: sha512-7PlfuReN8692IKQIdCxwir1AOaP5THfNkp0Uc4BKr2na+9lALNit7ub9l3/R7MP8aV61+mHKRGiqEKRIwu6iiQ==}
 
-  '@vitest/snapshot@1.5.2':
-    resolution: {integrity: sha512-CTEp/lTYos8fuCc9+Z55Ga5NVPKUgExritjF5VY7heRFUfheoAqBneUlvXSUJHUZPjnPmyZA96yLRJDP1QATFQ==}
+  '@vitest/snapshot@1.5.3':
+    resolution: {integrity: sha512-K3mvIsjyKYBhNIDujMD2gfQEzddLe51nNOAf45yKRt/QFJcUIeTQd2trRvv6M6oCBHNVnZwFWbQ4yj96ibiDsA==}
 
-  '@vitest/spy@1.5.2':
-    resolution: {integrity: sha512-xCcPvI8JpCtgikT9nLpHPL1/81AYqZy1GCy4+MCHBE7xi8jgsYkULpW5hrx5PGLgOQjUpb6fd15lqcriJ40tfQ==}
+  '@vitest/spy@1.5.3':
+    resolution: {integrity: sha512-Llj7Jgs6lbnL55WoshJUUacdJfjU2honvGcAJBxhra5TPEzTJH8ZuhI3p/JwqqfnTr4PmP7nDmOXP53MS7GJlg==}
 
-  '@vitest/utils@1.5.2':
-    resolution: {integrity: sha512-sWOmyofuXLJ85VvXNsroZur7mOJGiQeM0JN3/0D1uU8U9bGFM69X1iqHaRXl6R8BwaLY6yPCogP257zxTzkUdA==}
+  '@vitest/utils@1.5.3':
+    resolution: {integrity: sha512-rE9DTN1BRhzkzqNQO+kw8ZgfeEBCLXiHJwetk668shmNBpSagQxneT5eSqEBLP+cqSiAeecvQmbpFfdMyLcIQA==}
 
   '@webassemblyjs/ast@1.12.1':
     resolution: {integrity: sha512-EKfMUOPRRUTy5UII4qJDGPpqfwjOmZ5jeGFwid9mnoqIFK+e0vqoi1qH56JpmZSzEL53jKnNzScdmftJyG5xWg==}
 
   '@webassemblyjs/floating-point-hex-parser@1.11.6':
     resolution: {integrity: sha512-ejAj9hfRJ2XMsNHk/v6Fu2dGS+i4UaXBXGemOfQ/JfQ6mdQg/WXtwleQRLLS4OvfDhv8rYnVwH27YJLMyYsxhw==}
 
@@ -864,16 +864,16 @@
     resolution: {integrity: sha512-GHTSNSYICQ7scH7sZ+M2rFopRoLh8t2bLSW6BbgrtLsahOIB5iyAVJf9GjWK3cYTDaMj4XdBpM1cA6pIS0Kv2w==}
     engines: {node: '>= 0.4'}
 
   callsites@3.1.0:
     resolution: {integrity: sha512-P8BjAsXvZS+VIDUI11hHCQEv74YT67YUi5JJFNWIqL235sBmjX4+qx9Muvls5ivyNENctx46xQLQ3aTuE7ssaQ==}
     engines: {node: '>=6'}
 
-  caniuse-lite@1.0.30001614:
-    resolution: {integrity: sha512-jmZQ1VpmlRwHgdP1/uiKzgiAuGOfLEJsYFP4+GBou/QQ4U6IOJCB4NP1c+1p9RGLpwObcT94jA5/uO+F1vBbog==}
+  caniuse-lite@1.0.30001615:
+    resolution: {integrity: sha512-1IpazM5G3r38meiae0bHRnPhz+CBQ3ZLqbQMtrg+AsTPKAXgW38JNsXkyZ+v8waCsDmPq87lmfun5Q2AGysNEQ==}
 
   chai@4.4.1:
     resolution: {integrity: sha512-13sOfMv2+DWduEU+/xbun3LScLoqN17nBeTLUsmDfKdoiC1fr0n9PU4guu4AhRcOVFk/sW8LyZWHuhWtQZiF+g==}
     engines: {node: '>=4'}
 
   chalk@2.4.2:
     resolution: {integrity: sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==}
@@ -1029,16 +1029,16 @@
   doctrine@3.0.0:
     resolution: {integrity: sha512-yS+Q5i3hBf7GBkd4KG8a7eBNNWNGLTaEwwYWUijIYM7zrlYDM0BFXHjjPWlWZ1Rg7UaddZeIDmi9jF3HmqiQ2w==}
     engines: {node: '>=6.0.0'}
 
   dom-helpers@5.2.1:
     resolution: {integrity: sha512-nRCa7CK3VTrM2NmGkIy4cbK7IZlgBE/PYMn55rrXefr5xXDP0LdtfPnblFDoVdcAfslJ7or6iqAUnx0CCGIWQA==}
 
-  electron-to-chromium@1.4.750:
-    resolution: {integrity: sha512-9ItEpeu15hW5m8jKdriL+BQrgwDTXEL9pn4SkillWFu73ZNNNQ2BKKLS+ZHv2vC9UkNhosAeyfxOf/5OSeTCPA==}
+  electron-to-chromium@1.4.754:
+    resolution: {integrity: sha512-7Kr5jUdns5rL/M9wFFmMZAgFDuL2YOnanFH4OI4iFzUqyh3XOL7nAGbSlSMZdzKMIyyTpNSbqZsWG9odwLeKvA==}
 
   emoji-regex@8.0.0:
     resolution: {integrity: sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==}
 
   enhanced-resolve@5.16.0:
     resolution: {integrity: sha512-O+QWCviPNSSLAD9Ucn8Awv+poAkqn3T1XY5/N7kR7rQO9yfSGWkYZDwpJ+iKF7B8rxaQKWngSqACpgzeapSyoA==}
     engines: {node: '>=10.13.0'}
@@ -1270,16 +1270,16 @@
     resolution: {integrity: sha512-WOBp/EEGUiIsJSp7wcv/y6MO+lV9UoncWqxuFfm8eBwzWNgyfBd6Gz+IeKQ9jCmyhoH99g15M3T+QaVHFjizVA==}
     engines: {node: '>=4'}
 
   globals@13.24.0:
     resolution: {integrity: sha512-AhO5QUcj8llrbG09iWhPU2B204J1xnPeL8kQmVorSsy+Sjj1sk8gIyh6cUocGmH4L0UuhAJy+hJMRA4mgA4mFQ==}
     engines: {node: '>=8'}
 
-  globalthis@1.0.3:
-    resolution: {integrity: sha512-sFdI5LyBiNTHjRd7cGPWapiHWMOXKyuBNX/cWJ3NfzrZQVa8GI/8cofCl74AOVqq9W5kNmguTIzJ/1s2gyI9wA==}
+  globalthis@1.0.4:
+    resolution: {integrity: sha512-DpLKbNU4WylpxJykQujfCcwYWiV/Jhm50Goo0wrVILAv5jOr9d+H+UR3PhSCD2rCCEIg0uc+G+muBTwD54JhDQ==}
     engines: {node: '>= 0.4'}
 
   globby@11.1.0:
     resolution: {integrity: sha512-jhIXaOzy1sb8IyocaruWSn1TjmnBVs8Ayhcy83rmxNJ8q2uWKCAj3CnJY+KpGSXCueAPc0i05kVvVKtP1t9S3g==}
     engines: {node: '>=10'}
 
   gopd@1.0.1:
@@ -1643,16 +1643,16 @@
   minimatch@3.1.2:
     resolution: {integrity: sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==}
 
   minimatch@9.0.4:
     resolution: {integrity: sha512-KqWh+VchfxcMNRAJjj2tnsSJdNbHsVgnkBhTNrW7AjVo6OvLtxw8zfT9oLw1JSohlFzJ8jCoTgaoXvJ+kHt6fw==}
     engines: {node: '>=16 || 14 >=14.17'}
 
-  mlly@1.6.1:
-    resolution: {integrity: sha512-vLgaHvaeunuOXHSmEbZ9izxPx3USsk8KCQ8iC+aTlp5sKRSoZvwhHh5L9VbKSaVC6sJDqbyohIS76E2VmHIPAA==}
+  mlly@1.7.0:
+    resolution: {integrity: sha512-U9SDaXGEREBYQgfejV97coK0UL1r+qnF2SyO9A3qcI8MzKnsIFKHNVEkrDyNncQTKQQumsasmeq84eNMdBfsNQ==}
 
   ms@2.1.2:
     resolution: {integrity: sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==}
 
   nanoid@3.3.7:
     resolution: {integrity: sha512-eSRppjcPIatRIMC1U6UngP8XFcz8MQWGQdt1MTBQ7NaAmvXDfvNxbvWV3x2y6CdEUciCSsDHDQZbhYaB8QEo2g==}
     engines: {node: ^10 || ^12 || ^13.7 || ^14 || >=15.0.1}
@@ -1946,16 +1946,16 @@
     hasBin: true
     peerDependencies:
       rollup: 2.x || 3.x || 4.x
     peerDependenciesMeta:
       rollup:
         optional: true
 
-  rollup@4.17.1:
-    resolution: {integrity: sha512-0gG94inrUtg25sB2V/pApwiv1lUb0bQ25FPNuzO89Baa+B+c0ccaaBKM5zkZV/12pUUdH+lWCSm9wmHqyocuVQ==}
+  rollup@4.17.2:
+    resolution: {integrity: sha512-/9ClTJPByC0U4zNLowV1tMBe8yMEAxewtR3cUNX5BoEpGH3dQEWpJLr6CLp0fPdYRF/fzVOgvDb1zXuakwF5kQ==}
     engines: {node: '>=18.0.0', npm: '>=8.0.0'}
     hasBin: true
 
   rrweb-cssom@0.6.0:
     resolution: {integrity: sha512-APM0Gt1KoXBz0iIkkdB/kfvGOwC4UuJFeG/c+yV7wSc7q96cG/kJ0HiYCnzivD9SB53cLV1MlHFNfOuPaadYSw==}
 
   run-parallel@1.2.0:
@@ -2247,16 +2247,16 @@
   undici-types@5.26.5:
     resolution: {integrity: sha512-JlCMO+ehdEIKqlFxk6IfVoAUVmgz7cU7zD/h9XZ0qzeosSHmUJVOzSQvvYSYWXkFXC+IfLKSIffhv0sVZup6pA==}
 
   universalify@0.2.0:
     resolution: {integrity: sha512-CJ1QgKmNg3CwvAv/kOFmtnEN05f0D/cn9QntgNOQlQF9dgvVTHj3t+8JPdjqawCHk7V/KA+fbUqzZ9XWhcqPUg==}
     engines: {node: '>= 4.0.0'}
 
-  update-browserslist-db@1.0.13:
-    resolution: {integrity: sha512-xebP81SNcPuNpPP3uzeW1NYXxI3rxyJzF3pD6sH4jE7o/IX+WtSpwnVU+qIsDPyk0d3hmFQ7mjqc6AtV604hbg==}
+  update-browserslist-db@1.0.14:
+    resolution: {integrity: sha512-JixKH8GR2pWYshIPUg/NujK3JO7JiqEEUiNArE86NQyrgUuZeTlZQN3xuS/yiV5Kb48ev9K6RqNkaJjXsdg7Jw==}
     hasBin: true
     peerDependencies:
       browserslist: '>= 4.21.0'
 
   uri-js@4.4.1:
     resolution: {integrity: sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==}
 
@@ -2270,21 +2270,21 @@
     resolution: {integrity: sha512-wa7YjyUGfNZngI/vtK0UHAN+lgDCxBPCylVXGp0zu59Fz5aiGtNXaq3DhIov063MorB+VfufLh3JlF2KdTK3xg==}
 
   vite-bundle-visualizer@1.1.0:
     resolution: {integrity: sha512-cmi5OuS7Eta5keTJmCTEbBBA7gOsUQ4K44W5dbsP+n/X0GIilIIFbJeXF120MQpTxdiZ/GIx4A9zkPEcKpPAog==}
     engines: {node: ^18.19.0 || >=20.6.0}
     hasBin: true
 
-  vite-node@1.5.2:
-    resolution: {integrity: sha512-Y8p91kz9zU+bWtF7HGt6DVw2JbhyuB2RlZix3FPYAYmUyZ3n7iTp8eSyLyY6sxtPegvxQtmlTMhfPhUfCUF93A==}
+  vite-node@1.5.3:
+    resolution: {integrity: sha512-axFo00qiCpU/JLd8N1gu9iEYL3xTbMbMrbe5nDp9GL0nb6gurIdZLkkFogZXWnE8Oyy5kfSLwNVIcVsnhE7lgQ==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
 
-  vite@5.2.10:
-    resolution: {integrity: sha512-PAzgUZbP7msvQvqdSD+ErD5qGnSFiGOoWmV5yAKUEI0kdhjbH6nMWVyZQC/hSc4aXwc0oJ9aEdIiF9Oje0JFCw==}
+  vite@5.2.11:
+    resolution: {integrity: sha512-HndV31LWW05i1BLPMUCE1B9E9GFbOu1MbenhS58FuK6owSO5qHm7GiCotrNY1YE5rMeQSFBGmT5ZaLEjFizgiQ==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
     peerDependencies:
       '@types/node': ^18.0.0 || >=20.0.0
       less: '*'
       lightningcss: ^1.21.0
       sass: '*'
@@ -2303,23 +2303,23 @@
       stylus:
         optional: true
       sugarss:
         optional: true
       terser:
         optional: true
 
-  vitest@1.5.2:
-    resolution: {integrity: sha512-l9gwIkq16ug3xY7BxHwcBQovLZG75zZL0PlsiYQbf76Rz6QGs54416UWMtC0jXeihvHvcHrf2ROEjkQRVpoZYw==}
+  vitest@1.5.3:
+    resolution: {integrity: sha512-2oM7nLXylw3mQlW6GXnRriw+7YvZFk/YNV8AxIC3Z3MfFbuziLGWP9GPxxu/7nRlXhqyxBikpamr+lEEj1sUEw==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
     peerDependencies:
       '@edge-runtime/vm': '*'
       '@types/node': ^18.0.0 || >=20.0.0
-      '@vitest/browser': 1.5.2
-      '@vitest/ui': 1.5.2
+      '@vitest/browser': 1.5.3
+      '@vitest/ui': 1.5.3
       happy-dom: '*'
       jsdom: '*'
     peerDependenciesMeta:
       '@edge-runtime/vm':
         optional: true
       '@types/node':
         optional: true
@@ -2467,42 +2467,42 @@
   '@ampproject/remapping@2.3.0':
     dependencies:
       '@jridgewell/gen-mapping': 0.3.5
       '@jridgewell/trace-mapping': 0.3.25
 
   '@babel/code-frame@7.24.2':
     dependencies:
-      '@babel/highlight': 7.24.2
+      '@babel/highlight': 7.24.5
       picocolors: 1.0.0
 
   '@babel/compat-data@7.24.4': {}
 
-  '@babel/core@7.24.4':
+  '@babel/core@7.24.5':
     dependencies:
       '@ampproject/remapping': 2.3.0
       '@babel/code-frame': 7.24.2
-      '@babel/generator': 7.24.4
+      '@babel/generator': 7.24.5
       '@babel/helper-compilation-targets': 7.23.6
-      '@babel/helper-module-transforms': 7.23.3(@babel/core@7.24.4)
-      '@babel/helpers': 7.24.4
-      '@babel/parser': 7.24.4
+      '@babel/helper-module-transforms': 7.24.5(@babel/core@7.24.5)
+      '@babel/helpers': 7.24.5
+      '@babel/parser': 7.24.5
       '@babel/template': 7.24.0
-      '@babel/traverse': 7.24.1
-      '@babel/types': 7.24.0
+      '@babel/traverse': 7.24.5
+      '@babel/types': 7.24.5
       convert-source-map: 2.0.0
       debug: 4.3.4
       gensync: 1.0.0-beta.2
       json5: 2.2.3
       semver: 6.3.1
     transitivePeerDependencies:
       - supports-color
 
-  '@babel/generator@7.24.4':
+  '@babel/generator@7.24.5':
     dependencies:
-      '@babel/types': 7.24.0
+      '@babel/types': 7.24.5
       '@jridgewell/gen-mapping': 0.3.5
       '@jridgewell/trace-mapping': 0.3.25
       jsesc: 2.5.2
 
   '@babel/helper-compilation-targets@7.23.6':
     dependencies:
       '@babel/compat-data': 7.24.4
@@ -2512,107 +2512,107 @@
       semver: 6.3.1
 
   '@babel/helper-environment-visitor@7.22.20': {}
 
   '@babel/helper-function-name@7.23.0':
     dependencies:
       '@babel/template': 7.24.0
-      '@babel/types': 7.24.0
+      '@babel/types': 7.24.5
 
   '@babel/helper-hoist-variables@7.22.5':
     dependencies:
-      '@babel/types': 7.24.0
+      '@babel/types': 7.24.5
 
   '@babel/helper-module-imports@7.24.3':
     dependencies:
-      '@babel/types': 7.24.0
+      '@babel/types': 7.24.5
 
-  '@babel/helper-module-transforms@7.23.3(@babel/core@7.24.4)':
+  '@babel/helper-module-transforms@7.24.5(@babel/core@7.24.5)':
     dependencies:
-      '@babel/core': 7.24.4
+      '@babel/core': 7.24.5
       '@babel/helper-environment-visitor': 7.22.20
       '@babel/helper-module-imports': 7.24.3
-      '@babel/helper-simple-access': 7.22.5
-      '@babel/helper-split-export-declaration': 7.22.6
-      '@babel/helper-validator-identifier': 7.22.20
+      '@babel/helper-simple-access': 7.24.5
+      '@babel/helper-split-export-declaration': 7.24.5
+      '@babel/helper-validator-identifier': 7.24.5
 
-  '@babel/helper-plugin-utils@7.24.0': {}
+  '@babel/helper-plugin-utils@7.24.5': {}
 
-  '@babel/helper-simple-access@7.22.5':
+  '@babel/helper-simple-access@7.24.5':
     dependencies:
-      '@babel/types': 7.24.0
+      '@babel/types': 7.24.5
 
-  '@babel/helper-split-export-declaration@7.22.6':
+  '@babel/helper-split-export-declaration@7.24.5':
     dependencies:
-      '@babel/types': 7.24.0
+      '@babel/types': 7.24.5
 
   '@babel/helper-string-parser@7.24.1': {}
 
-  '@babel/helper-validator-identifier@7.22.20': {}
+  '@babel/helper-validator-identifier@7.24.5': {}
 
   '@babel/helper-validator-option@7.23.5': {}
 
-  '@babel/helpers@7.24.4':
+  '@babel/helpers@7.24.5':
     dependencies:
       '@babel/template': 7.24.0
-      '@babel/traverse': 7.24.1
-      '@babel/types': 7.24.0
+      '@babel/traverse': 7.24.5
+      '@babel/types': 7.24.5
     transitivePeerDependencies:
       - supports-color
 
-  '@babel/highlight@7.24.2':
+  '@babel/highlight@7.24.5':
     dependencies:
-      '@babel/helper-validator-identifier': 7.22.20
+      '@babel/helper-validator-identifier': 7.24.5
       chalk: 2.4.2
       js-tokens: 4.0.0
       picocolors: 1.0.0
 
-  '@babel/parser@7.24.4':
+  '@babel/parser@7.24.5':
     dependencies:
-      '@babel/types': 7.24.0
+      '@babel/types': 7.24.5
 
-  '@babel/plugin-transform-react-jsx-self@7.24.1(@babel/core@7.24.4)':
+  '@babel/plugin-transform-react-jsx-self@7.24.5(@babel/core@7.24.5)':
     dependencies:
-      '@babel/core': 7.24.4
-      '@babel/helper-plugin-utils': 7.24.0
+      '@babel/core': 7.24.5
+      '@babel/helper-plugin-utils': 7.24.5
 
-  '@babel/plugin-transform-react-jsx-source@7.24.1(@babel/core@7.24.4)':
+  '@babel/plugin-transform-react-jsx-source@7.24.1(@babel/core@7.24.5)':
     dependencies:
-      '@babel/core': 7.24.4
-      '@babel/helper-plugin-utils': 7.24.0
+      '@babel/core': 7.24.5
+      '@babel/helper-plugin-utils': 7.24.5
 
-  '@babel/runtime@7.24.4':
+  '@babel/runtime@7.24.5':
     dependencies:
       regenerator-runtime: 0.14.1
 
   '@babel/template@7.24.0':
     dependencies:
       '@babel/code-frame': 7.24.2
-      '@babel/parser': 7.24.4
-      '@babel/types': 7.24.0
+      '@babel/parser': 7.24.5
+      '@babel/types': 7.24.5
 
-  '@babel/traverse@7.24.1':
+  '@babel/traverse@7.24.5':
     dependencies:
       '@babel/code-frame': 7.24.2
-      '@babel/generator': 7.24.4
+      '@babel/generator': 7.24.5
       '@babel/helper-environment-visitor': 7.22.20
       '@babel/helper-function-name': 7.23.0
       '@babel/helper-hoist-variables': 7.22.5
-      '@babel/helper-split-export-declaration': 7.22.6
-      '@babel/parser': 7.24.4
-      '@babel/types': 7.24.0
+      '@babel/helper-split-export-declaration': 7.24.5
+      '@babel/parser': 7.24.5
+      '@babel/types': 7.24.5
       debug: 4.3.4
       globals: 11.12.0
     transitivePeerDependencies:
       - supports-color
 
-  '@babel/types@7.24.0':
+  '@babel/types@7.24.5':
     dependencies:
       '@babel/helper-string-parser': 7.24.1
-      '@babel/helper-validator-identifier': 7.22.20
+      '@babel/helper-validator-identifier': 7.24.5
       to-fast-properties: 2.0.0
 
   '@cspotcode/source-map-support@0.8.1':
     dependencies:
       '@jridgewell/trace-mapping': 0.3.9
 
   '@esbuild/aix-ppc64@0.20.2':
@@ -2760,86 +2760,86 @@
   '@nodelib/fs.walk@1.2.8':
     dependencies:
       '@nodelib/fs.scandir': 2.1.5
       fastq: 1.17.1
 
   '@popperjs/core@2.11.8': {}
 
-  '@react-aria/ssr@3.9.2(react@18.3.1)':
+  '@react-aria/ssr@3.9.3(react@18.3.1)':
     dependencies:
       '@swc/helpers': 0.5.11
       react: 18.3.1
 
   '@remix-run/router@1.16.0': {}
 
   '@restart/hooks@0.4.16(react@18.3.1)':
     dependencies:
       dequal: 2.0.3
       react: 18.3.1
 
   '@restart/ui@1.6.8(react-dom@18.3.1(react@18.3.1))(react@18.3.1)':
     dependencies:
-      '@babel/runtime': 7.24.4
+      '@babel/runtime': 7.24.5
       '@popperjs/core': 2.11.8
-      '@react-aria/ssr': 3.9.2(react@18.3.1)
+      '@react-aria/ssr': 3.9.3(react@18.3.1)
       '@restart/hooks': 0.4.16(react@18.3.1)
       '@types/warning': 3.0.3
       dequal: 2.0.3
       dom-helpers: 5.2.1
       react: 18.3.1
       react-dom: 18.3.1(react@18.3.1)
       uncontrollable: 8.0.4(react@18.3.1)
       warning: 4.0.3
 
-  '@rollup/rollup-android-arm-eabi@4.17.1':
+  '@rollup/rollup-android-arm-eabi@4.17.2':
     optional: true
 
-  '@rollup/rollup-android-arm64@4.17.1':
+  '@rollup/rollup-android-arm64@4.17.2':
     optional: true
 
-  '@rollup/rollup-darwin-arm64@4.17.1':
+  '@rollup/rollup-darwin-arm64@4.17.2':
     optional: true
 
-  '@rollup/rollup-darwin-x64@4.17.1':
+  '@rollup/rollup-darwin-x64@4.17.2':
     optional: true
 
-  '@rollup/rollup-linux-arm-gnueabihf@4.17.1':
+  '@rollup/rollup-linux-arm-gnueabihf@4.17.2':
     optional: true
 
-  '@rollup/rollup-linux-arm-musleabihf@4.17.1':
+  '@rollup/rollup-linux-arm-musleabihf@4.17.2':
     optional: true
 
-  '@rollup/rollup-linux-arm64-gnu@4.17.1':
+  '@rollup/rollup-linux-arm64-gnu@4.17.2':
     optional: true
 
-  '@rollup/rollup-linux-arm64-musl@4.17.1':
+  '@rollup/rollup-linux-arm64-musl@4.17.2':
     optional: true
 
-  '@rollup/rollup-linux-powerpc64le-gnu@4.17.1':
+  '@rollup/rollup-linux-powerpc64le-gnu@4.17.2':
     optional: true
 
-  '@rollup/rollup-linux-riscv64-gnu@4.17.1':
+  '@rollup/rollup-linux-riscv64-gnu@4.17.2':
     optional: true
 
-  '@rollup/rollup-linux-s390x-gnu@4.17.1':
+  '@rollup/rollup-linux-s390x-gnu@4.17.2':
     optional: true
 
-  '@rollup/rollup-linux-x64-gnu@4.17.1':
+  '@rollup/rollup-linux-x64-gnu@4.17.2':
     optional: true
 
-  '@rollup/rollup-linux-x64-musl@4.17.1':
+  '@rollup/rollup-linux-x64-musl@4.17.2':
     optional: true
 
-  '@rollup/rollup-win32-arm64-msvc@4.17.1':
+  '@rollup/rollup-win32-arm64-msvc@4.17.2':
     optional: true
 
-  '@rollup/rollup-win32-ia32-msvc@4.17.1':
+  '@rollup/rollup-win32-ia32-msvc@4.17.2':
     optional: true
 
-  '@rollup/rollup-win32-x64-msvc@4.17.1':
+  '@rollup/rollup-win32-x64-msvc@4.17.2':
     optional: true
 
   '@sinclair/typebox@0.27.8': {}
 
   '@swc/helpers@0.5.11':
     dependencies:
       tslib: 2.6.2
@@ -2850,32 +2850,32 @@
 
   '@tsconfig/node14@1.0.3': {}
 
   '@tsconfig/node16@1.0.4': {}
 
   '@types/babel__core@7.20.5':
     dependencies:
-      '@babel/parser': 7.24.4
-      '@babel/types': 7.24.0
+      '@babel/parser': 7.24.5
+      '@babel/types': 7.24.5
       '@types/babel__generator': 7.6.8
       '@types/babel__template': 7.4.4
       '@types/babel__traverse': 7.20.5
 
   '@types/babel__generator@7.6.8':
     dependencies:
-      '@babel/types': 7.24.0
+      '@babel/types': 7.24.5
 
   '@types/babel__template@7.4.4':
     dependencies:
-      '@babel/parser': 7.24.4
-      '@babel/types': 7.24.0
+      '@babel/parser': 7.24.5
+      '@babel/types': 7.24.5
 
   '@types/babel__traverse@7.20.5':
     dependencies:
-      '@babel/types': 7.24.0
+      '@babel/types': 7.24.5
 
   '@types/eslint-scope@3.7.7':
     dependencies:
       '@types/eslint': 8.56.10
       '@types/estree': 1.0.5
 
   '@types/eslint@8.56.10':
@@ -2922,136 +2922,136 @@
 
   '@types/unist@2.0.10': {}
 
   '@types/urijs@1.19.25': {}
 
   '@types/warning@3.0.3': {}
 
-  '@typescript-eslint/eslint-plugin@7.7.1(@typescript-eslint/parser@7.7.1(eslint@8.57.0)(typescript@5.4.5))(eslint@8.57.0)(typescript@5.4.5)':
+  '@typescript-eslint/eslint-plugin@7.8.0(@typescript-eslint/parser@7.8.0(eslint@8.57.0)(typescript@5.4.5))(eslint@8.57.0)(typescript@5.4.5)':
     dependencies:
       '@eslint-community/regexpp': 4.10.0
-      '@typescript-eslint/parser': 7.7.1(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/scope-manager': 7.7.1
-      '@typescript-eslint/type-utils': 7.7.1(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/utils': 7.7.1(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/visitor-keys': 7.7.1
+      '@typescript-eslint/parser': 7.8.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/scope-manager': 7.8.0
+      '@typescript-eslint/type-utils': 7.8.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.8.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/visitor-keys': 7.8.0
       debug: 4.3.4
       eslint: 8.57.0
       graphemer: 1.4.0
       ignore: 5.3.1
       natural-compare: 1.4.0
       semver: 7.6.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
     optionalDependencies:
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
 
-  '@typescript-eslint/parser@7.7.1(eslint@8.57.0)(typescript@5.4.5)':
+  '@typescript-eslint/parser@7.8.0(eslint@8.57.0)(typescript@5.4.5)':
     dependencies:
-      '@typescript-eslint/scope-manager': 7.7.1
-      '@typescript-eslint/types': 7.7.1
-      '@typescript-eslint/typescript-estree': 7.7.1(typescript@5.4.5)
-      '@typescript-eslint/visitor-keys': 7.7.1
+      '@typescript-eslint/scope-manager': 7.8.0
+      '@typescript-eslint/types': 7.8.0
+      '@typescript-eslint/typescript-estree': 7.8.0(typescript@5.4.5)
+      '@typescript-eslint/visitor-keys': 7.8.0
       debug: 4.3.4
       eslint: 8.57.0
     optionalDependencies:
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
 
-  '@typescript-eslint/scope-manager@7.7.1':
+  '@typescript-eslint/scope-manager@7.8.0':
     dependencies:
-      '@typescript-eslint/types': 7.7.1
-      '@typescript-eslint/visitor-keys': 7.7.1
+      '@typescript-eslint/types': 7.8.0
+      '@typescript-eslint/visitor-keys': 7.8.0
 
-  '@typescript-eslint/type-utils@7.7.1(eslint@8.57.0)(typescript@5.4.5)':
+  '@typescript-eslint/type-utils@7.8.0(eslint@8.57.0)(typescript@5.4.5)':
     dependencies:
-      '@typescript-eslint/typescript-estree': 7.7.1(typescript@5.4.5)
-      '@typescript-eslint/utils': 7.7.1(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/typescript-estree': 7.8.0(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.8.0(eslint@8.57.0)(typescript@5.4.5)
       debug: 4.3.4
       eslint: 8.57.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
     optionalDependencies:
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
 
-  '@typescript-eslint/types@7.7.1': {}
+  '@typescript-eslint/types@7.8.0': {}
 
-  '@typescript-eslint/typescript-estree@7.7.1(typescript@5.4.5)':
+  '@typescript-eslint/typescript-estree@7.8.0(typescript@5.4.5)':
     dependencies:
-      '@typescript-eslint/types': 7.7.1
-      '@typescript-eslint/visitor-keys': 7.7.1
+      '@typescript-eslint/types': 7.8.0
+      '@typescript-eslint/visitor-keys': 7.8.0
       debug: 4.3.4
       globby: 11.1.0
       is-glob: 4.0.3
       minimatch: 9.0.4
       semver: 7.6.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
     optionalDependencies:
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
 
-  '@typescript-eslint/utils@7.7.1(eslint@8.57.0)(typescript@5.4.5)':
+  '@typescript-eslint/utils@7.8.0(eslint@8.57.0)(typescript@5.4.5)':
     dependencies:
       '@eslint-community/eslint-utils': 4.4.0(eslint@8.57.0)
       '@types/json-schema': 7.0.15
       '@types/semver': 7.5.8
-      '@typescript-eslint/scope-manager': 7.7.1
-      '@typescript-eslint/types': 7.7.1
-      '@typescript-eslint/typescript-estree': 7.7.1(typescript@5.4.5)
+      '@typescript-eslint/scope-manager': 7.8.0
+      '@typescript-eslint/types': 7.8.0
+      '@typescript-eslint/typescript-estree': 7.8.0(typescript@5.4.5)
       eslint: 8.57.0
       semver: 7.6.0
     transitivePeerDependencies:
       - supports-color
       - typescript
 
-  '@typescript-eslint/visitor-keys@7.7.1':
+  '@typescript-eslint/visitor-keys@7.8.0':
     dependencies:
-      '@typescript-eslint/types': 7.7.1
+      '@typescript-eslint/types': 7.8.0
       eslint-visitor-keys: 3.4.3
 
   '@ungap/structured-clone@1.2.0': {}
 
-  '@vitejs/plugin-react@4.2.1(vite@5.2.10(@types/node@20.11.5)(terser@5.27.0))':
+  '@vitejs/plugin-react@4.2.1(vite@5.2.11(@types/node@20.11.5)(terser@5.27.0))':
     dependencies:
-      '@babel/core': 7.24.4
-      '@babel/plugin-transform-react-jsx-self': 7.24.1(@babel/core@7.24.4)
-      '@babel/plugin-transform-react-jsx-source': 7.24.1(@babel/core@7.24.4)
+      '@babel/core': 7.24.5
+      '@babel/plugin-transform-react-jsx-self': 7.24.5(@babel/core@7.24.5)
+      '@babel/plugin-transform-react-jsx-source': 7.24.1(@babel/core@7.24.5)
       '@types/babel__core': 7.20.5
       react-refresh: 0.14.2
-      vite: 5.2.10(@types/node@20.11.5)(terser@5.27.0)
+      vite: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
     transitivePeerDependencies:
       - supports-color
 
-  '@vitest/expect@1.5.2':
+  '@vitest/expect@1.5.3':
     dependencies:
-      '@vitest/spy': 1.5.2
-      '@vitest/utils': 1.5.2
+      '@vitest/spy': 1.5.3
+      '@vitest/utils': 1.5.3
       chai: 4.4.1
 
-  '@vitest/runner@1.5.2':
+  '@vitest/runner@1.5.3':
     dependencies:
-      '@vitest/utils': 1.5.2
+      '@vitest/utils': 1.5.3
       p-limit: 5.0.0
       pathe: 1.1.2
 
-  '@vitest/snapshot@1.5.2':
+  '@vitest/snapshot@1.5.3':
     dependencies:
       magic-string: 0.30.10
       pathe: 1.1.2
       pretty-format: 29.7.0
 
-  '@vitest/spy@1.5.2':
+  '@vitest/spy@1.5.3':
     dependencies:
       tinyspy: 2.2.1
 
-  '@vitest/utils@1.5.2':
+  '@vitest/utils@1.5.3':
     dependencies:
       diff-sequences: 29.6.3
       estree-walker: 3.0.3
       loupe: 2.3.7
       pretty-format: 29.7.0
 
   '@webassemblyjs/ast@1.12.1':
@@ -3269,18 +3269,18 @@
 
   braces@3.0.2:
     dependencies:
       fill-range: 7.0.1
 
   browserslist@4.23.0:
     dependencies:
-      caniuse-lite: 1.0.30001614
-      electron-to-chromium: 1.4.750
+      caniuse-lite: 1.0.30001615
+      electron-to-chromium: 1.4.754
       node-releases: 2.0.14
-      update-browserslist-db: 1.0.13(browserslist@4.23.0)
+      update-browserslist-db: 1.0.14(browserslist@4.23.0)
 
   buffer-from@1.1.2: {}
 
   cac@6.7.14: {}
 
   call-bind@1.0.7:
     dependencies:
@@ -3288,15 +3288,15 @@
       es-errors: 1.3.0
       function-bind: 1.1.2
       get-intrinsic: 1.2.4
       set-function-length: 1.2.2
 
   callsites@3.1.0: {}
 
-  caniuse-lite@1.0.30001614: {}
+  caniuse-lite@1.0.30001615: {}
 
   chai@4.4.1:
     dependencies:
       assertion-error: 1.1.0
       check-error: 1.0.3
       deep-eql: 4.1.3
       get-func-name: 2.0.2
@@ -3444,18 +3444,18 @@
 
   doctrine@3.0.0:
     dependencies:
       esutils: 2.0.3
 
   dom-helpers@5.2.1:
     dependencies:
-      '@babel/runtime': 7.24.4
+      '@babel/runtime': 7.24.5
       csstype: 3.1.3
 
-  electron-to-chromium@1.4.750: {}
+  electron-to-chromium@1.4.754: {}
 
   emoji-regex@8.0.0: {}
 
   enhanced-resolve@5.16.0:
     dependencies:
       graceful-fs: 4.2.11
       tapable: 2.2.1
@@ -3475,15 +3475,15 @@
       es-errors: 1.3.0
       es-object-atoms: 1.0.0
       es-set-tostringtag: 2.0.3
       es-to-primitive: 1.2.1
       function.prototype.name: 1.1.6
       get-intrinsic: 1.2.4
       get-symbol-description: 1.0.2
-      globalthis: 1.0.3
+      globalthis: 1.0.4
       gopd: 1.0.1
       has-property-descriptors: 1.0.2
       has-proto: 1.0.3
       has-symbols: 1.0.3
       hasown: 2.0.2
       internal-slot: 1.0.7
       is-array-buffer: 3.0.4
@@ -3522,15 +3522,15 @@
       call-bind: 1.0.7
       define-properties: 1.2.1
       es-abstract: 1.23.3
       es-errors: 1.3.0
       es-set-tostringtag: 2.0.3
       function-bind: 1.1.2
       get-intrinsic: 1.2.4
-      globalthis: 1.0.3
+      globalthis: 1.0.4
       has-property-descriptors: 1.0.2
       has-proto: 1.0.3
       has-symbols: 1.0.3
       internal-slot: 1.0.7
       iterator.prototype: 1.1.2
       safe-array-concat: 1.1.2
 
@@ -3821,17 +3821,18 @@
 
   globals@11.12.0: {}
 
   globals@13.24.0:
     dependencies:
       type-fest: 0.20.2
 
-  globalthis@1.0.3:
+  globalthis@1.0.4:
     dependencies:
       define-properties: 1.2.1
+      gopd: 1.0.1
 
   globby@11.1.0:
     dependencies:
       array-union: 2.1.0
       dir-glob: 3.0.1
       fast-glob: 3.3.2
       ignore: 5.3.1
@@ -4136,15 +4137,15 @@
       prelude-ls: 1.2.1
       type-check: 0.4.0
 
   loader-runner@4.3.0: {}
 
   local-pkg@0.5.0:
     dependencies:
-      mlly: 1.6.1
+      mlly: 1.7.0
       pkg-types: 1.1.0
 
   locate-path@6.0.0:
     dependencies:
       p-locate: 5.0.0
 
   lodash.merge@4.6.2: {}
@@ -4197,15 +4198,15 @@
     dependencies:
       brace-expansion: 1.1.11
 
   minimatch@9.0.4:
     dependencies:
       brace-expansion: 2.0.1
 
-  mlly@1.6.1:
+  mlly@1.7.0:
     dependencies:
       acorn: 8.11.3
       pathe: 1.1.2
       pkg-types: 1.1.0
       ufo: 1.5.3
 
   ms@2.1.2: {}
@@ -4333,15 +4334,15 @@
   picocolors@1.0.0: {}
 
   picomatch@2.3.1: {}
 
   pkg-types@1.1.0:
     dependencies:
       confbox: 0.1.7
-      mlly: 1.6.1
+      mlly: 1.7.0
       pathe: 1.1.2
 
   possible-typed-array-names@1.0.0: {}
 
   postcss@8.4.38:
     dependencies:
       nanoid: 3.3.7
@@ -4391,15 +4392,15 @@
   react-bootstrap-icons@1.11.4(react@18.3.1):
     dependencies:
       prop-types: 15.8.1
       react: 18.3.1
 
   react-bootstrap@2.10.2(@types/react@18.3.1)(react-dom@18.3.1(react@18.3.1))(react@18.3.1):
     dependencies:
-      '@babel/runtime': 7.24.4
+      '@babel/runtime': 7.24.5
       '@restart/hooks': 0.4.16(react@18.3.1)
       '@restart/ui': 1.6.8(react-dom@18.3.1(react@18.3.1))(react@18.3.1)
       '@types/react-transition-group': 4.4.10
       classnames: 2.5.1
       dom-helpers: 5.2.1
       invariant: 2.2.4
       prop-types: 15.8.1
@@ -4442,15 +4443,15 @@
     dependencies:
       object-assign: 4.1.1
       react: 18.3.1
       react-is: 18.3.1
 
   react-syntax-highlighter@15.5.0(react@18.3.1):
     dependencies:
-      '@babel/runtime': 7.24.4
+      '@babel/runtime': 7.24.5
       highlight.js: 10.7.3
       lowlight: 1.20.0
       prismjs: 1.29.0
       react: 18.3.1
       refractor: 3.6.0
 
   react-test-renderer@18.3.1(react@18.3.1):
@@ -4458,15 +4459,15 @@
       react: 18.3.1
       react-is: 18.3.1
       react-shallow-renderer: 16.15.0(react@18.3.1)
       scheduler: 0.23.2
 
   react-transition-group@4.4.5(react-dom@18.3.1(react@18.3.1))(react@18.3.1):
     dependencies:
-      '@babel/runtime': 7.24.4
+      '@babel/runtime': 7.24.5
       dom-helpers: 5.2.1
       loose-envify: 1.4.0
       prop-types: 15.8.1
       react: 18.3.1
       react-dom: 18.3.1(react@18.3.1)
 
   react@18.3.1:
@@ -4476,15 +4477,15 @@
   reflect.getprototypeof@1.0.6:
     dependencies:
       call-bind: 1.0.7
       define-properties: 1.2.1
       es-abstract: 1.23.3
       es-errors: 1.3.0
       get-intrinsic: 1.2.4
-      globalthis: 1.0.3
+      globalthis: 1.0.4
       which-builtin-type: 1.1.3
 
   refractor@3.6.0:
     dependencies:
       hastscript: 6.0.0
       parse-entities: 2.0.0
       prismjs: 1.27.0
@@ -4512,43 +4513,43 @@
 
   reusify@1.0.4: {}
 
   rimraf@3.0.2:
     dependencies:
       glob: 7.2.3
 
-  rollup-plugin-visualizer@5.12.0(rollup@4.17.1):
+  rollup-plugin-visualizer@5.12.0(rollup@4.17.2):
     dependencies:
       open: 8.4.2
       picomatch: 2.3.1
       source-map: 0.7.4
       yargs: 17.7.2
     optionalDependencies:
-      rollup: 4.17.1
+      rollup: 4.17.2
 
-  rollup@4.17.1:
+  rollup@4.17.2:
     dependencies:
       '@types/estree': 1.0.5
     optionalDependencies:
-      '@rollup/rollup-android-arm-eabi': 4.17.1
-      '@rollup/rollup-android-arm64': 4.17.1
-      '@rollup/rollup-darwin-arm64': 4.17.1
-      '@rollup/rollup-darwin-x64': 4.17.1
-      '@rollup/rollup-linux-arm-gnueabihf': 4.17.1
-      '@rollup/rollup-linux-arm-musleabihf': 4.17.1
-      '@rollup/rollup-linux-arm64-gnu': 4.17.1
-      '@rollup/rollup-linux-arm64-musl': 4.17.1
-      '@rollup/rollup-linux-powerpc64le-gnu': 4.17.1
-      '@rollup/rollup-linux-riscv64-gnu': 4.17.1
-      '@rollup/rollup-linux-s390x-gnu': 4.17.1
-      '@rollup/rollup-linux-x64-gnu': 4.17.1
-      '@rollup/rollup-linux-x64-musl': 4.17.1
-      '@rollup/rollup-win32-arm64-msvc': 4.17.1
-      '@rollup/rollup-win32-ia32-msvc': 4.17.1
-      '@rollup/rollup-win32-x64-msvc': 4.17.1
+      '@rollup/rollup-android-arm-eabi': 4.17.2
+      '@rollup/rollup-android-arm64': 4.17.2
+      '@rollup/rollup-darwin-arm64': 4.17.2
+      '@rollup/rollup-darwin-x64': 4.17.2
+      '@rollup/rollup-linux-arm-gnueabihf': 4.17.2
+      '@rollup/rollup-linux-arm-musleabihf': 4.17.2
+      '@rollup/rollup-linux-arm64-gnu': 4.17.2
+      '@rollup/rollup-linux-arm64-musl': 4.17.2
+      '@rollup/rollup-linux-powerpc64le-gnu': 4.17.2
+      '@rollup/rollup-linux-riscv64-gnu': 4.17.2
+      '@rollup/rollup-linux-s390x-gnu': 4.17.2
+      '@rollup/rollup-linux-x64-gnu': 4.17.2
+      '@rollup/rollup-linux-x64-musl': 4.17.2
+      '@rollup/rollup-win32-arm64-msvc': 4.17.2
+      '@rollup/rollup-win32-ia32-msvc': 4.17.2
+      '@rollup/rollup-win32-x64-msvc': 4.17.2
       fsevents: 2.3.3
 
   rrweb-cssom@0.6.0: {}
 
   run-parallel@1.2.0:
     dependencies:
       queue-microtask: 1.2.3
@@ -4842,29 +4843,29 @@
       call-bind: 1.0.7
       has-bigints: 1.0.2
       has-symbols: 1.0.3
       which-boxed-primitive: 1.0.2
 
   uncontrollable@7.2.1(react@18.3.1):
     dependencies:
-      '@babel/runtime': 7.24.4
+      '@babel/runtime': 7.24.5
       '@types/react': 18.3.1
       invariant: 2.2.4
       react: 18.3.1
       react-lifecycles-compat: 3.0.4
 
   uncontrollable@8.0.4(react@18.3.1):
     dependencies:
       react: 18.3.1
 
   undici-types@5.26.5: {}
 
   universalify@0.2.0: {}
 
-  update-browserslist-db@1.0.13(browserslist@4.23.0):
+  update-browserslist-db@1.0.14(browserslist@4.23.0):
     dependencies:
       browserslist: 4.23.0
       escalade: 3.1.2
       picocolors: 1.0.0
 
   uri-js@4.4.1:
     dependencies:
@@ -4875,72 +4876,72 @@
   url-parse@1.5.10:
     dependencies:
       querystringify: 2.2.0
       requires-port: 1.0.0
 
   v8-compile-cache-lib@3.0.1: {}
 
-  vite-bundle-visualizer@1.1.0(rollup@4.17.1):
+  vite-bundle-visualizer@1.1.0(rollup@4.17.2):
     dependencies:
       cac: 6.7.14
       import-from-esm: 1.3.4
-      rollup-plugin-visualizer: 5.12.0(rollup@4.17.1)
+      rollup-plugin-visualizer: 5.12.0(rollup@4.17.2)
       tmp: 0.2.3
     transitivePeerDependencies:
       - rollup
       - supports-color
 
-  vite-node@1.5.2(@types/node@20.11.5)(terser@5.27.0):
+  vite-node@1.5.3(@types/node@20.11.5)(terser@5.27.0):
     dependencies:
       cac: 6.7.14
       debug: 4.3.4
       pathe: 1.1.2
       picocolors: 1.0.0
-      vite: 5.2.10(@types/node@20.11.5)(terser@5.27.0)
+      vite: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
     transitivePeerDependencies:
       - '@types/node'
       - less
       - lightningcss
       - sass
       - stylus
       - sugarss
       - supports-color
       - terser
 
-  vite@5.2.10(@types/node@20.11.5)(terser@5.27.0):
+  vite@5.2.11(@types/node@20.11.5)(terser@5.27.0):
     dependencies:
       esbuild: 0.20.2
       postcss: 8.4.38
-      rollup: 4.17.1
+      rollup: 4.17.2
     optionalDependencies:
       '@types/node': 20.11.5
       fsevents: 2.3.3
       terser: 5.27.0
 
-  vitest@1.5.2(@types/node@20.11.5)(jsdom@24.0.0)(terser@5.27.0):
+  vitest@1.5.3(@types/node@20.11.5)(jsdom@24.0.0)(terser@5.27.0):
     dependencies:
-      '@vitest/expect': 1.5.2
-      '@vitest/runner': 1.5.2
-      '@vitest/snapshot': 1.5.2
-      '@vitest/spy': 1.5.2
-      '@vitest/utils': 1.5.2
+      '@vitest/expect': 1.5.3
+      '@vitest/runner': 1.5.3
+      '@vitest/snapshot': 1.5.3
+      '@vitest/spy': 1.5.3
+      '@vitest/utils': 1.5.3
       acorn-walk: 8.3.2
       chai: 4.4.1
       debug: 4.3.4
       execa: 8.0.1
       local-pkg: 0.5.0
       magic-string: 0.30.10
       pathe: 1.1.2
       picocolors: 1.0.0
       std-env: 3.7.0
       strip-literal: 2.1.0
       tinybench: 2.8.0
       tinypool: 0.8.4
-      vite: 5.2.10(@types/node@20.11.5)(terser@5.27.0)
-      vite-node: 1.5.2(@types/node@20.11.5)(terser@5.27.0)
+      vite: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
+      vite-node: 1.5.3(@types/node@20.11.5)(terser@5.27.0)
       why-is-node-running: 2.2.2
     optionalDependencies:
       '@types/node': 20.11.5
       jsdom: 24.0.0
     transitivePeerDependencies:
       - less
       - lightningcss
```

### Comparing `bowtie_json_schema-2024.5.1/frontend/tsconfig.json` & `bowtie_json_schema-2024.5.2/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/public/favicon.svg` & `bowtie_json_schema-2024.5.2/frontend/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/DialectReportView.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/DialectReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/ReportDataHandler.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/ReportDataHandler.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/index.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/assets/landscape-logo.svg` & `bowtie_json_schema-2024.5.2/frontend/src/assets/landscape-logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/CopyToClipboard.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/CopyToClipboard.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/FilterSection.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/FilterSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/NavBar.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/NavBar.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/OtherImplementations.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/OtherImplementations.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/Cases/CaseItem.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/Cases/CaseItem.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/Cases/CaseResultSvg.test.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/Cases/CaseResultSvg.test.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/Cases/CaseResultSvg.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/Cases/CaseResultSvg.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/Cases/CasesSection.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/Cases/CasesSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/Cases/SchemaDisplay.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/Cases/SchemaDisplay.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/DragAndDrop/DragAndDrop.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/DragAndDrop/DragAndDrop.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/ImplementationReportView/DialectCompliance.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/ImplementationReportView/DialectCompliance.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   implementationReport: ImplementationReport;
 }> = ({ implementationReport }) => {
   const { implementation, dialectCompliance } = implementationReport;
 
   return (
     <Card className="mx-auto mb-3 col-md-9">
       <Card.Header>Compliance</Card.Header>
-      <Card.Body>
+      <Card.Body className="overflow-x-auto">
         <Table className="table-hover sm">
           <thead>
             <tr>
               <th rowSpan={2} scope="col" className="text-center align-middle">
                 Supported Dialects
               </th>
               <th colSpan={3} className="text-center">
```

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
               {mapLanguage(implementation.language)}
             </span>
             <span>{implementation.name}</span>
           </span>
           <EmbedBadges implementation={implementation} />
         </Card.Header>
 
-        <Card.Body>
+        <Card.Body className="overflow-x-auto">
           <Table>
             <tbody>
               <tr>
                 <th>Homepage</th>
                 <td>
                   <Link to={implementation.homepage}>
                     {implementation.homepage}
```

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/Modals/DetailsButtonModal.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/Modals/DetailsButtonModal.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/RunInfo/RunInfoSection.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/RunInfo/RunInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2024.5.2/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/Summary/ImplementationRow.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/Summary/ImplementationRow.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/Summary/SummarySection.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/Summary/SummarySection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/components/Summary/SummaryTable.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/components/Summary/SummaryTable.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/context/BowtieVersionContext.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/context/BowtieVersionContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/context/ThemeContext.tsx` & `bowtie_json_schema-2024.5.2/frontend/src/context/ThemeContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/data/Badge.test.ts` & `bowtie_json_schema-2024.5.2/frontend/src/data/Badge.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/data/Badge.ts` & `bowtie_json_schema-2024.5.2/frontend/src/data/Badge.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/data/Dialect.ts` & `bowtie_json_schema-2024.5.2/frontend/src/data/Dialect.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/data/Site.test.ts` & `bowtie_json_schema-2024.5.2/frontend/src/data/Site.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/data/parseReportData.test.ts` & `bowtie_json_schema-2024.5.2/frontend/src/data/parseReportData.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2024.5.2/frontend/src/data/parseReportData.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/.java-implementations-pmd-ruleset.xml` & `bowtie_json_schema-2024.5.2/implementations/.java-implementations-pmd-ruleset.xml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/clojure-json-schema/Dockerfile` & `bowtie_json_schema-2024.5.2/implementations/clojure-json-schema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj` & `bowtie_json_schema-2024.5.2/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/cpp-valijson/bowtie_valijson.cpp` & `bowtie_json_schema-2024.5.2/implementations/cpp-valijson/bowtie_valijson.cpp`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/dotnet-jsonschema-net/.gitignore` & `bowtie_json_schema-2024.5.2/implementations/dotnet-jsonschema-net/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/dotnet-jsonschema-net/Program.cs` & `bowtie_json_schema-2024.5.2/implementations/dotnet-jsonschema-net/Program.cs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/go-gojsonschema/bowtie_gojsonschema.go` & `bowtie_json_schema-2024.5.2/implementations/go-gojsonschema/bowtie_gojsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/go-gojsonschema/go.sum` & `bowtie_json_schema-2024.5.2/implementations/go-gojsonschema/go.sum`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/go-jsonschema/bowtie_jsonschema.go` & `bowtie_json_schema-2024.5.2/implementations/go-jsonschema/bowtie_jsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-json-schema/BowtieJsonSchema.java` & `bowtie_json_schema-2024.5.2/implementations/java-json-schema/BowtieJsonSchema.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-json-schema/build.gradle` & `bowtie_json_schema-2024.5.2/implementations/java-json-schema/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.5.2/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.5.2/implementations/java-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java` & `bowtie_json_schema-2024.5.2/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-jsonschemafriend/build.gradle` & `bowtie_json_schema-2024.5.2/implementations/java-jsonschemafriend/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/build.gradle.kts` & `bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/justfile` & `bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/justfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/gradle/libs.versions.toml` & `bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/gradle/libs.versions.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt` & `bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/Support.kt` & `bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/Support.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt` & `bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt` & `bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt` & `bowtie_json_schema-2024.5.2/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/js-ajv/bowtie_ajv.js` & `bowtie_json_schema-2024.5.2/implementations/js-ajv/bowtie_ajv.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/js-ajv/package-lock.json` & `bowtie_json_schema-2024.5.2/implementations/js-ajv/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/js-hyperjump/bowtie_hyperjump.js` & `bowtie_json_schema-2024.5.2/implementations/js-hyperjump/bowtie_hyperjump.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/js-jsonschema/bowtie_jsonschema.js` & `bowtie_json_schema-2024.5.2/implementations/js-jsonschema/bowtie_jsonschema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts` & `bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt` & `bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt` & `bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt` & `bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt` & `bowtie_json_schema-2024.5.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/lua-jsonschema/Dockerfile` & `bowtie_json_schema-2024.5.2/implementations/lua-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/lua-jsonschema/bowtie_jsonschema.lua` & `bowtie_json_schema-2024.5.2/implementations/lua-jsonschema/bowtie_jsonschema.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/lua-jsonschema/json.lua` & `bowtie_json_schema-2024.5.2/implementations/lua-jsonschema/json.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/php-opis-json-schema/bowtieJsonSchema.php` & `bowtie_json_schema-2024.5.2/implementations/php-opis-json-schema/bowtieJsonSchema.php`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/python-fastjsonschema/bowtie_fastjsonschema.py` & `bowtie_json_schema-2024.5.2/implementations/python-fastjsonschema/bowtie_fastjsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/python-jschon/bowtie_jschon.py` & `bowtie_json_schema-2024.5.2/implementations/python-jschon/bowtie_jschon.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/python-jsonschema/bowtie_jsonschema.py` & `bowtie_json_schema-2024.5.2/implementations/python-jsonschema/bowtie_jsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/ruby-json_schemer/bowtie_json_schemer.rb` & `bowtie_json_schema-2024.5.2/implementations/ruby-json_schemer/bowtie_json_schemer.rb`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/rust-boon/Cargo.lock` & `bowtie_json_schema-2024.5.2/implementations/rust-boon/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/rust-boon/Dockerfile` & `bowtie_json_schema-2024.5.2/implementations/rust-boon/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/rust-boon/src/main.rs` & `bowtie_json_schema-2024.5.2/implementations/rust-boon/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/rust-jsonschema/Cargo.lock` & `bowtie_json_schema-2024.5.2/implementations/rust-jsonschema/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -937,26 +937,26 @@
 checksum = "836fa6a3e1e547f9a2c4040802ec865b5d85f4014efe00555d7090a3dcaa1090"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `bowtie_json_schema-2024.5.1/implementations/rust-jsonschema/Dockerfile` & `bowtie_json_schema-2024.5.2/implementations/rust-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/rust-jsonschema/src/main.rs` & `bowtie_json_schema-2024.5.2/implementations/rust-jsonschema/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/scala-mjs-validator/Harness.scala` & `bowtie_json_schema-2024.5.2/implementations/scala-mjs-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/scala-mjs-validator/build.sbt` & `bowtie_json_schema-2024.5.2/implementations/scala-mjs-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/scala-rc-circe-json-validator/Harness.scala` & `bowtie_json_schema-2024.5.2/implementations/scala-rc-circe-json-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/scala-rc-circe-json-validator/build.sbt` & `bowtie_json_schema-2024.5.2/implementations/scala-rc-circe-json-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts` & `bowtie_json_schema-2024.5.2/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/tests/test_github.py` & `bowtie_json_schema-2024.5.2/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/tests/test_hypothesis.py` & `bowtie_json_schema-2024.5.2/tests/test_hypothesis.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,14 +33,34 @@
         implementations=strategies.implementations(min_size=n, max_size=n),
     )
     seq_cases, results = data.draw(strategy)
     # all implementations have results
     assert len(results) == n * len(seq_cases)
 
 
+@given(strategies.cases_and_results())
+@settings(suppress_health_check=[HealthCheck.too_slow])
+def test_cases_and_results_generates_correct_test_results(cases_results):
+    """
+    The number of test results for each test case matches the number of tests.
+    """
+    seq_cases, seq_results = cases_results
+    for seq_case in seq_cases:
+        results = [
+            seq_result.result
+            for seq_result in seq_results
+            if seq_result.seq == seq_case.seq
+        ]
+        assert all(
+            len([each.result_for(i) for i in range(len(seq_case.case.tests))])
+            == len(seq_case.case.tests)
+            for each in results
+        )
+
+
 @given(strategies.cases_and_results(min_cases=2))  # no point for 1
 @settings(suppress_health_check=[HealthCheck.too_slow])
 def test_cases_are_unique_by_default(cases_results):
     seq_cases, _ = cases_results
     assert len({each.case.uniq() for each in seq_cases}) == len(seq_cases)
 
 
@@ -66,15 +86,30 @@
 @given(strategies.known_dialects)
 def test_known_dialects(dialect):
     assert dialect.uri.host_str == "json-schema.org"
 
 
 @given(strategies.report_data())
 @settings(suppress_health_check=[HealthCheck.too_slow], deadline=None)
-def test_report_data_generates_implementations_with_metadata(data):
-    assert Report.from_input(data).implementations
+def test_report_data_generates_implementations_which_support_the_dialect(data):
+    report = Report.from_input(data)
+    assert all(
+        report.metadata.dialect in each.dialects
+        for each in report.implementations
+    )
+
+
+@given(strategies.report_data())
+@settings(suppress_health_check=[HealthCheck.too_slow], deadline=None)
+def test_report_data_generates_boolean_schemas_only_when_supported(data):
+    report = Report.from_input(data)
+    if not report.metadata.dialect.has_boolean_schemas:
+        assert not any(
+            isinstance(case.schema, bool)
+            for case, _ in report.cases_with_results()
+        )
 
 
 @given(strategies.report_data(fail_fast=just(True)))
 @settings(suppress_health_check=[HealthCheck.too_slow], deadline=None)
 def test_report_data_can_be_marked_fail_fast(data):
     assert Report.from_input(data).did_fail_fast
```

### Comparing `bowtie_json_schema-2024.5.1/tests/test_integration.py` & `bowtie_json_schema-2024.5.2/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,22 @@
 from jsonschema.validators import validator_for
 from markdown_it import MarkdownIt
 from markdown_it.tree import SyntaxTreeNode
 import pexpect
 import pytest
 import pytest_asyncio
 
-from bowtie._cli import bowtie_schemas_registry
 from bowtie._commands import ErroredTest, TestResult
-from bowtie._core import Dialect, Implementation, Test, TestCase
+from bowtie._core import (
+    Dialect,
+    Implementation,
+    Test,
+    TestCase,
+    bowtie_schemas_registry,
+)
 from bowtie._report import EmptyReport, InvalidReport, Report
 
 Test.__test__ = TestCase.__test__ = TestResult.__test__ = (
     False  # frigging py.test
 )
```

### Comparing `bowtie_json_schema-2024.5.1/tests/test_report.py` & `bowtie_json_schema-2024.5.2/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/tests/test_schemas.py` & `bowtie_json_schema-2024.5.2/tests/test_schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 Test Bowtie's schemas for proper functionality.
 """
 
 from jsonschema.validators import validator_for
 import pytest
 
-from bowtie._cli import bowtie_schemas_registry
-from bowtie._core import Dialect
+from bowtie._core import Dialect, bowtie_schemas_registry
 
 DRAFT2020 = Dialect.by_alias()["2020"]
 REGISTRY = DRAFT2020.current_dialect_resource() @ bowtie_schemas_registry()
 
 TEST = {
     "description": "a test",
     "instance": 37,
```

### Comparing `bowtie_json_schema-2024.5.1/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2024.5.2/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/cli/info.json` & `bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json` & `bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/io/v1.json` & `bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2222222222222222%*

 * *Differences: {"'$id'": "'tag:bowtie.report,2024:models:dialect'",*

 * * "'additionalProperties'": 'False',*

 * * "'description'": "'Dialect metadata for a dialect of JSON Schema'",*

 * * "'properties'": "OrderedDict([('uri', OrderedDict([('description', 'The URI representing this "*

 * *                 "dialect, also known as its dialect identifier'), ('readOnly', True), ('type', "*

 * *                 "'string'), ('format', 'uri')])), ('prettyName', OrderedDict([('description', 'A "*

 * *                 "human-readable name for the dialect'), (' […]*

```diff
@@ -1,76 +1,53 @@
 {
-    "$defs": {
-        "case": {
-            "$anchor": "case",
-            "additionalProperties": false,
-            "description": "An individual test case, consisting of a single schema and one or more instances to validate under it",
-            "properties": {
-                "comment": {
-                    "description": "Any additional comments about the test case",
-                    "type": "string"
-                },
-                "description": {
-                    "description": "A (human-readable) short description of this test case",
-                    "type": "string"
-                },
-                "registry": {
-                    "description": "A collection of schemas (with URIs) which tests may reference (via $ref) and expect to be retrievable. They should be registered in whatever mechanism is expected by the implementation.",
-                    "propertyNames": {
-                        "format": "uri"
-                    },
-                    "type": "object"
-                },
-                "schema": {
-                    "$comment": "the URI used here is a sort of 'magic' URI set by Bowtie during runs, which will resolve to (effectively) the meta-schema for the current dialect being run by Bowtie. E.g. when running tests using the Draft 2020-12 dialect, the URI will resolve to the schema `{\"$ref\": \"https://json-schema.org/draft/2020-12/schema\"}`. This sort of dynamically set value is necessary, as schemas are supposed to be valid under the current dialect being spoken by Bowtie, but that's not known until runtime.",
-                    "$ref": "tag:bowtie.report,2023:ihop:__dialect__",
-                    "description": "A valid JSON Schema."
-                },
-                "tests": {
-                    "description": "A set of related tests all using the same schema",
-                    "items": {
-                        "$ref": "tag:bowtie.report,2023:models:test"
-                    },
-                    "minItems": 1,
-                    "type": "array"
-                }
+    "$id": "tag:bowtie.report,2024:models:dialect",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
+    "additionalProperties": false,
+    "description": "Dialect metadata for a dialect of JSON Schema",
+    "properties": {
+        "aliases": {
+            "default": [],
+            "description": "Other names by which someone may refer to this dialect, officially or otherwise. Such aliases should unambiguously refer to this dialect and no other, so they should be unique not just in the array but also globally, though they may be so short so as to never be used in practice other than when it is clear that dialects are being referred to. For instance simply the number '7' is so short that no one would likely use it in conversation, but would unambiguously refer to the Draft 7 dialect. The dialect's short name is implicitly considered an alias, so it need not appear in this list but should generally be included when using these aliases.",
+            "items": {
+                "type": "string"
             },
-            "required": [
-                "description",
-                "schema",
-                "tests"
-            ],
-            "type": "object"
+            "type": "array",
+            "uniqueItems": true
+        },
+        "firstPublicationDate": {
+            "description": "The date when the dialect was first published publicly as a document",
+            "format": "date",
+            "readOnly": true,
+            "type": "string"
+        },
+        "hasBooleanSchemas": {
+            "default": true,
+            "description": "Does the dialect have a notion of boolean schemas?",
+            "readOnly": true,
+            "type": "boolean"
         },
-        "command": {
-            "oneOf": [
-                {
-                    "$ref": "tag:bowtie.report,2023:ihop:command:start"
-                },
-                {
-                    "$ref": "tag:bowtie.report,2023:ihop:command:dialect"
-                },
-                {
-                    "$ref": "tag:bowtie.report,2023:ihop:command:run"
-                },
-                {
-                    "$ref": "tag:bowtie.report,2023:ihop:command:stop"
-                }
-            ],
-            "required": [
-                "cmd"
-            ],
-            "type": "object",
-            "unevaluatedProperties": false
+        "prettyName": {
+            "description": "A human-readable name for the dialect",
+            "readOnly": true,
+            "type": "string"
         },
-        "version": {
-            "$anchor": "version",
-            "const": 1,
-            "description": "The current version of this protocol, to be incremented if changed",
-            "type": "integer"
+        "shortName": {
+            "description": "A shorter, slug-like name for the dialect (with no punctuation or spaces) but which still should be unique",
+            "pattern": "[a-z]+[a-z0-9-]*",
+            "readOnly": true,
+            "type": "string"
+        },
+        "uri": {
+            "description": "The URI representing this dialect, also known as its dialect identifier",
+            "format": "uri",
+            "readOnly": true,
+            "type": "string"
         }
     },
-    "$id": "tag:bowtie.report,2023:ihop",
-    "$schema": "https://json-schema.org/draft/2020-12/schema",
-    "description": "Input/output specification for Bowtie, a meta-validator for JSON Schema validator implementations",
-    "title": "Bowtie IO Protocol"
+    "required": [
+        "firstPublicationDate",
+        "prettyName",
+        "shortName",
+        "uri"
+    ],
+    "type": "object"
 }
```

### Comparing `bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json` & `bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json` & `bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json` & `bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/tests/fauxmplementations/lintsonschema/schemas/models/test.json` & `bowtie_json_schema-2024.5.2/tests/fauxmplementations/lintsonschema/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/.gitignore` & `bowtie_json_schema-2024.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/LICENSE` & `bowtie_json_schema-2024.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/README.rst` & `bowtie_json_schema-2024.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/hatch_build.py` & `bowtie_json_schema-2024.5.2/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/pyproject.toml` & `bowtie_json_schema-2024.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.1/PKG-INFO` & `bowtie_json_schema-2024.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bowtie-json-schema
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://docs.bowtie.report/
 Project-URL: Homepage, https://bowtie.report/
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author-email: Julian Berman <Julian+bowtie@GrayVines.com>
```


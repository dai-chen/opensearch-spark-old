# OpenSearch Flint

OpenSearch Flint is ... It consists of two modules:

- `flint-core`: a module that contains Flint specification and client.
- `flint-spark-integration`: a module that provides Spark integration for Flint and derived dataset based on it.

## Documentation

Please refer to the [Flint Index Reference Manual](./docs/index.md) for more information.

## Prerequisites

+ Spark 3.3.1
+ Scala 2.12.14

## Usage

To use this application, you can run Spark with Flint extension:

```
spark-sql --conf "spark.sql.extensions=org.opensearch.flint.FlintSparkExtensions"
```

## Build

To build and run this application with Spark, you can run:

```
sbt clean standaloneCosmetic/publishM2
```
then add org.opensearch:opensearch-spark_2.12 when run spark application, for example,
```
bin/spark-shell --packages "org.opensearch:opensearch-spark_2.12:0.1.0-SNAPSHOT"
```

## Code of Conduct

This project has adopted an [Open Source Code of Conduct](../CODE_OF_CONDUCT.md).

## Security

If you discover a potential security issue in this project we ask that you notify AWS/Amazon Security via our [vulnerability reporting page](http://aws.amazon.com/security/vulnerability-reporting/). Please do **not** create a public GitHub issue.

## License

See the [LICENSE](../LICENSE.txt) file for our project's licensing. We will ask you to confirm the licensing of your contribution.

## Copyright

Copyright OpenSearch Contributors. See [NOTICE](../NOTICE) for details.

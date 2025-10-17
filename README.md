# YesSQL!
A curated list of creative, amazing ways to use SQL.

This list is a result of the constant research activities we do at [Vettabase](https://vettabase.com).

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) Inspired by the `awesome-*` trend on GitHub.

## What's in the Name

YesSQL! is a late reaction to NoSQL.

NoSQL is negative marketing. It advertised itself as a movement of databases missing an SQL interface. They described SQL as something old, frustrating, that doesn't scale.
They had no feature in common. The whole NoSQL marketing was based on a negative statement: the lack of a feature.
But negative marketing has a fundamental problem: it says almost nothing about what you're trying to promote.
Technically an asteroid, a cat and a piece of wood are all NoSQL, as they lack an SQL interface.

Later, the wind changed. NoSQL databases started to implement NoSQL. For example, Cassandra has an SQL subset that makes sense for their domain, and called it CQL.
And they tried to convince us that they never meant "no SQL", they actually meant "Not Only SQL". They even wrote this on Wikipedia. But those of us who were there
know that it's a lie.

Now, the trend is exactly the opposite: using SQL in new, creative ways! New software projects implement SQL in completely unexpected contexts.
This list contains projects of this type.

## YesSQL! List

* [Apache Calcite](https://calcite.apache.org/) - A Java framework that processes SQL queries and uses them to read data from heterogeneous data sources. [Adapters](https://calcite.apache.org/docs/adapter.html) implement access to different data sources.
* [Dolt](https://www.doltlab.com/)(MySQL-compatible) and [DoltgreSQL](https://github.com/dolthub/doltgresql) (Postgres-compatible) - Databases with git-like capabilities, implemented via Go stored procedures. Databases can also be pushed to the public [DoltHub](https://www.dolthub.com/) or private hubs. Data versioning is useful to create different versions of a database, keeping all versions updated. A possible use case is what-if analysis.
* [IaSQL](https://iasql.com/) - PostgreSQL-based database that allows to see an AWS infrastructure data in a relational way. Data can be modified in SQL. When a transaction is committed, changes are applied to the infrastructure using the AWS API.
* [ksqlDB](https://www.confluent.io/product/ksqldb/) - An SQL database that streams data from Kafka.
* [MindsDB](https://mindsdb.com/) - An SQL interface that reads data from heterogeneous data sources and can answer queries about the future. Future data are generated using machine learning algorithms. Many prediction modules are supported, including external APIs. More [integrations](https://github.com/mindsdb/mindsdb/tree/main/mindsdb/integrations/handlers) can easily be implemented as Python modules. This includes models and data sources. Both MySQL and PostgreSQL dialects are supported, as well as non-SQL interfaces.
* [osquery](https://osquery.io/) - Shows information about the system where osquery is installed, in a relational manner. Suitable for servers, laptops, Docker servers, Ec2 instances, and more. It can run as a daemon or it can run just when it's invoked to run a query.
* [Steampipe](https://steampipe.io/) - Based on PostgreSQL or SQLite, it's designed to show information from any API as relational data. New plugins can be implemented in Go. Many plugins exist to read data from cloud infrastructures, business applications, and more.
* [Trino](https://trino.io/) - A distributed SQL engine to run queries across heterogeneous data sources.

It's also worth mentioning that some traditional relational databases support reading heterogenous, non-relational data sources and see them as local tables:
* [MariaDB CONNECT](https://mariadb.com/docs/server/server-usage/storage-engines/connect/introduction-to-the-connect-engine)
* [PostgreSQL FDW](https://wiki.postgresql.org/wiki/Foreign_data_wrappers)


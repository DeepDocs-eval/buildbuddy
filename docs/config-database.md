---
id: config-database
title: Database Configuration
sidebar_label: Database
---

## Section

`database:` The database section configures the database that BuildBuddy stores metadata in. **Required**

## Options

**Required**

- `driver` The driver to use: one of sqlite3, mysql, or postgresql.
- `endpoint` Typically the host:port combination or file path for SQLite.

## Example sections

### SQLite

```yaml title="config.yaml"
database:
  data_source: "sqlite3:///tmp/buildbuddy.db"
```

### MySQL

```yaml title="config.yaml"
database:
  data_source: "mysql://buildbuddy_user:pAsSwOrD@tcp(12.34.56.78)/buildbuddy_db"
```

### PostgreSQL

```yaml title="config.yaml"
database:
  data_source: "postgresql://buildbuddy_user:pAsSwOrD@12.34.56.78:5433/buildbuddy_db"
```

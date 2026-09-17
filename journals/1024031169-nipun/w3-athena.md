# Week 3 — Database Implementation, PostgreSQL Migration and Project Repository

## Problem / Challenge

The main technical task during this week was implementing the database planned during the previous week.

Initially, we wanted a simple way to create and test the database without setting up a complete database server environment. Therefore, SQLite was selected for the initial implementation.

However, after creating and testing the database structure, we decided to migrate the database to PostgreSQL so that the project could use a more suitable relational database system for further development.

A second challenge was organizing the project files and documentation in a Git repository according to the required project structure.

## Problems Faced
1. SQLite to PostgreSQL Migration

The initial database was created in SQLite, but the project later required PostgreSQL.
This required checking the database schema and ensuring that tables, relationships and data types were compatible with PostgreSQL.

2. Git Push Rejection

While pushing the project to GitHub, the following error was encountered:
```text
! [rejected] main -> main (fetch first)
```

error: failed to push some refs to the remote repository

The issue occurred because the remote repository already contained commits that were not present in the local repository.
The local repository therefore had to synchronize with the remote repository before pushing the local changes.

## Solution

The database was first created and tested using SQLite.
After validating the schema, the database structure was converted to PostgreSQL.

The migration process involved:
```text
Database Design
      ↓
SQLite Implementation
      ↓
Schema Testing
      ↓
PostgreSQL Conversion
      ↓
PostgreSQL Database
```
The relational structure and foreign-key relationships were retained during the migration.


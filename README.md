# Periodic Table Database

This repository contains my solution for the **Build a Periodic Table Database** project from the **freeCodeCamp Relational Database Certification**.

## Project Overview

The project uses a PostgreSQL database to store information about chemical elements and a Bash script to retrieve element data from the command line.

The `element.sh` script accepts an atomic number, chemical symbol, or element name as an argument and returns the corresponding information from the database.

Example:

```bash
./element.sh 1
```

or:

```bash
./element.sh H
```

or:

```bash
./element.sh Hydrogen
```

The output includes:

* Atomic number
* Element name
* Chemical symbol
* Element type
* Atomic mass
* Melting point
* Boiling point

If no argument is provided, the script asks the user to provide an element. If the element cannot be found in the database, an appropriate message is displayed.

## Technologies

* PostgreSQL
* SQL
* Bash
* Git

## Files

* `element.sh` — Bash script used to query the database and display element information.
* `periodic_table.sql` — PostgreSQL database dump containing the database structure and data.

## Database Structure

The database is organized around the following main tables:

* `elements`
* `properties`
* `types`

The script retrieves data by joining these tables using the atomic number and element type identifiers.

## Certification

This project was completed as part of the **freeCodeCamp Relational Database Certification**.

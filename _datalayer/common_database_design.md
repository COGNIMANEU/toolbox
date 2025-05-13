---
title: "Database Design for Manufacturing Data"
weight: 1
description: "The system provides a unified interface for interacting with different database backends (PostgreSQL, MySQL, SQLite) while maintaining consistent behavior across applications. It implements an adapter design pattern that allows for switching between different database systems with minimal code changes."
license: "https://img.shields.io/badge/License-Unlicense-lightgrey"
trl: "https://img.shields.io/badge/TRL-7-green"
link: "https://github.com/COGNIMANEU/pilot03-data-common-database-design"
github: "https://github.com/COGNIMANEU/pilot03-data-common-database-design"
---

## Name
Database Design for Manufacturing Data

## Description
The system provides a unified interface for interacting with different database backends (PostgreSQL, MySQL, SQLite) while maintaining consistent behavior across applications. It implements an adapter design pattern that allows for switching between different database systems with minimal code changes.

### Features

- Modular architecture with manager classes for different data types
- Support for PostgreSQL, MySQL, and SQLite backends
- Consistent API for CRUD operations across database types
- Type hinting for better developer experience
- Comprehensive error handling and logging
- Environment-based configuration
- Support for JSON data storage and retrieval

## Type
Design

## Layer
Database

## HRL
3.0

## Partners
Montimage, IRT, CROOM

## Pilot
Pilot 03 - CROOM

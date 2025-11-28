# MongoDB - Step by Step Tutorial

Practical MongoDB tutorial with examples organized by topic, based on [Platzi's MongoDB course](https://github.com/platzi/curso-mongodb-intro).

## Requirements

- Docker and Docker Compose
- MongoDB extension for VSCode (to run .mongodb files)

## Installation

1. Start MongoDB with Docker:
```bash
docker-compose up -d
```

2. MongoDB will be available at `localhost:27017`

## Project Structure

This repository contains two main learning paths:

### 📁 `src/` - Advanced Topics (Schema Design & Relationships)

Advanced MongoDB concepts focusing on data modeling, validations, and relationship patterns.

**Validations**
- [01-test](src/01-test) - Initial connection and test
- [02-validation-string](src/02-validation-string) - String validation
- [03-validation-numbers](src/03-validation-numbers) - Number validation
- [04-validation-subdocs](src/04-validation-subdocs) - Subdocument validation
- [05-validation-regex](src/05-validation-regex) - Validation with regular expressions
- [06-validation-tips](src/06-validation-tips) - Validation tips

**Relationships**
- [07-1-1-embed](src/07-1-1-embed) - 1-to-1 embedded relationship
- [08-1-1-referenced](src/08-1-1-referenced) - 1-to-1 referenced relationship
- [09-1-N-embed](src/09-1-N-embed) - 1-to-N embedded relationship
- [10-1-N-referenced](src/10-1-N-referenced) - 1-to-N referenced relationship
- [11-N-N](src/11-N-N) - N-to-N relationship
- [12-N-N-circular](src/12-N-N-circular) - N-to-N circular relationship

**Patterns & Optimization**
- [13-desnormalization](src/13-desnormalization) - Denormalization
- [14-pattern-computed](src/14-pattern-computed) - Computed pattern
- [15-dropping-db](src/15-dropping-db) - Drop database

### 📁 `src_old/` - Fundamentals (CRUD & Query Operations)

Basic MongoDB operations and query fundamentals.

**Getting Started**
- [01-playground](src_old/01-playground) - MongoDB playground introduction
- [02-docker](src_old/02-docker) - Docker setup
- [03-mongosh](src_old/03-mongosh) - MongoDB Shell basics

**CRUD Operations**
- [04-insert-doc](src_old/04-insert-doc) - Insert single document
- [05-insert-many-docs](src_old/05-insert-many-docs) - Insert multiple documents
- [07-update-mani-docs](src_old/07-update-mani-docs) - Update multiple documents
- [08-update-arrays](src_old/08-update-arrays) - Update arrays
- [09-upsert](src_old/09-upsert) - Upsert operations
- [10-delete-docs](src_old/10-delete-docs) - Delete documents

**Query Operators**
- [11-eq-ne](src_old/11-eq-ne) - Equality and inequality operators
- [12-operators](src_old/12-operators) - Comparison operators
- [13-examples-operators copy](src_old/13-examples-operators copy) - Operator examples
- [14-regex](src_old/14-regex) - Regular expressions in queries
- [17-logic-operators](src_old/17-logic-operators) - Logical operators (AND, OR, NOT)
- [18-expresive-operators](src_old/18-expresive-operators) - Expressive operators

**Advanced Queries**
- [15-projection](src_old/15-projection) - Field projection
- [16-query-array](src_old/16-query-array) - Query arrays
- [19-array-subdocs](src_old/19-array-subdocs) - Arrays and subdocuments
- [20-aggregation](src_old/20-aggregation) - Aggregation framework
- [21-sort-limit](src_old/21-sort-limit) - Sorting, limiting, and pagination

## Usage

Each folder contains `.mongodb` files that you can run directly in VSCode with the MongoDB extension.

Example:
```javascript
use("database_name")
db.collection.find()
```

## Learning Path

**Recommended order:**

1. Start with `src_old/` to learn MongoDB fundamentals (CRUD, queries, operators)
2. Move to `src/` for advanced topics (schema design, validations, relationships, patterns)

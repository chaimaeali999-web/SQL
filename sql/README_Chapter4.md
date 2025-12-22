# Chapter 4 -- Creating Tables with Data Types and Constraints

## Objective

Be able to create SQL tables by choosing appropriate data types and
defining basic constraints to ensure data integrity.

## Key Concepts

-   CREATE TABLE statement
-   Data types: INT, VARCHAR, TEXT, DATE, BOOLEAN
-   Primary key (PRIMARY KEY)
-   Constraints: NOT NULL, UNIQUE, DEFAULT, AUTO_INCREMENT
-   Foreign key (FOREIGN KEY)

## Theory

The CREATE TABLE command is used to define the structure of a table. - A
primary key uniquely identifies each record. - Foreign keys create
relationships between tables and maintain consistency.

## Example

``` sql
CREATE TABLE Utilisateur (
  id INT AUTO_INCREMENT PRIMARY KEY,
  nom VARCHAR(100) NOT NULL,
  email VARCHAR(100) UNIQUE,
  mot_de_passe VARCHAR(255) NOT NULL
);
```

## Blog Database Tables

-   Utilisateur
-   Article (linked to Utilisateur)
-   Commentaire (linked to Article)

## Verification

-   SHOW TABLES; → list all tables
-   DESCRIBE TableName; → display table structure

## Key Points

-   Every table must have a primary key.
-   Data types must match the type of information stored.
-   Foreign keys ensure relational consistency.

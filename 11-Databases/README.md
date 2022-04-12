# FHIR and Databases

This set of videos explores FHIR and databases interactions.

## Video Links

* [Overview](https://youtu.be/c-I04rtBZLc)
* [Creating a WebAPI Project](https://youtu.be/a1eS3z0am6E)
* Docker backends:
  * Apache Cassanda
  * Microsoft SQL Server
  * MongoDB

## Overview - FHIR and Databases

* General problem: How Do I Store My Data?
  * Spoiler: depends
* FHIR and Database Models
  * IDs, arrays, references, hierarchies, extensions, etc.
  * Looking at a Patient
    * `.name`, `.address`, `.telecom`, `.contact`, `.generalPractitioner`...
* How/What to Store? FHIR as DB Schema vs. Serialized in a DB Field or File
  * FHIR as DB Schema
    * Identify key data
    * Relational (RBDMS)
      * Determine schema layers (tables, etc.)
      * Define indexes
      * Map all elements to/from db
      * ORMs
        * Can struggle with models
        * Changes to FHIR version or SDK can break your system
    * Non-relational (NoSQL - e.g., document store)
      * Determine models / schemas (keyspaces, stores, etc.)
      * Define filters, indexes, etc.
      * Example Pros
        * Fewer design decisions
        * Less transformation = less code
      * Example Cons
        * Indexing nested data can be costly (time+storage)
          * Without indexes, queries can be slow
        * Finding some elements can be hard (e.g., extensions)
  * Serialized in a DB Field or File
    * Identify key data
    * Storage location for data (in DB vs blob/filesystem)
    * Relational (RBDMS), NoSQL (e.g., graph database)
      * Determine schema layers (tables, fields, keys, etc.)
        * How much do you normalize?
      * Define indexes
      * ORMs more useful
      * Need to be careful with data syncrhonization
    Not discussed:
    * Version management (e.g., FHIR R4 vs R5)


## Databases

* [Apache Cassandra](cassandra.md)
* [Microsoft SQL Server](mssql.md)
* [MongoDB](mongodb.md)

## Other Tools

* [DB Designer](https://www.dbdesigner.net/)

## FHIR Links

* [FHIR R4](http://hl7.org/fhir/)
  * [FHIR Patient Resource](http://hl7.org/fhir/patient.html)

# Week 2

## Prerequisites
- Resources
  * TOPCIT
    + An IT assessment tool used to assess the skills and competencies of information technology specialists and software developers, focusing on the abilities required to perform effectively in professional roles.
    + Originates from South Korea, primarily used for examinations, guaging the level of skill of every participant.
- Lessons and Targets 
  * Understanding and Using Data. In designing and automation of databases and the foundations of what we call databases.

## Databases
- Focus: __Data__
- Main Figure:
```
INPUT -> PROCESS -> OUTPUT
```
- Example:
```
Encoding -> Programmers -> Information
```
> Example: Self serving printng kiosk; requiring an input file, the processing of said file, and the output (e.g. costs).

### Evolution of Databases:
- File Cabinets - Before 1950s
  * Bugs came from physical bugs.
- Magnetic Tapes - 1950s and early 1960s
  * _Cassettes_ are an example of magnetic tapes.
  * The files in in magnetic tapes are only able to be accessed sequentially, read and writen to in a form of a sequence.
  * Reading data sequentially dramatically increased read and write time, needing a significant amount of time before the required data is read.
- Hard Disk Drives
  * Removes the old problem of needing to read and write data sequentially in favor of mechanically moving disks, cutting down on time to milliseconds.
  * The moving parts made it susceptible to damages when abruptly events occur, e.g. shut down abruptly.
- Solid State Drives
  * This is now the current day Database Storage.
  * Databases are now able to store images and media.
### Organization
- Databases must be organized in order to store, retrieve, and manage data effiently.
- Types of Databases:
  * Relational Databases
    + The most popular type of database today, being stored in __tables__ with each __row__ representing records and each __column__ representing the attributes of each records.
    + Every single piece of information has a relationship with every other piece of information. Accounting for every data value in the database with a __unique identity__ in the form of a record.
    + All records in this type of database must be tabulated and tabularized therefore, every row of data in the database is linked with another row with a __primary__ key.
    + Similaryly, every table is linked with another table using a foreign key.
    + Scaling and traversing through data in a Relational Database is a lightweight task in comparison to other database types, i.e. Hierchical Databases.
  * NoSQL
    + A non-SQL or non-relational database wherein it provides mechanisms for storing and retrieving data that does not rely on traditional table-based relational models.
    * Instead, it uses flecible data models like key-value pairs, documents, column families, or graphs, making it ideal for handling unstructured, semi-structured, and structured data.
<!-- Fundatmental Systems Design: ig research more about it? the professor said something about using TOPCIT -->

## Information Systems
- Foundation
  * _Fact_ -> __Phenomenon__
    + A state of disorder in reality, __something that exists__ without being observed by others.
  * _Data_ -> __Factual Data__
    + Realistic data that exists widely in the real world.
    + Are __raw__, __unorganized__ pieces of facts or figure which can be collected, discovered, investigated, or obtained from sources, which is commonly in the real world.
  * _Information_ -> __Treatment__
    + When data is organized into meaningful patterns, they become information.
    + Are the __organized__, __classified__ or __systemized__ data which provides __meaningful__ insights.
    + When data are prcessed in a certain form, the information necessary for achieving a specific pupose is created.
  * _Knowledge_ -> __Added Value, Generalization, and Decision-making__
    + Are __generalizations__ from separate pieces of concrete information.
    + Created while analyzing and studying the meaning and relationship of informational data.
    + Therefore, information can vary significantly depending on how one assigns meaning to informatized data, analyzes the relationship, and judges the values of the human being. 
  * _Wisdom_ -> __Internalized Ability__
    + A state in which an individual can __understand and apply knowledge__.
    + The mental ability to acquire, understand, apply, and develop knowledge.
  * _Databases_ 
    + Are an __organized collection__ of logically related data stored for easy access and retrieval.
- Types of Data Processing
> Different types of databases store data differently,
- Batch Processing.
  * Collects batch amounts of data during a certain period and only processed periodically.
  * Characteristics: System-Centered process
    + The users must adjust to the System. 
    + Low processing costs and high system performance are required.
    + Preparatory work is required; Collecting, classifying, and organizaing raw data -> Writing in a file.
    + Standby time is required, immediate processing is not supported
    + Modifying the process is complex and only modifyable after the information is processed.
- Real-time Processing
  * Data are processed the immediately after a transaction occurs.
    + example: Online Processing.
  * Characteristics: User-centered processing. 
    + The systems must adjust to the users. 
    + High Processing cost and low system performance cost. 
    + Preparatory work is not required.
    + Data currency is maintained.
    + Difficult to maintain, repair, or restore. 
- Distributed Processing
  * Data are processed by connecting processors and databases, which are geographically dispered over the network.
  * Characteristics: Client/Server System
    + Improves the operation speed and reliability.
    + Increases the efficient use of resource.
    + Software development is difficult, and the security level and degree of design complexity are relatively high.
  * Server
    + Is a computer or software program on a network that stores data and gives services, files, or resources for other computers, often called clients.
    * A single client is all it takes for a server to form.
  * Client
    + A user that utilize the capabilities of a server, or a "customer" of a server.

<!-- Review TOPCIT, focusing on the technical aspects of creating databases. Finals; create a pretty decent database, manually creating the database design. -->
<!-- Project
  * create a text file database
  * CRUD
  * maximum of 5 columns / date inputs (entries)
-->
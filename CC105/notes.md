### Entity-Relationship Diagrams
- Database
	- Collection of information that's organized for easy:
		- Storage,
		- Management,
		- Updates, and
		- Retrieval
	- There is a lot that is moving in a database.
- Entify-Relationship Diagrams (ERDs)
	- Provides a visual way to understand how data is related and how it works together. 
	- Entity
		- An object, can be:
			- A person,
			- A place, or
			- A thing
		- That is tracked in the database.
		- Example:
			- When buying a product in an online shopping website, e.g. Amazon.com.
			- The entity can be the customer, the order, or the product.
	- Attributes
		- Entities can have properties or traits.
	- Note:
		- Enities are always depicted as ROWS
		- Attributes are always depicter as COLUMNS
	- Relationships
		- Describes how entities interact with each other.
		- When there is a line that connects to or more entities together, there is an interaction that is happening between them.
		- Relationships have notations that are attached to each interactions, these notations are called Cardinality.
		- Cardinality
			- Help define the relationship in a numerical context.
			- Particularly in:
				- Minumums, and
				- Maximums
			- Diagram:
				![[CC105-14.png]]
			- Look up an the Cardinality of an ER Diagram ~~since Markdown is goated~~
		- Example:
			- The cardinality between a Customer and an Order, presents two questions:
				- Customers to Orders
					1. What is the minimum number of orders that a customer can have?
					2. What is the maximum number of orders that a customer can have?
				- Orders to Customers
					1. What is the minimum amount of customers that an order may have?
					2. What is the maximum amount of customers that an order may have?
			- Note that:
				- Customers to Orders
					- A customer can exist, but can have zero orders (O sign)
					- A customer can have an infinite number of orders (crowsfoot sign)
				- Orders to Customers
					- A specific order can only have one customers (l sign)
		- #kulangyungvideo
			- Optional zero-to-one
				- O and One line
			- Optional zero-to-many
				- 0 and Many Lines
			- Mandatory one-to-one
				- 1 and One Line
			- Mandatory one-to-many
				- 1 and Many Lines
- How to make ERDs
	- Uses Lucidchart
		- Free just by logging in or signing up.

## TOPCIT Reviewer - Understanding Data and Databases
### 1. Understanding Data
- A) Concept and characteristics of data, information, and knowledge.
	1. Fact
		- Phenomenon
		- a state of disorder in reality
		- something that exists without being observed by others
	2. Data
		- Factual Data
		- refers to the collected resource itself
		- discovered, investigated, collected, and created in the real world
		- data are related to a fact
		- natural state free of the values and judgements of human beings
		- data that exists widely in the real world
		- simple facts that are not for a specific purpose
	3. Information
		- Treatment and Processing
		- data that are organized, classified, and systemized
		- necessary for achieving a specific purpose
		- data that are organized into meaningful patterns
		- data are treated and processed by a certain program
		- achieves a specific purpose
	4. Knowledge
		- Added value, generalization, and decision-making
		- generalized from several items of concrete information
		- created while analyzing and studying the meaning and relationship of informational data
		- correlations between information
		- a way as to make decisions or created added value
		- information of the same type is grouped together
		- human interpretation and meanings
		- used for decision-making for creation, and added value is created
	5. Wisdom
		- Internalized ability
		- a state where an individual can understand and apply knowledge
		- mental ability to aquire, understand, apply, and develop knowledge

B) Concept and Characteristics of data processing types.
- Data processing system
	- core element of the information system
	- directly elated to the computer
	- depends on the type of data processing
	- how data is organized and accessed
1. Batch processing system
	- data that is collected for a certain period
	- processing it all at once
	- System-centered processing method
		- low processing cost
		- high system performance required
	- Prepatory work is required
		- collecting, classifying and organizing
		- raw data -> writing in a file
	- Standby time is required
		- immediate processing now supported
	- modifying data is complex and difficult, only until files are processed collectively
	- Example: 
		- Payroll processing system, 
		- grade processing system, 
		- utility bill processing system, etc.
2. Online processing system
	- Real-time processing system
	- immediate processing of data
	- User-centered processing method
		- high processing cost
		- low system performance required
	- Prepatory is not required
	- Data currency is maintained
	- difficult to maintin, repair or restore
	- Example: 
		- Seat reservation processing systems for airlines and railroads, 
		- bank deposit processing systems, 
		- stock account systems for securities companies, etc.
3. Distributed processing system
	- connects processors and databases
	- geographically dispersed over the network
	- improves operation speed and reliability
	- increases the efficiency use of resources
	- software development is difficult
	- security level and degree of design complexity are relatively high.

### 2. Understanding the Database
- A) Concept and characteristics of a file processing system. 
	- File processing system
		- method of storing and retrieving paper documents
		- widely used before the computer was invented
		- began to include computerized records in the 1960s
		- designed to arrange and manage the data recorded by the user on a physical disk
		- hierarchical file system with a directory structure
		- each application program accesses an individual file to process in order to search, input, delete, and modify it
	1. Characteristics of the file processing system
		- application program should directly implement the logical file structure designed by the application programmer as a physical file structure
		- data access method implemented only when knowing the physical data structure very well
		- sharing data naturally becomes difficult in an environment where each application program has its own data
		- one file ultimately exists only for one application only
	2. Problems with the file system
		- inability to guarantee data independence
		- program dependent
		- problem of ensuring data consistency (time dependence of a file)
		- problem of ensuring data integrity (values semantically the same should remain identical)
		- low sharing and use convenience
		- low economic feasibility and poor security management

- B) Concept and characteristics of the database 
	- Concept of the database
		- characteristics of integration, operation, storing, and sharing
		- manages duplicated data in one place as intensively as possible to eliminate duplication to the maximum
		- Data Classification
			- Integrated data: 
				- same data are not duplicated in principle, minimal redundancy, controlled redundancy
			- Stored data:
				- data saved in a storage medium that can be accessed by a computer (tape, disk, etc.)
			- Operational data: 
				- required to perform the unique functions of an organization (temporary data are not operational data)
			- Shared data: 
				- jointly owned, maintained, and used by several application programs within an organization
	- Characteristics of the database
		- Real-time accessibility:
			- real-time response to occasional and informal queries
		- Continuous evolution: 
			- update, insert, delete dynamic characteristics keeping the current state accurately
		- Concurrent sharing:
			- supports the concurrent sharing of the same data in different ways
		- Content reference:
			- processing the contents of data requested by the user by values rather than by location or address
### 3. Understanding the Database System
- A) The concept and components of the database system (DBS) 
	- Database system (DBS)
		- computer-centered system 
		- creates necessary information by storing and managing data in a database
	- Components of the database system
		- database, database language, user, and database management system (DBMS)
		- Database: 
			- a set of operational data integrated and stored with minimal redundancy
		- Database language: 
			- a tool that provides an interface between people and system
		- Users: 
			- database administrator (DBA), database application programmer, database user
		- Database management system (DBMS): 
			- system software that provides database construction and utilization functions
    
- B) Data independence and ANSI-SPARC's 3-level database architecture. 
	1. Background to introduction of the concept of data independence (reason for its necessity)
		- reduce continuously increasing maintenance costs, data complexity, and duplicated data
		- maintain independence between the screen and the database against users' constantly evolving requirements
		- three-schema architecture proposed by the special subcommittee of the X3 committee under ANSI
		- reduce interference in changes by separating the user's view from the view by which the database is actually expressed
	2. 3-level database architecture of ANSI-SPARC
		- composed of an external phase, a conceptual phase, and an internal phase
		- Types of schema
			- External schema: personal database schema viewed by everyone in each user's phase; individual database users or application programmer
			- Conceptual schema: database of the entire organization described, integrating all users' perspectives and relationship between data
			- Internal schema: format in which the database is physically stored; expresses how data are actually saved in a physical device
	3. Data independence of two areas
		- Types of independence:
			- Logical independence: 
				- when a concept schema is changed, an external schema and application program are not affected
			- Physical independence: 
				- when an internal schema is changed, an external/conceptual schema and application program are not affected
    4. Relationship between mapping and independence
		-  Types of mapping
			- External/conceptual mapping: 
				- logical thought
				- correlation between the external view and the conceptual view is defined
			- Conceptual/internal mapping: 
				- physical mapping
				- correlation between the conceptual view and the stored database is defined
    
- C) Definition and key roles of the database administrator (DBA) and data architect (DA) Database administrator (DBA)
	1. Roles of the database administrator (DBA)
		- takes responsibility for the configuration and overall administration of the database to ensure proper performance
	    - Tasks and roles of the DBA
			- Data modeling: 
				- modeling according to business, physical data modeling, semi-normalization, performance modeling
			- Physical database design: 
				- index design, storage space design, clustering design, partition design
			- Tuning: 
				- improvement of performance according to index distribution chart, join relationship, and transactions
			- Database building: 
				- creation of a table space, data file space, database object, parameters, and backup structure
			- Database operation: 
				- backup/restoration, monitoring of memory and performance on a regular basis
			- Database standardization: 
				- definition of a glossary and a domain, management of enterprise meta-data
	2. Role of the data architect (DA
		- establishes, models, and systemizes the policies and standards for data-related elements
		- Roles of the DA
			- Establishment of a data management system: 
				- metadata, distribution/integration, ILM, monitoring, log management, failure management
			- Establishment of data governance: 
				- standards related to entire data, definitions of terms and domains, data dictionary
			- Performance of data modeling: 
				- conceptual modeling > logical modeling > physical modeling
			- Establishment of data security systems: 
				- controlling user access, data encryption, access logs, transaction traceability
    
- D) Concept and functions of the DBMS 
	1. Concept of the DBMS
		- system contrived to solve the problem of the file system, dependency and redundancy
		- software system that manages the database so that it can be shared by all application programs as a mediator
	2. Functions of the DBMS
		- controls duplication from the aspects of data storage, development, and maintenance
		- enables data sharing among multiple users
		- controls access to data by unauthorized users
		- provides various types of interfaces to diverse users
		- expresses the complex relationships that exist between data
		- ensures the integrity of the database
	3. Conceptual Diagram and main functions of the DBMS
		- DBMS components
			- DDL compiler: 
				- processes schema specified in DDL as internal schema (metadata) and stores it in the system catalog
			- Query processor: 
				- processes advanced queries submitted by general users (analyzed, parsed, and compiled)
			- DML pre-compiler:
				- extracts DML commands inserted into an application program
			- DML compiler: 
				- generates an object code by parsing and compiling the received DML command
			- Runtime database handler:
				- database access is managed at runtime (search or update executed using storage data manager)
			- Transaction manager: 
				- checks compliance with integrity constraints and user rights, performs restoration during failures
			- Stored data manager: 
				- manages access to the user database and catalog stored in the disk

## TOPCIT Reviewer - Understanding Databases Types
### 1. Types of Databases
- A) Development process of the database
	- hierarchical and network databases were used in the early days but had consistency issues
	- relational databases appeared in the 1970s to resolve these problems
	- object-oriented databases combining object-oriented technology appeared in the 1990s
	- evolving to support large-capacity business environments like XML and NoSQL
	![[CC105-18.png]]

- B) Major types of databases
	1. Hierarchical database
		- hierarchically stores data in a tree format representing relationships between subordinates and superiors
		- oldest database with a hierarchical structure (1960s)
		- maintains a dependent relationship by connecting with physical pointers
		- difficult to change data structures or perform unexpected random searches
	2. Network database
		- stores data by expanding the tree form of a hierarchical database into a network form
		- uses pointers to maintain a many-to-many relationship between records and to link data
		- extracts data quickly but entails high maintenance costs and complex systems
		- records can have pointers to children, sibling records, and parent records
	3. Relational database (RDB)
		- based on the relational data model proposed by E.F. Codd in the 1970s
		- stores characters, numbers, and date information in a two-dimensional structure (column, row)
		- based on mathematical set theory for predictable performance and mathematical optimization
		- allows anyone to easily search for desired information using a simple query language
	4. Object-oriented database (OODB)
		- emerged to search and store unstructured complex information based on an object model
		- supports user-defined data types and inheritance
		- accesses information based on navigation using the reference structure between objects
		- structure of information in the program is the same as the database schema
		- basic database management functions were found to be weak in an enterprise environment
### 2. Object Relational Database
- A) Object relational database (ORDB)
	- combines the existing relational database with the concept of the object-oriented database
	- supports user-defined data types: users can define and use new types of data
	- supports reference types: data can be accessed on navigation using a reference structure
	- supports nested tables: one column in a table can be composed of another table
	- supports large-scale objects: uses LOB as a basic data type for images, audio, and video
	- supports table inheritance relationships: specifies the inheritance relationship between tables

|Characteristics|Description|
|---|---|
|Support user-defined data types|Users can define and use new types of data in addition to basic data types.|
|Supports the reference type|Data can be accessed on navigation using the reference structure in such a way that one object records refers to another object record.|
|Supports a nested table|A data model with a complex structure can be designed because one column in a table is composed of another table.|
|Supports large-scale obejcts|Supports LOB (Large Object) as a basic data type for large-scale unstructured data such as images, audio, and video.|
|Supports table inheritance relationships|Accomodates the advantages of the object-oriented database by specifying the inheritance relationship between tables.|
### 3. Understanding XML
- A) Extensible Markup Language (XML)
	- standard language used to structure and exchange data in a web environment
	- characteristics
		- simplicity: 
			- simplifies SGML by eliminating unused functions
		- openness: 
			- can be used together with HTML and can exchange meta-data
		- scalability: 
			- can create its own tags and supports self-description
		- structure: 
			- understood by humans and machines, separates content from expression
		- hierarchical structure: 
			- supports structure search and full text search

	B) Schematic diagram and components of XML
	- Definition:
	    - XML Is composed of XML Document Type Detinition (DTD) and the XML schema for specifying XML: the XPath for processing XML documents: and XQuery, Extensible Stylesheet Language (XSL), XML Linking Language (XLL), etc. To create an XML document, it is necessary to fully understand the XML components and the basic syntax.
	- Diagram of XML configuration:  
	    ![[CC105-19.png]]

- C) XML configuration: XML components
	- XML DTD: 
		- XML Document Type Definition XML DTD
		- document that defines the form of an XML document in a consistent structure
	- XML Schema: 
		- high-level data definition language that replaces DTD for more complex data types
	- XPath: 
		- language expressing extended queries so search conditions can be included in the path
	- XQuery: 
		- standard query language that extracts information from an XML file like a database
	- XSL/XSLT: 
		- XSL (Extensible Stylesheet Language)
			- specifies the style sheet used to express or convert XML data into different forms
		- XSLT (Extensible Stylesheet Language Transformation)
			- part of XSL, converts an XML doc into a different type like HTML
			- can be displayed on general browsers
	- XLL: 
		- The extensible Linking Language (XLL)
		- displays the connection and relationship between XML elements (XLink, XPointer)
			- XLink: Recognizes and processes hyperlinks
			- XPointer: An address of the element in an XML document.

- D) Structure and major components of the XML processor
	- XML processor
		- XML parser: 
			- checks and inspects the grammar and syntax structure of an XML document
		- XML syntax analyzer: 
			- analyzes the syntax structure (SAX, DOM)
		- XSL engine: 
			- converts an XML document to a document format with expression information
	![[CC105-20.png]]

- E) XML document creation procedure
	- XML creation procedure:  
    ![[CC105-21.png]]

- F) DTD concept and creation procedure
	- Document Type Definition (DTD)
		- file that explicitly declares the structure and contents of an XML document
		- types of declaration: element type, attribute list, entity, and notation
		- can be declared internally within the XML document or applied externally
	- Types of DTD declaration:
		
		| Definition | Decalration | Yes |
		| --- | --- | ---|
		| Element type creation      | - element type declaration  | <!ELEMENT element name~> |
		| Attribute list declaration | - attribute type declaration | <!ATTLIST element name~> |
		| Entity declaration         | - entity declaration  | <!ENTITY ~>              |
		| Notation declaration       | - notation declaration <br>- non-xml data processing: Images, etc. | <!NOTATION name ~>       |

	- DTD creation procedure:
		1. Step 1: DTD declaration 
			- Describing the process of declaring DTD

			| Example 1                                                                                  | Example 2                                                                                        |
			| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
			| \<! DOCTYPE Root_Element [  <br>\<ELEMENT Root_Element(...)>  <br><...>  <br><...>  <br>]> | \<!DOCTYPE books[  <br>\<!ELEMENT book(title, author>)>  <br>\<!ELEMENT title(#PCDATA>)>  <br>]> |
			
		2. Step 2: Declarating an element type

			| \<!ELEMENT element_name(con tent_model)>              | \<!ELEMENT books(book*)>                            |
			| ----------------------------------------------------- | --------------------------------------------------- |
			| [Note] The asterisk* symbol indicates a case in which | an element is omitted or may appear multiple times. |
			|                                                       |                                                     |
			        
		3. Step 3: Combining XML and DTD
			- Determines whether the DTD declaration and definition part will be created inside XML or saved as an external file.
			- Internal declaration
				- Defines the DTD in an XML document.
			- External declaration
				- Applies the DTD (Document type declaration) part to an XML document.

- G) Concept and characteristics of XML Schema, and comparison with DTD
	- XML Schema
		- introduced to replace DTD to enable the creation of data types
		- supports complex structure definitions and namespaces (abstract entities distinguishing elements)
		- features fully object-oriented scalability and extensive data types
	- Comparison of the XML Schema and DTD:
		
		|Item|XML Schema|DTD|
		|---|---|---|
		|Writing grammar|Complies with XML 1.0|EBNF + pseudo|
		|Structure|Complex|Relatively simple|
		|Namespace|Supported (Multiple namespaces can be used in a document)|Not supported (Used once in a document)|
		|DOM Support|DOM is supported and can be used because it is XML|Not supported|
		|Dynamic schema support|Supported (Selecting at runtime. Subject to change due to an interaction.)|Not supported (DTD can actually read only.)|
		|Data type|Extensive data type|Very limited data type|
		|Scalability|Fully object-oriented scalability|Extension using string subsitution|
		|Openness|Content model that supports open and closed modification|Closed structur|

- H) Characteristics od XQuery
	- XQuery
		- query language used to search an XML-based database
		- technology neutral and standardized based on W3C-based XQuery 1.0
		- easy to implement using simple syntax similar to SQL (for, let, where, return)
	-   Characteristics of XQuery
		
		|Characteristics|Description|
		|---|---|
		|Technology neutral|A technology that is standardized based on W3C-based XQuery 1.0.|
		|XML-based query language|DA data search and storage technology using XML.  <br>A language that is originated from an XML query language called Quilt and which includes the XPath expression.  <br>The result of the query statement written in XQuery is the list of nodes indicating a tree structure, not an XML document.|
		|Simple and easy to implement|Easy to implement using syntax similar to SQL, such as for, let, where, and return (FLWR).|

- I) Concept and characteristics of XLL
	- XLL
		- standard language that performs link functions in an XML document
		- provides a two-way link between resources and extended pointers for resource locating
		- link types include simple, extended, locator, group, and document
	
### 4. Understanding Various Database Types
- Multimedia database
	- developed to efficiently search and manage large capacity, complex, unstructured multimedia data
	- built using file-based, RDBMS-based (CLOB/BLOB), OODBMS-based, or ORDBMS-based formats
- Main memory database (MMDB)
	- manages and manipulates a database by keeping it in the main memory
	- disk I/O does not occur, meaning performance is incredibly fast
	- hardward-based error recovery is used due to the volatility of the main memory
	- hashing and T-tree indexing algorithms optimized for a memory environment are used
- Embedded database
	- developed for embedded systems with limited memory and special performance goals
	- provides essential functions only after reducing overheads to use minimum RAM and disk
	- supports communication between different devices and porting to various platforms
- Mobile database
	- exclusively used by mobile devices to process field data and synchronize with a central server
	- installed in small capacity devices equipped with limited CPU and memory
	- provides data replication and synchronization with the database of the existing server
- Spatial database
	- set of non-spatial data (letters/numbers) and spatial data represented by coordinate values
	- includes geometry, geographical objects, and topology for spatial relationships
	- uses new indexes (R-tree index) and operations to process large amounts of data quickly
- Column base database
	- physically stores data based on columns rather than rows
	- resolves the limits of analyzing large-scale data at high speed
	- physical structure prevents reading unnecessary data, vastly improving efficiency
	- Comparison of the column base database and row base database  
![[CC105-23.png]]![[CC105-24.png]]
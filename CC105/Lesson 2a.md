### > [Table of Contents](../main.md)
# CC105
---
## Targets
- Recent trends and major issues:
	- The "database" was created in the late 1960s to manage and use data more efficiently than the computer environment which used the file system in the early days. 
	- Since then, the basic model of database has evolved continuously into relational, object-oriented, and object relational types of database, having started as a network model. 
	- Currently, the object relational model is the most widely used model in the market. 
	- In addition, the internal data model and the structure of the database were a matter of interest in the past. 
	- However, the importance of database processing performance was highlighted with regard to the processing of large-scale data, as the problem of performance degradation became increasingly serious due to the rapid increase in the amount of digital data. 
	- Accordingly, the relevant technology has expanded to include new types of databases, such as the column-type database which places emphasis on database performance and scalability rather than data relations, NoSQL, etc.
- Learning objectives:
	1. To be able to explain the data model and the structure of each type of database. 
	2. To be able to explain the concept and characteristics of the object relational database (ORDB). 
	3. To be able to understand and write an XML document. 
	4. To be able to explain various database systems.
- Reasons to understand database types
	- The relational database and the object relational database, which are based on E.F. Lodd s hormalization theory of 1970, have mainly been used in the existing workplace, because data consistency was important in workplaces where OLTP (Online Transaction Processing) jobs were dominant. However, the processing of diverse types of data and the rapid processing of large quantities of data are required these days. Therefore, DBMS vendors are developing DBMS functions in such a way that the advantages of each type of database can be introduced and applied. 
	- As a result, if we know the background to database development and the basic concepts of the major types of database, we can easily understand the functions and purposes of the various DBMSs used for various purposes in the workplace and get help in strategically selecting a DBMS that is optimized for the characteristics and purposes of the business in question.

## Understanding Types of Database
### 1. Types of Databases
- A) Development process of the database
	- Definition:
		- The hierarchical and network databases that developed the data structure used in existing applications were the main types of database used in the early days. However, these databases had a big problem in that it was difficult to maintain consistency. To resolve these problems, relational databases appeared in the 1970s. Since then, databases have developed continuously around relational database technology. 
		- In the 1990s, user-defined data and multimedia data needed to be managed, but existing relational data models could not handle such complex data. Accordingly, an object-oriented database combining object-oriented technology, which began to gain attention from the mid-1980s, and a database appeared. Since then, an object-oriented database that combines the advantages of both the relational database and the object-oriented database has appeared and been widely used until now. Databases are evolving from simple business applications to large-capacity and complex business environment supports to respond to changes in the IT market and technology, such as the XML database, which emerged as a response to the development of the Internet environment, and the NoSQL, which was developed to process big data.
	- Application area of the database by era:
		![[CC105-18.png]]
- B) Major types of databases
	- 1. Hierarchical database
		- Definition:
			- A hierarchical database hierarchically stores data in a tree format of the relationship between subordinates and superiors. 
			- Although this database has the advantages of rapid data access and easy prediction of data usage, it cannot adapt to changing business processes easily.
		- Characteristics:
			- It is the oldest database with a hierarchical structure (1960s). 
			- Each hierarchical structure maintains a dependent relationship by connecting with physical pointers. 
			- It is difficult to change the data structure when the business process is changed after building a database.
			- It is difficult to perform unexpected random search.
	2. Network database
		- Definition:
			- A network database stores data by expanding the tree form of a hierarchical database into a network form. 
			- Pointers are used to maintain a many-to-many relationship between records and to link data.
		- Characteristics:
			- It was developed in the early 1970s to solve the problems with the hierarchical database. 
			- Data can be extracted quickly and effectively by adding links between hierarchical structures.
			- High maintenance costs and backlog are entailed by the complex type system. 
			- Programmers must understand the structure to write a program. 
			- A record can have pointers to children and sibling records and to parent records, which was not possible with the hierarchical database.
	3. Relational database (RDB)
		- Definition:
			- The relational database is based on the relational data model proposed by E.F. Codd in the 1970s. 
			- Major commercial products include Oracle, SQL Server, DB2, Informix, Sybase, and Ingres.
		- Characteristics:
			- The model itself is simple. The database stores characters/numbers/date information in a two-dimensional structure (column, row). 
			- The model is based on mathematical theory - particularly the set theory of mathematics. Therefore, the performance of the system to be developed can be predicted and verified mathematically, and various operations can be mathematically optimized.
			- Existence of query language - Anyone can easily search for desired information by learning a simple query language in the 4GL format. 
			- Contiguous support for technology that keeps pace with the circumstances of the times - Supports the client/ server architecture, large-scale parallel processing, etc
	4. Object-oriented database (OODB)
		- Definition:
			- The relational database cannot create new types of data or expand existing types, and has difficulty processing unstructured complex information such as multimedia. 
			- Also, the standard query language "SQL" expresses data relationships by values, making it difficult to find and process mutually related entities when expressing a complex object. 
			- Accordingly, a database that can search and store information based on an object model emerged, namely. the object-oriented database. 
			- Major commercial products include ObjectStore, O2, Objectivity, and Uni-SQL.
		- Characteristics:
			- User-defined data types are supported, and inheritance can be specified. 
			- Unstructured complex information can be modeled. 
			- Information can be accessed based on navigation using the reference structure between objects. 
			- The structure of information in the program is also same as that of the database schema.
		- Note:
			- The object-oriented database was not distributed widely in the market because its basic database management functions were found to be weak, such as transaction processing, number of supported concurrent users, backup and recovery, etc., and system safety and performance were never proven in an enterprise environment.
### Object Relational Database
- A) Object relational database (ORDB)
	1. Concept of the object relational database
		- Even though the object-oriented database was introduced to solve the weakness of the relational database regarding new advanced applications, it showed certain limitations in terms of its use in an enterprise environment. 
		- To overcome this the obiect relational database was introduced by combining the existing relational database with the concept of the object-oriented database and expanding its functions. 
		- Currently, most commercial databases are object relational databases, such as Oracle's Oracle9i, IBM's DB2 UDB, and Microsoft's SQL Server.
	2. Characteristics of the object relational database
		- Characteristics of the object relational database

			| Characteristics | Description |
			| --- | --- |
			| Support user-defined data types | Users can define and use new types of data in addition to basic data types. |
			| Supports the reference type | Data can be accessed on navigation using the reference structure in such a way that one object records refers to another object record. |
			| Supports a nested table | A data model with a complex structure can be designed because one column in a table is composed of another table. |
			| Supports large-scale obejcts | Supports LOB (Large Object) as a basic data type for large-scale unstructured data such as images, audio, and video. |
			| Supports table inheritance relationships | Accomodates the advantages of the object-oriented database by specifying the inheritance relationship between tables. |

### Understanding XML
- A) Concepts and characteristics of Extensible Markup Language (XML)
	- Definition:
		- HTML (HyperText Markup Language) is mainly used to create and format web documents in a web environment, but it remains unsuitable for specifying structured data extracted from a database. 
		- Therefore, the World Wide Web Consortium (W3C) has developed an extensible markup language (XML) as a standard language that is used to structure and exchange data in a web environment.
	- Characteristics:
		1. Simplicity: 
			- XML can simplify SGML (unused functions have been eliminated, while major functions have been retained). 
		2. Openness: 
			- XML can be used together with HTML on the web, and can exchange meta-data.
		3. Scalability:
			- It can create its own tags and supports self-description.
		4. Structure can be understood both by humans and machines: 
			- Makes it easy to compare and collect data. 
		5. Separation of content and expression: 
			- The format can be changed according to the user's preferences (increased reusability). 
		6. Hierarchical structure: 
			- Supports structure search and full text search.
		7. Unicode: 
			- Supports multiple languages.
- B) Schematic diagram and components of XML
	- Definition:
		- XML Is composed of XML Document Type Detinition (DTD) and the XML schema for specifying XML: the XPath for processing XML documents: and XQuery, Extensible Stylesheet Language (XSL), XML Linking Language (XLL), etc. To create an XML document, it is necessary to fully understand the XML components and the basic syntax.
	- Diagram of XML configuration:
		![[CC105-19.png]]
- C) XML configuration
	- XML components:

		| Component | Description |
		| --- | --- |
		| XML DTD | XML Document Type Definition XML DTD <br> A document that defines the form of an XML document in a consistent structure. XML DTD is used to validate XML. |
		| XML Schema | High-level data definition language used to specify the structure of an XML document by replacing XML DTD. <br> More complex data types than XML DTD can be declared. |
		| XPath | A language that expresses extended queries so that the search condition can be included in the XML path expression. |
		| XQuery | A standard XML query language that can extract intended information from an XML file as if using a database. |
		| XSL/XSLT | XSL (Extensible Stylesheet Language) is a language that specifies the style sheet, which is used to express XML data in various different forms. <br> XSLT (Extensible Stylesheet Language Transformation) is a part of XSL that converts an XML document into a different type of document (such as HTML) so that it can be displayed on general browsers. |
		| XLL | The extensible Linking Language (XLL) displays the connection and relationship between XML elements. <br> XLink: Recognizes and processes hyperlinks. <br> XPointer: An address of the element in an XML document. |

- D) Structure and major components of the XML processor
	- Structure and components of the XML processor:
		![[CC105-20.png]]
	- XML Components

		| Component | Function
		| --- | --- |
		| XML parser | Checks and inpects the grammar and syntax structure of an XML document (validation check). |
		| XML syntax analyzer | Analyzes the syntax structure of an XML document (SAX, DOM). |
		| XSL engine | Converts an XML docuemnt to a document format with expression information. |

- E) XML document creation procedure
	- XML creation procedure:
		![[CC105-21.png]]

- F) DTD concept and creation procedure
	- Definition:
		- Document Type Definition (DTD) is a file that explicitly declares the structure of an XML document by defining the structure and contents of that docuemnt. 
		- There are types of DTD declaration, shown in the table below.
	- Types of DTD declaration:

		| Definition | Decalration | Yes |
		| --- | --- | --- |
		| Element type creation | - element type declaration | \<!ELEMENT element name~> |
		| Attribute list declaration | - attribute type declaration | \<!ATTLIST element name~> |
		| Entity declaration | - entity declaration | \<!ENTITY ~> |
		| Notation declaration | - notation declaration <br> - non-xml data processing: Images, etc. | \<!NOTATION name ~> |

	- DTD creation procedure
		1. Step 1: DTD declaration - Describing the process of declaring DTD

			| Example 1 | Example 2 |
			| --- | --- |
			| \<! DOCTYPE Root_Element \[<br> \<ELEMENT Root_Element(...)><br> \<...><br> \<...><br> ]> | \<!DOCTYPE books\[<br> \<!ELEMENT book(title, author>)><br> \<!ELEMENT title(#PCDATA>)><br> ]> |

		2. Step 2: Declarating an element type

			| \<!ELEMENT element_name(con tent_model)> | \<!ELEMENT books(book*)> |
			| --- | --- |
			| \[Note] The asterisk* symbol indicates a case in which | an element is omitted or may appear multiple times. |

		3. Step 3: Combining XML and DTD
			- Determines whether the DTD declaration and definition part will be created inside XML or saved as an external file. 
			- Internal declaration
				- Defines the DTD in an XML document. 
			- External declaration
				- Applies the DTD (Document type declaration) part to an XML document.

- G) Concept and characteristics of XML Schema, and comparison with DTD
	- Definition:
		- The existing DTD cannot limit or extend the data type or range of certain information, and the DTD description grammar differs from the XML description grammar, which requires understanding of both the DTD and XML grammars. 
		- As a result, the XML schema was introduced to replace the DTD and to enable the creation of a data type that can process a document more easily.
		- Supporting data types: More complex types of data than the existing DTD can be created, and new types can be created and used. 
			- Supporting complex structure definition: Another schema document can be included in a schema document using the Schema location directive. 
			- Supporting a namespace: XML Schema supports a namespace. 
			- Namespace: An abstract entity that can distinguish elements when extracting elements from an XML document type and combining them with other documents, and when processing multiple documents at the same time.
	- Comparison of the XML Schema and DTD:

		| Item | XML Schema | DTD |
		| --- | --- | --- |
		| Writing grammar | Complies with XML 1.0 | EBNF + pseudo  |
		| Structure | Complex | Relatively simple |
		| Namespace | Supported (Multiple namespaces can be used in a document) | Not supported (Used once in a document) |
		| DOM Support | DOM is supported and can be used because it is XML | Not supported |
		| Dynamic schema support | Supported (Selecting at runtime. Subject to change due to an interaction.) | Not supported (DTD can actually read only.) |
		| Data type | Extensive data type | Very limited data type |
		| Scalability | Fully object-oriented scalability | Extension using string subsitution |
		| Openness | Content model that supports open and closed modification | Closed structure |
- H) Characteristics od XQuery
	- Definition:
		- XQuery is a query language that is used to search an XML-based database, and can extract information from XML files as if using a database.
	- Characteristics of XQuery

		| Characteristics | Description |
		| --- | --- |
		| Technology neutral | A technology that is standardized based on W3C-based XQuery 1.0. |
		| XML-based query language | DA data search and storage technology using XML. <br> A language that is originated from an XML query language called Quilt and which includes the XPath expression. <br> The result of the query statement written in XQuery is the list of nodes indicating a tree structure, not an XML document. |
		| Simple and easy to implement | Easy to implement using syntax similar to SQL, such as for, let, where, and return (FLWR). |

- I) Concept and characteristics of XLL
	- XLL is a standard language that performs link functions in an XML document, such as linking XML documents and setting specific locations within an XML document. XLL was introduced to overcome the limitations of HTML-based simple hyperlinks and to provide various approaches to using resources on the web. XLL supports various hyperlink methods and two-way links between link resources. XLL can use some of the required web resources by using XPointer or XPath, and is used as a core technology in X-Internet, etc. 
		- Supports two types, i.e. Xpointer when moving within the same document, and XInik when moving between different pages, etc. 
		- Provides a two-way link between resources. 
		- Provides an extended pointer (XPointer) for resource locating. 
		- Link type: Simple, Extended, Locator, Group, Document.

### Understanding Various Database Types
- A) Multimedia database
	- Definition:
		- The multimedia database was developed to efficiently search and manage unstructured multimedia data characterized by their large capacity and complexity, such as text, image, audio, video, etc. 
		- Existing databases face limitations due to the exponential increase of unstructured/multimedia data, and an object-oriented approach, the synchronized representation of multimedia, and the concept of time-dependent modeling were used to model various types of unstructured data.
	- Bulding a multimefia database

		| How to build | Main content |
		| --- | --- |
		| File based | Used for simple search-oriented VOD (Video On Demand). <br> It is difficult to support the function for restoring concurrent data access rights (DBMS functions are not used.) |
		| RDBMS based | Stores ASCIl text data in the CLOB (Character Large Object) field. <br> Stores the image/video/audio in the BLOB (Binary Large Object) field. <br> It is difficult to build a complete multimedia database. |
		| OODBMS based | Defines the classes for each media using the user-defined class and user-defined method function. <br> It is incompatible with existing databases. |
		| ORDBMS based | Supports the CL OB and BL OB field to store mono media. <br> Defines the types for each media using user-defined types and functions. |

- B) Main memory database (MMDB)
	- Definition:
		- Unlike general commercial databases in which a database is stored on a disk, the main memory database manages and manipulates a database by keeping it in the memory. 
		- The current trend is that the main memory database is actively used due to business demands, such as securing the competitiveness of an enterprise through quick decision-making, and the revolutionary development of related technologies such as the release of 64-bit OS, the reduction of memory prices, etc. 
		- The MMDB has the following characteristics due to the fact that the database runs in the main memory.
	- Characteristics:
		- Disk I/O does not occur because alloperations are performed in the main memory.
		- Performance is good because disk I/O, which degrades performance in the disk-based database, is rare. 
		- Hardware-based error recovery techniques are used due to the volatility of the main memory. 
		- A disk is used for backup and logging Hashing and T-tree indexing algorithm optimized for a memory environment is used. 
		- Types of commercial main memory databases can be updated at [link](https://en.wikipedia.org/wiki/List_of_in-memory_databases).
- C) Embedded database
	- Definition:
		- General commercial databases are not suitable for the embedded system, which has limited memory and special performance goals. 
		- The embedded database was developed for the embedded system, so as to allow specific functions to be used in a limited embedded environment. 
		- As a result, the embedded database has the following technical characteristics.
	- Characteristics:
		- It provides essential functions only after reducing overheads to use minimum RAM and disk. 
		- It supports communication between different devices to allow communication with the database in a central server. 
		- It supports porting to the various platforms of the embedded system. 
		- It satisfies the performance requirements of the real-time OS of the embedded system. 
		- The list of commercial embedded databases can be updated at [link](http://embedded-databases.com).
- D) Mobile database
	- Definition:
		- The mobile database is exclusively used by mobile devices. The mobile database, which is installed in a mobile device, processes the data generated during field work and sends them to the central server for synchronization.
		- Due to the distinct characteristics of installation in a mobile device, a mobile database should be independent from various platforms and operation systems, should recover quickly from failures, and should be optimized for a limited mobile environment. 
		- As a result, the mobile database has the following characteristics.
	- Characteristics:
		- The database can be installed in a small capacity device equipped with a limited CPU and memory. 
		- It is provided as an embedded form that integrates data and applications. 
		- It has the function of data replication and synchronization with the database of the existing server. 
		- Commercial mobile databases include Sybase SQL Anywhere, Oracle Lite, Microsoft SQL Server Compact, SQLite, and IBM DB2 Everyplace.
- E) Spatial database
	- Definition:
		- A spatial database is a set of non-spatial data represented by letters and numbers and spatial data represented by coordinate values. 
		- The spatial database was initially developed because a technology for processing "unstructured data", such as the geographic information system, was needed as a core technology for a type of guided missile that strikes a preset target by tracking the target's location using geographical information. 
		- Thereafter, the spatial database was introduced full scale, as the market was expanded to include services that store and manage values for specific locations using geographical information, such as GIS and location information check.
	- Definition:
		- Geometry, a geographical object, and topology for the spatial relationship between objects are included. 
		- Unstructured data can be processed: large amounts of data can be processed quickly. 
		- Spatial (topological, geometric) characteristics are reflected. 
		- New index and operation (R-tree index) are used to sort data that cannot be sorted. 
		- Expressive data model that can express complex information. Supports the combination of spatial data and non-spatial data.
- F) Column base database
	- Definition:
		- A column base database physically stores data based on columns. 
		- The data storage method of the relational database is not defined as row base or column base, but general relational databases use a physical storage structure based on rows. 
		- However, a way to store data with this structure reached the limit in analyzing large-scale data at high speed because its physical structure required that unnecessary data should be also read. 
		- The concept of column storage did not suddenly appear recently. Rather, this concept was studied relatively early on, including TAXIR, which was developed in 1969 for searching biological information.
		- Recently, as the demand for the rapid processing of large amounts of data increased, a function that partially borrowed the concept of the column store such as the column store index, column store base DBMS, and hybrid DBMS supporting both structures were developed from the mid2000s. 
		- Column base database technology is now being actively used in the DBMS market, together with the main memory database.
		- The column base database has the following structure and characteristics compared to the row-based database.
	- Comparison of the column base database and row base database
		![[CC105-23.png]]![[CC105-24.png]]
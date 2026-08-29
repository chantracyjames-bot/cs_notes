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

## TOPCIT Reviewer
### 1. Understanding Data
- A) Concept and characteristics of data, information, and knowledge.
	1. Data
		- Data refers to the __collected resource itself__, which are the basic data __discovered, investigated, collected, and created__ in the real world. 
		- That is, __data are related to a fact__, which refers to a __natural state free of the values and judgments__ of human heings.
	2. Information
		- Information refers to various __data that are organized, classified, and systematized__ for certain purposes according to certain rules. 
		- When data are processed in a certain form, the information necessary for __achieving a specific purpose__ is created.
	3. Knowledge
		- Knowledge refers to matter that is __generalized from several items of concrete information__.
		- It is __created while analyzing and studying__ the meaning and relationship of informational data. 
		- __Correlations between information should be established__ to convert information into knowledge. 
		- Therefore, information can vary significantly depending on how one assigns meaning to __informatized data, analyzes the relationship, and judges the values__ of the human being. 
		- Enterprises and institutions manage such information or knowledge in such __a way as to make decisions or create added value__.
	- Data, information, and knowledge:

	| Item | Definition and characteristics | Key point |
	| --- | --- | --- |
	| Fact | A state of disorder in reality. Something that exists without being observed by others. | __Phenomenon__ |
	| Data | Realistic data that exist widely in the real world. <br> Several simple facts that have not yet been evaluated for a specific purpose. | __Factual Data__ |
	| Information | When data are organized into meaningful patterns, they become information. <br> Data are treated and processed by a certain program (form) in order to create information necessary for achieving a specific purpose. | __Treatment and processing__ |
	| Knowledge | Information of the same type is accumulated and organized into a generalized form. <br> A state to which human interpretations and meanings are given. <br> Information is used for decision-making or creation, and added value is created. | __Added value, generalization, and decision making__ |
	| Wisdom | A state in which an individual can understand and apply knowledge. <br> The mental ability to acquire, understand, apply, and develop knowledge. | __Internalized ability__ |

- B) Concept and Characteristics of data processing types.
	- Definition:
		- The data processing system, which is the core element of the information system, and is directly related to the computer, can be divided into batch processing, online processing, and distributed processing system depending on the type of data processing, in other words, how the data are organized and accessed.
	1. __Batch processing system__
		- Data is __collected for a certain period__ or a certain amount to __process it at once__.
		- __System-centered processing method__. (__Low__ processing cost and __high__ system performance are required.) 
		- __Preparatory work is required__. (__Collecting, classifying, and organizing__ raw data -> Writing in a file) 
		- __Standby time is required__. (__Immediate processing__ is not supported.) 
		- The procedure of modifying changes is complex and difficult until files are processed collectively. 
		- Example: Payroll processing system, grade processing system, utility bill processing system, etc.
	2. __Online processing system__
		- When the __data are transfered to a computer__, the computer __immediately processes__ the data. (__Real-time processing system__)
		- __User-centered processing method__. (It incurs a __high__ processing cost and __low__ system performance is required.) 
		- __Preparatory work is not required__. 
		- __Data currency is maintained__. 
		- __Difficult to maintain, repair, or restore__. 
		- Example: Seat reservation processing systems for airlines and railroads, bank deposit processing systems, stock account systems for securities companies, etc.
	3. __Distributed processing system__
		- Data are processed by __connecting processors and databases__, which are __geographically dispersed__, over the network. 
		- Operated in the form of a __client/server system__. 
		- __Improves the operation speed and reliability__. 
		- Increases the __efficient use of resources__.
		- Software developement is difficult, and the security level and degree of design complexity are relatively high.

### 2. Understanding the Database
- A) Concept and characteristics of a file processing system.
	- Definition:
		- The term "_file processing system_" refers to a method of __storing and retrieving paper documents__ that was widely used before the computer was invented. However, the meaning of the term began to include computerized records in the __1960s__. Such a file system is __designed to arrange and manage the data__ recorded by the user on a __physical disk__. In general, a __hierarchical file system with a directory structure__ is used. 
		- Each application program in a file system accesses an individual __file to process, in order to search, input, delete, and modify it__. 
		- For example, if a file system is used when a certain web service system saves the user's log-in history, the application program that saves the login history has a unique form according to the characteristics of the application program, depending on the sequence in which the information to be saved is arranged, and the unit of classification of such information.
	1. Characteristics of the file processing system.
		- The application program should directly __implement the logical file structure__ designed by the application programmer as a __physical file structure__. 
		- Application programmers can __implement the data access method__ in the application program only __when they know the physical data structure__ very well. 
		- __Sharing data naturally becomes difficult__ in an environment where __each application program has its own data__. Therefore, __one file ultimately exists only for one application__ only.
	2. Problems with the file system
		- __Inability to guarantee data independence__.
			- Program dependent.
		- __Problem of ensuring data consistency__.
			- Time dependence of a file (which has a different value depending on the time of retrieval). 
		- __Problem of ensuring data integrity__.
			- Values that are semantically the same should remain identical. 
		- __Low sharing and use convenience__.
			- Low economic feasibility and poor security management.
- B) Concept and characteristics of the database
	1. Concept of the database
		- Definition:
			- The database has the characteristics of __integration, operation, storing, and sharing__. 
			- In the past, data were inevitably saved in duplicate when recorded on paper, because even the same data could not be shared in real time. 
			- Data were also saved in several files in duplicate even when the file system was in use. 
			- The database, however, manages duplicated data in one place as intensively as possible to eliminate duplication to the maximum.
		- Data Classification:

			| Classification | Contents |
			|---|---|
			| __Integrated data__ | This means that the same data are not duplicated in principle. <br> - __Minimal redundancy__ <br> - __Controlled redundancy__ |
			| __Stored data__ | Data are __saved in a storage medium__ that can be accessed by a computer (tape, disk, etc.). | 
			| __Operational data__ | Data which are __required to perform the unique functions__ of an organization. (Temporary data used while performing a task, such as simple input/output, are not operational data) |
			| __Shared data__ | Data which are __jointly owned, maintained, and used by several application programs__ within an organization. |
	2. Characteristics of the database
		- Definition:
			- The shared database can be accessed in real time using the programming language, and is constantly changing due to the input, modification and deletion of data. 
			- The database can also be accessed and shared by multiple users simultaneously, and it has the characteristic of being referable by using the contents of data.
		- Characteristics of the database:

			| Item | Contents |
			|---|---|
			| __Real-time accessibility__ | __Real-time response__ to occasional and informal queries. |
			| __Continuous evolution__ | __Update, insert, delete__: Dynamic characteristics (keeping the current state accurately during such changes). |
			| __Concurrent sharing__ | Supports the concurrent __sharing of the same data in different ways__. |
			| __Content reference__ | Refer to __processing the contents of data requested__ by the user, (that is, __by values__) rather than by location or address. |

### 3. Understanding the Database System
- A) The concept and components of the database system (DBS)
	1. Definition of the database system
		- Definition:
			- The term 'DBS' refers to a __computer-centered system__ that creates necessary information by __storing and managing data__ in a database.
		- Figure:
			![[CC105-15.png]]
	2. Components of the database system
		- Definition:
			- As regards the processing of data stored in a database, there is a user who processes it, a language that can manipulate and read data in the database, and DBMS software that enables the processing of all data. 
			- That is, a database system is composed of four attributes: database, database language, user, and database management system (DBMS).
		- DBS components:

			| Item | Contents |
			| --- | --- |
			| __Database__ | A set of __operational data integrated and stored with minimal redundancy__, so that the multiple application systems of an __organization can share it__. |
			| __Dataase language__ | A tool that provides an __interface between people and system__. |
			| __Users__ | __Database administrator__ (_DBA_), __database application programmer, database user__. |
			| __Database management system__ (_DBMS_) | System software that __provides database construction and utilization functions__. |
- B) Data independence and ANSI-SPARC's 3-level database architecture.
	1. Background to introduction of the concept of data independence (reason for its necessity)
		- Figure:
			![[CC105-16.png]]
		- Definition:
			- To understand data independence, it is helpful to understand the background to the introduction of the concept of data independence. The opposite of data independence can be defined as data dependency. Here, the subject of dependency generally refers to an application program. An application is the interface object which interacts with users and handles the user requirements. It can be said that data dependency has the purpose of reducing continuously increasing maintenance costs, data complexity, and the number of duplicated data. The concept of data independence was also introduced to maintain independence between the screen and the database against the users' constantly evolving requirements. 
			- It can be said that data independence is a three-schema architecture, which was proposed by the special subcommittee of the X3 committee under the American Standards Institute (ANSI) for the DBMS and its interfaces.
			- The main purpose of this three-schema architecture was to reduce interference in changes, by separating the user's view of the database from the view by which the database is actually expressed. When data independence is secured, the independence of each view can be maintained, data can be changed without affecting the view by layer, and different DDL (data definition language) and DML (data manipulation language) can be provided according to the schema by phase.
	2. 3-level database architecture of ANSI-SPARC
		- Definition:
			- The data independence model, which is based on the 3-level database architecture proposed by ANSI/SPARC, presents a model __composed of an external phase, a conceptual phase, and an internal phase__, none of which interferes with the others.
		- Types of schema:

			| Item | Contents | Remarks |
			| --- | --- | --- |
			| __External schema__ | An external schema is __composed of several users' viewpoints__ in the view phase, that is, a personal database schema viewed by everyone in each user's phase. <br> Individual database users or the database accessed by the application programmer are defined. | __User's viewpoint Schema composition according to accessed characteristics__ |
			| __Conceptual schema__ | Composed of one conceptual schema in the conceptual phase. The database of the entire organization is described, which has integrated all its users' perspectives.  <br> The database of the entire organization is described, which has integrated the data needed by all application systems or users, including the data saved in the database and the schema that expresses the relationship between the data. | __Integrated perspective__ |
			| __Internal schema__ | An internal schema is composed of an internal phase and an internal schema. The format in which the database is physically stored. <br> A schema that expresses how data are actually saved in a physical device. | __Physical storage structure__. |
	3. Data independence of two areas
		- Definition:
			- As the concept of data independence can be separated into these three phases, there are two terms that specify the independence of each area, namely '__logical independence__' and '__physical independence__'.
		- Types of independence:

			| Type | Contents | Characteristics |
			|---|---|---|
			| __Logical independence__ | When a __concept schema is changed__, an __external schema is not affected__. <br> An application program is not affected by a change in the logical structure. | Changeable according to the users' characteristics. <br> The integrated structure can be changed. |
			| __Physical independence__ | When an __internal schema is changed__, an __external/conceptual schema is not affected__. <br> An application program and a conceptual schema are not affected by a structural change of the storage device. | A conceptual structure can be changed without affecting a physical structure. <br> A physical structure can be changed without affecting a conceptual structure. |
	4. Relationship between mapping and independence
		- Definition:
			- The English word "mapping" can be translated into "sasang" in Korean, which can be defined as a "bridge that connects independent concepts". 
			- Broadly speaking, there are two types of mapping in data independence.
		- Types of mapping:

			| Finishing | Contents | Example |
			| --- | --- | --- |
			| __External/conceptual mapping__ (logical thought) | The __correlation between the external view and the conceptual view is defined__. | A view can have different types of fields depending on the user's access type. The field type of a conceptual view is not changed. |
			| __Conceptual/internal mapping__ (physical mapping) | The __correlation between the conceptual view and the stored database is defined__. | If the structure of the stored database changes, conceptual/ internal mapping should change to keep the conceptual schema intact. |
- C) Definition and key roles of the database administrator (_DBA_) and data architect (_DA_)
	1. Roles of the database administrator
		- Definition:
			- The _DBA_ __takes responsibility for the configuration and overall administration of the database__ to ensure that the functions of the database system are performed properly. 
		- Tasks and roles of the DBA: 

			| Functional tasks | Technology details | Role |
			| --- | --- | ---| 
			| __Data modeling__ | Data __modeling according to business__. Physical data modeling __according to a storage environment__. <br> __Semi-normalization, performance modeling__. | Role Plays the __role of a physical model for analysis/design__ when implementing a project.| 
			| __Physical database design__ | __Index design, storage space design__. __Clustering design, partition design, etc__. | Physical design __according to the physical space environment, server, DBMS__ - Plays the __role of the designer__ |
			| __Tuning__ (performance improvement) | __Improvement of performance__ according to the index distribution chart, join relationship, and type and number of transactions. |  Plays the __role of the tuner__. | 
			| __Database building__ | Creation of a table space and a data file space. <br> Creation of a database object. <br> Setting of parameters and specifying of a backup structure. | Plays the __role of the developer__. |
			| __Database operation__ | Backup/restoration.<br> Monitoring of memory and performance on a regular basis. | Plays the __role of the operator__. |
			| __Database standardization__ | Definition of a glossary and a domain. Management of enterprise meta-data. | __Manages the database or data standardization__. |
	2. Roles of the data architect (DA)
		- Definition:
			- A data architect __establishes, models, and systemizes the policies and standards__ for data-related elements such as __data, database, data standard, and data security__.
		- Roles of the data architect:

			| Role | Details | Key roles |
			| --- | --- | --- |
			| __Establishment of a data management system__ | Establishment of systems for metadata, data distribution/ integration, information lifecycle management (ILM), performance and capacity monitoring system, log management system, failure management system, etc. | __Establishment of data governance__ |
			| __Establishment of data standards__ | Establishment of standards related to entire data, such as definitions of terms and domains, data dictionary, metadata standards, etc. | __Maintaining consistency is very important__. |
			| __Performance of data modeling__ | Conceptual modeling > Logical modeling > Physical modeling | __Important roles in the structure of the entire data architecture__ |
			| __Establishment of data security systems__ | Establishment of systems for controlling user access, tables, views, etc., data encryption, access logs, transaction traceability, etc. | __Management of data security__ |
- D) Concept and functions of the DBMS
	1. Concept of the DBMS
		- A system contrived to __solve the problem of the file system, dependency and redundancy__.
		- A software system that __manages the database__ so that it can be shared dy all application programs as a __mediator between the application program and data__.
	2. Functions of the DBMS
		- There is a file structure that __stores a database, and memory and major processes__ to process the file structure in DBSM. 
			- Controls duplication from the aspects of data storage, and development and maintenance. 
			- Enables data sharing among multiple users.
			- Controls access to data by unauthorized users. 
			- Provides various types of interfaces to diverse users. 
			- Expresses the complex relationships that exist between data. 
			- Ensures the integrity of the database.
	3. Conceptual diagram and main functions of the DBMS
		- Definition:
			- There is a file structure that stores a database, and memory and major processes to process the file structure in DBSM.
		- Figure:
			![[CC105-17.png]]
		- DBMS components:

			| Component | Description |
			| --- | --- |
			| __DDL compiler__ | Processes the schema __specified in the DDL as an internal schema__, i.e. metadata, and __stores it in the system catalog__. <br> All DBMS modules should __access and use this catalog information when necessary__. |
			| __Query processor__ | Processes advanced queries __submitted by general users__. l.e. queries are __analyzed, parsed, and compiled__. Then, the database access code is created and sent to the runtime DB handler for execution. |
			| __DML pre-compiler__ | __DML commands inserted__ into an application program are extracted and sent to the DML compiler to be compiled as an object code for database access. |
			| __DML compiler__ | A DML compiler __generates an object code__ by parsing and compiling the received DML command. | 
			| __Runtime database handler__ | Database access is __managed at runtime__. That is, database operations such as __search or update are executed__ in the database using the storage data manager. | 
			| __Transaction manager__ | The transaction manager __checks compliance with integrity constraints and the user's rights__ while accessing the database. <br> __Performs restoration__ when controlling transactions concurrently or when a __failure__ occurs. |
			| __Stored data manager__ | The stored data manager __manages access to the user database and catalog stored in the disk__. (Request to the file manager of the OS.) |

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
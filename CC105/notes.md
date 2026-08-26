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
- Concept and characteristics of data, information, and knowledge.
	1. Data
		- Data refers to the collected resource itself, which are the basic data discovered, investigated, collected, and created in the real world. 
		- That is, data are related to a fact, which refers to a natural state free of the values and judgments of human heings.
	2. Information
		- Information refers to various data that are organized, classified, and systematized for certain purposes according to certain rules. 
		- When data are processed in a certain form, the information necessary for achieving a specific purpose is created.
	3. Knowledge
		- Knowledge refers to matter that is generalized from several items of concrete information.
		- It is created while analyzing and studying the meaning and relationship of informational data. 
		- Correlations between information should be established to convert information into knowledge. 
		- Therefore, information can vary significantly depending on how one assigns meaning to informatized data, analyzes the relationship, and judges the values of the human being. 
		- Enterprises and institutions manage such information or knowledge in such a way as to make decisions or create added value.
	- Data, information, and knowledge:

	| Item | Definition and characteristics | Key point |
	| --- | --- | --- |
	| Fact | A state of disorder in reality. Something that exists without being observed by others. | Phenomenon |
	| Data | Realistic data that exist widely in the real world. <br> Several simple facts that have not yet been evaluated for a specific purpose | Factual Data |
	| Information | When data are organized into meaningful patterns, they become information. <br> Data are treated and processed by a certain program (form) in order to create information necessary for achieving a specific purpose. | Treatment and value |
	| Knowledge | Information of the same type is accumulated and organized into a generalized form. <br> A state to which human interpretations and meanings are given. <br> Information is used for decision-making or creation, and added value is created. | Added value, generalization, and decision making |
	| Wisdom | A state in which an individual can understand and apply knowledge. <br> The mental ability to acquire, understand, apply, and develop knowledge. | Internalized ability |

- Concept and Characteristics oc data processing types.
	- Definition:
		- The data processing system, which is the core element of the information system, and is directly related to the computer, can be divided into batch processing, online processing, and distributed processing system depending on the type of data processing, in other words, how the data are organized and accessed.
	1. Batch processing system
		- Data is collected for a certain period or a certain amount to process it at once.
		- System-centered processing method. (Low processing cost and high system performance are required.) 
		- Preparatory work is required. (Collecting, classifying, and organizing raw data -> Writing in a file) 
		- Standby time is required. (Immediate processing is not supported.) 
		- The procedure of modifying changes is complex and difficult until files are processed collectively. 
		- Example: Payroll processing system, grade processing system, utility bill processing system, etc.
	2. Online processing system
		- When the daya are transfered to a computer, the computer immediately processes the data. (Real-time processing system)
		- User-centered processing method. (It incurs a high processing cost and low system performance is required.) 
		- Preparatory work is not required. 
		- Data currency is maintained. 
		- Difficult to maintain, repair, or restore. 
		- Example: Seat reservation processing systems for airlines and railroads, bank deposit processing systems, stock account systems for securities companies, etc.
	3. Distributed processing system
		- Data are processed by connecting processors and databases, which are geographically dispersed, over the network. 
		  Operated in the form of a client/server system. 
		- Improves the operation speed and reliability. 
		- Increases the efficient use of resources.
		- Software developement is difficult, and the security level and degree of design complexity are relatively high.

### 2. Understanding the Database
- Concept and characteristics of a file processing system.
	- Definition:
		- The term "file processing system" refers to a method of storing and retrieving paper documents that was widely used before the computer was invented. However, the meaning of the term began to include computerized records in the 1960s. Such a file system is designed to arrange and manage the data recorded by the user on a physical disk. In general, a hierarchical file system with a directory structure is used. 
		- Each application program in a file system accesses an individual file to process, in order to search, input, delete, and modify it. 
		- For example, if a file system is used when a certain web service system saves the user's log-in history, the application program that saves the login history has a unique form according to the characteristics of the application program, depending on the sequence in which the information to be saved is arranged, and the unit of classification of such information.
	1. Characteristics of the file processing system.
		- The application program should directly implement the logical file structure designed by the application programmer as a physical file structure. 
		- Application programmers can implement the data access method in the application program only when they know the physical data structure very well. 
		- Sharing data naturally becomes difficult in an environment where each application program has its own data. Therefore, one file ultimately exists only for one application only.
	2. Problems with the file system
		- Inability to guarantee data independence.
			- Program dependent.
		- Problem of ensuring data consistency.
			- Time dependence of a file (which has a different value depending on the time of retrieval). 
		- Problem of ensuring data integrity.
			- Values that are semantically the same should remain identical. 
		- Low sharing and use convenience.
			- Low economic feasibility and poor security management.
- Concept and characteristics of the database
	1. Concept of the database
		- Definition:
			- The database has the characteristics of integration, operation, storing, and sharing. 
			- In the past, data were inevitably saved in duplicate when recorded on paper, because even the same data could not be shared in real time. 
			- Data were also saved in several files in duplicate even when the file system was in use. 
			- The database, however, manages duplicated data in one place as intensively as possible to eliminate duplication to the maximum.
		- Data Classification:

			| Classification | Contents |
			|---|---|
			| Integrated data | This means that the same data are not duplicated in principle. <br> - Minimal redundancy <br> - Controlled redundancy |
			| Stored data | Data are saved in a storage medium that can be accessed by a computer (tape, disk, etc.). | 
			| Operational data | Data which are required to perform the unique functions of an organization. (Temporary data used while performing a task, such as simple input/output, are not operational data) |
			| Shared data | Data which are jointly owned, maintained, and used by several application programs within an organization. |
	2. Characteristics of the database
		- Definition:
			- The shared database can be accessed in real time using the programming language, and is constantly changing due to the input, modification and deletion of data. 
			- The database can also be accessed and shared by multiple users simultaneously, and it has the characteristic of being referable by using the contents of data.
		- Characteristics of the database:

			| Item | Contents |
			|---|---|
			| Real-time accessibility | Real-time responce to occasional and informal queries. |
			| Continuous evolution | Update, insert, delete: Dynamic characteristics (keeping the current state accurately during such changes). |
			| Concurrent sharing | Supports the concurrent sharing of the same data in different ways. |
			| Content reference | Refer to processing the contents of data requested by the user, (that is, by values) rather than by location or address. |

### 3. Understanding the Database System
- The concept and components of the database system (DBS)
	1. Definition of the database system
		- Definition:
			- The term 'DBS' refers to a computer-centered system that creates necessary information by storing and managing data in a database
		- Figure:
			![[CC105-15.png]]
	2. Components of the database system
		- Definition:
			- As regards the processing of data stored in a database, there is a user who processes it, a language that can manipulate and read data in the database, and DBMS software that enables the processing of all data. 
			- That is, a database system is composed of four attributes: database, database language, user, and database management system (DBMS).
		- DBS components:

			| Item | Contents |
			| --- | --- |
			| Database | A set of operational data integrated and stored with minimal redundancy, so that the multiple application systems of an organization can share it. |
			| Database language | A tool that provides an interface between people and system. |
			| Users | Database administrator (DBA), database application programmer, database user. |
			| Database management system (DBMS) | System software that provides database construction and utilization functions. |
- Data independence and ANSI-SPARC's 3-level database architecture.
	1. Background to introduction of the concept of data independence (reason for its necessity)
		- Figure:
			![[CC105-16.png]]
		- Definition:
			- To understand data independence, it is helpful to understand the background to the introduction of the concept of data independence. The opposite of data independence can be defined as data dependency. Here, the subject of dependency generally refers to an application program. An application is the interface object which interacts with users and handles the user requirements. It can be said that data dependency has the purpose of reducing continuously increasing maintenance costs, data complexity, and the number of duplicated data. The concept of data independence was also introduced to maintain independence between the screen and the database against the users' constantly evolving requirements. 
			- It can be said that data independence is a three-schema architecture, which was proposed by the special subcommittee of the X3 committee under the American Standards Institute (ANSI) for the DBMS and its interfaces.
			- The main purpose of this three-schema architecture was to reduce interference in changes, by separating the user's view of the database from the view by which the database is actually expressed. When data independence is secured, the independence of each view can be maintained, data can be changed without affecting the view by layer, and different DDL (data definition language) and DML (data manipulation language) can be provided according to the schema by phase.
	2. 3-level database architecture of ANSI-SPARC
		- Definition:
			- The data independence model, which is based on the 3-level database architecture proposed by ANSI/SPARC, presents a model composed of an external phase, a conceptual phase, and an internal phase, none of which interferes with the others.
		- Types of schema:

			| Item | Contents | Remarks |
			| --- | --- | --- |
			| External schema | An external schema is composed of several users' viewpoints in the view phase, that is, a personal database schema viewed by everyone in each user's phase. <br> Individual database users or the database accessed by the application programmer are defined. | User's viewpoint Schema composition according to accessed characteristics |
			| Conceptual schema | Composed of one conceptual schema in the conceptual phase. The database of the entire organization is described, which has integrated all its users' perspectives.  <br> The database of the entire organization is described, which has integrated the data needed by all application systems or users, including the data saved in the database and the schema that expresses the relationship between the data. | Integrated perspective |
			| Internal schema | An internal schema is composed of an internal phase and an internal schema. The format in which the database is physically stored. <br> A schema that expresses how data are actually saved in a physical device. | Physical storage structure.
	3. Data independence of two areas
		- Definition:
			- As the concept of data independence can be separated into these three phases, there are two terms that specify the independence of each area, namely 'logical independence' and 'physical independence.
		- Types of independence:

			| Type | Contents | Characteristics |
			|---|---|---|
			| Logical independence | When a concept schema is changed, an external schema is not affected. <br> An application program is not affected by a change in the logical structure. | Changeable according to the users' characteristics. <br> The integrated structure can be changed. |
			| Physical independence | When an internal schema is changed, an external/ conceptual schema is not affected. <br> An application program and a conceptual schema are not affected by a structural change of the storage device. | A conceptual structure can be changed without affecting a physical structure. <br> A physical structure can be changed without affecting a conceptual structure. |
	4. Relationship between mapping and independence
		- Definition:
			- The English word "mapping" can be translated into "sasang" in Korean, which can be defined as a "bridge that connects independent concepts". 
			- Broadly speaking, there are two types of mapping in data independence.
		- Types of mapping:

			| Finishing | Contents | Example |
			| --- | --- | --- |
			| External/conceptual mapping (logical thought) | The correlation between the external view and the conceptual view is defined. | A view can have different types of fields depending on the user's access type. The field type of a conceptual view is not changed. |
			| Conceptual/internal mapping (physical mapping) | The correlation between the conceptual view and the stored database is defined. | If the structure of the stored database changes, conceptual/ internal mapping should change to keep the conceptual schema intact. |
- Definition and key roles of the database administrator (DBA) and data architect (DA)
	1. Roles of the database administrator
		- Definition:
			- The DBA takes responsibility for the configuration and overall administration of the database to ensure that the functions of the database system are performed properly. 
		- Tasks and roles of the DBA: 

			| Functional tasks | Technology details | Role |
			| --- | --- | ---| 
			| Data modeling | Data modeling according to business. Physical data modeling according to a storage environment. <br> Semi-normalization, performance modeling. | Role Plays the role of a physical model for analysis/design when implementing a project.| 
			| Physical database design | Index design, storage space design. Clustering design, partition design, etc. | Physical design according to the physical space environment, server, DBMS - Plays the role of the designer |
			| Tuning (performance improvement) | Improvement of performance according to the index distribution chart, join relationship, and type and number of transactions. |  Plays the role of the tuner. | 
			| Database building | Creation of a table space and a data file space. <br> Creation of a database object. <br> Setting of parameters and specifying of a backup structure. | Plays the role of the developer. |
			| Database operation | Backup/restoration.<br> Monitoring of memory and performance on a regular basis. | Plays the role of the operator. |
			| Database standardization | Definition of a glossary and a domain. Management of enterprise meta-data. | Manages the database or data standardization. |
	2. Roles of the data architect (DA)
		- Definition:
			- A data architect establishes, models, and systemizes the policies and standards for data-related elements such as data, database, data standard, and data security.
		- Roles of the data architect:

			| Role | Details | Key roles |
			| --- | --- | --- |
			| Establishment of a data management system | Establishment of systems for metadata, data distribution/ integration, information lifecycle management (ILM), performance and capacity monitoring system, log management system, failure management system, etc. | Establishment of data governance |
			| Establishment of data standards | Establishment of standards related to entire data, such as definitions of terms and domains, data dictionary, metadata standards, etc. | Maintaining consistency is very important. |
			| Performance of data modeling | Conceptual modeling > Logical modeling > Physical modeling | Important roles in the structure of the entire data architecture |
			| Establishment of data security systems | Establishment of systems for controlling user access, tables, views, etc., data encryption, access logs, transaction traceability, etc. | Management of data security |
- Concept and functions of the DBMS
	1. Concept of the DBMS
		- A system contrived to solve the problem of the file system, dependency and redundancy.
		- A sortware system that manages the database so that it can besnared dy all application programs as a medlph between the application program and data.
	2. Functions of the DBMS
		- There is a file structure that stores a database, and memory and major processes to process the file structure in DBSM. 
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
			| DDL compiler | Processes the schema specified in the DDL as an internal schema, i.e. metadata, and stores it in the system catalog. <br> All DBMS modules should access and use this catalog information when necessary. |
			| Query processor | Processes advanced queries submitted by general users. l.e. queries are analyzed, parsed, and compiled. Then, the database access code is created and sent to the runtime DB handler for execution. |
			| DML pre-compiler | DMU commands inserted into an application proaram are extracted and sant to the DNM compiler to be compiled as an object code for database access. |
			| DML compiler | A DML compiler generates an object code by parsing and compiling the received DML command. | 
			| Runtime database handler | Database access is managed at runtime. That is, database operations such as search or update are executed in the database using the storage data manager. | 
			| Transaction manager | The transaction manager checks compliance with integrity constraints and the user's rights while accessing the database. <br> Performs restoration when controlling transactions concurrently or when a failure occurs. |
			| Stored data manager | The stored data manager manages access to the user database and catalog stored in the disk. (Request to the file manager of the OS.) |

## Understanding Types of Database
### 1. Types of Databases
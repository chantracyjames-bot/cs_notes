### > [Table of Contents](../main.md)
# CC105
---
## Target
- Recent trends and major issues
	- According to the annual White Paper on the Data Industry published by the Korea Data Agency, the domestic data-related market is showing a steady growth trend. 
	- The trend also shows that interest in the diversity and availability of data is increasing significantly. 
	- Considering this trend, the fields of data utilization, database construction, and data solutions seem to be maintaining a steady rate of growth in all industries in Korea. 
	- It is also obvious that personnel requirements in the related fields will increase significantly in the coming years. 
	- Likewise, we can anticipate the main trends of business, such as the spread of the cloud platform to the data environment, increased interest in data quality management, and increased decision-making based on data. 
	- Judging from these trends, it is evident that competence related to the processing and utilization of data is becoming increasingly important.
- Learning Objectives
	1. To be able to explain the concepts and characteristics of data, information, and knowledge in the Information Age. 
	2. To be able to explain the concept and characteristics of data processing. 
	3. To be able to explain the concept and characteristics of the file handling system. 
	4. To be able to explain the concept and characteristics of the database. 
	5. To be able to explain the concepts and components of the database system. 
	6. To be able to explain the 3-level database architecture of ANSI-SPARC. 
	7. To be able to explain data independence. 
	8. To be able to explain the roles of the database administrator (DBA) and the concept of the data architect (DA).
	9. To be able to explain the concept and functions of the DBMS (Database Management System).
- Reasons to understand data and databases
	- T here are many cases in which a database is used llike an existing file system, and tabies are created in the database, but each table is actually dependent on individual applications, screens, and reports. For example, when developing a book management system for each team a booklist table can be created for each team during implementation of the database in the same way as managing books using Excel files. However, if tables are designed in the same way as Excel files, the advantages of the database, including integration, storage, operation, and sharing, cannot be utilized at all. 
	- In this case, the complexity of the application program also increases, causing problems that can lead to serious symptoms, such as an increase in the development cost, problems with data integrity (lack of consistency due to data duplication), and deterioration of data processing performance. Therefore, these problems can be prevented, and the advantages of the database can be maximized and applied to system development only when we understand the definition and characteristics of the database (integration, storage, operation, sharing) and its advantages, and apply them to practical business.

## Understanding Data and Databases
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

# > [Lesson 2a](/CC105/Lesson%202a.md)
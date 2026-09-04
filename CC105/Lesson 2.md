### < [Back](./Lesson%201.md) :---: [Next](./Lesson%203.md) >
# > [CC105](./CC105.md) - Information Management
### Lesson 2
---
## Entity Relationship Modeling
- Concept and Definition
	- An Entity-Relationshtip (ER) model is the mainstream approach for conceptual data modeling.
	- The ER model is a detailed, logical representation of the data for an organization or for a business area.
	- Expressed in terms of entities in the business, the relationships—or associations—among these entities, and the attributes—or properties—of both the entities and their relationships.
	- Normally expressed as an ER diagram, which is a graphical representation of an ER model
	- Sample Entity Relationship Diagram (Mermaid Syntax):
		```mermaid
		erDiagram
			SUPPLIER ||--o{ SHIPMENT : "SENDS"
			SHIPMENT }o--|{ ITEM : "INCLUDES"
			SUPPLIER }|--o{ ITEM : "SUPPLIES"
			
			PRODUCT }|--|{ ITEM : "USED IN"
			PRODUCT }|--o{ ORDER : "REQUESTS"
			ORDER }o--|| CUSTOMER : "SUBMITS"
		
		```
- Entity-Relationship Model Notations:
	- ER Model Notation Symbols:
![[../.images/CC105/CC105-0.png]]
	- ER Model Relationship Degrees:
![[../.images/CC105/CC105-2.png]]
	- ER Model Relationship Cardinalities:
![[../.images/CC105/CC105-1.png]]
## Entity-Relationship Model Constructs
### Entities
- Definition:
	- A person, place, object, event, or concept in the user environment.
	- About which the organization wishes to maintain data on.
- Symbol:
	- Rectangle
- Examples:
	- Person: EMPLOYEE, STUDENT, PATIENT
	- Place: CITY, STATE, COUNTRY
	- Object: MACHINE, BUILDING, AUTOMOBILE
	- Event: SALE, REGISTRATION, RENEWAL
	- Concept: ACCOUNT, COURSE, ORDER
- Entity Type
	- Is a collection of entities that share common properties or characteristics.
	- An entity type is described just once in a database.
	- The entity type name is always singular in capital letters.
	- Types of Enitities
		- Strong Entity Type
			- Definition:
				- Is one that exists independently of other entity types.
				- Always have an attribute or a combination of attributes—or an identifier—that uniquely distinguish each insteance of that entity type.
			- Symbol:
				- Single-lined Rectangle
		- Weak Entity Type
			- Definition:
				- Is an entity type whose existence depends on some other entity type.
				- It has now business meaning and is not needed in the ER diagram without the entity on which it depends on.
				- A weak entity type does not have its own identifier,
				- The entity type on which the weak entity type depends on is called the identifying owner—or simply owner.
			- Symbol:
				- Double-lined Rectangle
- Entity Instance
	- Is a single occurence of an entity type.
	- Many instances of an entity type may be in a database.
### Attributes
- Definition:
	- Is a property or characteristic of an entity type—or a relationship—that is of th interest to the organization.
	- In diagramsm it is connected to the entity—or relationship—by a line
	- Attribute names: proper casing, a dash between the words, underlined—if the attribute is an identifier.
- Symbol:
	- Ellipse
- Example:
	- STUDENT: Student-ID, Student-Name, Major
	- EMPLOYEE: Employee-ID, Employee-Name, Skill
- Types of Attributes:
	- Simple Attributes
		- Definition:
			- Is a type of attribute that cannot be broken down into smaller components
			- Example:
				- Street, City, Province, and Postal-Code.
				- First-Name, Middle-Name, Last-Name
	- Composite Attributes
		- Definition:
			- Is an attribute that can be broken down into component attributes.
			- In ER diagrams, the component attributes can appear above or below the composite attribute.
			- A simple (or atomic) attribute is an attribute that cannot be broken down into smaller components.
		- Example:
			- Address — can be broken down into Street, City, Province, etc.
			- Name — can be broken down into First-Name, Middle-Name, Last-Name
	- Single-valued Attributes
		- Definition:
			- An attribute that can only take one value for a given entity instance.
		- Example:
			- Age, ID, etc.
	- Multi-valued Attributes
		- Definition:
			- Are attributes that may take on more than one value for a given entity instance.
		- Symbol:
			- Double-lined Ellipse
		- Example:
			- Phone Number — can be a Landline or a Mobile Number.
			- Skill — can be more than one skills.
	- Derived Attributes
		- Definition:
			- Are attributes that are able to be calculated from related attribute values from the same entity or from other entities in the ER model.
			- It can also be calculated from data not in the database, such as today's date, the current time, etc.
		- Symbol:
			- Dashed-line Ellipse
		- Example:
			- Years-Employed — can be taken from Date-Employed.
- Identifier:
	- Definition:
		- Is an attribute—or combination of attributes—that uniquely indentifies individual instances of an entity type.
		- For instance, an attribute such as Student-Name is not a candidate indentifier or key, since many students may potentially have the same name and students, like all people, can change their names
	- Composite Indentifier:
		- Definition:
			- Is an identifier that consists of a composite attribute.
		- Example:
			- Flight-ID — consisting of the Flight-Number and Date.
### Relationships
- Definition:
	- Is the "glue" that holds together the various components of an ER model.
	- An association among the instances of one or more entity types that is of interest to the organization.
	- Name : with a single verb phrase; past tense; descriptive.
- Symbol:
	- Diamond
- Example:
	- Diagram:
		``` mermaid
		erDiagram
		direction LR
			COURSE }|--|{ EMPLOYEE : Completes
		
		EMPLOYEE {
			int Employee-ID
			string Employee-Name
		}
		COURSE {
			int Course-ID
			string Course-Title
		}
		```
	- Explanation:
		- COURSE represents the training course that may be taken by employees.
		- EMPLOYEES represents the individuals who may partake in courses.
		- Completes tracks courses that have been competed by particular employees.
		- a many-to-many relationship, since each employee may complete any number of courses.
- Relationsip Types
	- Is a "meaningful association" between—or among—entity types.
	- meaningful association implies that the relationship allows us to answer to questions that could be answered given only by entity types.
- Relationship Instance
	- Is an association between—or among—entity instances, where each relationship instance includes exactly one entity from each participating entity type.
- Associative Entities
	- Definition:
		- The presence of one of more attributes on a relationship that the relationship can be represented as an entity type.
	- Example:
		- Diagram of attributes on a relationship:
			![[../.images/CC105/CC105-3.png]]
		- Diagram of an associative entity:
			![[../.images/CC105/CC105-4.png]]
	- When to convert to Associative Entities?
		- If all of the relationships for the participating entity types are "many" relationships.
		- If the resulting associative entity type has independent meaning to end users, and preferably can be indentified with a single-attribute identifier.
		- If the associative entity has once or more attributes, in addition to the identifier.
		- If the associative entity participates in one or more relationships independent of the entities related in the associative relationships.
	- Cardinality
		- Definition:
			- The conversion of a relationship to an associative entity caused the relationship cardinality notation to move.
			- The "many" cardinality now terminates at the associative entity, rather than at each participating eneity type.
			- The previous diagram (Diagram of attributes on a relationship) indicates that an employee may complete one or many courses, and that a course may have one or more employees completing it.
			- The new diagram (Diagram of an associative entity) shows that an employee may be awarded more than one certificate, and that a course may have awarded many certificates.
		- Cardinality Constraints
			- For instance, suppose there are two entity types, A and B, that are connected by a relationship.
			- A cardinality constraint specifies the number of instances, of entity B that can (or must) be associated with each instance of entity A.
			- Diagram:
				![[../.images/CC105/CC105-9.png]]
				- Treat Entity A as MOVIE and Entity B as VIDEOTAPE.
		- Minimum and Maximum Cardinality
			- Minimum Cardinality
				- Is the minimum number of instances of an entity that may be associated with each instance of another entity.
			- Maximum Cardinality
				- Is the maximum number of instances of an entity that may be associated with a single occurence of another entity
			- Diagram:
				![[../.images/CC105/CC105-10.png]]
				- Treat MOVIE as the Minimum Cardinality and VIDEOTAPE as the Maximum Cardinality.
		- Example:
			- Cardinality in Ternary Relationships with Associative Entities:
				![[../.images/CC105/CC105-11.png]]
- Degree of Relationships
	- Definition:
		- The number of entity types that participate in that relationship.
		- The three most common relationship degrees:
			- Unary — degree of 1
			- Binary — degree of 2
			- Trinary — degree of 3
		- Technically, higehr-degree relationships are possible, but they are rarely encountered in practice. These types of relationship degrees are called N-nary Relationships.
	- Examples:
		- Unary Relationship Diagram:
			![[../.images/CC105/CC105-5.png]]
		- Binary Relationship Diagram:
			![[../.images/CC105/CC105-6.png]]
		- Trinary Relationship Diagram:
			![[../.images/CC105/CC105-7.png]]
		- Trinary Relationship with Associative Entity Diagram:
			![[../.images/CC105/CC105-8.png]]
- Example:
	- Modeling Time-Dependent Data:
		- Before:
			![[../.images/CC105/CC105-12.png]]
		- After:
			![[../.images/CC105/CC105-13.png]]
- Exercise:
	- Given:
		- A university has a large number of courses in its catalog.
		- Each course is uniquely identified by its course number.
		- The university records all course names and units per course.
		- Each course may have one or more different courses as prerequisites, or may have no prerequisites at all.
		- Similarly, a particular course may be a prerequisite for any number of courses, or may not be a a prerequisite for any course at all.
	- Solution:
		``` mermaid
		erDiagram 
			COURSE { 
				string course_number PK "Unique course number" 
				string course_name "Name of the course" 
				int units "Units per course" } 
				
			COURSE ||--o{ PREREQUISITE : "has prerequisite" 
			COURSE ||--o{ PREREQUISITE : "is prerequisite for" 
			
			PREREQUISITE { 
				string course_number PK, FK 
				string prerequisite_course_number PK, FK 
			}
		```

# > [Lesson 3](./Lesson%203.md)
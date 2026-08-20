### > [Table of Contents](../main.md)
# CC105
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
![[CC105-0.png]]
	- ER Model Relationship Degrees:
![[CC105-2.png]]
	- ER Model Relationship Cardinalities:
![[CC105-1.png]]
## Entity-Relationship Model Constructs
- Entities
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
- Attributes
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

# # > [Lesson 3](CC105/Lesson%203.md)
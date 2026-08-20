### > [Table of Contents](../main.md)
# CC105
---
## Entity-Relationship Model Constructs
- Relationships
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
				![[CC105-3.png]]
			- Diagram of an associative entity:
				![[CC105-4.png]]
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
					![[CC105-9.png]]
					- Treat Entity A as MOVIE and Entity B as VIDEOTAPE.
			- Minimum and Maximum Cardinality
				- Minimum Cardinality
					- Is the minimum number of instances of an entity that may be associated with each instance of another entity.
				- Maximum Cardinality
					- Is the maximum number of instances of an entity that may be associated with a single occurence of another entity
				- Diagram:
					![[CC105-10.png]]
					- Treat MOVIE as the Minimum Cardinality and VIDEOTAPE as the Maximum Cardinality.
			- Example:
				- Cardinality in Ternary Relationships with Associative Entities:
					![[CC105-11.png]]
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
				![[CC105-5.png]]
			- Binary Relationship Diagram:
				![[CC105-6.png]]
			- Trinary Relationship Diagram:
				![[CC105-7.png]]
			- Trinary Relationship with Associative Entity Diagram:
				![[CC105-8.png]]
- Diagrams:
	- Modeling Time-Dependent Data:
		- Before:
			![[CC105-12.png]]
		- After:
			![[CC105-13.png]]
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

# > [Lesson 4](CC105/Lesson%204.md)
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
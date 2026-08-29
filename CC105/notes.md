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

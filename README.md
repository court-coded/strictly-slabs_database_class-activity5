\#slabs \_database\_class-activity5



\*\*A. entity:\*\*

an entity is a thing we store data about ,it becomes a table. 

\*\*example:\*\* A book is an entity. Another is a customer or Author. The bookstore needs to keep a list of all books it sells.



\*\*B. Relationship\*\*

A relationship is the link or connection between two entities , it shows how they work together.

\*\*example:\*\* A 'customer' \*\*PLACES\*\* an 'Order'. The relationship is "PLACES".A customer can place many orders, but each order belongs to one customer



\*\*C. Attribute\*\*   

A detail about am entity.it becomes a column 

\*\*example\*\* For the 'Book' entity , attributes are 'BookID' , 'Titles', 'Prices', ISBN', and 'stockQuantity'. 'Titles' describes what the book is called .



\### Data model levels

\*\*conceptual data model:\*\*

**-\*\***what is  it :\*\* A high-level, simple model that shows WHAT data the business needs. It shows Entities and Relationships only, no technical details like data types. 



\*\*logical data model:\*\*

Defines HOW the system should be implemented regardless of the specific DBMS .created by data architects and business analysts to map technical  rules and structures.



\*\*physical data model\*\*

describes HOW the system will be implemented using specific DBMS like (PostgreSQL)created by DBA and developers for actual database creation.



\## Section 3: 



\### ER Mapping 

\*\*Relationship:\*\* customer PLACES order 



\*\*Entity 1: Customer\*\* 

\-customerID (primary key)

\-FirstName

\-LastName

\-Email

\-Phone



\*\*Entity 2: Order\*\*

\-OrderID(primaykey)

\-OrderDate

\-TotalAmount

\-CustomerID(Foreign key)

\*\*Cardinality:\*\* One-to-many(1:M)

\*\*Explanation:\*\* One customercan place MANY Orders,but each order belongs to only ONE Customer.That is why we put CustomerID inside the Order table a foreign key to link them.


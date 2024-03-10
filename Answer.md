1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

Ans: ONE-TO-MANY Relationship.

Explaination: The relationship between the "Product" and "Product_Category" entities in the diagram is a one-to-many relationship, denoted by the "1" near the "product_category" entity and the crow's foot near the "product" entity. This indicates that one record in the "Product_Category" table can be associated with many records in the "Product" table. In practical terms, this means that each product belongs to one category, while each category can encompass many products. The connection is established through the "category_id" field in the "Product" table, which acts as a foreign key that references the "id" field in the "Product_Category" table.



2. How could you ensure that each product in the "Product" table has a valid category assigned to it?

Ans: category_id is the foreign key 🗝 in product table

Explaination: To ensure that each product in the "Product" table has a valid category assigned to it, the "category_id" column should be set up as a foreign key that references the "id" column of the "product_category" table. Additionally, you should not allow null values in the "category_id" column to enforce that each product must have a category. This can be done during the creation of the table or by altering the table structure to add a foreign key constraint.
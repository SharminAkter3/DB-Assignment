## Question & Answer

#### Question 1
Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

Answer 1

The relationship between the "Product" and "Product_Category" entities is a one-to-many relationship. This means that one category can have multiple products associated with it, but each product can only belong to one category. The relationship is established through the "category_id" column in the "Product" table, which references the primary key "id" column in the "Product_Category" table.

#### Question 2
How could you ensure that each product in the "Product" table has a valid category assigned to it?

Answer 2

To guarantee that every product is correctly categorized, we implement a system that cross-checks each product's assigned category. We do this by linking the "category_id" column in the "Product" table to the "id" column in the "Product_Category" table using a special rule called a foreign key constraint. This rule ensures that whenever a product is added or updated, its category ID must match an existing category in the "Product_Category" table. It's like ensuring each product is assigned to a valid category before it's officially stored in our system, which helps keep our data organized and accurate.

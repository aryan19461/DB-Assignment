Answer 1 ) Product holds the products with Id, name ,sku etc while the product_category holds the cross-relation between one or many products.

Answer 2 )To ensure data integrity, create a foreign key constraint between the "Product" and "Category" tables. This will ensure that each product has a valid category assigned to it. When you insert a new product, you must provide a valid CategoryID that already exists in the "Category" table. If you try to insert an invalid CategoryID, the database will raise a foreign key constraint violation error.


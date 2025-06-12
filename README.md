# **Tableau-Project**

## Objective
To Build a Sales and Customer Dashboard on Tableau to provide valuable insights about the data.

## Architecture
![image](https://github.com/user-attachments/assets/41a2c8a5-1478-4d8a-bc85-4d9f8a11c7ea)


## Data Model
This project uses multiple datasets in the .csv format. These datasets have both fact as well and dimension tables. The project uses data of 2020-2023. Therefore STAR schema is used to build the data model.

## Data Catalog

### Overview
Data catalog is the short description of the data which is used to increase the readability of the code and helps the viewers to get a better understanding about the data before processing it. 

#### 1. Customers
**Purpose**: Stores all details about the customers. It is a dimension table of size 2 x 793
**Columns**: 

| Column        | Data Type                  | Description     |
|----------------|------------------------------|------------|
| Customer ID | STRING   | Contains Customer ID in the string format e.g (AA-10315)   |
| Customer Name | STRING  | Contains customer name in string format  |


#### 2. Location
**Purpose**: Stores all details about the location. It is a dimension table of size 5 x 632. 
**Columns**: 

| Column        | Data Type                  | Description     |
|----------------|------------------------------|------------|
| Postal Code | Geographic Role: ZIP Code/Postcode   | Contains the postal code of the city e.g (73034, etc.)   |
| City |  Geographic Role: City  | Contains the name of the city e.g (Houston, etc.)  |
| State | Geographic Role: State   | Contains the name of the state e.g (Texas, etc.)   |
| Region |  Geographic Role: Region  | Contains the region e.g (Central, East, etc.)  |
| Country/Region | Geographic Role: Country   | Contains the name of the country e.g United States |


#### 3. Products
**Purpose**: Stores all details about the products. It is a dimension table of size 4 x 1894.
**Columns**: 

| Column        | Data Type                  | Description     |
|----------------|------------------------------|------------|
| Product ID | STRING  | Contains the product id in string format e.g (FUR-BO-10000112, etc.)   |
| Category |  STRING  | Contains the category of the product e.g (Furniture, etc.)  |
| Sub category | STRING   | Contains the sub category of the product e.g (Bookcases, etc.)   |
| Product Name |  STRING  | Contains the product name e.g (Hon Metal Bookcases,Putty etc.)  |


#### 4. Orders
**Purpose**: Stores all details about the orders. It is a fact table of size 13 x 9994.
**Columns**: 

| Column        | Data Type                  | Description     |
|----------------|------------------------------|------------|
| Row ID | INT  | Contains the row id in number format e.g (1, 2, .... etc.)   |
| Order ID |  STRING  | Contains the order id in the string format e.g (CA-2022-152156, etc.)  |
| Order Date | DATE   | Contains the order date in date format e.g (08-11-2022, etc.)   |
| Ship Date |  DATE  | Contains the shipping date in date format e.g (11-11-2022, etc.)  |
| Customer ID | STRING  | Contains the customer id in string format from the customer table e.g (CG-12520, etc.)   |
| Segment |  STRING  | Contains the segment of the customers in string format e.g (Consumer, Corporate etc.)  |
| Postal Code | Geographic Role: ZIP Code/Postcode   | Contains the postal code of the city from locaton table e.g (42420, etc.)   |
| Product ID |  STRING  | Contains the product id from the products table e.g (FUR-BO-10000112, etc.)  |
| Sales |  FLOAT  | Contains the sales in the decimal number format e.g (783.55, etc.)  |
| Quantity | INT  | Contains the quantity of the products in number format e.g (2, 4, etc.)   |
| Discount |  FLOAT  | Contains the discount in the decimal number format e.g (0.450000, etc.)  |
| Profit |  FLOAT  | Contains the profit in the decimal number format e.g (41.91, etc.)  |


# License
This project uses MIT license which ensures that this project is open to use, modify and download. Feel free to have a look. 







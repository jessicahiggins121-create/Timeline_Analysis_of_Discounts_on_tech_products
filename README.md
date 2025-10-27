# Timeline_Analysis_of_Discounts_on_tech_products
Business Analysis using data cleaning and quality methodology to condunct analysis on the average discounts, and revenues used from Jan 2017 - Mar 2018 

Goal: to understand whether or not it’s beneficial to discount products.
Insights were: the max beneficial discount was around 30% off products all other discount higher than that did not increase the sales of tech products as much. 


#### Collaborators: Analysis was done with: `<tanishtara>`:<https://github.com/tanishtara> & `<Irine>`:https://github.com/irinedivya<https://github.com/irinedivya>
## Source: ENIAC Sales Datasets 
Data - provided by WBS Coding School 
- Note orders, orderlines, and products have corrupted values in price columns, and are missing over values such as description.
 During Data cleaning and quality checks around 80% of data was removed during conservative analysis. 
## Data description

* **orders.csv** – Every row in this file represents an order.
    * _order_id_ – a unique identifier for each order
    * _created_date_ – a timestamp for when the order was created
    * _total_paid_ – the total amount paid by the customer for this order, in euros
    * _state_ 
        * “Shopping basket” – products have been placed in the shopping basket
        * “Place Order” – the order has been placed, but is awaiting shipment details 
        * “Pending” – the order is awaiting payment confirmation
        * “Completed” – the order has been placed and paid, and the transaction is completed.
        * “Cancelled” – the order has been cancelled and the payment returned to the customer.

<br>

* **orderlines.csv** – Every row represents each one of the different products involved in an order.
    * _id_ – a unique identifier for each row in this file
    * _id_order_ – corresponds to orders.order_id
    * _product_id_ – an old identifier for each product, nowadays not in use
    * _product_quantity_ – how many units of that product were purchased on that order
    * _sku_ – stock keeping unit: a unique identifier for each product
    * _unit_price_ – the unitary price (in euros) of each product at the moment of placing that order
    * _date_ – timestamp for the processing of that product<br>

<br>

* **products.csv**
    * _sku_ – stock keeping unit: a unique identifier for each product
    * _name_ – product name
    * _desc_ – product description
    * _price_ – base price of the product, in euros
    * _promo_price_ – promotional price, in euros
    * _in_stock_ – whether or not the product was in stock at the moment of the data extraction
    * _type_ – a numerical code for product type<br>

<br> 

* **brands.csv**
    * _short_ – the 3-character code by which the brand can be identified in the first 3 characters of products.sku
    * _long_ – brand name
 
## Key Findings & Results
1) Average discount of 30% shows the most growth in orders
2) Holiday's impact orders and having lower discounts will not affect orders
3) Top products were in repairs, upgrades and accessories

## Technologies Used
Programming language(s)
- Python
Key libraries and frameworks
- pandas, seaborn

## Environment:
- Google Colab 
## Project Structure
#### Data files: 
- `<cleaned and quality>`:<https://drive.google.com/drive/folders/17eSb1EA2aW0fK5pHEEhAnzdH8EeRqik_?usp=drive_link>
- `<original>`:<https://drive.google.com/drive/folders/13OGwxS4tp-HjQRhCtpPfhJDnipnb90dm?usp=sharing>
  
#### Project files: 
- Data exploration
- Data cleaning
- Data quality check
- Creation of catagories
- Data Analysis

📈 Visualisations
🔗 How to Use This Project
Direct link to your main notebook (make sure it’s public if in Colab)

Any setup instructions needed
How to reproduce your results
What files to look at first

Template:
1. Main Analysis: View the complete analysis uploaded in files
2. Data: Download dataset from or use the file in the data linked above
3. Run the Code: Open notebook in Google Colab run all cells once you have uploaded the data to where you are working from
4. Dependencies: import Pandas and Seaborn

🚀 Future Work
I would like to see if we could get customer orders and see if we had onetime 
customers or return becauese that was a question posed by the martkeing team. 

Potential improvements to analysis would be: 
1) Using product types more to explore if there were season trends when they were bought.
2) See if I can reduce the amount of data removed during the cleaning process if I can go back
3) Attempt to do trend forcasing with timedate-analysis
Additional questions you would explore
4) Real-time Analysis: Implement live customer scoring system
5)A/B Testing: Design experiments to validate retention strategies

 ## Contact

LinkedIn: [Jessica Higgins](https://www.linkedin.com/in/jessicahiggins-rde/)

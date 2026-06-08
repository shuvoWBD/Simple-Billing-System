# Simple-Billing-System

A Simple Billing System is a software application that helps a business calculate the cost of products purchased by customers and generate a bill or invoice automatically.

**Project Overview**

This project is a Python-based billing and inventory management system developed for an electronic store. The system allows customers to purchase products, calculate total costs, apply discounts based on purchase amount, generate invoices automatically, and update product inventory after each purchase. The application is divided into multiple modules to improve code organization, maintainability, and scalability. The system reads product information from a stock file, processes customer purchases, calculates discounts, generates detailed invoices in text format, and updates the available stock after each transaction.


**✨Key Features**

**1. Product Inventory Management**
   
   . Reads product data from a text file (products.txt).
   
   . Displays available products, prices, and quantities.
   
   . Updates stock after every purchase.
   

**Functions Used:**

    .  read_file()

**2. Customer Purchase Processing**

      . Allows customers to select products.
      
      . Accepts multiple product purchases in a single transaction.
      
      . Validates product availability.
      
     . Checks stock quantity before confirming purchase.


  **Functions Used:**

      . purchase()
      
      . Dictionary (q) for storing purchased items.
      
      . Loops (while, for)
      
      . Conditional statements (if-elif-else)
      

**3. Exception Handling**

     . Prevents invalid quantity inputs.
     
     . Ensures users enter numeric values when required.

  **Techniques Used:**

      try:
      except:


  **4. Automated Discount Calculation**

       The system provides discounts based on total purchase amount:

        | Purchase Amount | Maximum Discount |
        
        | --------------- | ---------------- |
        
        | Below 5000      | No Discount      |
        
        | 5000 - 9999     | Up to 5%         |
        
        | 10000+          | Up to 10%        |


    **Functions Used:**

        . Conditional Statements
        
         . Arithmetic Operations


  **5. Invoice Generation**
  
         . Automatically generates a unique invoice file.
         . Saves invoice as .txt format.
         . Includes:
         
               - Customer Name
               - Purchased Products
               - Quantity
              -  Unit Price
              -  Discount
              -  Final Amount
              -  Date & Time


   **Libraries Used:**

             . import datetime


   **6. Date and Time Management**
   
             . Generates unique invoice names using current date and time.
             
             . Records transaction timestamp.
             

**Functions Used:**

             datetime.datetime.now()


**7. File Handling**

           . The project performs various file operations:


**Reading Product Data**

              open("products.txt", "r")


**Writing Invoice**

            open(invoice_name, "w")


**Updating Inventory**

             write.over_write()


 **8. Modular Programming**

The project follows a modular design using separate Python files:


        | Module      | Purpose               |
        
        | ----------- | ---------------------------- |

        | main.py     | Main program execution       |

        | read.py     | Read product inventory       |

        | purchase.py | Customer purchase processing |

        | write.py    | Inventory update after sales |


This improves:

    . Code reusability.
    
    . Maintainability.
    
    . Readability.


**Python Concepts Used**

**Functions**

      read_file()
      
       purchase()
       
       over_write()


 **Loops**

        for loop
        
        while loop


**Conditional Statements**

        if
        
       elif
       
       else


 **Exception Handling**

         try
         
         except


   **Dictionaries**

           q = {}
           

   **Lists**     

          L = []


**File Handling**

         open()
         
         readlines()
         
         write()
         
         close()


**Date & Time**

         datetime


**String Manipulation**

          upper()
          
          replace()
          
          split()

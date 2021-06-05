# cat2

----------------------------------------------------------------------------------
Inventory-Management-System
----------------------------
Overview:
This application was designed for a small company to use as an inventory management solution. The user is able to create multiple inventories across different products locations. The user is also able to run a report across all products to create a master reorder list. 

    Register Page:
    ---------------
This is where a user can create a new account. Since the software is used for a specific companies inventory a company code is required to create an account. When all the information is entered and validated on the server side, the password is then salted and hashed with bcryptjs and all of the information is stored on the db. The user is redirected to the login page where they can use their new credentials to login.
           Login Page:
           -----------

           Here a user may login if they have already created an account. The user is authenticated with passport.js and the password handled by bcryptjs. When a user is succesfully authenticated the authentication is stored in a session so the user can access protected routes.

           Home Page
           ----------
The home page gives a broad overview of the use of the application. The navigation bar on the right side allows the user to navigate to inventory or reports. The logout button ends the session.

     Inventory Page
     -------------

The inventory page displays a list of vehicles/locations and also allows a user to create a new one. Clicking on a specific vehicle will get the inventory for that specific vehicle. Both vehicle and items support all CRUD operations.
               Reports Page:
               ------------
    The reports page compares current inventory quantity to the reorder point set on each item. All items with a quantity below the reorder point are then displayed in a ordered list.
               How to use:
               -------------
             run php artisan serve command,after getting server to use  
             login with username=admin@gmail.com and password=admin and then press enter key to proceed.

           ITS FEATURES:
           ------------
           ==>IWe used inventory_mini as a database to store the daily recod.  
           Technologies Used
           ----------------
           -Laravel framework
           -css,jquery,js,html,php and so on..
       License:
       ------------
        Basically, feel free to use and re-use any way you want.

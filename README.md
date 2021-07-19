All module should have namespace "OM" , All Submission should be only through git account , Everyone need to create a folder name will their own name , in that folder there will be another folder named OM , and all your module will be in the same firectory , for example Ritesh/OM/Modulename
---------------------------------------





Create a module to show best selling products to customer order succesfull mail (difficulty level:2)
------------------------------------------------------------------------------
Requirements:

1. Best Seller product should be send along the order  confirmation mail with the heading "You May Also Like"


Create a module so that admin can change customer password (difficulty level:2)
-------------------------------------------------------------------------------

Explanation : magento do not allow admin to view customer password , sometime customer forgets its password and contact admin , Admin should have provision to reset customer password

Requirements:

1. Admin should be able to change customer password from the admin.
2. Customer should get an email intimation that his/her password has been changed by admin , please contact admin to know your password 


Create a new module so that customer can enter Gst Number into the system (difficulty level:4)
--------------------------------------------------------------------------
Requirements:

1. Customer should be able to insert Gst number at the time of registration.
2. Customer should be able to view + edit gst number from his account. 
3. Admin should be able to edit view + edit gst number from backend. 
4. No manual entry should be into the database (either use installSchema.php or db_schema.xml)

Order Review functionality  (difficulty level : 5)
------------------------------------------------------------------------------

Requirements:

1. Customer should get a mail for  the feedback on the recently  ordered product/products , order id and item should  be listed  on it  .
2. Email  template  should be configurable from the backend , admin should be able to change the text  
3. Customer  should  have provision to mark order exprience with stars from 1 to  5 , five being exellent  , 1 for poor
4. Email should be  send to user after 1  day  of  the order , This  should be configurable from the  backend ,so  that admin can change this. (that means , you  have to create cron funcitonality)
5. Admin should  be able  to  view  customer feedbacks  and  there should be provision to  download the reviews  in csv  from the admin.


Create a new module so that customer can update its photo (difficulty level:5)
--------------------------------------------------------------------------
Requirements:

1. Customer should be able to insert photo at the time of registration.
2. Customer should be able to view + edit photo from his account. 
3. Admin should be able to edit view + edit photo from backend. 
4. No manual entry should be into the database (either use installSchema.php or db_schema.xml)
5.Customer photo should be visible on (minicart+header section)


Crate a shipping method where the customer can select a warehouse to  pick up the item itself instead of  home delivery (difficulty level:8)
------------------------------------------------------------------------------------------------
Explanation : Customer want to order jacuzzi bathtub of  ceremic and  due to  its excetional weight , it is  non deliverable  and the customer have to go directly to  the nearest  warehouse to receive their  item  


Create a new module so that customer can enter po number (purchase order number) at the time of placing an order (difficulty level:9)
----------------------------------------------------------------------------------------------------------------

Explanation :Purchase Order number is special number that the admin assign to customer through offline means or when the customer visit their store, Po number is just like a token which the customer get in exchange of money (just like we go to golgappa store and purchase a token by giving money and that token we provide in exchange of golgappa) . When the customer has po number , he does not have to pay at the time of checkout , instead he has to input po number and should be able to place the order.    

Requirements:
1. there will be a new payment method with the name po number , on clicking on po number a new input field will be shown where the customer will enter po number and place the order .
2. PO Number should be required field if po number payment method is selected . 
3. Customer and Admin both should be able to View po number 
4. Po number should be visible on customer invoice .
5. Order should be treated as payment is complete , Order status should be processing.

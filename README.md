All module should have namespace "OM" , All Submission should be only through git account , Everyone need to create a folder name will their own name , in that folder there will be another folder named OM , and all your module will be in the same directory , for example Ritesh/OM/Modulename
---------------------------------------

Remove customer account links  (difficulty level:1)
------------------------------------------------------------------------------
Requirements: admin do not have downlodable product , yet when the customer goes to account section , Download Product link is shown 
1. Remove the link My Downloadable Products and Stored Payment Methods from customer account and move "Newsletter Subscriptions" link at the bottom . 
2. using css to hint any element is not allowed , all customisations should be from  .xml files

Remove Header and footer from the checkout pages  (difficulty level:1)
------------------------------------------------------------------------------
Requirements: when the customer  proceed to  checkout ,the  admin want  to  remove header and  footer  so  that customer does  not  get temptation to go back or to  click  another link ,

1. no header or  footer should  be present at last step  i.e websiteurl.com/checkout , the url with name  checkout should not contain header  or  footer or minicart  or menu or  category ..header  and  footer should be completly  removed 
2. using css to  hide any element is not  allowed  

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


Create a  magento controller to show dynamic data  (difficulty level:2)
------------------------------------------------------------------------------
Requirements: 

1. create a magento controller  with the url websiteurl/offers which show 2 image  banners on the  website . 
2. admin should be  able to  change these 2  images for  web  as well as  for  mobile ..that means if he wants to show  different images for mobile and different  images for website , he  should be able to  do  so
3. url in both mobile  and website  should be same ,using  css  is  not  allowed  to  hide any image.(hint: you need to  create new theme for mobile different  from desktop )

Create an extension for automatic related products (difficulty level:3)
-------------------------------------------------------------------------------

Explanation : related product functionality in magento work on product level , admin has to enter related products for each individual prouct and upload that data manually for each product , admin has a large inventory and do not want to manage related products but still wants to show them on fromtend based on certian condition 

Requirements:

1. Related product should appear for all product automatically
2. Related products should be actually related , If customer open a certian category then related products should be also shown to that specific category
3. related product price should also be similar to current product , bariation should not be more than 25% of actual price of product .

Create a module to disable add to cart functionality if the product price is less than 500 (difficulty level:4)
------------------------------------------------------------------------------
Requirements: seller want to disable add to cart for any item whose amount is less than 500 , keep in mind if the product cost is 100 and customer orders 5 quantities than add to cart should work 

1. admin should be able to insert mimum amount for add to cart , product wise.
2. admin should be able to select product on which minimum amount coundition should be applicable , if he remove the consition on specific product of 10 rs , than add to cart should work , but keep in mind customer will still not be able to place the order if total cart amount is less than 500.
3. customer should not be able to  place order if the cart minimum amount is not greator than 500
4. cart minimum amount should be configurable from backend
5. admin should not be able to insert negetive number or string in the minimum amount for add to cart or for checkout 
6. also keep in mind that if order total is already greator than 500 , then add to cart should work even if customer order product of 10 rs

Create a new module so that customer can enter Gst Number into the system (difficulty level:4)
--------------------------------------------------------------------------
Requirements:

1. Customer should be able to insert Gst number at the time of registration.
2. Customer should be able to view + edit gst number from his account. 
3. Admin should be able to edit view + edit gst number from backend. 
4. No manual entry should be into the database (either use installSchema.php or db_schema.xml)

Create a  banner slider extension (difficulty level:4)
--------------------------------------------------------------------------
Requirements:

1. banner slider should be visible on the homepage. 
2. there should be provision to add+edit+delete banners from the backend.
3. there should be provision for alernate image for mobile if website is viewed in mobile 
4. banner links should be configurable from backend , admin should also have the ability to rearrange banner position from the backend so that he could decide which one will load first .

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
4. No manual entry should be into the database (either use installSchema.php or db_schema.xml).
5. Customer photo should be visible on (minicart+header section)


Create a shipping method where the customer can select a warehouse to  pick up the item itself instead of  home delivery (difficulty level:8)
------------------------------------------------------------------------------------------------
Explanation : Customer want to order jacuzzi bathtub of  ceremic and  due to  its excetional weight , it is  non deliverable  and the customer have to go directly to  the nearest  warehouse to receive their  item  

Requirements:
1. There should be an new shipping method named pickup from warehouse 
2. on clicking the shipping method there should be a select down from where customer can select the warehouse near to him for example 
a.) pickup from gurgaon warehouse 
b.) pickup from faridabad
c.) pickup from delhi 
3. on selecting a warehouse its address should be displayed to user 
4. Customer shipment charges should be zero if warehouse delivery is selected , as customer will pickup order itself from warehouse.
5. Admin should have provision to add+delte+edit a warehouse name and its address
6. Order mail and shiping invoice should have warehouse address mentioned on it .

Create a new module so that customer can enter po number (purchase order number) at the time of placing an order (difficulty level:9)
----------------------------------------------------------------------------------------------------------------

Explanation :Purchase Order number is special number that the admin assign to customer through offline means or when the customer visit their store, Po number is just like a token which the customer get in exchange of money (just like we go to golgappa store and purchase a token by giving money and that token we provide in exchange of golgappa) . When the customer has po number , he does not have to pay at the time of checkout , instead he has to input po number and should be able to place the order.    

Requirements:
1. there will be a new payment method with the name po number , on clicking on po number a new input field will be shown where the customer will enter po number and place the order .
2. PO Number should be required field if po number payment method is selected . 
3. Customer and Admin both should be able to View po number 
4. Po number should be visible on customer invoice .
5. Order should be treated as payment is complete , Order status should be processing.

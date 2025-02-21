# Task for develop new functionallity

## When a user signs up for the newsletter, receives a one-time 5% discount code to use in web store.

1. User registers for the newsletter
2. After registration, system automatically sent to users email address message with 5% discount
3. Discount code is assigned to particular user
4. Discount code is one-time only
5. Discount code covers value of entire order in cart (5%)
6. Discount code deactivated after payment is processed by web shop system
7. Generated discount code is stored in database and include information:
    * id
    * discount code
    * generated date
    * user
    * used (yes/no)
    * used date
    * order number
8. In web shop admin panel, admin can on/off "newsletter discount" mechanism manually, or automatically after a certain
   period of time
9. When "newsletter discount" mechanism OFF, still can use discount code

# Bug reports

| Parameter          | Content                                                                                                                                                                               |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|	
| Title              | User is able to login into webapp using old password                                                                                                                                  |
| Priority           | 	(set by Product Owner)                                                                                                                                                               |
| Severity	          | Critical                                                                                                                                                                              |
| Browser	           | Google Chrome ; Firefox ; Microsoft Edge ; Safari                                                                                                                                     |
| Environment        | 	http://www.example-url-adress-test-env.com/login-page                                                                                                                                |
| Branch	            | test-branch-software                                                                                                                                                                  |
| Issue location     | 	http://www.example-url-adress-test-env.com/login-page                                                                                                                                |
| PRECONDITIONS	     | 1.	Standard user account<br/><p>1.1 email: example@email.com<br/>1.2 old password: Old#Password123<br/>1.3 new password: New#Password123*<br/><p>2.User already changed password once |
| STEPS TO REPRODUCE | 1.	Go to login page http://www.example-url-adress-test-env.com/login-page <br/>2. Login in to web app using old password                                                              |
| ACTUAL RESULTS     | User is able login into webapp using old password                                                                                                                                     |
| EXPECTED RESULTS   | 1. User is  NOT able login into webapp using old password<br/>2. „Incorrect username or password” message is displayed                                                                |
| COMMENTS           | none                                                                                                                                                                                  |

| Parameter          | Content                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|	
| Title              | At web shop cart section user is able to increase quantity more than real product stock                                                                                                                                                                                                                                                                                                                                                                                         |
| Priority           | 	(set by Product Owner)                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Severity	          | Critical                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Browser	           | Google Chrome ; Firefox ; Microsoft Edge ; Safari                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Environment        | 	http://www.web-shop-test-env.com                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Branch	            | product-page-new-feature                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Issue location     | 	http://www.example-url-adress-test-env.com/login-page                                                                                                                                                                                                                                                                                                                                                                                                                          |
| PRECONDITIONS	     | 1.	Example-product-001 quantity = 2                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| STEPS TO REPRODUCE | 1. Login in to buyer account<br/>2. Go to product page http://www.web-shop-test-env.com/example-product-001<br/>3. Add item in to cart – effect: cart qty = 1<br/>4. Add item in to cart second time – effect: cart qty = 2<br/>5. Add item in to cart third time – effect: system display message "No products in stock" ; cart qty = 2<br/>6. Display cart page to proceed to checkout and payment<br/>7. At cart page increase example-product-001 quantity using „+” button | 
| ACTUAL RESULTS     | 1. message  "No products in stock" was NOT displayed<br/>2. example-product-001 quantity was increased to 3<br/> 3. total order amount was increased                                                                                                                                                                                                                                                                                                                            |
| EXPECTED RESULTS   | 1. message  "No products in stock"  was displayed<br/>2. example-product-001 quantity = 2                                                                                                                                                                                                                                                                                                                                                                                       |
| COMMENTS           | none                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

### [Main Page](../README.md)
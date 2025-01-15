System Feature 

Order food by choosing different menu item, quantity
Get valid payment information from payment Microservices 
Send Email about order information to customer 


/************API Overview  Order Microservice*****************/

Method	              Path	                                                  Description
POST	       |http://localhost:9001/api/orders/	                     |create order, using sample data (data/order.json)
GET	           |http://localhost:9001/api/orders/	                     |get all orders
GET	           |http://localhost:9001/api/orders/{orderId}	             |get an order by order id.
GET	           |http://localhost:9001/api/orders//{userId}/orders	     |get all the orders placed by one user


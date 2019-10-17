# Edge Computing

![edge](https://github.com/kmranrg/ProductDetection/blob/master/static/img/edge.png)

### Requirement
Kirana is a retail store looking for more digitalized way of expanding their business. They want to use a more systematic way of checkout system and reduce their human work force at billing counters.
Help Kirana devise a system that allows automatic detection of product using camera. The detection of product must be wrt the size of the product, type of product and automatically take the cost of product to make a bill of materials at checkout. This has to be done in real-time without sending the data to cloud for processing as some of these stores can be in remote areas with intermittent connectivity and Kirana do not want customers to wait due to latency issues for connectivity.
Example: If a toothpaste is placed in front of the camera, it should detect the product, according to the size and weight of toothpaste it must understand what the price of the product is. The details of each product scanned is then presented at the bill of materials for payment.
Please note, Kirana has Edge Servers that are not compute intensive.

### Things to do:
* Build a ML model for product detection based on the mentioned parameters.
-> Size of product
(When a customer keeps a product in front of the camera, it should detect the product by determining the size of product. It should be able to distinguish between the products of same brand, but of different size. Refer the toothpaste example above.)
* Train the ML Model.
* Create a web application named ‘Kirana Product Billing’ for Product Detection and Billing. Integrate it with the trained ML model and show the details of the bill for products bought by the customer.

### Expected Output:
1. Open ‘Kirana Product Billing’ web application.
2. Upload image of a product for detection (You can also use desktop/Laptop camera for product detection)
3. Based on the image, perform product detection through the ML model built for detecting product based on size of product.
4. Once product is detected, directly add the corresponding Product ID, Product Name, Quantity and Cost of detected product to the Bill of Materials.
5. Repeat the above steps for atleast 5-6 products. Amongst these products, include 2-3 images of the same product, but in different size. Example: If a customer buys three toothpaste in small, medium and large size each.
6. After images of all products are uploaded, show the final bill of materials. It should display the following details
  * Sr. No.
  * Product ID(This is a unique ID which will be different for all the products regardless of the brand and size
  * Name of Product
  * Quantity
  * Cost of product
  * Final Cost of Product = (Quantity*Cost of Product)
  * Highlight ‘Final Cost’ by performing addition on the final cost of all the products bought

### My Raspberry Pi 3B+ Working Model

![rp-1](https://github.com/kmranrg/ProductDetection/blob/master/static/img/raspberry_pi_model_1.jpg)

# Enterprise Product Service v2
The Enterprise Product Service is designed to be the one-stop-shop for product data. It was dynamically generated from Swagger and deployed to a web app service in Azure PaaS.

## Product Data
Product data is the base data that is on all products. This is a limited set of data elements but is common to all products. As products change, product variants are created.

### Example fields being returned:
* Brand
* Care
* Category
* Foo

## Product Variants
Product variants are used to describe unique features of a product. This means that sizes, colors, etc. are included and defined.

## How does it work?
![Enterprise Product Servicev1.png](assets/images/digitalservicefabric.png)
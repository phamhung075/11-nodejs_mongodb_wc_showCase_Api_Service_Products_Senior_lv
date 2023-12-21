This is a personal project series based on the lessons by @anonystick ([https://github.com/anonystick](https://github.com/anonystick)).
## 1. [Authentication and API Key Management (HS256)](https://github.com/phamhung075/2-nodejs_mongodb_wc_showCase_Dynamic_for_ApiKey_and_Permissions_HS256/tree/master)

## 2. [ErrorHandler ApiResponse](https://github.com/phamhung075/3-nodejs_mongodb_wc_showCase_ErrorHandler_API)

## 3. [Success Handler ApiResponse](https://github.com/phamhung075/4-nodejs_mongodb_wc_showCase_ApiResponseUseClass/tree/master?tab=readme-ov-file)

## 4. [SignUp and Login Public Access](https://github.com/phamhung075/5-nodejs_mongodb_wc_showCase_SignUpLogin)

## 5. [Logout Authentication](https://github.com/phamhung075/6-nodejs_mongodb_wc_showCase_LogoutAuthentication)
## 6. [Refresh Token and Token Verification](https://github.com/phamhung075/7-nodejs_mongodb_wc_showCase_RefreshToken_verifyToken)
## 7. [Schema for Products in E-commerce](https://github.com/phamhung075/8-nodejs_mongodb_wc_showCase_Schema_Products_Ecommerce)
## 8. API for Products Using Factory Pattern

### Introduction

`11-nodejs_mongodb_wc_showCase_Api_Service_use_Factory_Pattern_Products_Senior_lv`  is a senior-level upgrade of our existing Node.js application, aimed at showcasing intricate product management capabilities within a MongoDB framework. This version introduces complex functionalities, sophisticated code design patterns, and enhanced performance optimizations, catering to the skills and challenges at a senior developer level.

### Version Junior Upgrade Highlights

Enhanced Product Model (`./models/product.model.js`): The product schema has been upgraded with additional attributes and validation rules to better represent complex product data.

Advanced Product Service (`./services/product.service.js`): Includes refined business logic and data handling methods, offering a more comprehensive approach to product management.

Improved Authentication Mechanism (`./services/authenticationV2.js`): Introduces a more robust and secure authentication system, ensuring better data protection and user management.

Revamped Product Controller (`./controllers/product.controller.js`): Features more efficient request handling and response generation for product-related operations.
### Version Senior Upgrade Highlights

- **Sophisticated Product Model** (`./models/product.model.js`): Enhanced to handle intricate product attributes, complex validations, and relationships, reflecting real-world e-commerce product complexities.
- **Advanced Product Service** (`./services/product.service.xxx.js`): Incorporates complex business logic, advanced data processing techniques, and performance optimizations for handling large-scale product data.
- **Robust Product Controller** (`./controllers/product.controller.js`): Upgraded to manage a broader spectrum of product-related operations, with refined error handling and response management strategies.



### Installation

- Clone the repository:

    `git clone https://github.com/phamhung075/11-nodejs_mongodb_wc_showCase_Api_Service_use_Factory_Pattern_Products_Senior_lv.git`
    
- Change to the directory:

    `cd 11-nodejs_mongodb_wc_showCase_Api_Service_use_Factory_Pattern_Products_Senior_lv`
    
- Install dependencies:
 
    `npm install`
    

### Features

- **Factory Pattern Implementation**: Utilizes the factory pattern in creating services for product management, enhancing code modularity and reusability.
- **Product Service** (`./services/product.service.xxx.js`): Central service for product operations, created using the factory pattern.
- **Product Controller** (`./controllers/product.controller.js`): Manages product-related API routes and request handling.
- **Product Routes** (`./routes/product.route.js`): Defines API endpoints for product management activities like creating, reading, updating, and deleting products.

### Usage
- This version is designed for senior developers, featuring complexities that simulate real-world challenges in product data management.
- The application now efficiently handles extensive and intricate product operations, making it an ideal reference for advanced Node.js and MongoDB implementations.

### MongoDB Connection

- Connect to MongoDB using: `mongodb://localhost:27017/ecommerce`

### Additional Notes

- This project can be used as a reference or starting point for building scalable and maintainable e-commerce applications.
- The factory pattern implementation provides a template for structuring services in Node.js applications.

### Postman Examples

- **Signup**, **Login**, **Logout** examples as in the previous project.
- **Token Refresh** examples as in the previous project.
- **Create Product** examples.

``` 
@url_dev=http://localhost:3052/v1/api/product/

### create product
POST {{url_dev}}
Content-Type: application/json
x-api-key: [API_KEY]
x-client-id: [SHOP_ID]
authorization: [ACCESS_TOKEN]

{
	"product_name" : "Leggings polaire gris",
	"product_price" : 500,
	"product_type" : "Clothing",
	"product_thumb" : "product_thumb",
	"product_quantity" : 10,
	"product_attributes" : {
		"brand": "Boss",
		"size" : "S",
		"material": "coton"
	}
}
```

``` 
@url_dev=http://localhost:3052/v1/api/product/

### create product
POST {{url_dev}}
Content-Type: application/json
x-api-key: [API_KEY]
x-client-id: [SHOP_ID]
authorization: [ACCESS_TOKEN]

{
    "product_name" : "iPhone 16 64GB",
    "product_description" : "New product",
    "product_price" : 500,
    "product_type" : "Electronic",
    "product_thumb" : "product_thumb",
    "product_quantity" : 5,
    "product_attributes" : {
        "manufacturer": "Apple",
        "model" : "iPhone 16",
        "color": "Gold"
    }
}
```

``` 
@url_dev=http://localhost:3052/v1/api/product/

### create product
POST {{url_dev}}
Content-Type: application/json
x-api-key: [API_KEY]
x-client-id: [SHOP_ID]
authorization: [ACCESS_TOKEN]

{
    "product_name" : "furniture 1B",
    "product_description" : "New product",
    "product_price" : 500,
    "product_type" : "Furniture",
    "product_thumb" : "product_thumb",
    "product_quantity" : 5,
    "product_attributes" : {
        "brand": "FUR",
        "size" : "100",
        "material": "Paper"
    }
}
```
For more detailed examples, refer to see [README.png](./help11.png).

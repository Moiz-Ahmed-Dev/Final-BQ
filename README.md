# ShoeSavvy.com - MERN Stack
Welcome to the ShoeSavvy.com project! This is a full-stack MERN (MongoDB, Express, React, Node.js) application designed to provide an online platform for buying different products.

## Features
* User registration and authentication system.

* Browse books by category, product name, description and price.

* Add products to the shopping cart and proceed to checkout.

* Track order status and delivery information by email.

* Leave reviews and ratings for products.

* Manage user profiles and track order history.

* Responsive and user-friendly UI.

## Visit

You can visit the live demo of the app [ShoeSavvy.com](https://plum-barracuda-robe.cyclic.cloud)

----------------------------------------------------------------------------------------------------

## Frontend Routes

1. ### Login Page
* Path: "/"
* Component: LoginPage
* Description: Landing page of the application.
* Access: If token is set, navigates to home page.
  
2. ### Sign-up Page
* Path: "/SignUp"
* Component: SignupPage
* Access: If token is set, navigates to home page.
* Description: Allows new users to sign up for the application.

3. ### Home Page

* Path: "/Categories"
* Component: HomePage
* Description: After login successfully, allow users to access on the application.

4. ### Category Page

* Path: "/products/category/:categoryName"
* Component: CategoryPage
* Description: Lists of categories for users to explore.
  
5. ### Products Page

* Path: "/products/:productID"
* Component: ProductPage
* Description: Lists of products by categories for users to explore.
 
6. ### Cart Page

* Path: "/CartList"
* Component: CartList
* Description: Lists of products adding by user in Cart list.

7. ### Page Not Found
* Path: "*"
* Component: Page404
* Description: Renders when no matching route is found.
-----------------------------------------------------------------------------------------------------

## Backend/API Routes

1. ### Users routes   
 POST "/api/login"
* Component: loginUser
* Description: Log in a user by providing their email and password.

POST "/api/signup"
* Component: signupUser
* Description: Signup a new user by providing their user name, password, and unique email.


2. ### Categories routes
GET "/api/get-all-categories"
* Component: getAllCategories
* Description: Retrieve a list of all categories.

GET "/api/get-category-by-id"
* Component: getCategoryByID
* Description: Retrieve a category by its ID.
  

3. ### Products routes
GET "/api/get-product-by-category"
* Component: getProductByCategory
* Description: Retrieve a products by its Category.

GET "/api/get-all-products"
* Component: getAllProducts
* Description: Retrieve a list of products.  

4. ### Orders routes
POST "/api/place-order"
* Component: placeOrder
* Description: User can confirm his order by filling all the required fields and get confirmation message by email.

GET "/api/get-all-orders" (only Admin)
* Component: getAllOrders
* Description: Retrieve a list of all orders (admin only) .

------------------------------------------------------------------------------------------------------ 

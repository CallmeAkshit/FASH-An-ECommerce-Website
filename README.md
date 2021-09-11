# Ecommerce Website (Contributors - Akshit Bansal and Jyoti Vakare)


![grab-landing-page](https://github.com/CallmeAkshit/FASH-An-ECommerce-Website/blob/master/MERN%20Demo.gif)

## Demo Link

https://ecommerce-myntra-clone.herokuapp.com/

## About this site
●	Cloned an ecommerce website from frontend till backend.

●	Added features like Sign-in/Login page, Product listing page, product detail page, Cart Features, Payment Integration

●	Incorporated Payment Integration with Razorpay. 

●	Designed REST APIs for frontend to interact with database and integrated APIs with frontend code.

# API Specs

## Get cart associated with the session id

GET /api/carts/me

Sample Response Body:
{

	"id": "cartid"
	
}

Status: 201 (Cart returned), 500 (sessionid is invalid)

## List all products
GET /api/products/

Sample Response Body:

{

    uniq_id: {type : String},
    crawl_timestamp: {type : String},
    product_id: {type : String},
    link:{type : String},
    size:{type : String},
    variant_sku:{type : String},
    brand:{type : String},
    care_instructions:{type : String},
    dominant_material:{type : String},
    title:{type : String},
    actual_color:{type : String},
    dominant_color:{type : String},
    product_type:{type : String},
    images:{type : String},
    body:{type : String},
    product_details:{type : String},
    size_fit:{type : String},
    complete_the_look:{type : String},
    type:{type : String},
    variant_price:{type : String},
    variant_compare_at_price:{type : String},
    ideal_for:{type : String},
    is_in_stock:{type : String},
    inventory:{type : String}
    
}

Status: 201 (Product returned), 500 (Internal Server error), 201 (No product found)

## List products by category Male (Boys, Men, Unisex)

GET /api/products/men
GET /api/products/boys
GET /api/products/unisex

Sample Response Body: 

{

    uniq_id: {type : String},
    crawl_timestamp: {type : String},
    product_id: {type : String},
    link:{type : String},
    size:{type : String},
    variant_sku:{type : String},
    brand:{type : String},
    care_instructions:{type : String},
    dominant_material:{type : String},
    title:{type : String},
    actual_color:{type : String},
    dominant_color:{type : String},
    product_type:{type : String},
    images:{type : String},
    body:{type : String},
    product_details:{type : String},
    size_fit:{type : String},
    complete_the_look:{type : String},
    type:{type : String},
    variant_price:{type : String},
    variant_compare_at_price:{type : String},
    ideal_for:{type : String},
    is_in_stock:{type : String},
    inventory:{type : String}
    
}

Status: 201 (Product returned), 500 (Internal Server error), 201 (No product found)

## List products by category Female (Girls, Women, Unisex)

GET /api/products/Women
GET /api/products/Girls

Sample Response Body: 

{

    uniq_id: {type : String},
    crawl_timestamp: {type : String},
    product_id: {type : String},
    link:{type : String},
    size:{type : String},
    variant_sku:{type : String},
    brand:{type : String},
    care_instructions:{type : String},
    dominant_material:{type : String},
    title:{type : String},
    actual_color:{type : String},
    dominant_color:{type : String},
    product_type:{type : String},
    images:{type : String},
    body:{type : String},
    product_details:{type : String},
    size_fit:{type : String},
    complete_the_look:{type : String},
    type:{type : String},
    variant_price:{type : String},
    variant_compare_at_price:{type : String},
    ideal_for:{type : String},
    is_in_stock:{type : String},
    inventory:{type : String}
    
}

Status: 201 (Product returned), 500 (Internal Server error), 201 (No product found)

## List products by brand

GET /api/products/brand/:brandName

Sample Response Body: 

{

    uniq_id: {type : String},
    crawl_timestamp: {type : String},
    product_id: {type : String},
    link:{type : String},
    size:{type : String},
    variant_sku:{type : String},
    brand:{type : String},
    care_instructions:{type : String},
    dominant_material:{type : String},
    title:{type : String},
    actual_color:{type : String},
    dominant_color:{type : String},
    product_type:{type : String},
    images:{type : String},
    body:{type : String},
    product_details:{type : String},
    size_fit:{type : String},
    complete_the_look:{type : String},
    type:{type : String},
    variant_price:{type : String},
    variant_compare_at_price:{type : String},
    ideal_for:{type : String},
    is_in_stock:{type : String},
    inventory:{type : String}
    
}

Status: 201 (Product returned), 500 (Internal Server error), 201 (No product found)

## List products by product ID

GET /api/products/productID/:productID

Sample Response Body: 

{

    uniq_id: {type : String},
    crawl_timestamp: {type : String},
    product_id: {type : String},
    link:{type : String},
    size:{type : String},
    variant_sku:{type : String},
    brand:{type : String},
    care_instructions:{type : String},
    dominant_material:{type : String},
    title:{type : String},
    actual_color:{type : String},
    dominant_color:{type : String},
    product_type:{type : String},
    images:{type : String},
    body:{type : String},
    product_details:{type : String},
    size_fit:{type : String},
    complete_the_look:{type : String},
    type:{type : String},
    variant_price:{type : String},
    variant_compare_at_price:{type : String},
    ideal_for:{type : String},
    is_in_stock:{type : String},
    inventory:{type : String}
    
}


Status: 201 (Product returned), 500 (Internal Server error), 201 (No product found)

## List products sorted by price and category

GET /api/products/brand/:brandName/sortBy/:sortType

Sample Response Body: 

{

    uniq_id: {type : String},
    crawl_timestamp: {type : String},
    product_id: {type : String},
    link:{type : String},
    size:{type : String},
    variant_sku:{type : String},
    brand:{type : String},
    care_instructions:{type : String},
    dominant_material:{type : String},
    title:{type : String},
    actual_color:{type : String},
    dominant_color:{type : String},
    product_type:{type : String},
    images:{type : String},
    body:{type : String},
    product_details:{type : String},
    size_fit:{type : String},
    complete_the_look:{type : String},
    type:{type : String},
    variant_price:{type : String},
    variant_compare_at_price:{type : String},
    ideal_for:{type : String},
    is_in_stock:{type : String},
    inventory:{type : String}
    
}


Status: 201 (Product returned), 500 (Internal Server error), 201 (No product found)

## Add a new product to Cart

POST /api/cart
Sample Request Body:

{

	"cartItem" : { productId: String, qty: Number, pricePerUnit: Number, brand : String, title : String, images: String }
	
}

Sample Response Body:
{

	"id": "sessionID"
	
}

Status: 201 (Product Added to Cart), 400 (SessionID/ cartItem not in request), 500 (Error while adding cart to Item)

## Update quantity of a product in Cart

PUT /api/cart

Sample Request Body:
{

	"productID": "1234",
	"qty": "1",
	
}

Sample Response Body:
{

	"id": "cartid"
	
}

Status: 204 (Item updated to cart), 400 (Invalid Session ID or Invalid Product ID) 400 (Qty missing in request) 400 (Empty Body Sent in request)

# Delete a Product from Cart

DELETE /api/cart/:productID

Status: 201 (product removed from cart), 500 (Internal Server Error), 400 (Product ID not present in request)

# Create Order 

POST /api/orders

Sample Request Body: {user_id,amount,currency,status}

All the values are fetched from the session ID.

Sample Response Body:
{
    amount,
    currency,
    orderId,
    //This is required by client to co-ordinate with razorpay
    rzpOrderId: rzpOrder.id
 }
 
Status: 201 (Order Created), 500 (Order creation failed with Razorpay)

# Update order status on payment completion/failure.

PUT /api/orders/:orderID

Sample Response Body:
{

	"id": "orderID"
	
}

Status: 204 (Payment Succesful), 400 (Payment failed) 400 (Empty Body Sent in request)






















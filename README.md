# D-Baesics - Ecommerce and Inventory Management System

D'Baesic Apparel's Ecommerce and Inventory Management System, powered by Java Spring Boot and Thymeleaf, integrates the Stripe API. Launched successfully, it doubled sales to 10k orders, featuring an admin dashboard for 50% increased productivity by tracking sales, costs, and product performance. A game-changer in online retail.

## Overview

D'Baesics Ecommerce and Inventory Management System is a Java Spring Boot-based application designed to streamline online shopping and inventory management processes. With integrated features such as secure user authentication, seamless payment processing through the Stripe API, and a user-friendly admin dashboard, this system aims to enhance the overall online retail experience.

## Key Features

- **User Authentication**: Secure login/signup functionality for users.
- **Shopping Cart**: Add, view, update, and remove items with ease.
- **Checkout and Payment**: Seamless payment processing using the Stripe API.
- **Inventory Management**: Admin dashboard for efficient inventory control.
- **Real-time Shipping Updates**: Track order status and receive timely shipping updates.

# Online Shopping Platform

## User Stories (For the User):

### Story 1
As a shopper, I need to be able to add items to my shopping cart so I can purchase them.

**Acceptance Criteria:**
- Select item, click button to add item to cart.
- Item is in cart.

**Size:** SMALL

### Story 2
As a shopper, I need to be able to view the items in my shopping cart so I can decide if I want to purchase them.

**Acceptance Criteria:**
- Select item, add to cart.
- Select link to “view cart” and item is present.

**Size:** MEDIUM

### Story 3
As a shopper, I want to be able to update the quantity of items in my shopping cart so I can adjust my purchase quantity.

**Acceptance Criteria:**
- In the cart view, change the quantity of a selected item.
- Total price is updated accordingly.

**Size:** SMALL

### Story 4
As a shopper, I need the ability to remove items from my shopping cart in case I change my mind about a purchase.

**Acceptance Criteria:**
- In the cart view, click a button to remove a selected item.
- Cart is updated without that item.

**Size:** SMALL

### Story 5
As a shopper, I want to see the total cost of the items in my shopping cart, including taxes and any applied discounts.

**Acceptance Criteria:**
- Cart view displays the total cost with a detailed breakdown.

**Size:** MEDIUM

### Story 6
As a shopper, I need the option to apply a promotional code or voucher to my shopping cart to avail discounts.

**Acceptance Criteria:**
- During checkout, a field to enter a promotional code.
- Applying it reflects the discounted price.

**Size:** MEDIUM

### Story 7
As a shopper, I want to proceed to the checkout page with a single click to save time, using Stripe API.

**Acceptance Criteria:**
- Prominent and easily accessible "Checkout" button in the cart view.
- Leads directly to the checkout page.

**Size:** SMALL

### Story 8
As a shopper, I need to enter my shipping address during checkout to ensure accurate delivery.

**Acceptance Criteria:**
- Checkout process includes a step for entering and validating the shipping address.

**Size:** MEDIUM

### Story 9
As a shopper, I want to select my preferred payment method during checkout for a seamless payment experience.

**Acceptance Criteria:**
- Checkout process includes a step for choosing a payment method.

**Size:** MEDIUM

### Story 10
As a shopper, I want to receive an order confirmation email after completing my purchase.

**Acceptance Criteria:**
- Email sent to the shopper's registered email address confirming the order details.

**Size:** SMALL

### Story 11
As a shopper, I need the option to save multiple shipping addresses for future orders.

**Acceptance Criteria:**
- User profile includes a feature to add and manage multiple shipping addresses.

**Size:** MEDIUM

### Story 12
As a shopper, I want to see real-time shipping updates and tracking information for my order.

**Acceptance Criteria:**
- After completing the purchase, track the order status and receive timely updates on shipping progress.

**Size:** LARGE

## User Stories (For the Business Owner):

### Managing Inventory:

### Story 13
As a business owner, I want to efficiently manage the inventory of products in my store.

**Acceptance Criteria:**
1. Add new products to the inventory with details (name, category, price, quantity).
2. Update product information, including price and quantity.
3. Mark products as out of stock or remove them.
4. System provides real-time updates on product quantity.

**Size:** MEDIUM

### Sales Report:

### Story 14
As a business owner, I want to generate comprehensive sales reports to track the performance of my store.

**Acceptance Criteria:**
1. Generate a sales report for a specific time period.
2. Report shows total revenue, number of orders, and average order value.
3. Break down sales by product, indicating best-selling items.
4. Allow export of the sales report in downloadable format (e.g., CSV, PDF).

**Size:** LARGE

### Customer Management:

### Story 15
As a business owner, I want to manage customer information and track their purchasing history.

**Acceptance Criteria:**
1. View a list of registered customers with names and contact details.
2. View a customer's past orders, including dates and purchased items.
3. Add notes or tags to individual customer profiles.

**Size:** MEDIUM

### Discount Management:

### Story 16
As a business owner, I want the ability to create and manage discounts for promotional purposes.

**Acceptance Criteria:**
1. Create discount codes with specified conditions.
2. System applies discounts automatically during checkout.
3. Set expiration dates for discount codes.
4. Track usage and effectiveness of each discount code.

**Size:** MEDIUM

### Order Tracking:

### Story 17
As a business owner, I want to easily track and manage the status of customer orders.

**Acceptance Criteria:**
1. System provides a dashboard displaying the current status of all orders.
2. Filter orders by status (e.g., pending, shipped, delivered).
3. Receive timely notifications for critical order events.

**Size:** SMALL

## System Architecture

### Backend (Java Spring Boot)

1. **Controllers**: Create controllers to handle different functionalities.
2. **Service Layer**: Implement services to encapsulate business logic.
3. **Data Access Layer**: Utilize Spring Data JPA for database access.
4. **Models**: Define Java classes for entities like Product, User, Cart, Order, and Inventory.
5. **Security**: Implement security features using Spring Security if required.

### Frontend (Thymeleaf with HTML/CSS/Bootstrap)

- Develop frontend interfaces for end-users and business owners using HTML, CSS, and Bootstrap.

## Database Design

### Entity Relationship Diagram (ERD)

1. **Product**: ID, Name, Description, Price, Quantity, Category, Image URL.
2. **User**: ID, Username, Password (hashed), Email.
3. **Cart**: ID, User ID.
4. **Order**: ID, User ID, Order Date, Status (e.g., Pending, Shipped).
5. **CartItem**: ID, Product ID, Quantity.
6. **Inventory**: ID, Product ID, Purchase Cost, Sale Price.

## Development Milestones

- **January 15, 2024**: Initial navigation setup and Product table creation.

## Testing

- Perform comprehensive testing of each feature to ensure functionality and security.

## Deployment

- Deploy the application to a suitable server for public access.

## Maintenance

- Regularly update dependencies and address any reported issues.

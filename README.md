# DC-Delivery-docs


##  How It Works

This section explains how the DC Delivery system operates across different user roles (Customer, Restaurant, Driver, Admin).

---

###  1. Customer Flow

**Steps:**
1. User opens the app and logs in (Firebase Auth)
2. They browse restaurants and menus
3. They add items to cart and place the order
4. Order is confirmed and sent to the respective restaurant
5. They track the order in real-time
6. Once delivered, they can rate the restaurant/driver


###  2. Restaurant Flow

**Steps:**
1. Restaurant receives the order via the Restaurant App or dashboard
2. They accept or reject the order
3. If accepted, they prepare the order and mark it as "Ready for Pickup"


###  3. Driver Flow

**Steps:**
1. Available orders are sent to drivers via Firebase Cloud Messaging
2. Driver accepts the order and navigates to the restaurant
3. Picks up the food and delivers it to the customer
4. Marks the delivery as complete


### 4. Admin Flow

**Steps:**
1. Admin logs into the backend dashboard
2. Can view:
   - Orders (pending, in progress, completed)
   - Registered users and restaurants
   - Reports (daily orders, earnings, etc.)
3. Can manually add products or manage restaurants


### 🌐 System Integration Overview

| Component          | Tech Used      |
|--------------------|----------------|
| Frontend           | Flutter         |
| Backend            | Laravel         |
| Authentication     | Firebase Auth   |
| Notifications      | Firebase Cloud Messaging |
| Maps & Navigation  | Google Maps API |
| Payments           | PayFast / Razorpay |

---

> This flow gives a high-level understanding of how each user interacts with the DC Delivery system and where the code responsible for it lives.

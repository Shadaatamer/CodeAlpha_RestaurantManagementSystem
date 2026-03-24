# Restaurant Management System

A backend API built using Node.js, Express, and MongoDB to manage restaurant operations including menu, tables, and orders.

---

## 🚀 Features

- Create and view menu items  
- Create and manage restaurant tables  
- Place customer orders  
- Automatically calculate total order price  
- Mark tables unavailable when an order is placed  
- Complete orders and free tables again  
- View all orders with menu and table details  

---

## 🛠️ Tech Stack

- Node.js  
- Express.js  
- MongoDB (Mongoose)  

---

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/Shadaatamer/CodeAlpha_RestaurantManagementSystem.git
Install dependencies:
npm install
Create a config.env file in the root folder:
DATABASE=your_mongodb_connection_string
PORT=3000
Run the server:
npm start
📌 API Endpoints
🍔 Menu

Create Menu Item
POST /menu

{
  "name": "Burger",
  "description": "Beef burger",
  "price": 120
}

Get All Menu Items
GET /menu

Get Single Menu Item
GET /menu/:id

🪑 Tables

Create Table
POST /table

{
  "tableNumber": 1
}

Get All Tables
GET /table

Update Table Availability
PATCH /table/:id

🧾 Orders

Place Order
POST /order

{
  "table": "table_id_here",
  "items": [
    {
      "menuItem": "menu_item_id_here",
      "quantity": 2
    }
  ]
}

Get All Orders
GET /order

Complete Order
PATCH /order/:id/complete

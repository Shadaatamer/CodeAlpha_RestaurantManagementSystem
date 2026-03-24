
# Restaurant Management System

A backend API built using Node.js, Express, and MongoDB to manage restaurant operations including menu, tables, and orders.

## 🚀 Features

- Create and view menu items  
- Create and manage restaurant tables  
- Place customer orders  
- Automatically calculate total order price  
- Mark tables unavailable when an order is placed  
- Complete orders and free tables again  
- View all orders with menu and table details  

## 🛠️ Tech Stack

- Node.js  
- Express.js  
- MongoDB (Mongoose)  

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/Shadaatamer/CodeAlpha_RestaurantManagementSystem.git
````

2. Install dependencies:

```bash
npm install
```

3. Create a `config.env` file:

```env
DATABASE=your_mongodb_connection_string
PORT=3000
```

4. Run the server:

```bash
npm start
```

## 📌 API Endpoints

### Menu

**POST /menu**

```json
{
  "name": "Burger",
  "description": "Beef burger",
  "price": 120
}
```

**GET /menu**

**GET /menu/:id**

---

### Tables

**POST /table**

```json
{
  "tableNumber": 1
}
```

**GET /table**

**PATCH /table/:id**

---

### Orders

**POST /order**

```json
{
  "table": "table_id_here",
  "items": [
    {
      "menuItem": "menu_item_id_here",
      "quantity": 2
    }
  ]
}
```

**GET /order**

**PATCH /order/:id/complete**



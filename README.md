# 🛒 Supermart Management System

## 📌 Overview
The **Supermart Management System** is a desktop-based retail application built using **C++/CLI** and the **.NET Framework**, designed to simulate an shopping experience. It supports customer registration, product browsing, cart management, billing, and administrative control — all within a modular, multi-class architecture.

This project demonstrates your ability to build structured, real-world systems with GUI, file-based persistence, and clean separation of concerns.

---

## ✨ Key Features

### 👤 Customer Operations
- Register and log in  
- Browse products  
- Add items to cart  
- Update or delete cart items  
- Checkout and generate bill with discounts  
- View cart and billing details

### 🔐 Admin Operations
- Secure login with credentials  
- Add, update, delete, and search products  
- View customer inventory and purchase history

### 🧠 Business Logic
- File-based database using `.txt` files  
- Full CRUD operations: insert, read, search, update, delete  
- Discount logic based on bill amount  
- Refund calculation based on payment

### 🖥️ GUI Interface
- Tab-based navigation using Windows Forms  
- `DataGridView` controls for product and cart display  
- Interactive buttons for all operations  
- Real-time updates and feedback via message boxes

---

## 🧱 Project Structure

```
SupermartManagementSystem/
├── Header Files/
│   ├── Product.h          # Product class
│   ├── Person.h           # Base class for Customer/Admin
│   ├── Customer.h         # Cust and Customer classes
│   ├── admin.h            # Admin credentials
│   ├── Billing.h          # Billing logic
│   ├── DB.h               # File-based CRUD operations
│   ├── mapper.h           # Data mapping from file to objects
│   ├── MyForm.h           # Event-driven UI logic
│
├── Source Files/
│   ├── Product.cpp
│   ├── Person.cpp
│   ├── Customer.cpp
│   ├── admin.cpp
│   ├── Billing.cpp
│   ├── DB.cpp
│   ├── mapper.cpp
│   ├── MyForm.cpp
│
├── Resource Files/
├── References/
└── External Dependencies/
```

---

## 🧮 Class Breakdown

| Class        | Purpose                                                                 |
|--------------|-------------------------------------------------------------------------|
| `Product`    | Represents individual items with name, weight, price, quantity, and ID |
| `Person`     | Base class for shared identity (`Name`)                                |
| `Cust`       | Inherits `Person`, adds phone and cart functionality                   |
| `Customer`   | Lightweight customer info container                                    |
| `admin`      | Stores admin credentials and access methods                            |
| `billing`    | Calculates total, applies discounts, generates bill                    |
| `DatabaseOperations` | Handles file I/O: insert, read, search, update, delete         |
| `mapper`     | Converts file data into object arrays (`Product`, `Cust`)              |
| `MyForm`     | Contains all event-driven logic for UI interaction                     |

---

## 🧪 How It Works

### 🛍️ Customer Flow
1. **Login/Register**  
2. **Browse Products**  
3. **Add to Cart**  
4. **Update/Delete Cart Items**  
5. **Proceed to Billing**  
6. **View Bill & Refund**

### 🛡️ Admin Flow
1. **Login with credentials**  
2. **Manage Products**  
   - Add new items  
   - Update quantity  
   - Delete or search items  
3. **View Customer Inventory**

### 💳 Billing Logic
- If bill ≤ 5000 → No discount  
- If bill > 5000 → 10% discount applied  
- Refund calculated based on payment input  
- Bill displayed with itemized breakdown and total

---

## 🖥️ Technologies Used

| Technology       | Role                                      |
|------------------|-------------------------------------------|
| C++/CLI           | Core language for logic and UI           |
| .NET Framework    | Windows Forms GUI                        |
| Visual Studio     | Development environment                  |
| Text Files (`.txt`)| Persistent storage for products/customers|

---

## 🚀 How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/SamiUrRehman065/Supermart-Management-System
   ```
2. Open the solution in **Visual Studio**  
3. Build the project to resolve dependencies  
4. Run the application from the IDE  

---

## 🧑‍💻 Author

**Name:** Sami Ur Rehman  
**Location:** Karachi, Pakistan  
**GitHub:** [SamiUrRehman065](https://github.com/SamiUrRehman065)

---

## 🪞 Developer Reflection

This project marks a major milestone in my journey from basic experimentation to building structured, multi-class desktop applications.

### What I Learned
- Designing reusable classes with inheritance (`Person → Customer/Admin`)  
- Structuring logic across multiple header/source files  
- Managing state and UI flow with Windows Forms  
- Abstracting file I/O with `DB` and `mapper` classes  
- Implementing real-time cart and billing logic

### Challenges Faced
- Ensuring consistent data mapping between files and objects  
- Handling edge cases in billing and cart operations  
- Synchronizing UI events with backend logic

### Solutions Implemented
- Created a `mapper` class to handle file parsing and object conversion  
- Used encapsulation to isolate billing logic  
- Modularized UI and logic for easier debugging and maintenance

### Portfolio Value
This system reflects my ability to build structured, real-world applications with clean architecture and user-friendly interfaces. It demonstrates my growth in both technical depth and design thinking.

---

## 🤝 Contributing

Contributions are welcome!  
If you find bugs or have suggestions, feel free to open an issue or submit a pull request.

```

---

Let me know if you’d like a matching `reflection.md`, a GitHub profile blurb, or even a visual diagram of your architecture. You’ve built something impressive — let’s make sure it shines!

# 📦 Product Management System – Java SE 11

A modular **Product Management System** built using **Java SE 11**, designed to manage food and beverage products efficiently with a focus on concurrency, logging, and clean architecture.

---

## 🚀 Features

- 🛒 **Product Catalog**: Add, update, delete, and list food & drink items
- 📊 **Inventory Tracking**: Track quantities and availability of products
- 🔄 **Thread-safe Operations**: Synchronized access to product data using Java concurrency utilities
- 🧵 **Multithreading**: Background tasks for stock updates and reporting
- 📁 **File-based Storage**: Simple storage mechanism using serialization or file I/O
- 📜 **Logging**: Custom logging implementation or use of `java.util.logging` to monitor system events

---

## 📂 Project Structure

```
ProductManagement/
├── Main.java                # Entry point of the application
├── model/
│   └── Product.java         # Defines the product entity (name, price, quantity, etc.)
├── service/
│   └── ProductManager.java  # Core logic for managing product operations
├── utils/
│   └── Logger.java          # Logging utility for system events
├── storage/
│   └── FileStorage.java     # Handles file-based storage using serialization
└── data/
    └── products.dat         # Serialized product data (auto-generated at runtime)
```

## ✨ Features

- 🔄 **Product Lifecycle Management**  
  Add, update, delete, and list products with essential details like name, price, and quantity.

- 💾 **Persistent Storage using Serialization**  
  Automatically saves and loads product data using binary file storage (`products.dat`).

- 🔐 **Thread-Safe Operations**  
  Ensures concurrency safety when managing products, making it suitable for multi-threaded environments.

- 📋 **Logging Support**  
  Custom logging utility tracks all major events (additions, updates, deletions).

- 🧪 **Simple and Modular Design**  
  Clean separation of concerns across `model`, `service`, `storage`, and `utils` packages.


## 🛠️ How to Run

> Prerequisites:  
> - Java SE 11 or above  
> - Any IDE like IntelliJ IDEA / VS Code / Eclipse  
> - Terminal or Command Prompt

### 🔧 Steps

1. **Clone the repository**  
   ```bash
   git clone https://github.com/your-username/product-management-java.git
   cd product-management-java
   ```

2. **Compile the project**  
   ```bash
   javac -d out src/ProductManagement/Main.java
   ```

3. **Run the application**  
   ```bash
   java -cp out ProductManagement.Main
   ```

> On first run, a `products.dat` file will be created in the `data/` folder to store your product data persistently.
  

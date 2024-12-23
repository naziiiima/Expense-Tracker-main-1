# **Expense Tracker**  
### _A Personal Finance Management Tool_

Welcome to **Expense Tracker**, a sleek and powerful desktop application designed to help you manage your personal expenses with ease. Developed with **Java** and **PostgreSQL**, this application provides an intuitive user interface using **JavaFX**, enabling you to track, filter, and manage your financial records efficiently.

---

## **🚀 Project Overview**

**Expense Tracker** allows users to:

- **Add Expenses**: Enter details like description, amount, category, and date.
- **View All Expenses**: Display a list of all recorded expenses in an organized format.
- **Filter Data**: Easily filter expenses by month or category.
- **Update Expenses**: Modify existing records for better accuracy.
- **Delete Expenses**: Remove specific records or all records in one click.

Built for both beginners and experienced users, this app simplifies personal finance management with a clean, responsive interface.

---

## **💡 Features**

- **Add Expenses**: Enter details such as description, amount, category, and date for each expense.
- **View All Expenses**: View all expenses in a table with easy-to-read columns.
- **Filter Data**:  
  - **By Month**: View expenses for a specific month.  
  - **By Category**: Filter by predefined categories like Food, Transport, etc.
- **Update Expenses**: Modify the description, amount, or category of an existing record.
- **Delete Expenses**: Delete specific expenses or remove all records in the database.

---

## **🛠 Technologies Used**

- **Programming Language**: Java (Version 11 or higher)
- **UI Framework**: JavaFX for a sleek, modern interface
- **Database**: PostgreSQL for data storage
- **Integration**: JDBC for smooth communication with the database

---

## **📋 Setup Guide**

### **1. Prerequisites**

Before running the project, ensure the following are installed:

- **JDK** (Java Development Kit): Version 11 or higher
- **PostgreSQL**: For database setup and management
- **IDE**: IntelliJ IDEA, Eclipse, or any Java IDE of your choice

---

### **2. Database Configuration**

1. **Create Database**: Open PostgreSQL and create a new database:

    ```sql
    CREATE DATABASE expense_tracker;
    ```

2. **Run SQL Script**: Execute the provided `setup.sql` script to:
    - Create necessary tables (`expenses`, `categories`).
    - Populate the `categories` table with sample data.

3. **Verify Tables**: Ensure the following tables are created:
    - `categories`: Stores predefined expense categories.
    - `expenses`: Stores detailed records of user expenses.

---

### **3. Application Configuration**

1. Open the `DatabaseConnection.java` file.
2. Update the following database connection details:

    ```java
    private static final String URL = "jdbc:postgresql://localhost:5432/expense_tracker";
    private static final String USER = "your_username";
    private static final String PASSWORD = "your_password";
    ```

---

### **4. Running the Application**

1. Import the project into your IDE.
2. Locate and open the `HelloApplication.java` file.
3. Run the `main` method to launch the application.

---

## **💼 Usage Instructions**

### **Add an Expense**
1. Enter the following details:
   - **Description**: A short note (e.g., "Coffee").
   - **Amount**: Numeric value (e.g., "5.00").
   - **Category**: Select from predefined categories (e.g., "Food").
   - **Date**: Format: YYYY-MM-DD (e.g., "2024-12-23").
2. Click **"Add Expense"** to save the record.

---

### **View All Expenses**
1. Click **"View All Expenses"** to display all recorded expenses in a structured table.

---

### **Filter Expenses**
1. **By Month**: Enter the month in **YYYY-MM** format (e.g., "2024-12") and click **"Filter by Month"**.
2. **By Category**: Select a category from the dropdown and click **"Filter by Category"**.

---

### **Update an Expense**
1. Enter the **description** of the expense you want to update.
2. Modify any field (amount, category, etc.).
3. Click **"Update Expense"**.

---

### **Delete an Expense**
1. **Specific Record**: Enter the description and click **"Delete Expense by Description"**.
2. **All Records**: Click **"Delete All Expenses"** to remove everything from the database.

---

## **📁 Project Structure**

```plaintext
src/
├── org.example.expensetracker/
│   ├── DatabaseConnection.java   # Handles database connection
│   ├── Expense.java              # Expense model class
│   ├── ExpenseDAO.java           # CRUD operations for expense records
│   ├── HelloController.java      # UI logic controller
│   ├── HelloApplication.java     # Entry point for the application
│   └── resources/
│       ├── hello-view.fxml       # FXML layout for the user interface
│       └── expense-tracker.jpg   # Background image for the UI
└── setup.sql                     # SQL script to set up the database

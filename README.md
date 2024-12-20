---

# 💸 Expense Tracker  

An intuitive and efficient expense tracking application designed to help you manage your finances with ease. Track your spending, categorize expenses, and filter them effortlessly.  

---

## 🛠️ **Setup Instructions**

### 1. **Create Database**  
- Open PostgreSQL and create a database:  
```sql
CREATE DATABASE expense_tracker;
```  

### 2. **Run SQL Script**  
- Execute the provided `setup.sql` file to:  
  - Create necessary tables (`expenses`, `categories`).  
  - Populate the `categories` table with sample data.  

### 3. **Verify Tables**  
- Ensure the following tables are created:  
  - `categories` - Predefined expense categories.  
  - `expenses` - Detailed records for your expenses.  

---

## ⚙️ **Application Configuration**

1. Open the `DatabaseConnection.java` file.  
2. Update the database connection details:  
```java
private static final String URL = "jdbc:postgresql://localhost:5432/expense_tracker";
private static final String USER = "your_username";
private static final String PASSWORD = "your_password";
```  

---

## 🚀 **Running the Application**

1. Import the project into your IDE.  
2. Locate the `HelloApplication.java` file.  
3. Run the `main` method to launch the application.  

---

## 📖 **Usage Instructions**

### **Add Expense**
- Enter the following details:  
  - **Description:** A short note about the expense (e.g., "Coffee").  
  - **Amount:** Numeric value (e.g., "5.00").  
  - **Category:** Select a predefined category (e.g., "Food").  
  - **Date:** Enter in `YYYY-MM-DD` format.  
- Click **"Add Expense"** to save the record.  

### **View All Expenses**
- Click **"View All Expenses"** to display all expense records.  

### **Filter Expenses**
- **By Month:** Enter the month in `YYYY-MM` format (e.g., "2024-12") and click **"Filter by Month"**.  
- **By Category:** Select a category from the dropdown menu and click **"Filter by Category"**.  

### **Update Expense**
- Enter the description of the expense you want to update.  
- Modify any field and click **"Update Expense"**.  

### **Delete Expense**
- **Specific Record:** Enter the description and click **"Delete Expense by Description"**.  
- **All Records:** Click **"Delete All Expenses"** to clear the database.  

---

## 📂 **Project Structure**

```plaintext
src/
├── org.example.expensetracker/
│   ├── DatabaseConnection.java   # Handles database connection
│   ├── Expense.java              # Expense model class
│   ├── ExpenseDAO.java           # Database Access Object (CRUD operations)
│   ├── HelloController.java      # Controller for UI logic
│   ├── HelloApplication.java     # Entry point for the application
│   └── resources/
│       ├── hello-view.fxml       # FXML layout for UI
│       └── expense-tracker.jpg   # Background image for the interface
└── setup.sql                     # SQL script for database setup
```

---

## 🎨 **Future Enhancements**

- 📊 Add graphical visualizations (e.g., pie charts for category breakdown).  
- 👥 Implement user authentication for multi-user support.  
- 🔄 Include recurring expenses and income tracking.  
- 📱 Develop a mobile-friendly version.  

---

## 📷 **Screenshots**

### **Main Interface**  
*(Screenshot of the application's main window)*  

### **Adding an Expense**  
*(Screenshot of the "Add Expense" feature)*  

### **Filter by Category**  
*(Screenshot of filtered results by category)*  

---

## 🌟 **Contributing**
Contributions are welcome! Feel free to submit a pull request or open an issue for suggestions.  

---

## 📄 **License**
This project is licensed under the [MIT License](LICENSE).  

---

Make your finances simpler with **Expense Tracker**! ✨  

---

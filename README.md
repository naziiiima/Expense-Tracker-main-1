# Expense-Tracker-main
## Project Overview
Expense Tracker is a desktop application built with Java and PostgreSQL for efficient management and analysis of personal expenses. 
The application features a clean, user-friendly interface created using JavaFX, with database connectivity handled via JDBC. 
It allows users to track, filter, and manage their financial records effectively.

## Features
Add Expenses: Enter description, amount, category, and date for each expense.
View All Expenses: Display all recorded data in a structured format.
### Filter Data:
- By Month: View expenses for a specific month.
- By Category: Filter expenses by predefined categories (e.g., Food, Transport).
- Update Expenses: Modify existing records.
- Delete Expenses: Remove specific or all records from the database. 
### Technologies Used
- Programming Language: Java (11+)
- UI Framework: JavaFX
### Database: PostgreSQL
- Integration: JDBC for database communication
- Setup Guide
  
## 1. Prerequisites
Before running the project, ensure you have the following installed:

- JDK (Java Development Kit): Version 11 or higher
- PostgreSQL: For database setup and management
- IDE: IntelliJ IDEA, Eclipse, or any preferred IDE
  
## 2. Database Configuration
Create Database: Open PostgreSQL and create a database:
sql
Копировать код
CREATE DATABASE expense_tracker;
Run SQL Script: Execute the provided setup.sql file to:
Create necessary tables (expenses, categories).
Populate the categories table with sample data.
Verify Tables: Ensure the following tables are created:
categories for predefined expense categories.
expenses for storing detailed records.
3. Application Configuration
Open the DatabaseConnection.java file.
Update the following database connection details:
java
Копировать код
private static final String URL = "jdbc:postgresql://localhost:5432/expense_tracker";
private static final String USER = "your_username";
private static final String PASSWORD = "your_password";
4. Running the Application
Import the project into your IDE.
Locate the HelloApplication.java file.
Run the main method to launch the application.
Usage Instructions
Add Expense
Enter the following details:
Description: A short note about the expense (e.g., "Coffee").
Amount: Numeric value (e.g., "5.00").
Category: Select a predefined category (e.g., "Food").
Date: Enter in YYYY-MM-DD format.
Click "Add Expense" to save the record.
View All Expenses
Click "View All Expenses" to display all expense records.
Filter Expenses
By Month: Enter the month in YYYY-MM format (e.g., "2024-12") and click "Filter by Month".
By Category: Select a category from the dropdown menu and click "Filter by Category".
Update Expense
Enter the description of the expense you want to update.
Modify any field and click "Update Expense".
Delete Expense
Specific Record: Enter the description and click "Delete Expense by Description".
All Records: Click "Delete All Expenses" to clear the database.
Project Structure
plaintext
Копировать код
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
Future Enhancements
Add graphical visualizations (e.g., pie charts for category breakdown).
Implement user authentication for multi-user support.
Include recurring expenses and income tracking.
Develop a mobile-friendly version.
Screenshots
Main Interface (Add screenshot showing the application's main window)

Adding an Expense (Add screenshot of the "Add Expense" feature)

Filter by Category (Add screenshot of filtered results by category)


# Smart Expense Tracker 💰

## 🌐 Full-Stack Web Application (v2.0)

A professional **full-stack expense tracking application** with:

- **Spring Boot REST API** backend (14 endpoints)
- **React-style modern frontend** with glassmorphism design
- **Spring Data JPA** database persistence
- **H2/MySQL** database support

Originally a CLI-based personal finance management system, now upgraded to a production-ready web application demonstrating real-world full-stack development skills and industry best practices.

## 🎯 Project Overview

The **Smart Expense Tracker** is a command-line application that helps users manage their income and expenses with robust categorization, reporting, and data persistence features. Built entirely using Core Java with no external dependencies, this project showcases clean architecture, design patterns, and industry-standard coding practices.

## ✨ Features

### Core Functionality

- ✅ **Add Income** - Track income from various sources (Salary, Freelance, Investment, etc.)
- ✅ **Add Expense** - Record expenses with 9 predefined categories
- ✅ **View All Transactions** - Display complete transaction history
- ✅ **Smart Summaries** - Daily, Weekly, and Monthly financial reports
- ✅ **Advanced Search** - Filter by date range or category
- ✅ **Savings Tracker** - Calculate and monitor total savings
- ✅ **Category Breakdown** - Analyze spending patterns with percentage breakdowns
- ✅ **Delete Transactions** - Remove incorrect entries with confirmation
- ✅ **Data Persistence** - Auto-save to CSV file

### Technical Highlights

- 🏗️ **MVC Architecture** - Clean separation of concerns
- 🎨 **OOP Principles** - Abstraction, Encapsulation, Inheritance, Polymorphism
- 📦 **Collections Framework** - ArrayList, HashMap, Streams
- 📅 **Modern Date/Time API** - LocalDate and DateTimeFormatter
- 🛡️ **Exception Handling** - Comprehensive error management
- 📁 **File I/O** - CSV-based data storage
- ✅ **Input Validation** - Robust user input validation

## 📁 Project Structure

```
SmartExpenseTracker/
├── src/
│   └── com/
│       └── expensetracker/
│           ├── model/                  # Data Models
│           │   ├── Transaction.java    # Abstract base class
│           │   ├── Income.java         # Income subclass
│           │   ├── Expense.java        # Expense subclass
│           │   ├── Category.java       # Expense categories enum
│           │   └── TransactionType.java
│           ├── service/                # Business Logic
│           │   ├── TransactionService.java  # CRUD operations
│           │   ├── ReportService.java       # Analytics & reports
│           │   └── FileService.java         # Data persistence
│           ├── util/                   # Utilities
│           │   ├── Constants.java      # App constants
│           │   ├── DateUtil.java       # Date operations
│           │   └── ValidationUtil.java # Input validation
│           ├── MenuHandler.java        # CLI interactions
│           └── ExpenseTrackerApp.java  # Main entry point
├── data/
│   └── transactions.csv               # Auto-generated data file
├── README.md
└── JDBC_UPGRADE_GUIDE.md
```

## 🚀 How to Run

### Prerequisites

- Java Development Kit (JDK) 8 or higher
- Command line/Terminal access

### Compilation

```powershell
# Navigate to project directory
cd C:\Users\skk\OneDrive\C0deAlpha\SmartExpenseTracker

# Compile all Java files
javac -d bin src/com/expensetracker/*.java src/com/expensetracker/model/*.java src/com/expensetracker/service/*.java src/com/expensetracker/util/*.java
```

### Execution

```powershell
# Run the application
java -cp bin com.expensetracker.ExpenseTrackerApp
```

## 💡 Usage Examples

### Adding an Income

```
1. Add Income
Description: Monthly Salary
Amount (₹): 50000
Date (yyyy-MM-dd) [Press Enter for today]: 2026-01-01
Source (Salary/Freelance/Investment/Other): Salary
✓ Income added successfully!
```

### Adding an Expense

```
2. Add Expense
Description: Groceries
Amount (₹): 2500
Date (yyyy-MM-dd) [Press Enter for today]:
Category: FOOD
✓ Expense added successfully!
```

### Viewing Monthly Summary

```
MONTHLY SUMMARY - JANUARY
═══════════════════════════════════════════════════════════
Total Income   : ₹        50,000.00
Total Expense  : ₹        15,750.00
───────────────────────────────────────────────────────────
Net Savings    : ₹        34,250.00 ✓
Transactions   : 8
═══════════════════════════════════════════════════════════
```

### Category-wise Breakdown

```
CATEGORY-WISE EXPENSE BREAKDOWN
═══════════════════════════════════════════════════════════
CATEGORY             AMOUNT         PERCENTAGE
───────────────────────────────────────────────────────────
Food & Dining        ₹      5,500.00          34.92%
Travel & Transport   ₹      4,200.00          26.67%
Entertainment        ₹      3,050.00          19.37%
Shopping & Personal  ₹      2,000.00          12.70%
Utilities & Bills    ₹      1,000.00           6.35%
───────────────────────────────────────────────────────────
TOTAL                ₹     15,750.00        100.00%
═══════════════════════════════════════════════════════════
```

## 🎓 OOP Concepts Demonstrated

### 1. **Abstraction**

- `Transaction` as abstract base class with `display()` and `toCSV()` abstract methods
- Service interfaces for business logic abstraction

### 2. **Encapsulation**

- Private fields with public getters/setters
- Data validation in setters
- Immutable IDs

### 3. **Inheritance**

- `Income` and `Expense` extend `Transaction`
- Code reuse and specialization

### 4. **Polymorphism**

- Runtime method dispatch for `display()` and `toCSV()`
- Different implementations in `Income` and `Expense`

### 5. **Composition**

- Services composed of other services
- Dependency injection pattern

## 🏆 Resume-Ready Bullet Points

Use these on your resume or LinkedIn:

- ✅ Developed a **Smart Expense Tracker** CLI application using **Core Java** with **MVC architecture** to manage personal finances with income tracking, expense categorization, and financial reporting
- ✅ Implemented **OOP principles** (Abstraction, Inheritance, Polymorphism) with abstract `Transaction` class and concrete `Income`/`Expense` subclasses for extensible design
- ✅ Utilized **Java Collections Framework** (ArrayList, HashMap) and **Streams API** for efficient data processing and analytics
- ✅ Built **data persistence layer** using file I/O with CSV format, including auto-save functionality and error recovery mechanisms
- ✅ Designed **service layer architecture** with TransactionService, ReportService, and FileService for clean separation of concerns
- ✅ Integrated **LocalDate/LocalDateTime API** for accurate date handling with custom utilities for daily, weekly, and monthly summaries
- ✅ Implemented **comprehensive exception handling** and **input validation** for robust error management and user-friendly feedback
- ✅ Created **modular package structure** following industry standards with model, service, util, and controller layers

## 📊 Technical Stack

| Category            | Technology                                   |
| ------------------- | -------------------------------------------- |
| **Language**        | Java 8+                                      |
| **Architecture**    | MVC Pattern                                  |
| **Data Structures** | ArrayList, HashMap, LinkedHashMap            |
| **Date/Time**       | LocalDate, DateTimeFormatter                 |
| **File I/O**        | BufferedReader, BufferedWriter               |
| **Design Patterns** | Service Layer, Dependency Injection, Factory |
| **Persistence**     | CSV File Storage                             |

## 🔧 Advanced Features

### Smart Date Handling

- Auto-fill today's date
- Date range validation
- Period-based filtering (daily/weekly/monthly)

### Comprehensive Validation

- Amount must be positive
- Non-empty descriptions
- Valid date formats
- Category verification

### User-Friendly CLI

- Formatted tables with proper alignment
- Unicode symbols for visual appeal
- Color-coded messages (success/error)
- Confirmation prompts for destructive actions

### Potential Features

- 🗄️ Database integration (MySQL/PostgreSQL)
- 📧 Email reporting
- 📊 Export to PDF/Excel
- 🔐 User authentication
- 💹 Budget limits and alerts
- 📱 REST API for web/mobile frontend
- 📉 Data visualization with charts

## 🎯 Learning Outcomes

This project demonstrates:

- Real-world software architecture design
- Industry-standard coding practices
- Clean, maintainable, and scalable code
- Problem-solving and logical thinking
- File persistence without databases
- Complete SDLC from design to testing

## 👨‍💻 Author

**Smart Expense Tracker Team**  
Version 1.0 - January 2026

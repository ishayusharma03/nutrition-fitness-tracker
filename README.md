# 🥗 Personalized Nutrition and Fitness Tracking System

> A desktop application for monitoring dietary intake and fitness activities, built with Java, JavaFX, and MySQL.

---

## 📌 Overview

This is a full-featured desktop application that enables users to track their daily nutrition and fitness activities in one place. Built using Java and JavaFX with a MySQL backend, it follows clean OOP principles for a maintainable and extensible codebase.

---

## ✨ Features

- 🍽️ **Nutrition Tracking** – Log daily meals and monitor caloric/macronutrient intake
- 🏋️ **Fitness Activity Logging** – Record workouts and physical activities
- 📊 **Health Dashboard** – Visual overview of daily progress and trends
- 🗄️ **Persistent Storage** – MySQL database integration via JDBC for reliable data management
- 👤 **User Profiles** – Personalized health records per user
- 🖥️ **Interactive UI** – Clean and intuitive JavaFX interface

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Language | Java |
| UI Framework | JavaFX |
| Database | MySQL |
| DB Connectivity | JDBC |
| Architecture | Object-Oriented Programming (OOP) |

---

## 🚀 Getting Started

### Prerequisites
- Java 11+
- MySQL 8.0+
- JavaFX SDK

```bash
# Clone the repository
git clone https://github.com/ishayu-sharma/nutrition-fitness-tracker.git
cd nutrition-fitness-tracker

# Set up the database
mysql -u root -p < schema.sql

# Configure DB credentials in config.properties
# db.url=jdbc:mysql://localhost:3306/fitness_tracker
# db.user=your_username
# db.password=your_password

# Compile and run
javac --module-path /path/to/javafx/lib --add-modules javafx.controls,javafx.fxml -d out src/**/*.java
java --module-path /path/to/javafx/lib --add-modules javafx.controls,javafx.fxml -cp out Main
```

---

## 📁 Project Structure

```
nutrition-fitness-tracker/
├── src/
│   ├── Main.java                   # Entry point
│   ├── controllers/                # JavaFX controllers
│   ├── models/                     # Data models (User, Meal, Activity)
│   ├── database/                   # JDBC connection & queries
│   └── views/                      # FXML layout files
├── resources/
│   └── fxml/                       # UI layout files
├── schema.sql                      # MySQL database schema
├── config.properties               # DB configuration
└── README.md
```

---

## 🏗️ OOP Design Principles Applied

- **Encapsulation** – All model fields are private with controlled access via getters/setters
- **Inheritance** – Base `User` class extended for different user roles
- **Polymorphism** – Activity types handled through a common interface

---

## 👤 Author

**Ishayu Sharma**  
[LinkedIn](https://linkedin.com/in/ishayu-sharma-567a252b2) · [Email](mailto:ishayusharma03@gmail.com)

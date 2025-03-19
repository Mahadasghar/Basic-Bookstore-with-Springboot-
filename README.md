

# 📖 Bookstore Management System (Spring Boot)

A simple **Bookstore Management System** built using **Spring Boot** with **H2 Database** for backend storage and a minimal frontend using **Thymeleaf & CSS**.

## 🚀 Project Overview

This application allows users to:
- **Add** new books with title, author, and ISBN.
- **Update** existing book details.
- **Delete** books from the system.
- **Search** books by title or author.
- **View** books in a scrollable list with only 5 visible at a time.

## 🛠️ Technologies Used
- **Spring Boot** (Backend)
- **Spring Data JPA** (Database Handling)
- **H2 Database** (In-memory storage)
- **Thymeleaf** (Frontend Templating)
- **CSS** (Basic UI Styling)

---

## 🏃 How to Run the Project in IntelliJ IDEA

### **Step 1: Clone or Download the Project**
If you haven't cloned the project yet, run:
```sh
git clone https://github.com/your-repo/bookstore.git
cd bookstore
```
### **Step 2: Open the Project in IntelliJ IDEA**
1. Open **IntelliJ IDEA**.
2. Click **File > Open** and select the project folder.
3. Wait for **Maven** to download dependencies.

### **Step 3: Run the Application**
1. Navigate to the `BookstoreApplication.java` file in `src/main/java/com/example/bookstore/`.
2. Click the **Run** button (or press `Shift + F10`).

The application will start on:  
👉 `http://localhost:8080`

---

## 📂 H2 Database Setup

This project uses an **H2 in-memory database**, meaning **data will be lost after the application restarts**.

### **Access H2 Console**
1. Open your browser and go to:  
   👉 `http://localhost:8080/h2-console`
2. Use the following credentials:
   - **JDBC URL:** `jdbc:h2:mem:bookstoredb`
   - **Username:** `sa`
   - **Password:** *(leave empty)*
3. Click **Connect**.

### **View Book Records in H2 Database**
Once connected, run the following SQL command:
```sql
SELECT * FROM book;
```

---

## 📜 API Endpoints

| Method | Endpoint         | Description           |
|--------|----------------|----------------------|
| GET    | `/api/books`    | Get all books       |
| POST   | `/api/books`    | Add a new book      |
| PUT    | `/api/books/{id}` | Update a book      |
| DELETE | `/api/books/{id}` | Delete a book      |

---

## 💡 Features
- **Only 5 books are shown at a time**, remaining are scrollable.
- **Duplicate author names & ISBNs are prevented** with a validation check.
- **Search bar** filters books by **title** or **author**.
- **Styled UI** for better user experience.

---

## 👨‍💻 Contribution & Issues
- Feel free to **fork** the project and submit PRs.

---

### 🎉 Happy Coding!
```

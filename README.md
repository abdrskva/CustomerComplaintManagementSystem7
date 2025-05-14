#  Customer Complaint Management System

This is a Java-based application designed to help organizations **log**, **track**, **resolve**, and **manage customer complaints** efficiently. The system supports both a **Command-Line Interface (CLI)** and a **Graphical User Interface (GUI)** using **JavaFX**. Data is stored in an **SQLite database**.

---

##  Developed by

**Salima Abdyrasakova**  
_COMCEH-23_  
**Project:** Complaint Resolution System



##  Project Goals

- Practice object-oriented programming in Java.
- Implement full **CRUD operations**.
- Ensure **data persistence** using files and then migrate to **SQLite**.
- Provide both CLI and GUI access to the complaint system.
- Learn to build a modular, testable and maintainable application.
- Bonus: Add **Login system**, **filtering**, **status updates**, and **CSV export**.

---

##  Features

 Create, view, update, and delete complaints  
 Track complaint status (Open / In Progress / Resolved)  
 Export and import complaints using **CSV**  
 Filter complaints by status  
 Login system with **Admin/User** roles  
 GUI with JavaFX  
 Database integration using SQLite  
 Modular architecture  
 Includes test cases  
 Fully documented code  

---

## Project Structure

CustomerComplaintManagementSystem/
├── src/
│ ├── model/
│ │ ├── Complaint.java
│ │ └── User.java
│ ├── service/
│ │ ├── ComplaintManager.java
│ │ └── AuthService.java
│ ├── util/
│ │ ├── FileHandler.java # earlier version with JSON
│ │ └── DatabaseHandler.java # final version using SQLite
│ ├── view/
│ │ ├── ComplaintView.java # JavaFX UI
│ │ └── JavaFXLoginView.java # Login screen
│ ├── Main.java # CLI version
│ └── MainFX.java # GUI version

---

##  Login Credentials

| Role   | Username | Password |
|--------|----------|----------|
| Admin  | `admin`  | `admin123`  |
| User   | `user`   | `user123`   |

> Admin can add, update, delete, and change statuses  
> User can only view complaints

---

## How to Run

###  Requirements

- JDK 17 or higher
- JavaFX SDK (download from [openjfx.io](https://openjfx.io))
- IntelliJ IDEA (recommended)

###  CLI Version

1. Open `Main.java`
2. Run the file
3. Follow the menu in terminal

###  GUI Version (JavaFX)

1. Open `MainFX.java`
2. Set **VM Options** in Run Configurations:


> Replace `/your/path/...` with your actual JavaFX SDK path  
> Example: `/Users/yourname/Downloads/javafx-sdk-21.0.1/lib`

3. Run the program and log in

---

##  Sample Test Cases

| Scenario              | Input                                 | Expected Output                       |
|-----------------------|----------------------------------------|----------------------------------------|
| Add Complaint         | Name: Salima, Issue: Not working       | New complaint saved with ID and status |
| View Complaints       | Select option 2 or login as User       | All complaints shown                   |
| Filter by Status      | Choose “Resolved”                      | Only resolved complaints listed        |
| Update Status         | Admin selects a row and updates        | Status changes in table and DB         |
| Export CSV            | Click Export button                    | complaints.csv created                 |
| Login Failure         | Wrong username/password                | "Invalid credentials" message          |

---

##  Improvements Table

| 🔧 Feature                                  | Included? | Why Add?                          |
|--------------------------------------------|-----------|-----------------------------------|
| Login System (Admin/User)                  |  Yes    | Bonus points + Realism            |
| Status Filtering                           |  Yes    | Easy navigation of complaint list |
| CSV Export                                 |  Yes    | Shareable and archivable records  |
| SQLite Database                            |  Yes    | Persistent and professional       |
| GUI Polish (Dark mode, etc.)               |  No     | For visual enhancement            |
| Multi-language Support                     |  No     | Future extension idea             |

---

## Tools Used

- Java 17+
- JavaFX 21
- SQLite (via JDBC)
- Gson (for old JSON version)
- IntelliJ IDEA
- DBeaver (to view/edit the database)

---

## 📸 Screenshots

<img width="1440" alt="Снимок экрана 2025-05-11 в 19 17 43" src="https://github.com/user-attachments/assets/3348d087-bb80-4325-9cf4-dd521d69d4db" />
<img width="1440" alt="Снимок экрана 2025-05-11 в 19 16 32" src="https://github.com/user-attachments/assets/54458925-f459-4fc5-a839-ada7d3bc6ee8" />
<img width="818" alt="Снимок экрана 2025-05-11 в 19 16 25" src="https://github.com/user-attachments/assets/53140ff4-5e5f-4f40-bfa7-6236f27e8f1d" />
<img width="1440" alt="Снимок экрана 2025-05-11 в 19 15 50" src="https://github.com/user-attachments/assets/9cdfb49e-3501-4db1-8c3b-c0c89a3bd797" />

---
# link to presentation 
https://www.canva.com/design/DAGnQKXDUBI/59Z6gODqZOSL6C03sfKx9w/edit?utm_content=DAGnQKXDUBI&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton


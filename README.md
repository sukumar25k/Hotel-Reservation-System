# 🏨 Hotel Reservation System

A **Java EE based Hotel Reservation System** built using **EJB (Enterprise Java Beans)**, **Servlets**, **JSP**, and **MySQL**.  
The system allows users to view available rooms, make reservations, and confirm bookings through a web interface.  

---

## 📂 Project Structure

```

HotelReservationSystem/
│── database/              # SQL scripts for database setup
│── HotelReservation-ejb/  # EJB Module (business logic, models, facades)
│── HotelReservation-war/  # WAR Module (servlets, JSPs, CSS, JS, images)
│── screenshots/           # Project screenshots
│── src/conf/              # Manifest configuration
│── build.xml              # Ant build file
│── LICENSE
│── README.md              # Project documentation

```

---

## 🚀 Features

- View available rooms with details  
- Make a reservation for a selected room  
- Confirm final reservation  
- Simple and clean web interface (JSP + CSS + Bootstrap)  
- Database-backed system with EJB session beans for business logic  

---

## 🛠️ Technologies Used

- **Java EE** (Servlets, JSP, EJB)  
- **MySQL** (Database)  
- **JDBC** (Database connectivity)  
- **HTML, CSS, Bootstrap** (Frontend)  
- **Apache Ant** (Build tool)  
- **NetBeans** (Recommended IDE)  

---

## 📸 Screenshots

### 🏠 Home Page
![Home](screenshots/home.PNG)

### 🛏 Available Rooms
![Available Rooms](screenshots/availableRooms.PNG)

### 📑 Final Reservation
![Final Reservation](screenshots/finalReservation.PNG)

---

## ⚙️ Setup Instructions

### 1️⃣ Prerequisites
- Install **JDK 8+**  
- Install **NetBeans (Java EE bundle)**  
- Install **GlassFish / Payara Server** (for EJB + WAR deployment)  
- Install **MySQL Server & Workbench**  

### 2️⃣ Database Setup
1. Open MySQL Workbench.  
2. Run the SQL script provided in:
```

database/sql\_queries.sql

````
3. This will create required tables for rooms and reservations.  

### 3️⃣ Import Project
1. Open NetBeans.  
2. Click **File → Open Project** and select `HotelReservationSystem-master`.  
3. Ensure that both `HotelReservation-ejb` and `HotelReservation-war` are recognized.  

### 4️⃣ Configure Persistence
- Update `HotelReservation-ejb/src/conf/persistence.xml` with your MySQL credentials:
```xml
<property name="javax.persistence.jdbc.url" value="jdbc:mysql://localhost:3306/hotel_db"/>
<property name="javax.persistence.jdbc.user" value="root"/>
<property name="javax.persistence.jdbc.password" value="yourpassword"/>
````

### 5️⃣ Deploy & Run

1. Clean and build the project (`Right-click → Clean and Build`).
2. Deploy to **GlassFish/Payara server**.
3. Access the system at:

   ```
   http://localhost:8080/HotelReservation-war
   ```

---

## 📖 Usage

* **Home Page** → Entry point of the system
* **Available Rooms** → Displays rooms fetched from DB
* **Reservation Page** → Make a booking
* **Final Reservation** → Confirm details

---

## 📌 Future Enhancements

* Add authentication for admin and users
* Implement online payment gateway
* Add email notifications for reservations
* Improve UI with modern frontend frameworks

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙌 Acknowledgements

* Java EE community
* NetBeans & GlassFish developers
* Bootstrap for styling

```

---

Do you want me to also make a **short version (350 chars)** for your GitHub project description like you asked earlier for the stock platform?
```

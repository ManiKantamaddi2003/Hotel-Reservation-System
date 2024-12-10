# 🏨 Hotel Reservation System

A simple **Hotel Reservation Management System** built using Java and MySQL. This project allows users to manage hotel room reservations, view existing reservations, and perform CRUD operations.

---

## 📝 Features

- ✅ **Reserve a Room**: Add guest details and assign a room.
- 📄 **View Reservations**: Display all current reservations.
- 🔍 **Get Room Details**: Retrieve room number by reservation ID and guest name.
- ✏️ **Update Reservation**: Modify guest and room details for an existing reservation.
- ❌ **Delete Reservation**: Remove a reservation from the system.

---

## 📂 Project Structure

📦 src
 └── com.main
     └── HotelReservation.java


- `HotelReservation.java`: Contains the main application logic.



## 🛠️ Technologies Used

- **Java** ![Java](https://img.shields.io/badge/Java-%23ED8B00.svg?style=flat-square&logo=java&logoColor=white)
- **MySQL** ![MySQL](https://img.shields.io/badge/MySQL-%2300f.svg?style=flat-square&logo=mysql&logoColor=white)
- **JDBC** for database connectivity.

---

## 🚀 How to Run

### Prerequisites
1. Install [Java JDK](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) and set up `JAVA_HOME`.
2. Install [MySQL](https://dev.mysql.com/downloads/installer/) and configure a database.

### Setup Instructions
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/hotel-reservation-system.git
   cd hotel-reservation-system
   ```
2. Set up the database:
   - Open MySQL and execute the script in [`database.sql`](database.sql) to create the database and table.
3. Configure database credentials in `HotelReservation.java`:
   ```java
   private static final String url = "jdbc:mysql://localhost:3306/hotel_db";
   private static final String username = "your_mysql_username";
   private static final String password = "your_mysql_password";
   ```
4. Compile and run the program:
   ```bash
   javac -d . HotelReservation.java
   java com.main.HotelReservation
   ```

---

## 🧩 Database Schema

### Table: `reservations`

| Column            | Type         | Description                             |
|--------------------|--------------|-----------------------------------------|
| `reservation_id`  | INT          | Unique ID (Primary Key, Auto Increment) |
| `guest_name`      | VARCHAR(100) | Name of the guest                      |
| `room_number`     | INT          | Room number being reserved             |
| `contact_number`  | VARCHAR(15)  | Contact number of the guest            |
| `reservation_date`| TIMESTAMP    | Auto-filled reservation timestamp      |

---

## 🤝 Contribution

Contributions are welcome! Feel free to:
- Fork the repository
- Create a feature branch
- Submit a pull request

Enjoy coding! 🎉

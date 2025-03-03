<img width="803" alt="image" src="https://github.com/user-attachments/assets/143dc0b9-29eb-4291-819e-acd710ab26e3" />

---

# Local DB for Hospital Services 💾

Database for `Hospiten`.

This repository contains the source code of the project focused on hospital management, developed in `Java` with a `MySQL` database connection. The system allows you to manage patients, doctors, appointments, and other key elements through a graphical interface and `SQL` queries.

The program is capable of:
1. Create a relational database
2. Accessing data history
3. Entering new records of patients and visits to the hospital
4. Formulating higher-level queries
All of this allow access to the most relevant data of each patient and information on the latest visits that permit improving the care provided at `Hospiten`.

## Technologies Used 🖥️

- **Language:** `Java` 
- **Database:** `MySQL`  
- **Tools:** `MySQL Workbench` and `PHPMyAdmin`  
- **Connector:** `JDBC` (Java Database Connectivity)  

## Requirements ☑️

Before running the project, make sure you meet the following requirements:

1. **`Java Development Kit (JDK)`:** Version 8 or higher.  
2. **`MySQL Server`:** Installed and running locally.  
3. **`MySQL Workbench`:** To manage the database.  
4. **`PHPMyAdmin`:** To visualize the records.  
5. **`JDBC Connector`:** Make sure to have the `mysql-connector-java-x.x.x.jar` file in the classpath.  

## Database Configuration 👷🏻‍♂️

1. **Import the database:**
   - Create a database named `proyectofinal` in `MySQL`.
   - Import the `proyectofinal.sql` file included in the repository using `MySQL Workbench` or `PHPMyAdmin`.

2. **Configure the user and password:**
   - Ensure that the user and password in the `Conexion.java` file match your local settings:
     ```java
     private static final String URL = "jdbc:mysql://localhost:3306/proyectofinal";
     private static final String USUARIO = "root";
     private static final String CLAVE = "";
     ```
     
## Running the Project 📊

1. Clone the repository:
   ```bash
   git clone https://github.com/Luisduran206/Local_DB_for_Hospital_Services.git

## Description of Files 🔍

The different Java files form the complete program. The different tasks to be executed were divided given the planning of the database models for this case.
- `Conexion.java`: Class that generates a direct connection between MYSQL Workbench and the program running in Java.
- `Consultar.java`: Class in which the graphical interface is designed and executed, contains all the input fields through which data enters the database.
- `Inicio.java`: Class in which the start interface is designed when the program is executed. Welcome Interface.
- `InscribirPaciente.java`: Class that captures the algorithm for registering a patient in the database. Interaction between the fields of the graphical interface and the restrictions required to generate a new record.
- `Main.java`: Main class of the database. Runs the entire program.
- `QueryViewer.java`: Class responsible for displaying the query history of a previous record.
- `RegistrarVisita.java`: Class whose function is to encode the process for entering the record of a new consultation in the hospital.
- `TestConexion.java`: Class where all queries, additions and deletions of records to the database are performed. The different functions structure different queries in SQL format with the information obtained from the different graphical interfaces.
---
For a better visualization of the graphical interface, make sure you have the image that is at the beginning of the `README.md` and change the location to the folder where it is located in `line 85` at `Inicio.java`:
```java
imagenFondo = ImageIO.read(new File("{Your_Path_to_Image}"));
```

---
Developed by Luis Durán Flores, luisduran206@gmail.com 

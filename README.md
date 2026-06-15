# aerovibetravels
# Aerovibe Travels 🌍✈️

Aerovibe Travels is a dynamic, full-stack travel management and booking website built using PHP and MySQL. This platform allows users to explore flight packages, view exotic destinations, manage travel bookings, and seamlessly plan their next adventure through an intuitive user interface. 

This project is optimized for local deployment using XAMPP and serves as an educational blueprint for understanding full-stack CRUD operations, relational database management, and dynamic PHP rendering.

---

## 🛠️ Features
* **Dynamic Destination Discovery:** Explore curated travel packages pulled directly from a MySQL backend.
* **Booking System:** User-friendly forms to reserve trips and manage travel itineraries.
* **Responsive UI/UX:** A modern, clean, and mobile-friendly interface designed for smooth navigation.
* **Secure Database Integration:** Prepared statements and secure data handling using PHP PDO/MySQLi.

---

## 🚀 Setup & Installation Guide for Students

Follow these step-by-step instructions to get the project running flawlessly on your local machine.

### Prerequisites
Before starting, ensure you have **XAMPP** installed on your system. If you don't have it, download and install it from [Apache Friends](https://www.apachefriends.org/).

---

### Step 1: Download or Clone the Repository
1. Click the green **Code** button at the top of this GitHub page.
2. Select **Download ZIP** (or clone it via terminal using `git clone <repository-url>`).
3. Extract the ZIP file if you downloaded it compressed.

### Step 2: Move the Project to XAMPP Local Server
For XAMPP to execute PHP files, the project folder must reside in the local server directory:
1. Copy your extracted project folder (make sure the folder is named `aerovibetravels`).
2. Navigate to your XAMPP installation directory:
   * **Windows:** `C:\xampp\htdocs\`
   * **Mac:** `/Applications/XAMPP/xamppfiles/htdocs/`
3. Paste the `aerovibetravels` folder directly inside the `htdocs` directory.

### Step 3: Start Apache and MySQL
1. Open the **XAMPP Control Panel**.
2. Click the **Start** buttons next to both **Apache** and **MySQL**.
3. Ensure their status indicators turn green.

### Step 4: Import the Database (phpMyAdmin)
To avoid standard database import errors, follow this exact sequence:
1. Open your web browser and navigate to: `http://localhost/phpmyadmin/`
2. In the left-hand sidebar, click on **New**.
3. Under **Create database**, enter the exact database name: `aerovibetravels` and click **Create**.
4. **Crucial:** Click directly on the newly created `aerovibetravels` database in the left sidebar to enter it. (The top bar should read `Server: localhost > Database: aerovibetravels`).
5. Click the **Import** tab on the top menu bar.
6. Click **Choose File** and locate the `aerovibetravels.sql` file located inside your project folder.
7. Scroll to the bottom and click **Import**. You should see a green success message.

### Step 5: Configure the Codebase Connection
1. Open the project folder in your preferred code editor (e.g., VS Code).
2. Locate the database configuration file (typically `config.php` or `connect.php`).
3. Verify that the database credentials match your local setup:
   ```php
   $host = "localhost";
   $user = "root";      // Default XAMPP username
   $password = "";      // Default XAMPP password is empty
   $dbname = "aerovibetravels";

### Step 6: Run the Website
Open your browser and navigate to the local server path:
👉 http://localhost/aerovibetravels/

The application should now load beautifully without any persistent loading screens!

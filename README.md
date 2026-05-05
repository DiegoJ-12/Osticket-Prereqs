#osTicket Prerequisites and Installation Lab(v1.18.3)
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>Project Overview</h1>
This lab demonstrates the preparation and setup of the required environment for installing osTicket v1.18.3 in a local XAMPP web server. The goal of this project is to simulate a real world IT help desk environment by configuring all prerequisitied neede for a successful osTicket deployment.


<h2>Purpose of the Lab</h2>
The purpose of this lab is to build and configure the foundational environment required for osTicket. This includes setting up a local web server, database services, and required software dependencies to support a functional help desk ticketing system.

<h2>Enviroment Setup</h2>

- Windows 10/11(Local Machine or Virtual Machine)
- XAMPP(Apache & MySQL)
- Web browser(Google Chrome or Microsoft Edge)

<h2>Software Requirements </h2>

- osTicket v1.18.3
- PHP
- MySQL
- Apache Web Server

<h2>Tools used </h2>
- XAMPP control panel
- phpMyAdmin
- File Explorer
- Web browser

<h2>Installation Steps</h2>
<p><img width="1525" height="974" alt="Screenshot 2026-05-01 010925" src="https://github.com/user-attachments/assets/ff161ee5-f127-4bbd-a75e-c34ceb5b7ffe" />
<p> Step 1: Go to the official XAMPP download page. https://www.apachefriends.org/download.html and download the latest version which will be "PHP 8.2.12"
(XAMPP is a free software package that lets you run a local web server on your computer)</p>
<p><img width="1413" height="994" alt="Screenshot 2026-05-01 011931" src="https://github.com/user-attachments/assets/86946050-7ec2-450f-8d57-df2d0d250489" />
 <p> Step 2: Run the installer and install application. After running the installer it will automatically create a folder in the c drive, set up screen will pop up with services we will select all. </p> 
<p><img width="958" height="589" alt="Screenshot 2026-04-30 214250" src="https://github.com/user-attachments/assets/b470ae64-59c1-49b9-ac54-a0ab325b5c05" />
<p> Step 3: After the "setup" installation screen a control panel will pop up after you complete the installation, make sure to start "Apache and MYSQL" severs</p>
<p><img width="1529" height="1018" alt="image" src="https://github.com/user-attachments/assets/184a0083-04ac-404e-a208-4588971d9435" />
<p> Step 4: Go to the official osTicket and download the latest version(v1.18.3) https://osticket.com/download/
<p> <img width="1515" height="895" alt="image" src="https://github.com/user-attachments/assets/3ee18782-e15e-48bf-a84e-ce719d147dc6" />
<p>Step 5: Delete the default files inside C:\xampp\htdocs and open the download files, extract all files into C:\xampp\htdocs.<p>
<p><img <img width="1534" height="1017" alt="image" src="https://github.com/user-attachments/assets/d9c5e75c-b49f-449e-869b-7abd77bbf382" />
<p> Step 6: Open OsTicket, you can open it by searching "localhost" on your webrowser and click on "upload" or on the control panel you can click the "admin"button for apache.</p>
<p><img width="1419" height="1022" alt="image" src="https://github.com/user-attachments/assets/666cdd2a-6ba4-4e5d-9166-bf8a01eca8f4" />
<p> Step 7: Enable the required extensions for osTicket. To enable these extensions go to the XAMPP control panel click on apache "config" and scroll down and open "PHP.INI". From here enable the required extensions ("gd", "imap", "intl" , "opcache") to enable, remove the ;(semicolon) in front of each extension line, then save the file and restart both apache and MySQL services from the XAMPP control panel.
<p><img width="1221" height="863" alt="image" src="https://github.com/user-attachments/assets/029d37d7-6a86-4d52-95db-3f67b9cef544" />
<p> Step 8: Rename the osTicket Configuration File. Navigate to This PC -> Local Disk (C:) -> xampp -> htdocs -> upload -> include, inside the "include folder, locate the file name "os-sampleonfig.php". Right click it and rename it to "ost-config.php".<p>
<p><img width="1535" height="1023" alt="image" src="https://github.com/user-attachments/assets/55fdf317-456c-4a11-ad5b-69556b3c92d1" />
<p> Step 9: Setup account details for "system settings" and "admin".
<p><img width="1535" height="1018" alt="image" src="https://github.com/user-attachments/assets/d3c35e45-1ebe-402d-9a26-c82a2b823ceb" />
<p> Step 10: Create the database, by opening phpMyAdmin through the XAMPP Control Panel (click the MySQL Admin button), then go to the Databases tab, enter osTicket as the database name, and click Create.
<p><img width="1532" height="1021" alt="image" src="https://github.com/user-attachments/assets/c688e9e5-5ffa-40f8-9657-1af42668dcd0" />
<p> Step 11: Create a database user by going to phpMyAdmin → User accounts → Add user account, then return to the osTicket setup page and enter those credentials under Database Settings.
<img width="1215" height="837" alt="image" src="https://github.com/user-attachments/assets/2e373026-609f-4cf9-bb90-f87b87efba5a" />
<p> Step 12: Change the permission of the "ost-config.php" file to read only for security purposes, navigate to This PC -> Local Disk(C:) -> xampp -> htdocs -> upload -> include 
right click on "os-config.php" -> Properties and on attributes change it to read-only. </p>
<p> <img width="1529" height="1021" alt="image" src="https://github.com/user-attachments/assets/8d5e3004-e1fe-4f00-bfcf-95844cff5c8e" />
Final step: Use your admin credentials to log in to the osTicket Staff Control Panel at(http://localhost/upload/scp/login.php).


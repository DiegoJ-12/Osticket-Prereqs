# Osticket-Prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
Project Purpose: This Project demonstrates the initial setup and preparation required to deploy a osTicket system in a Windows enviroment using XAMPP.
This projects covers the necessary prerequisites, including installing and configuring the local server stack (apche, PHP, MySQL) and preparing it for the osTicket Installation.<br />



<h2>Environments and Technologies Used:</h2>

- Operating System: Windows 10/11
- Server Stack: XAMPP(Apache, MySQL, PHP)
- Ticketing System: osTicket
- Database Tool: phpMyAdmin
- Web tools: Chrome Web Browser

<h2>Operating Systems Used </h2>

- Windows 11

<h2>List of Prerequisites</h2>

- Windows 10/11 operating system
- XAMPP installed (Apache, PHP, MySQL)
- osTicket installation package(.zip.file)
- Web Browser(Chrome or Edge)

<h2>Installation Steps</h2>
<p><<img width="1525" height="974" alt="Screenshot 2026-05-01 010925" src="https://github.com/user-attachments/assets/ff161ee5-f127-4bbd-a75e-c34ceb5b7ffe" />
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
<p> Final step: Enable the required extensions for osTicket. To enable these extensions go to the XAMPP control panel click on apache "config" and scroll down and open "PHP.INI". From here enable the required extensions ("gd", "imap", "intl" , "opcache") to enable, remove the ;(semicolon) in front of each extension line, then save the file and retart both apache and MySQL from the XAMPP control panel.

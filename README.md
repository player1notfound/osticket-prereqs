<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machines
- OsTicket Installation files


<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Right click the Start menu located at the bottom left corner of the pc and click "run." Type "control" in the blank box for access to the control panel. Under the control panel, click "Programs. Under "Programs and Feature," click on "Turn Windows Feature ON and Off" and turn on and expand Internet Information Services, World Wide Web services, Application Development Features, and check CGI and press OK. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install all the installation files necessary to proceed to the next step which is the creation of an OsTicket: 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After installing MySQL Server 5.5 Setup, launch the MySQL Server Instance Configuration Wizard, select Standard Configuration, and click Next twice which leads to the security option. At this stage, create a password with the username automatically default to root. After that, press next and the installation is complete. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Search for Internet Information Services(IIS) Manager through the Start menu, right click, and press run as administrator. Next, double click on PHP Manager, press Register on New PHP Version, and click on the three dots at the left where it opens your folder. Open This PC at the left hand tabs, Windows (C:), PHP, and double click on the php-cgi file. Make sure the file is selected as PHP executable at the bottom right corner above Cancel. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Restart Internet Information Services before proceeding with the program.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open two folders. One of which click on Downloads => OsTicket-v1.15.8 while on the other folder, go to This PC = Windows (C:) = inetpub = wwwroot. Drag the upload folder from OsTicket-v1.15.8 to wwwroot folder containing two iisstart files. Rename the upload folder to osTicket. Open the osTicket folder and rename ost-sampleconfig.php to ostconfig.php. Next, right click the file and proceed to Properties → Security → Advanced → Disable inheritance → Remove all inherited permissions from this object → add → Select a principal. After that, type everyone, press Check Names, and hit OK. Ensure that everything under Basic permissions are checked before clicking OK. Remember to Apply then press OK again. 
</p>
<br />


<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Under Internet Information Services (IIS) Manager, expand Sites then Default Web Site and double click on the osTickect folder. On the right click Browse *:80 (http) to which the osTicket Installer Support Ticket System website appears. Under osTicket folder in Internet Information Services (IIS) Manager, open PHP Manager and enable php_imap.dll, php_intl.dll, and php_opcache.dll.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Set up osTicket in the browser. This includes generating a dinstinctive helpdesk name and username. Launch HeidiSQL_12.3.0.6589_Setup. Create a new connection to the database by clicking New. The username is root and the password is the password created with MySQL. After entering the information, click Open. Right click Unnamed, expand Create new, and click Database. Enter osTicket for the name and click OK. This will be the code for MySQL Database in osTicket website.
  
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
For cleanup, head to This PC → Windows (C:) → inetpub → wwwroot → osTicket. Delete the setup folder. Set the Permissions of ost-config.php to Ready only by right opening the properties of ost-config.php → Security → Advanced → Edit. Uncheck "Full control", "Modify", and "Write." 
</p>
<br />
</p>
<br />

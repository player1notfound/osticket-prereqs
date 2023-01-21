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
- Install mysequeal
- Install c++ redistributable
- Item 5

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
Search for Internet Information Services(IIS) Manager through the Start menu, right click, and press run as administrator. Next, double click on PHP Manager, click on Register on New PHP Version. 
</p>
<br />

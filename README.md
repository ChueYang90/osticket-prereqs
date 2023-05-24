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

- Windows 10</b> (22H2)

<h2>List of Prerequisites</h2>

- Install / Enable IIS in Windows WITH CGI and Common HTTP Features
- Download and Install PHP Manager for IIS
- Download and Install Rewrite Module
- Create the directory C:\PHP
- Download PHP 7.3.8 and Extract Content into C:\PHP
- Dowload and install VC_redist.x86.exe.
- Download and install MySQL 5.5.62
- Open IIS as an Admin and Register PHP from within IIS then Reload IIS 
- Install osTicket v1.15.8
- Enable Extensions for osTicket in PHP Manager
- Rename: ost-sampleconfig.php and assign permissions
- Install HeidiSQL


<h2>Installation Steps</h2>


![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/ISS.png?raw=true)

<p>

</p>
<p>
Enabled the IIS in Windows via the Control Panel --> Programs --> Windows Features --> World Wide Web Services -> Application Development Features ->
[X] CGI
[X] Common HTTP Features

</p>
<br />

<p>
  
![PHP](https://github.com/ChueYang90/images/blob/main/PHP%20Manager.png?raw=true)
  
</p>
<p>
Download and Installed PHP Manager for IIS.
</p>
<br />

<p>
  
![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/Rewrite.png?raw=true)

</p>
<p>
 Download and installed Rewrite Module.
</p>
<br />

![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/PHP%20Directory.png?raw=true)

</p>
<p>
Created the directory C:\PHP for later use in the project.
</p>
<br />


![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/Extracted%20File.png?raw=true)

</p>
<p>
Downloaded PHP 7.3.8 and Extracted Content into C:\PHP.
</p>
<br />

![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/VC%20redist.png?raw=true)

</p>
<p>
Dowloaded and installed VC_redist.x86.exe.
</p>
<br />

![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/MySQL.png?raw=true)

</p>
<p>
Dowloaded and installed MySQL 5.5.62. When prompt selected Typical Setup and installed. After installation selected Standard Configuration then created a root password. 
</p>
<br />

![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/RegisterPHP.png?raw=true)

</p>
<p>
Opened IIS as Administrator and Registered PHP from within IIS. 
</p>
<br />


![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/PHP-Cgi.png?raw=true)

</p>
<p>
When prompted to select a path, the executable file from within the C:\PHP was selected. 
</p>
<br />

![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/Osticket%20upload.png?raw=true)


</p>
<p>
Install osTicket v1.15.8 then extracted and copied “upload” folder to c:\inetpub\wwwroot.
</p>
<br />


![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/osTicketRename.png?raw=true)

</p>
<p>
Renamed "Upload" folder to "osTicket".
</p>
<br />


![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/osTicketEnableExtensions.png?raw=true)

</p>
<p>
Reloaded IIS then selected sites -> Default -> osTicket
Double-click PHP Manager
Click “Enable or disable an extension”

</p>
<br />

![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/EnabledosTicketExtensions.png?raw=true)

</p>
<p>
Enabled the following extensions: php_imap.dll, php_intl.dll, php_opcache.dll
</p>
<br />

![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/RenameOsconfig.png?raw=true)


</p>
<p>
Renamed the file ost-sampleconfig.php from: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php to ost-config.php
</p>
<br />

![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/permissions.png?raw=true)

</p>
<p>
Acessed the permissions by right clicking the ost-config.php file --> Properties --> Security --> Advanced --> Disable inheritance -> Remove All
New Permissions -> Everyone -> All

</p>
<br />

![Enable IIS in Windows](https://github.com/ChueYang90/images/blob/main/Heidi.png?raw=true)

</p>
<p>
Installed HeidiSQL

</p>
<br />

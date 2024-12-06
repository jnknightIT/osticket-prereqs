<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- IIS and Management Console
- PHP and Rewrite Module
- MySQL
- HeidiSQL
- osTicket

- 

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/SRcqHga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a Windows 10 OS virtual machine. open control panel. Click "Programs". Click Turn Windows features on or off. Install and enable IIS management console in web management tools. Also, enable CGI and all of Common HTTP Features boxes (located in: world wide web services > application development features.) Install rewrite module. Install PHP manager. 
</p>
<br />

<p>
<img src="https://i.imgur.com/5ug46zA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a folder in C:\ called "PHP". Install PHP and unzip contents to PHP folder you created. install VC redist.x86.exe. Install MySqL (typical setup). Launch configuration wizard, select standard and create a name plus password. 
</p>
<br />

<p>
<img src="https://i.imgur.com/UGCqZa4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS as administrator. Register PHP inside of IIS. Stop and start server. Install osTicket. Extract "uploads" folder to C:\inetpub\wwwroot. Rename the folder "osTicket". Reload IIS (Stop and start server). Go to: sites > default > osTicket; on the far right of the window, click on "Browse*:80". Go to C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php and rename "ost-sampleconfig.php" to "ost-config.php". Right click on "ost-config.php" and click "proporties" go to security tab and click "Advanced" Assign file permissions to everyone (Disable inheritance > Remove All, New Permissions > Everyone > All). Next, you will need to enable PHP extensions before continuing with osTicket. Go back to IIS and go to "sites > default > osTicket. Double click on PHP manager and then click on "Enable or disable an extension".  Enable "php_imap.dll", "php_intl.dll" and "php_opcache.dll". If you refresh the browser, osTicket's PHP extension changes will be shown.
</p>
<br />

<p>
<img src="https://i.imgur.com/pZYAiBc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS as administrator. Register PHP inside of IIS. Stop and start server. Install osTicket. Extract "uploads" folder to C:\inetpub\wwwroot. Rename the folder "osTicket". Reload IIS (Stop and start server). Go to: sites > default > osTicket; on the far right of the window, click on "Browse*:80". Go to C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php and rename "ost-sampleconfig.php" to "ost-config.php". Right click on "ost-config.php" and click "proporties" go to security tab and click "Advanced" Assign file permissions to everyone (Disable inheritance > Remove All, New Permissions > Everyone > All). Next, you will need to enable PHP extensions before continuing with osTicket. Go back to IIS and go to "sites > default > osTicket. Double click on PHP manager and then click on "Enable or disable an extension".  Enable "php_imap.dll", "php_intl.dll" and "php_opcache.dll". If you refresh the browser, osTicket's PHP extension changes will be shown.
</p>

<br />

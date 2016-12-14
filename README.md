# Udacity_server
Udacity FSND Server Configuration

This file is the description file for the Linux Server Configuration Project.

The connection information for the server is 

```
 IP Address: 35.165.75.211 

 Live URL: http://35.165.75.211
```

The software running the application on the server includes the following:

|Server|      
|------|      
|Apache v2.4.7|
|UFW v0.34|
|mod-wsgi v3.4|

|Application|
|-----------|
|Python v2.7.6|
|PostgreSQL v9.3.15|
|Flask v0.11.1|
|oAuth2 Client v4.0.0|
|SQLAlchemy v1.1.4|

The configuration process involved the following steps:

1.  Connect to the server and create an admin account and a grader account.  Along with creating a ssh key for the admin account and granting the sudo ability to the admin and grader account.

2.  Update the repository database and upgrade all packages on the server.  Install the apache and libapache-mod-wsgi packages for the server.

3.  After verifying the accounts capability to login and use sudo righs, the ssh settings were modified to disable password login and block root account login.  Configure the server to allow the proper firewall port settings: 80 for HTTP, 2200 for SSH, and 123 for NTP.  

4.  Clone the catalog project from the altered git branch for the PostgreSQL database instead of SQLite.  Update the apache VirtualHost settings to use the catalog project code that is located outside the apache base directory.

5.  Get the PostgreSQL, Flask, oAuth2 Client, and SQLAlchemy packages downloaded and installed on the server.  

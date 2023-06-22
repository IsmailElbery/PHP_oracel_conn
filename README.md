<p align="center">
  <a href="" rel="noopener">
</p>

<h3 align="center">SEU - Task</h3>

<div align="center">

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/kylelobo/The-Documentation-Compendium.svg)](https://github.com/kylelobo/The-Documentation-Compendium/pulls)

</div>

---

<p align="center"> Check and solve some issues in a PHP code.
    <br> 
</p>

## 📝 Table of Contents

- [Connecting PHP Project to Oracle DB](#about)
- [Prerequisites](#rate_code)
- [Steps](#quality_problems)
- [Authors](#authors)

## 🧐 Connecting PHP Project to Oracle DB <a name = "about"></a>

This guide will walk you through the steps of making a connection between an existing PHP project (CodeIgniter or Laravel) and Oracle DB.
## 🏁 Prerequisites <a name = "rate_code"></a>
- PHP project (CodeIgniter or Laravel).
- Oracle DB.
- Oracle SQL Developer.
- Oracle Instant Client.


## 🚀 Steps <a name = "quality_problems"></a>

### Step 1: Download Oracle Instant Client

- Download the Oracle Instant Client from the following link: https://www.oracle.com/database/technologies/instant-client/downloads.html

- Choose the version that matches your OS and download it.

- Extract the downloaded file.

### Step 2: Download Oracle SQL Developer

- Download the Oracle SQL Developer from the following link: https://www.oracle.com/tools/downloads/sqldev-downloads.html

- Choose the version that matches your OS and download it.

- Extract the downloaded file.

### Step 3: Download Oracle DB

- Download the Oracle DB from the following link: https://www.oracle.com/database/technologies/oracle-database-software-downloads.html

- Choose the version that matches your OS and download it.

- Extract the downloaded file.

### Step 4: Create a new connection in Oracle SQL Developer

- Open Oracle SQL Developer.

- Click on the green plus sign to create a new connection.

- Enter the following information:

  - Connection Name: Any name you want.
  - Username: The username of the Oracle DB.
  - Password: The password of the Oracle DB.
  - Hostname: localhost
  - Port: 1521
  - SID: xe

- Click on Test to test the connection.

- Click on Connect to connect to the Oracle DB.

### Step 5: Add the Oracle Instant Client to the PHP project

- Copy the extracted folder from the Oracle Instant Client to the PHP project.

- Rename the folder to oci.

- Open the php.ini file and add the following line:

  - extension=oci\oci8_12c

### Step 6: Add the Oracle Instant Client to the PATH

- Open the Environment Variables.

- Add the path of the Oracle Instant Client to the PATH variable.

### Step 7: Add the Oracle Instant Client to the PATH

- Open the Environment Variables.

- Add the path of the Oracle Instant Client to the PATH variable.


### Step 8: Update the database.php file

- Open the database.php file.

- Update the following information:

  - hostname: localhost
  - username: The username of the Oracle DB.
  - password: The password of the Oracle DB.
  - database: xe
  - dbdriver: oci8_12c

### Step 9: Update the tnsnames.ora file

- Open the tnsnames.ora file.

- Add the following information:

  - xe =
    (DESCRIPTION =
    (ADDRESS = (PROTOCOL = TCP)(HOST = localhost)(PORT = 1521))
    (CONNECT_DATA =
    (SERVER = DEDICATED)
    (SERVICE_NAME = xe)
    )
    )

### Step 10: Update the php.ini file

- Open the php.ini file.

- Update the following information:

  - extension=oci\oci8_12c

### Step 11: Restart the Apache server

- Restart the Apache server.

- Now you can run the PHP project and it will connect to the Oracle DB.



## ✍️ Authors <a name = "authors"></a>

- [@IsmailElbery](https://github.com/IsmailElbery) - Idea & Initial work

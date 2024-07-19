# Setting up MySQL Server Locally

We'll use the MySQL server.

- MySQL server: https://dev.mysql.com/downloads/mysql/
- MySQL workbench: https://dev.mysql.com/downloads/workbench/

After downloading MySQL, Extract downloaded file & then for installing go to `bin` folder & then find `mysql configurator.exe` & then complete neccecary information & installation will be done.
Remember the path where you execute the installation.

You'll be asked to set a root password while installing MySQL server.

To interact with the MySQL server via the terminal use :

```
$ /path_to_MySQL/mysql/bin/mysql -u root -p
```

After that, It'll ask for password, Enter the correct password you set during installation & then you can use MySQL in terminal.

Alternatively, the [MySQL Workbench](https://www.mysql.com/products/workbench/) can be used to interact with a MySQL server (local or remote) via a GUI.
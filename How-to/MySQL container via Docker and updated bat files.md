# READ ME FIRST
These instructions will set up a mySQL server in a Docker container for your web application to connect at (by default)

# Starting and preparing Docker
In your cmd.exe
* docker-machine start
* docker-machine env (you should see DOCKER_HOST=tcp://192.168.99.100:2376 among other details)
* cd C:\docker-image-files (change directory to where you store a bunch of .bat)
* docker-machine env > docker-settings.bat
* docker-settings.bat (to apply settings given by docker-machine env command)
* docker ps -a (Check running Docker containers, should have none)
* load-and-start-mysql.bat
* docker exec -it mysql-populated bash

# Within BASH (you should see "root@someAlphanumeric" on the left)
* mysql -u root --password=****************askDan

# Within mySQL (you should see "mysql>" on the left)
* show databases;
* use db_grad_cs_1917
* show tables;
* Now you can write SQL queries 

# To connect to mySQL database within the server within the container via mySQL Workbench
* Launch mySQL Workbench
* Add new connection
* Input random name, ip and port as your Docker's (default: 192.168.99.100 port 3306)
* Input username and password
* Test Connection TADA!
* Double click the new connection, select database db_grad_cs_1917 by double clicking it
* Write your query (e.g. select * from users;)
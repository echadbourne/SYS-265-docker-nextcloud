# Docker Compose Nextcloud with MySQL database

This is a project for setting up a Nextcloud container that uses a MYSQL container as a database. The .yaml file maps port 80 for Nextcloud to port 8080 for the localhost.

Use `git clone https://echadbourne/SYS-265-docker-nextcloud` to easily clone the docker-compose.yaml file. Install git if needed.

Deploy this setup with docker compose, navigate to the folder the .yaml file is in and run the command `docker compose up -d`
 - This will start the download and execution for the containers in the background of the localhost

Once the containers are running you should be able to navigate to http://hostname:8080 to make an admin account. I found that after making an admin account I still needed to log into Nextcloud with default username and password "nextcloud" and "nextcloud"
 - Because the default username and password are simple and default, **Make sure to change this when you set it up!**

To shut down nextcloud, use `docker compose down` in the folder that contains the .yaml file

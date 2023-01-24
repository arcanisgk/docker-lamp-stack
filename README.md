# Docker Lamp Stack:
 Base docker architecture for the LAMP stack with entry point in public.

## READ all the Readme!!!

### Preparation for docker:

you need to have installed docker/docker desktop and version WSL2.0

### Installation of this setup:

1. Download or clone to where you want your project to be.
2. You should not put this in folders associated with Google Drive or One Drive this causes errors.
3. Navigate in the directories and go to app->Assets->docker/
4. Find the .env file, which you will open with your IDE or Reference Code Editor.
5. At this point, in the .env file at the end you will find the environment variables that you must edit to your liking:

```.dotenv
COMPOSE_PROJECT_NAME=YourProjectName
WEB_MASTER=yourcontacemail@email.com

#Database Default Access and Names
MYSQL_DATABASE=database-name
MYSQL_USER=database-user
MYSQL_ROOT_PASSWORD=database-root-password
MYSQL_PASSWORD=database-user-password

#Ports
HOST_MACHINE_UNSECURE_HOST_PORT=80
HOST_MACHINE_MYSQL_PORT=3306
HOST_MACHINE_PMA_PORT=81

#php Version referenced to bin/{php-version} can setup php74 or php81
PHPVERSION=php81
```

6. Once the variables have been edited, go to the root directory of your project, in this example case:

```
PS D:\Desarrollos\Personales\docker\docker-lamp-stack>:
```

7. run the installation command:

```
docker-compose up -d
```

Note 1: mysql data persistence (database) is physically located in: app->Assets->docker->data

Note 2: Installation takes several minutes; It is important that if you do not know how to use docker ... preferably you do it with a clean installation and that you have eliminated any installation remnants.

### Contributing:

Thank you for considering contributing to the Docker Lamp Stack project! The contribution guide can be found in the Docker Lamp Stack documentation.

### Security Vulnerabilities
If you discover a security vulnerability within Docker Lamp Stack, please create issue and please contact the author and/or security team instead.

## License

The Docker Lamp Stack project is open-source software licensed under the MIT license.


### Contributors
- (c) 2020 Walter Francisco Núñez Cruz icarosnet@gmail.com 

[![Donate](https://img.shields.io/static/v1?label=Donate&message=PayPal.me/wnunez86&color=brightgreen)](https://www.paypal.me/wnunez86/4.99USD)
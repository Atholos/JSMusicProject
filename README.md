**Music Upload Web Site Project**


**Authors**
```
Arttu Jokinen
Joachim Grotenfelt 
Markus Saronsalo
```
This Project is made for the Basic Concepts of Web Technology course, updated in 15/05/2019, and is currently running and can be accessed from [10.114.32.39/app/](http://10.114.32.39/app/).
**NOTE**: App can be only accessed from Metropolia UAC's intranet! You either have to be on site or use a vpn to connect to vpn.metropolia.fi. For this, you need student/teacher credentials!

**Built With**
```
JetBrains WebStorm, https://www.jetbrains.com/webstorm/ - Coding (CSS,HTML, JS)
PhpMyAdmin - SQL Database
ERDPlus, https://erdplus.com - Database ER model
CentOS7, https://www.centos.org/ - Used for Apache webserver and Node
```

**How To Use**

App usage is straightforward. 
1. You can view items without an user account.
2. To upload, you must register and login. 
3. To like images, you have to be logged in. The number inside the heart icon shows you the amount of likes.
4. While logged in, you can delete your own images.

**How to Deploy**
 1. Download this project to your machine.
 2. Unpack the ZIP-file.
 3. with node, run ```NPM install package.json```. This will get you all of the required dependencies. 
 4. You need an SQL database for the app to run properly. The database structure is in the musicproject.sql file.
    - Also a .env-file needs to be set up with the following content:
    ```
       DB_HOST: "host address for the database here" E.g. DB_HOST=localhost for localhost usage
       
       DB_USER: "database username here"
       
       DB_NAME: "database name here"
       
       DB_PASS: "database password here"
       ```
       
 5. After configuring the database and running the app, for example with nodemon, the app should work using your browser with the address: ```localhost:3000```

**DISCLAIMER**

Some of the features are still unimplemented, for example updating user information does not work in the current build even though it is included and accessible in the page structure.

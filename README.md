CellitWeb

=======================
![logo](https://user-images.githubusercontent.com/4268634/37671312-127709d0-2c31-11e8-8626-f4ff7bdc5ade.png)

Introduction
------------
Web application for the mobile device trade-in process

You will need to download and install:
------------
- node
- web server, like xampp
- SQL Server
- cellit.rar, download from here http://189.212.132.188/downloads/
- cellitDB.rar, download from here http://189.212.132.188/downloads/

Installation Windows
------------
- Restore the downloaded database (cellit.bak) in SQL Server

- Clone: git clone https://github.com/airsoftware-mx/cellit.git inside the "htdocs" folder. (Path: C:\xampp\htdocs)
- After unzipping cellit.rar you must copy folder "vendor" and paste inside your cloned project
- The same with the file "config.ini", you must obtain it from the previously unzippinp folder and paste in the following path of your "cellit" project: C:\xampp\htdocs\cellit_v3\config\autoload
- Open the config.ini file, change the parameters dev.cell.server, dev.cellit.user and dev.cellit.pass, corresponding to your instance in SQL Server.
- In a console, position yourself on the project path (C: \ xampp \ htdocs \ cellit_v3) and execute the following command:
`npm install`
- After it ends, execute the following command:
`grunt_build_dev`
- Open the application in a Web Browser
Possible Mistakes
------------
Xampp is missing the .dll to connect to SQL Server

![logo](https://user-images.githubusercontent.com/4268634/37671312-127709d0-2c31-11e8-8626-f4ff7bdc5ade.png)
# BgMobile
The BgMobile Web application is developed to work together with Pervacio Trade-In to manage the repurchase of mobile devices.
------------
## Getting Started
------------
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites
------------
- Git, download from here https://git-scm.com/download/win
- Node JS, download from here https://nodejs.org/en/download
- GruntJS, run your command shell as Administrator (for Windows) npm install -g grunt-cli.
- Web server. It can be xampp, that contains Apache and PHP 5.6. You could also install it separately.
- SQL Server 2012. Version 11.0.2. https://www.microsoft.com/en-US/download/details.aspx?id=29062
- cellit.rar, download from here http://189.212.132.188/downloads/
- Cellit Database. File .bak 

### Installing Windows
------------
- Restore the downloaded database (cellit.bak) in SQL Server
- Clone: git clone git clone -b dev-esr https://github.com/airsoftware-mx/cellit.git inside the "htdocs" folder. (Path: C:\xampp\htdocs)
- Change folder name cellit (cloned project) to cellit_v3
- After unzipping cellit.rar you must copy folder "vendor" and paste inside your cloned project
- The same with the file "config.ini", you must obtain it from the previously unzippinp folder and paste in the following path of your "cellit" project: C:\xampp\htdocs\cellit_v3\config\autoload
- Open the config.ini file, change the parameters dev.cell.server, dev.cellit.user and dev.cellit.pass, corresponding to your instance in SQL Server.
- In a console, position yourself on the project path (C: \ xampp \ htdocs \ cellit_v3) and execute the following command:
`npm install`
- After it ends, execute the following command:
`grunt dev`
- Open the application in a Web Browser, for example en Chrome access the link http://localhost/cellit_v3/
![website](https://user-images.githubusercontent.com/4268634/37685999-3d0c8b64-2c5b-11e8-8c52-1b6d9019c1f3.PNG)
------------
### Possible Mistakes
Xampp is missing the .dll to connect to SQL Server.
#### Solution
1. Download 3.2 of the SQLSRV drivers from here.
https://www.microsoft.com/en-us/download/details.aspx?id=20098
2. Do extract them to your "xampp installation path"\php\ext
3. Kindly ensure you see and keep the files : php_sqlsrv_56_ts.dll and php_pdo_sqlsrv_56_ts.dll
4. Restart your XAMPP server.



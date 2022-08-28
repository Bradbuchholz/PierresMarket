# Dr. Sillystringz's Factory
_By Brad Buchholz_
## Description

### _Dr. Sillystringz's Factory_
_You've been contracted by the factory of the famous Dr. Sillystringz to build an application to keep track of their machine repairs. You are to build an MVC web application to manage their engineers, and the machines they are licensed to fix. The factory manager should be able to add a list of engineers, a list of machines, and specify which engineers are licensed to repair which machines. There should be a many-to-many relationship between Engineers and Machines. An engineer can be licensed to repair (belong to) many machines (such as the Dreamweaver, the Bubblewrappinator, and the Laughbox) and a machine can have many engineers licensed to repair it._

## Technologies Used 
* C#
* dotnet
* .Net 5.0
* HTML
* CSS
* MYSQL
* Markdown   

## Setup / Installation 

1. Download and install **`dotnet 5.0`** on your computer. 
2. Clone the GitHub [repository](https://github.com/Bradbuchholz/Factory.Solution.git) onto your computer.
3. Make sure to have MySql Workbench installed on your computer.
4. Make sure to have dotnet-ef installed - this project uses **`version 5.0.1`**. I have it globally installed, but you can also install it just in this directory. 
5. Open the project in VScode or your terminal of choice. 
6. Create an `appsettings.json` file in the `Factory.Solution/Factory/` directory and add the following code, replacing anything in `square brackets` with the information it represents specific to the project database: 
```
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;database=[DATABASE-NAME-HERE];uid=[USER-ID-HERE];pwd=[YOUR-PASSWORD-HERE];"
  }
}


```
#### Example of complete appsettings.json
```
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;database=hair_salon;uid=Myusername;pwd=MySuperStrongPassword;"
  }
}
```
7. Open MySql Workbench and login to your server.
8. From your terminal navigate to the `Factory` folder and run the command **`dotnet ef database update`** to create the database from migrations.
9. Next use the command **`dotnet run`** in your terminal to launch the program.
10. The site should be avaialbe at the local host listed in your terminal. 

## Known Bugs 
* Application currently has bare bones UI, could use custom styling. 
## License
_Copyright (c) Brad Buchholz_
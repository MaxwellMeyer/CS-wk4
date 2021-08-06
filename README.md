# Factory

#### Written by Maxwell Meyer

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## Description

An MVC web app for a fictional factory built to demonstrate the application of a many-to-many relationship in a MySQL database. The app can store both Engineers and Machines, and the user can view a list of both, as well as their various shared attributes. Built utilizing code-first migrations via the MS Entity Framework.

## Applied Technologies

This project was built using:

- C# 9.0
- ASP.NET 5.0(https://dotnet.microsoft.com/download/dotnet/5.0)
- ASP.NET MVC
- MySQL and MySQL Workbench
  _ Razor
  _ Entity framework

### Instructions for Installing C# and .NET:

**1a.** _WINDOWS: Download the [64-bit .NET 5 SDK](https://dotnet.microsoft.com/download/dotnet/thank-you/sdk-5.0.102-windows-x64-installer). Clicking these links will prompt a **.exe** file download from Microsoft_.\
 \
 **1b.** MAC: Download this [.NET 5 SDK](https://dotnet.microsoft.com/download/dotnet/thank-you/sdk-5.0.100-macos-x64-installer). Clicking this link will prompt a **.pkg** file download from Microsoft.\
 \
 **2.** _Open the file and follow the steps provided by the installer for your OS_.\
 \
 **3.** _Confirm the installation is successful by opening a new Windows PowerShell OR Max Terminal window and running the command dotnet --version_.\

### Installation/Setup

1. View on Github

2. Alternatively, clone this repository to your computer and navigate to the cloned directory

3. Download MySQLWorkBench

4. Navigate to the `Factory` directory
5. Open with your preferred text editor
6. To setup a SQL database using MySQL:

   - Create an `appsettings.json` file in the `Factory` directory
   - Copy the text below and paste into the `appsettings.json` file, replacing `<password>` with your MySQL password:

   ```
     {
        "ConnectionStrings": {
           "DefaultConnection": "Server=localhost;Port=3306;database=maxwell_meyer;uid=root;pwd=<password>;"
         }
     }
   ```

   - Open your terminal and run the command: `mysql -uroot -p<mysql_password>` (replace `<mysql_password>` with your personal MySQL password) and hit enter to launch MySQL servers
   - Type the following commands to setup the database:
     - `CREATE DATABASE maxwell_meyer;` to make a new database
     - `USE maxwell_meyer;` to connect to the new database

7. In the Factory directory, run the terminal command `dotnet restore`

8. Now run `dotnet ef migrations add Initial` to build the Migrations Folder

9. Run `dotnet ef database update` to implement the database structure

10. Run `dotnet watch run` to run the application on your browser's local server at `http://localhost:5000`

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## License Information

You can find all applicable licensing information [here](https://opensource.org/licenses/MIT).

## Contact me!

Maxwell Meyer

maxreadswell@gmail.com

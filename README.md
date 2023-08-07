# Dr.Sillystringz Factory
### By _Alesandria Wild_
##### | Alesandria Wild               | [Github](https://github.com/ThatAltGirlAlesandria)| [LinkedIn](https://www.linkedin.com/in/alesandria-wild/)      |

## Technologies Used

* C#
* .NET-Core 2.2
* ASP.NET Core MVC
* Entity Framework Core
* MySql
* Visual Studio Code
* GitHub
* HTML
* CSS
* MDN Documents
* Dillinger.io
* learhowtoprogram.com
* Command Line

## Description

This web application was created to help Dr.Sillystringz make sure that there has been an engineer assigned to every machine in the factory, and vice versa. This project is meant to show my capabilities of utilizing many to many relationships with C# and migrations with git and SQL.

## Setup/Installation Requirements
* _Chrome web browser for best compatibility_
* _Have a prompt and editor to apply changes, like VSCode and GitBash_
 [Download here for VScode](https://code.visualstudio.com/download)
[Download here for GitBash](https://git-scm.com/downloads)
* _Installation of .Net 6.0 and C# for applied language_
[Download here](https://dotnet.microsoft.com/en-us/download/dotnet/6.0)
* _Afterword, download MySQL Server & Workbench_
[Download here](https://dev.mysql.com/downloads/mysql/)

## Step-by-step breakdown of how to download and run this program on your computer
* _Clone this repo by opening GitBash, and navigating to the location you wish to clone the repo to._
* _Navigate to the root directory of the project in the command line and run the following command_
```
$ git clone https://github.com/ThatAltGirlAlesandria/HairSalon.Solution.git
```
* _After cloning the repo in the location of your choice, set up your working environment by running_
```
$ dotnet build
```
* _Next create a .gitignore file in the root directory by typing the following into the command line_
```$ touch .gitignore``` 
* _Now, open your file in a text editor by typing in the command_
```
$ code .
```
* _Once your text editor launches, navigate to the .gitignore file and paste the following code and save the file_
```
obj
bin
appsettings.json
```
* _Now, open your command line again and make a commit. By making this commit BEFORE pushing to GitHub you will make sure the files that should be private/ not uploaded won't show. This is important because you don't want to share your username and password with everyone!_

#### Now that you have downloaded the repo and opened it in the text editor you need to open MySQL workbench.
* _Download [MySQL Workbench](https://www.mysql.com/downloads/) if you don't have it on your computer already_
* _After setting up your MySQL if you haven't done it already, in the Navigator make sure you are in the Administration Window_
* _Select Data Import/Restore from the menu_
* _In the Import Options pop-up window select, "Import from Self-Contained File"_
* _Navigate to the SQL file located in the root directory of the project you cloned called alesandria_wild.sql_
* _Under Default Schema to be Imported To, select the New Button_
* _Choose a name you would like for the database or continue to use alesandria_wild.sql if you're more comfortable with that_
* _Click OK_
* _You should see some tabs in the MySQL Workbench; navigate to the tab called "Import Progress" and click Start Import which is located in the bottom right corner of the tab_
* _Once you have finished the steps above locate the Schemas tab in the Navigator_
* _Right-click in the Schemas window of the Navigator and select Refresh All_
* _The database you just created should now appear in the Schema window_

#### Final steps, connecting your new database to the HairSalon program.
* _Open your command line application again_
* _Navigate to the production directory (should be called HairSalon)_
* _Open the text editor again using the same steps as above._
* _Now that you have opened the text editor again, you should see a new file listed called appsettings.json (we put this in the .gitignore file earlier)_
* _Open the file, and paste the following code_
```{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=[your_database];uid=[user-id];pwd=[password];"
  }
}
```
* _Replace [you_database] with the name of your database (alesandria_wild.sql)_
* _Replace [user-id] with your SQL username_
* _Replace [password] with your SQL password_
* _Lastly, in your command line type_
```
$ dotnet watch run
```
##### Your application is now up and running and should be visible to you in your browser! Congrats!

## Known Bugs

* None know currently.

## License

MIT Copyright 2023 Alesandria Wild

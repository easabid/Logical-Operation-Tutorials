CRUD - Logical Operations with C# and MSSQL
This repository contains all the CRUD (Create, Read, Update, Delete) logical operations built using C# with MSSQL as the database backend. The goal of this project is to demonstrate how to efficiently perform database operations using C# and SQL Server, covering all essential database interactions required for real-world applications.

🚀 Features
ADD – Insert new records into the database
Show – Retrieve data from the database and display it
Update – Modify existing records in the database
Edit – Make changes to data already added to the database
Delete – Remove records safely and securely
🛠️ Technologies Used
C# (for logic and UI)
MSSQL (Microsoft SQL Server) (for database management)
ADO.NET (for database connectivity and operations)


📥 Importing the .bacpac File
The .bacpac file for the database has been uploaded to this repository. You can import this file into your local SQL Server instance using the following steps:

|||||||  STEP BY STEP GUIDE  |||||||

Steps to Import the .bacpac File:
1. Download the .bacpac file
     Navigate to the repository where the .bacpac file is located.
     Download the file to your local machine.
2. Open SQL Server Management Studio (SSMS)
     Launch SQL Server Management Studio to work with SQL Server databases.

3. Import the .bacpac file
     In SSMS, right-click on Databases in the Object Explorer.
     Select Import Data-tier Application.
4. Follow the Import Wizard

     Click Next in the wizard.
     Select the Import from local disk option.
     Browse to the downloaded .bacpac file.
     Follow the prompts to import the database and assign it a name.

5.Update the Connection String in Your C# Project
     After importing the database, make sure to update the connection string in your C# project to reflect the newly restored database:

   SqlConnection conn = new SqlConnection(@"Data Source=MSI\SQLEXPRESS;Initial Catalog=""Crud Operation"";Integrated Security=True;");


6.Run the Project
     Once the connection string is properly set up, run the project to interact with the database and perform the CRUD operations.

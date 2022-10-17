# OnlineBloodBank

## Problem Statement
The ‘BLOOD BANK MANAGEMENT SYSTEM’ project is to interconnect all the blood banks, hospitals, donors into a single network, validation, store various data and information of blood of each individual. This system is used to store data over a centralized server which consists of database where the individual’s information cannot be accessed by a third party.
#### *Front-End Tool
**C#:** C# (pronounced "C-sharp") is an object-oriented programming language from Microsoft that aims to combine the computing power of C++ with the programming ease of Visual Basic. C# is based on C++ and contains features similar to those of Java. C# is designed to work with Microsoft's .Net platform.
#### *Back-End Tool
**Sqlite:** Sqlite is an in-process library that implements a self-contained, zero-configuration, server less, transactional SQL database engine. The source code for Sqlite exists in the public domain and is free for both private and commercial purposes.

## Connecting to a SQLITE database
Install-Package System.Data.SQLite -Version 3 
https://www.nuget.org/packages/System.Data.SQLite
```
using(SQLiteConnection con= new SQLiteConnection(@"Data Source=D:\test.db;"))
    {
        conn.Open();
        SQLiteCommand command = new SQLiteCommand("Select * from yourTable", conn);
        SQLiteDataReader reader = command.ExecuteReader();
        while (reader.Read())
        Console.WriteLine(reader["YourColumn"]);
        reader.Close();
    }
```
## Module Descrption
### *Login
In the login module there are two labels inside the textbooks namely email-id and password and an arrow button that leads the user to the next event searching page. The user has to enter the email-id and the password to login.
### *User Registration      
In user registration page user has to give the information to register to this database application. The information user has to give like name, phone number, address, email etc...,
### *Medical Institutes Registration
In medical institutes registration page medical institutes can register to this application for sharing blood related information and to search blood if it required. The medical institutes like blood banks or hospitals. 
### *Medical institutes details
In this page the user can see which medical institutes are register to this application and he can visit to nearby medical institutes and he can donate blood or he can receives blood if its emergency.
### *Donor details
In this module we can see the donor details of when he/she donates the blood and blood group and in which medical institutes the donated also we can get.
### *Orders details
Here we can get a details of orders like donation, receiving the blood and their prices with respective dates.
### *Stock details
Here in this module we can get in which medical institutes how much stock of blood is there.

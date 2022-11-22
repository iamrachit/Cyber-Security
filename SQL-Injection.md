# SQL Injection 

![image](https://user-images.githubusercontent.com/60937657/198902914-580df9a4-f051-4a21-a4ed-aeef2b2e94f7.png)

It is a code injection technique that might destroy database and it is one of the mose common web hacking techniques. SQL injcetion is the placement of malicious code in SQL statement, via web page input. SQL incjection usually occurs when you ask a user for input, like username and instead of the name the user gives a SQL statement that you will unknowingly run on your database. 

## Setup for SQL Injection 

**NOTE** We will use this repository for setting up - 

``` 
https://github.com/sakshamchoudhary/sql.git 
```

**Firstly we will install XAMPP** 

While intalling the xampp make sure it is not preinstalled and if that condition is fulfilled the we will got to below given link to intall the xampp. 

``` 
https://sourceforge.net/projects/xampp/
```

For Window;

``` 
https://sourceforge.net/projects/xampp/files/XAMPP%20Windows/5.5.19/xampp-win32-5.5.19-0-VC11-installer.exe/download
```

For Linux;

```
https://sourceforge.net/projects/xampp/files/XAMPP%20Linux/5.6.40/
```

## Understading the SQL and Major commands that can be used. 

SQL Stands for Structured Query Language, and the major command used in performing SQL Injection are given below;

Select : Used to select something or to retirieve the data form database 

Insert : Insert the value to database 

Update : To modify the data or to update the existing value 

Delete : Delete the value 

Order By : for sorting the columns

Schema : Schematic (Structure of database)

' : Sql value/commands which we want to check with database 

? : Query 

## Steps for performing SQL Injection 

1. Find the vulnerable link 

**inurl id= .com - can be used to find website**

We have brake the page by using " ' "

![image](https://user-images.githubusercontent.com/60937657/203272514-02d6327d-931e-4e8c-970b-ec3780bda1d1.png)

2. Join Query by using --+

**Next we will find how many number are there**

3. " Order By " Used to find the number of column 

![image](https://user-images.githubusercontent.com/60937657/203273611-ab5a2e1b-8266-48e9-b0a7-2fb09a182b3c.png)

![image](https://user-images.githubusercontent.com/60937657/203273683-a085cb7e-1722-4250-a938-8cdc7563ff09.png)

![image](https://user-images.githubusercontent.com/60937657/203292475-12cda540-ef5b-421c-be0a-861d580360d5.png)

As a result of above query we are getting 5 and 6 as a vulnerable columns 

![image](https://user-images.githubusercontent.com/60937657/203292614-0867c158-f3ec-4dde-b404-54ad0c19b35c.png)

While cracking the data;
We need to go throught Database -> Table -> Rows;


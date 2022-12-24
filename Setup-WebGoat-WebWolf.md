![image](https://user-images.githubusercontent.com/60937657/208461254-017f2bf1-ca45-44ea-ae43-28716fa355de.png)

# Setup WebGoat 

![image](https://user-images.githubusercontent.com/60937657/208536688-c44a1650-142d-4530-a881-956623a45537.png)

## Resourse used to setup WebGoat and WebWolf

- WebGoat github link - https://github.com/WebGoat/WebGoat
- Install Java JDK 17 :- https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html 

## Steps to setup WebGoat 

1. Install webgoat-server-8.2.2.jar and webwolf-8.2.2.jar from this link https://github.com/WebGoat/WebGoat/releases

![image](https://user-images.githubusercontent.com/60937657/208531683-a67c1219-28d8-4aaa-b5b4-0e384214ad12.png)

2. To setup WebGoat we need to setup java and to do that we need to intall java JDK 17 from the link given in resourse section. 

3. Transfer all the 3 files in the folder and name that folder as webgoat-prerequisites and then run jdk file. 

![image](https://user-images.githubusercontent.com/60937657/208532192-c273343c-307e-4f1d-ad07-72ae9ca25c94.png)

4. After setup java on the local machine open terminal and penetrate to webgoat-prerequisites 

To penetrate; use " cd + file location " 

![image](https://user-images.githubusercontent.com/60937657/208532682-48eeced7-2cd2-4e8f-9256-5be1a319bdf6.png)

After penetrating to webgoat-prerequisites file run the below given command to setup the webgoat. 

```
java -jar webgoat-server-8.2.2.jar
```

![image](https://user-images.githubusercontent.com/60937657/208534329-c2e6476d-b2c2-4991-9039-7635d529f88e.png)

5. Open browser and run ``` http://localhost:8080/WebGoat ``` 

Hooray ! WebGoat is running on the system. 

![image](https://user-images.githubusercontent.com/60937657/208524436-e7c31a3e-c397-4a40-9903-6c3e0dfa858c.png)

# Setup WebWolf 

![image](https://user-images.githubusercontent.com/60937657/209433363-1bdeeb47-d0e0-423f-9137-a6c512319f29.png)

# Steps to setup WebWolf 

1. After setup WebGoat on the local machine we can directly open the new terminal and penetrate to the file location where we have got the 3 files. 

![image](https://user-images.githubusercontent.com/60937657/209433521-85c8da1a-43f2-4ad9-abfa-31d9bef68a45.png)

To penetrate; use " cd + file location "

![image](https://user-images.githubusercontent.com/60937657/209433543-119bee09-7f0e-4fab-befb-b750febfc88a.png)

2. After penetrating to the file location, use the below given command to setup WebWolf on local machine. 

```java -Dfile.encoding=UTF-8 -Dwebwolf.port=9090 -jar webwolf-8.2.2.jar```

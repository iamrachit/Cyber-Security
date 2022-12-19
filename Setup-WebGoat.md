![image](https://user-images.githubusercontent.com/60937657/208461254-017f2bf1-ca45-44ea-ae43-28716fa355de.png)

# WebGoat 

![image](https://user-images.githubusercontent.com/60937657/208524436-e7c31a3e-c397-4a40-9903-6c3e0dfa858c.png)

## Resourse used to setup WebGoat

- WebGoat github link - https://github.com/WebGoat/WebGoat
- Install Java JDK 17 :- https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html 

## Steps to setup WebGoat 

1. Install webgoat-server-8.2.2.jar and webwolf-8.2.2.jar from this link https://github.com/WebGoat/WebGoat/releases

![image](https://user-images.githubusercontent.com/60937657/208531683-a67c1219-28d8-4aaa-b5b4-0e384214ad12.png)

2. To setup WebGoat we need to setup java and to do that we need to intall java JDK 17 from the link given in resourse section. 

3. Transfer all the 3 files in the folder and name that folder as webgoat-prerequisites and then run jdk file 

![image](https://user-images.githubusercontent.com/60937657/208532192-c273343c-307e-4f1d-ad07-72ae9ca25c94.png)

4. After setup java on the local machine open terminal and penetrate to webgoat-prerequisites 

To penetrate; use " cd + file location " 

![image](https://user-images.githubusercontent.com/60937657/208532682-48eeced7-2cd2-4e8f-9256-5be1a319bdf6.png)

After penetrating to webgoat-prerequisites file run the below given command to setup the webgoat 

```
java -jar webgoat-server-8.2.2.jar
```

![image](https://user-images.githubusercontent.com/60937657/208534329-c2e6476d-b2c2-4991-9039-7635d529f88e.png)

5. Open browser and run ``` http://localhost:8080/ ``` 

# XSS - Cross Site Scripting Attack 
This attack can also be called client side XSS

![image](https://user-images.githubusercontent.com/60937657/205972462-4843c529-a532-43b2-9a7a-59fa04f2729e.png)


## Short Notes

**1. DVWA is a predefined application with specific bulnerability and then we do practise on it but in the real scenario we have to keep few things in mind, firstly how the website is working and then we need to know which technology is being used to program that website.**

**2. XSS Payload is embedding of Java Script Code into HTML or PHP which share alert() or pop() widget which redirect to malicious/ fake page.** 

**3. "whatweb" command can be used in terminal to know about the technology used in the website for kali machine**

![image](https://user-images.githubusercontent.com/60937657/206000998-cc55130e-6bac-431e-8c58-002696f39cb7.png)

**4. When ever there is some input parameters like searchbox, login/sign up, subscription or contact form their is chance to find XSS attack (Reflected XSS).**

**5. Their are level of rating of vulnerability: Critical, High, Medium, Low and Informatiion Discoluser where Reflected XSS is a level low or medium vulnerability.**

## Performing XSS on DVWA 

1. Starting with low level of security in DVWA 

![image](https://user-images.githubusercontent.com/60937657/206422280-aaab1ab6-ce2f-4da8-a541-568b34868aaa.png)

While looking at view page source for the page, it is obsertved that in low security level the tags are not closed due to which we can enter code for performing XSS attack. 

![image](https://user-images.githubusercontent.com/60937657/206423194-5785210e-f909-4aae-9343-ac0a879315ae.png)

Understading the php code file by which we can see that there is no validation required. 

![image](https://user-images.githubusercontent.com/60937657/206423846-233fc949-ce16-469d-b0e8-a6f3172ed293.png)

So now we will add js code and try getting a pop up for the code 

```
<script>alert("hello")</script)
```

![image](https://user-images.githubusercontent.com/60937657/206425000-aa93c420-abd0-4e54-ac01-4d2cee5c5652.png)

2. Starting with the medium level of secuirty in DVWA 

![image](https://user-images.githubusercontent.com/60937657/206425544-2a422d5d-a7b5-469f-bdb0-b3d89b4f85f1.png)

By looking at the source code we can not see any major change as compared to low level of DVWA security level code used in reflect XSS attack. 

![image](https://user-images.githubusercontent.com/60937657/206426113-9af93e86-8d5d-4529-bd2d-cd3401f1e851.png)

![image](https://user-images.githubusercontent.com/60937657/206426263-4200f150-2c36-4178-b544-f36358c37e9a.png)

At php source code we can see there is a filter for script tag.

![image](https://user-images.githubusercontent.com/60937657/206426556-2829e5c3-74b3-4d58-9343-9a8e9e45685d.png)

For example if we add the same code like low level security level then we can not get script tag getting displayed because its been replaced. 

![image](https://user-images.githubusercontent.com/60937657/206427098-3ed1fea4-95f2-4b62-a3ff-6e556c7a6f81.png)

To bypass we need to serach for an another js function to find new approch to perform xss attack. 

```
<img src="x" onerror = alert("Hacking")>
```

![image](https://user-images.githubusercontent.com/60937657/206427882-b9232cf1-4adc-4e8a-b7da-806407d2a254.png)

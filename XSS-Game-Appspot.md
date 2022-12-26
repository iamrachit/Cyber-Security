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

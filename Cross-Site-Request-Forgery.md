# CSRF

![image](https://user-images.githubusercontent.com/60937657/199600106-b3421966-855d-40ae-a345-c38510e7f768.png)

## Cross Site Request Forgery

It is a web security vulnerability that allow the attacker to perform actions that they do not intend to perform by creating a forgery form with same link where the request is being placed in the server only in case when the requested token for a request are not being authenticated by the server. mainly forgery form can be created for static functionality available on the webiste like changing the password, deleting an account and etc. 

## Who is this working ?

1. We develop and exploit URL or script. 
2. Trick the victim with auto submission using javascript methodology. 

## Steps for performing this attack mannualy. 

1. Starting with DVWA 

Firstly open DVWA and change the security level to low and then going to CSRF for performing that attack. 

![image](https://user-images.githubusercontent.com/60937657/196027768-cee5d3d6-65d4-4cf0-9801-7a023685071a.png)

2. Clone the form 

Then clone the form and to do that we need right click in new password section in the form and then select inspect. 

![image](https://user-images.githubusercontent.com/60937657/196027973-e7c93ae1-fc44-4489-b810-1275cd9b90b5.png)

![image](https://user-images.githubusercontent.com/60937657/196028018-fba65eb1-cd3e-4c01-b404-61dde42bcf02.png)

3. Edit as html the entire form by right click the form action code line. 

![image](https://user-images.githubusercontent.com/60937657/196028127-ed407e19-3421-4150-8fd6-bb55dac3db8b.png)

Copy the entire code and paste in the text editor.

![image](https://user-images.githubusercontent.com/60937657/196028206-f7e78805-f78f-4875-a0db-92a835ef1352.png)

![image](https://user-images.githubusercontent.com/60937657/196028267-c21710d4-26c1-41a1-b3f6-630d44b6de4b.png)

Save the file in text editor with .html extension. 

4. Go back to DVWA and open CSRF 

Enter new password and confirm new password again and then click on the change button after it shows that password is change then copy the URL form the serch bar at the top. 

![image](https://user-images.githubusercontent.com/60937657/196028488-cbcb5fec-554b-44e8-b42a-2d771bc44a62.png)

5. Paste that URL to html folder where the form related code is saved. 

**note** The URL will be saved under the action variable as shown in the image below. 

![image](https://user-images.githubusercontent.com/60937657/196028578-7986a85e-1a7f-4d68-9039-5a09ce6f967e.png)

![image](https://user-images.githubusercontent.com/60937657/196028603-e8e88050-b61f-4135-ac95-fb6e416ae106.png)

URL till the directory location is only required other information in URL should be deleted. 

![image](https://user-images.githubusercontent.com/60937657/196028654-c3469462-a91e-4e96-8d0f-55a52237b6f1.png)

6. Save the file and drop it the browser to open it. Then change the password to check proper working of that HTML file. 

![image](https://user-images.githubusercontent.com/60937657/196028768-83c853f8-155e-4027-9434-2d0103a52328.png)

After your password is change you can then do some manuplation in the HTML file for directly changing the password without even actually showing anything and auto submitting the password. 

![image](https://user-images.githubusercontent.com/60937657/196031447-d6368feb-f21e-45f3-9e61-668b5eda53fb.png)

## Preventing CSRF attacks

The most robust way to defend against CSRF attacks is to include a CSRF token within relevant requests. The token should be:

1. Unpredictable with high entropy, as for session tokens in general.

2. Tied to the user's session.

3. Strictly validated in every case before the relevant action is executed.












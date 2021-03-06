# RBUCKET AUTH PACKAGE DOC

## Registration API

> This **API** contains the registration of the user 

> **POST :** https://harsh-auth-docker.herokuapp.com

> **Fields For Request are**
- **name :** Name of the user for registration
- **email :** It contains the email of the user
- **password :** password should be strong and should contains the ALPHANUMERIC characters
- **age :**  Age of the user 

> **Fields For Response are**
- **msg :** Response message after registration
- **User :** Contains the user info with activation code and many others fields etc

> **User** Contains the value illustrated below
- **role :** check wether the given user is admin or not
- **isVerified :** check whether email is verified or not **when isVerified is TRUE then email is verified and the activation token becomes empty and ViceVersa**
- **id :** User ID
- **name**
- **email**
- **age**
- **activationToken :** it's a verfication token 

 > **API DOMAIN or ADDRESS :  https://harsh-auth-docker.herokuapp.com**
 
 > **Email should not be same for registration**
 
 > when the verification Token or activationToken becomes empty then the email is verified and if it is not empty then email is not verified yet **to check the      email verifiaction check mail also**
 
 

## Login API

> This **API** contains the login of the user 

> **POST :** https://harsh-auth-docker.herokuapp.com/login

> **Fields For Request are**
- **email :** It contains the email of the user
- **password :** password should be strong and should contains the ALPHANUMERIC characters

> **Fields For Response are**
- **msg :** Response message after registration
- **User**

> **User** Contains the value illustrated below
- **role**
- **isVerified** 
- **id**
- **name**
- **email**
- **age**
- **activationToken**

 > **API DOMAIN or ADDRESS :  https://harsh-auth-docker.herokuapp.com/login**
 
 

## Resend API

> This API sends the activation link for email verification

> **POST :** https://harsh-auth-docker.herokuapp.com/resend

> **Fields For Request are**
- **email :** email for verification

> **Fields For Response are**
- **msg :** Response message

> **API DOMAIN or ADDRESS :  https://harsh-auth-docker.herokuapp.com/resend**

## Logout API

> This API is for logging out

> **POST :** https://harsh-auth-docker.herokuapp.com/logout

> **NO FIELDS FOR REQUEST**

> **RESPONSE :** It returns the String as a response

> **API DOMAIN or ADDRESS :  https://harsh-auth-docker.herokuapp.com/logout**

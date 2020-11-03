# RBUCKET AUTH PACKAGE DOC

## Registration API
This **API** contains the registration of the user 
**it has 2 methods**
**POST**
**GET**

**Fields For Request are**
**role :** it decides whether the given user is ADMIN or a USER
**name :** Name of the user for registration
**email :** It contains the email of the user
**password :** password should be strong and should contains the ALPHANUMERIC characters
**age :**  Age of the user 

**Fields For Response are**
**message :**
**status_code :**
**code :**
**isverified :** check for mail verification
**isemail :** check whether the email enter is already registered

### API DOMAIN or ADDRESS :  https://harsh-auth-docker.herokuapp.com

/login to login the users.

/resend to resend the link

/logout to logout the users.

/cook is the authenticated api

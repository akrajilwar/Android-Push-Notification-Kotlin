# Android Push Notification (Kotlin)
Create firebase project and add google_services.json to <b>Project/app</b> folder

## Postman:
Step 1. Set request method to <b>POST</b>  
Step 2. Set url `<i>https://fcm.googleapis.com/v1/projects/tik-tok-189ca/messages:send</i>`  
Step 3. Add Headers:  
<pre>Content-Type : application/json  
Authorization : Bearer <access-token>
</pre>  
Step 4. Add Body:  
<pre>{  
    "message": {  
        "token": "<Device Token>",  
        "notification": {  
            "body": "This is an FCM notification message!",  
            "title": "FCM Message"  
        },  
        "data": {  
            "message": "This is test message"  
        },  
        "android": {  
            "direct_boot_ok": true  
        }  
    }  
}</pre>  

Learn More  
[https://www.androidlearning.com/](https://www.androidlearning.com/)

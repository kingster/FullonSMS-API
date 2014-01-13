FullonSMS PHP API
=============

Send SMS Via FullonSMS from PHP.  

<del>Tested Working with FullonSMS. Supports upto 140 Characters</del> FullOnSms has added captcha verification for login, hence I will need to figure out something to bypass that. Feel free to send pull request for the same!


How to
-------
```php
<?php
    include('fullonsms-api.php');
    sendFullonSMS ( '9000012345' , 'password' , '987654321' , 'Hello World');   
    sendFullonSMS ( '9000012345' , 'password' , '987654321,9876501234' , 'Hello World');   
?>
```


GET/POST API
------------

Send SMS just making GET or POST Requests.

Incase u want to use the service from your application then the parameters for ur application would be

```
http://www.yourdomain.com/sendsms.php?uid=LOGIN_ID&pwd=PASSWORD&phone=XXXXXXXXX,YYYYYYYYY&msg=Hello+World

Parameters
uid = LOGIN_ID ( Your Login ID [either nickname or 10 Digit mobile no] )
pwd = PASSWORD ( Your Login Password )
phone = 10 Digit Mobile number. Incase of multiple numbers then numbers separated by comma (,)
msg = Your Message.
```


Note
-------
Please use this code on your own risk. The author is no way responsible for the outcome arising out of this.

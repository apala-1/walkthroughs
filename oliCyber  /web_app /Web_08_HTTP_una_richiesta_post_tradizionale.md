# URL
https://training.olicyber.it/challenges#challenge-347

# Concept
Here, we try to send post requests to a webpage to try and gain access to certain things / get desired output.

# Method
* The challenge asked us to send a POST request to this endpoint: http://web-08.challs.olicyber.it/login.
* We used curl and sent the username and password along with the mimeType.
* We used -X to send the username and password with values admin and admin.
* Then, we used -H to send the mimetype as ContentType= application/x-www-form-urlencoded

This is the entire curl code that we used:
```
curl.exe -H "Content-Type: application/x-www-form-urlencoded" 
         -X POST -d "username=admin&password=admin" 
         -v  http://web-08.challs.olicyber.it/login http://web-08.challs.olicyber.it/login
```

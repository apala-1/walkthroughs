# URL
https://training.olicyber.it/challenges#challenge-348

# Concept
We are supposed to send information to this URL:
http://web-09.challs.olicyber.it/login

But then using JSON to send the information in a POST request to solve the challenge.

# Method
We tried this first:
```
curl -X POST 
     -H "Content-Type: application/json" 
     -d '{"username": "admin","password": "admin"}' 
     -v http://web-09.challs.olicyber.it/login
```
But it gives an error: 

<!doctype html>
<html lang=en>
<title>400 Bad Request</title>
<h1>Bad Request</h1>
<p>The browser (or proxy) sent a request that this server could not understand.</p>
* Connection #0 to host web-09.challs.olicyber.it left intact

I couldnot figure out how to fix the above error.
So, we try python instead.

Opened powershell and used 
`python`

then we code:
```
import requests
url = "http://web-09.challs.olicyber.it/login"
data = '{"username": "admin", "password": "admin"'}'

r = requests.post(url=url, json=data)
print(r.text)
```

And we got our flag.

# URL
https://training.olicyber.it/challenges#challenge-349

# Concept
We were supposed to use the methods that were not in the Options as sometimes, it is possible that
the website crashes if not coded properly.

# Method
We used this code:
```
curl.exe -X POST -H "Content-Type: application/json"
         -u '{"username": "admin", "password": "admin"}'
         -v "http://web-10.challs.olicyber.it/"
```
and got the flag.

We are **allowed** to use other methods like `GET`, `HEAD`, `OPTIONS`,
But we used the ones that were not allowed.

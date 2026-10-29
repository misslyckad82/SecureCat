# **SecureCat** 



## Goal
This projects aim is to make a secure password generator. <br>
Passwords which cannot easily be typed (hence, decreasing the likelihood of social engineering(SE)[Note1]. <br>
The objective is to let the user get a secure password Which is controlled trough [Have-I-Been-Pwned?](https://haveibeenpwned.com/) & other well-known data leaks. <br>

## Function
This script makes a random 15-char password (incl. numbers, big and small chars) and others. <br>
The user is asked if the password is okay if the first password isn't.<br>
The user can thereafter choose to save the Password in a file. (Called a Cryptographic key-file) locally(on their own system). The file exists in same directory as `SecureCat.py`. <br>

## Future Improvements
 - Offline
 - Hash the Key file first. (It's not safe to just store a un-encrypted file[Note2])
 - Alternatively, save the password inside a external Password Manager
 - The user shall be able to feed in their own password and get a check trough the "Have I been Pwnd" site to see if its leaked<br>
   The password shall adhere to standards to be secure
 - Check the passwords against well-known pass-lists, like the `Rockyou.txt` list and many more

## Systemkrav
Python-scriptet works in the following environments:  <br>
 - Linux  <br>
 - Windows  <br>
 - Mac OS  <br>

## Instructions for execution
- Clone repot: `git https://github.com/misslyckad82/SecureCat.git` <br>
- Execute `SecureCat.py` in your terminal <br>

#### Powershell: <br>
- `cd <insert the path to SecureCat.py>` <br>
- `python SecureCat.py` <br>

#### Linux:  <br>
- `chmod +x SecureCat.py`
- `python3 SecureCat.py` <br>

#### Mac <br>
- `python3 SecureCat.py`

## Video <br>
- [At Youtube](https://youtu.be/UTZUxXx-QUo)


_____ 
##### Foot Notes
1. No password is inherently "social engineering" safe
2. We dont encrypt passwords in cryptography or infosec. The consensus of infosec is to Hash those. You encrypt the data using a hashed version of a password(such as, a keyfile)

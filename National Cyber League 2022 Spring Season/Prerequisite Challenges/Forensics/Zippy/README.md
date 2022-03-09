# Zippy (100 Points)
## We found this suspiciously named zip file, but it seems to be password protected. Can you get in?
<img width="372" src="https://user-images.githubusercontent.com/99063625/157494438-c7bbff80-b706-402d-9219-85d103f9c874.png">

# Walkthrough

For this challenge, I turned to the password-cracking tool, [john](https://www.kali.org/tools/john/), and the famous wordlist, [rockyou.txt](https://github.com/danielmiessler/SecLists/blob/master/Passwords/Leaked-Databases/rockyou.txt.tar.gz). With a wordlist, our password-cracking tool can make millions of satisfactory guesses for the zip file's password. 

![image](https://user-images.githubusercontent.com/99063625/157502077-a418dc3e-b994-4943-8129-7136b4046b24.png)

```sudo zip2john secrets.zip > hash-to-crack.txt ``` Generates a password hash for the zip file and outputs the hash to hash-to-crack.txt.
```cat hash-to-crack.txt``` Reads the content of newly created text file that contains the password hash.
```sudo john --format=zip hash-to-crack.txt --wordlist=/usr/share/wordlists/rockyou.txt``` Cracks the hash by utilizing passwords in the rockyou wordlist.

The john tool discovers the password for the zip file is ```aggies08```.

![image](https://user-images.githubusercontent.com/99063625/157504697-7a27fc40-7d15-4126-bf6f-b5279261c868.png)

![image](https://user-images.githubusercontent.com/99063625/157504789-50a9c3c1-f768-496b-80a4-8232f32e0689.png)

### The flag is: ```gigem{us3_b3tt3r_p4ssw0rd5}```

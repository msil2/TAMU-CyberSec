# Secret Number (100 Points)

## Can you find the secret number? http://ctf.cybr.club/secretnumber/.

<img width="372" alt="Screenshot 2022-02-05 011455" src="https://user-images.githubusercontent.com/99063625/152632596-cbe28853-5b55-4e3b-bd05-f2c4e94f0159.png">

# Walkthrough

For this web exploitation challenge, we are given a form that will only reveal the flag if we submit the correct "Secret Number."

![image](https://user-images.githubusercontent.com/99063625/152632729-edfac359-99f6-40ee-b838-9a93dd68b468.png)

Noticing a pattern, deduce what some other, unlisted options may be.

<img width="602" alt="Screenshot 2022-02-05 011643" src="https://user-images.githubusercontent.com/99063625/152632628-4cd8f82c-8ff3-4e7f-b625-2c24caf5bc6c.png">

*Inspect* the site for ways to submit potential answers that are currenlty unselectable.

<img width="428" alt="Screenshot 2022-02-05 012637" src="https://user-images.githubusercontent.com/99063625/152632876-83582361-a35f-455b-a2f9-fca8496067d6.png">

Submit the secret number for the flag.

![image](https://user-images.githubusercontent.com/99063625/157760816-d635e39e-2249-449a-831b-68c99a19cb48.png)

### The flag is: ```gigem{TraingleNumSeqNotSoSecret}```

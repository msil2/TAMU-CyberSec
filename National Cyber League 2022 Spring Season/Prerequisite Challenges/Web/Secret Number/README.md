# Secret Number (100 Points)

## Can you find the secret number? http://ctf.cybr.club/secretnumber/.

<img width="372" alt="Screenshot 2022-02-05 011455" src="https://user-images.githubusercontent.com/99063625/152632596-cbe28853-5b55-4e3b-bd05-f2c4e94f0159.png">

# Walkthrough

For this web exploitation challenge, we are given a form that will only reveal the flag if we submit the correct "Secret Number." With web exploit challenges, it never hurts to see if the flag is hidden in plain sight, already on the page. One way we can do this is by trying to highlight the entire page, in case the webmaster put some white text on a white background, or something like that. Still taking the page at face value, we might want to try if any of the numbers on the dropdown list actually end up working.  

![image](https://user-images.githubusercontent.com/99063625/157762040-61966942-2c75-4999-a5a1-7b1f69b124a0.png)

Though, you probably already guessed that this does not work. *However*, take notice that, after submitting a number from the dropdown list, the web address in your browser's URL bar updates to include "index.php." Websites that use PHP are delicious for hackers, so feel motivated to poke around a bit more!

<img width="602" alt="Screenshot 2022-02-05 011643" src="https://user-images.githubusercontent.com/99063625/152632628-4cd8f82c-8ff3-4e7f-b625-2c24caf5bc6c.png">

One thing I noticed after digging deeper is that the numbers listed in the dropdown menu follow a pattern: N1 + 2 = N2 (1 + 2 = 3), N2 + 3 = N3 (3 + 3 = 6), N3 + 4 = N4 (6 + 4 = 10), etc. Maybe following this pattern will lead us to the secret number? Maybe, but that doesn't matter until we can figure out how to submit any number we'd like to!

*Inspect* the site for ways to submit potential answers that are currenlty unselectable.

<img width="428" alt="Screenshot 2022-02-05 012637" src="https://user-images.githubusercontent.com/99063625/152632876-83582361-a35f-455b-a2f9-fca8496067d6.png">

Submit the secret number for the flag.

![image](https://user-images.githubusercontent.com/99063625/157760816-d635e39e-2249-449a-831b-68c99a19cb48.png)

### The flag is: ```gigem{TraingleNumSeqNotSoSecret}```

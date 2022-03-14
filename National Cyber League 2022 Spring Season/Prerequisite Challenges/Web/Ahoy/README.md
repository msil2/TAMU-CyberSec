# Ahoy (100 Points)
## Chips Ahoy! Everything you need is located on the webpage (http://ctf.cybr.club/ahoy/).

<img width="372" src=https://user-images.githubusercontent.com/99063625/158117541-99c531c7-88a9-445a-a13f-cb531de7728f.png>

# Walkthrough

The mention of "[Chips Ahoy!](https://www.snackworks.com/brands/chips-ahoy?Brand=CHIPS%20AHOY!)," a brand of cookies, immediately stands out. Referencing cookies in a web exploitation challenge can mean only one thing: this challenge involves manipulating web cookies. What we're about to learn is that cookies in the browser can be edited. Let's visit the site. 

![image](https://user-images.githubusercontent.com/99063625/158129840-618e8bf7-36be-4f7e-bcf9-d2dbf73739fc.png)

Immediately, the site tells us two things: we have to decode some Base64, and the web server has assigned certain permissions to our user. 

![image](https://user-images.githubusercontent.com/99063625/158131196-206cc3c8-79b0-4fed-89dc-35e3c6cf2f16.png)

Decoding the Base64 reveals what the site is really trying to tell us: our user has not been granted administrator privileges. If the cookie is storing these settings/permissions, then we should try to modify our user. [Firefox](https://www.mozilla.org/en-US/firefox/products/) keeps its *Cookies* under the [*Storage* Inspector](https://developer.mozilla.org/en-US/docs/Tools/Storage_Inspector). Sure enough, we see that ther is a "user" item in our *Cookies*, with current value, "string". 
 
![image](https://user-images.githubusercontent.com/99063625/158132758-6ce61e3c-e8ab-4f70-b1ac-5573a009f103.png)

We also see that this cookie is modifiable, or can accept any string as its value.

![image](https://user-images.githubusercontent.com/99063625/158134110-a82448a1-7f04-4505-8afc-eb66ed8f42f4.png)

After pressing *Enter* on our keyboard and refreshing the page, the site will now greet its newly recognized administrator with the flag.

![image](https://user-images.githubusercontent.com/99063625/158134449-dcc433fd-c43a-42bf-8372-9c5a7b50830a.png)

### The flag is ```gigem{c00kiesC00kiesYummyYum}```.

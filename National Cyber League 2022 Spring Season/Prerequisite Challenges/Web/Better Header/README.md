# Better Header (100 Points)
## Can you find the flag by visiting this webpage http://ctf.cybr.club/betterheader/?

![image](https://user-images.githubusercontent.com/99063625/158115052-04516aa6-3efc-40e6-ad78-b58d535ae574.png)

# Walkthrough

The title of the challenge seems to clue us in on the scope of the challenge: web headers. This means that a good place to start looking is our browser's [*Network Monitor*](https://developer.mozilla.org/en-US/docs/Tools/Network_Monitor) (I use Firefox, so I have linked to Mozilla's documentation). By examing the HTTP requests our browser has made for this site, we can take a look at some *Headers*.

![image](https://user-images.githubusercontent.com/99063625/158116254-c7c4d821-07e0-4091-9d02-dd055f66cf79.png)

### The flag is ```gigem{f0undH3ad3rFl4g}```.

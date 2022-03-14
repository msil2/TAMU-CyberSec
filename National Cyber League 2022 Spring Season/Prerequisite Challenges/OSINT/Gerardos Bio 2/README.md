# Gerardos Bio 2 (100 Points)
## Gerardo recently started using [Twitter](https://twitter.com/gerardo_2001_), but he hasn't filled out his bio yet. He's recently gotten into astrology and wants to include his Mars sign in his bio. Can you help him out?

## The flag is in the format of gigem{sign_degrees_minutes_seconds}

## Example: Aquarius 8°00'44" is gigem{aquarius_8_00_44}

<img width="372" src=https://user-images.githubusercontent.com/99063625/158137190-bd46f69e-4a15-4e06-900d-3a18be95cb89.png>

# Walkthrough

[A previous challenge](https://github.com/mrubensilva/TAMU-CyberSec/tree/main/National%20Cyber%20League%202022%20Spring%20Season/Prerequisite%20Challenges/OSINT/Gerardos%20Bio%201#the-flag-is-gigem12232001) revealed that Gerardo's birthday was December 23rd, 2001. Unfortunately, if you want to figure out somebody's [Mars sign](https://cafeastrology.com/whats-my-mars-sign.html), you need more than just their birthday. 

<img width="600" src=https://user-images.githubusercontent.com/99063625/158138505-18ca4d32-5381-44c9-94e9-0dd5cefc8f2c.png>

In fact, we need to comb through Gerardo's Twitter (linked in the challenge prompt) for leads on his time of birth and his birth city. We can find Gerardo's time of birth pretty easily, as [one tweet](https://twitter.com/gerardo_2001_/status/1477823900591529984?s=20&t=DTlIkvduuX6ic-NFX0V_BA) spells it out for us.

![image](https://user-images.githubusercontent.com/99063625/158139359-054a07ba-ffaf-49e4-a907-51e3279fd448.png)

Gerardo was born at 8:00am.

To find the last piece of the puzzle, Gerardo's birth city, we look to [one other tweet](https://twitter.com/gerardo_2001_/status/1481405190267981831?s=20&t=DTlIkvduuX6ic-NFX0V_BA), in which Gerardo muses about his home.

![image](https://user-images.githubusercontent.com/99063625/158140560-737a41db-6648-4086-8070-d1a5eb924eb2.png)

If the city pictured in this tweet is Gerardo's birth city, then we are all set, because we can easily use this image to conduct a [Reverse Image Search](https://support.google.com/websearch/answer/1325808?hl=en&co=GENIE.Platform%3DDesktop) (Powered by Google).

![image](https://user-images.githubusercontent.com/99063625/158141367-069bce2c-587e-499e-8cf0-732907b1bf83.png)

We figure out that Gerardo hails from San Antonio, Texas, United States.

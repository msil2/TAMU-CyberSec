
![image](https://user-images.githubusercontent.com/99063625/154577182-0efd7e7c-8b01-407c-ba35-59e51a9dd34b.png)

# DIRECTIONS:

1. Register an account at https://ctf.cybr.club/ with your TAMU email (this is important since we'll use this email to send your NCL voucher).

2. Start solving challenges! The target number of points required to complete the prereq is 500 points. Once you finish, request a voucher at https://forms.gle/XBEeVhFW41p5YtkN8.

3. If you have questions, ask anyone with the ncl-helper role. While we can't give you the solutions, we can give pointers on what to research, provided you've done your best to solve the challenge already.

# RULES:

1. Be nice to everyone → this is beginner friendly… keyword in every sense: FRIENDLY

2. Don't share or steal flags. An Aggie does not lie, cheat, or steal or tolerate those who do.

3. Blind brute force is never required. Never brute force flags; dirbuster or equivalent is not necessary; challenges which require repeated iterations will clearly offer you the ability to do so.

4. Don't attack the infrastructure. If you find a security vulnerability, please responsibly disclose that information to an officer.

# NOTE: For the pwn challenges and the oracle crypto challenge, you will need to connect to our server with the following script:

```
from pwn import *

context.log_level = "debug"
# change sni="whatever" to the challenge you want to connect to
io = remote("ctf.cybr.club", 443, ssl=True, sni="smash")

# this is just an example, put your actual exploit here
io.interactive()

# or, if you want to send stuff
io.sendline("haha funny")
# let's see if we got a line back
print(io.recvline())
```

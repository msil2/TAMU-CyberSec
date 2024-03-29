# Document (100 Points)

## I found this on the back of a famous US political document after putting some lemon juice on it. What does it mean, who put it there? What is the flag?

```Zi vse Gehxzr rj vse Lnbbsq Vxceej, ig Wfqhv vz ffrf i abui rprwevb Ialsp, pskautwfk Nwdtzcx, qbfxvg oodelbwp Wvcyqlieqhl, svqgiue ywf gki ezmdog lsshrep, piofwhr wlg reeekiz Jhphlrv, gbosz{F0rue1tlt10g_0n_hu3_Xr1v3o_Sk4t3l} ibq viefrv tam Pyhwutnxs hn Zveitey ko hcffhpxps rnw wie Ssueeiimg, rb rvflie agl sfwedwijh mpwf Fspdtztnbwbq jqc tye Nvwghh Ueakel wt Npittcr.```

<img width="372" alt="Screenshot 2022-02-05 004323" src="https://user-images.githubusercontent.com/99063625/152631872-d80ee86a-ef52-43be-9faf-dd799926a12b.png">

# Walkthrough

The challenge prompt references the greatest movie of all time, [National Treasure](https://en.wikipedia.org/wiki/National_Treasure_(film)), where masterful actor [Nicolas Cage](https://www.homestuck.com/story/darkcage) reveals a message hidden within the [Declaration of Independence](https://www.archives.gov/founding-docs/declaration-transcript).

![image](https://user-images.githubusercontent.com/99063625/152631865-c1a25c4e-6c17-4e9f-86a3-f36658b9f5ed.png)

Keeping that in mind, you can take a look at the ciphertext. You may notice that there is a part of the ciphertext that looks like it contains the flag, e.g, curly braces. Except, the characters are shifted around a whole bunch.

<img width="900" alt="Screenshot 2022-02-05 004925" src="https://user-images.githubusercontent.com/99063625/152631956-897b50d0-1819-42e0-9985-8d4dec8f7cf1.png">

*However*, after looking really closely, you might notice that this ciphertext actually doesn't resemble the Declaration of Independence all that much, even after considering it's a scrambled mess. Still, let's not drop this lead altogether. Personally, I think this particular order of characters looks a lot like *another* important historical document from US history: the United States Constitution, specifically, [The Preamble](https://constitutioncenter.org/interactive-constitution/preamble).

<img width="900" alt="Screenshot 2022-03-09 205601" src="https://user-images.githubusercontent.com/99063625/157580189-da2fb445-71ca-45e5-90c6-e969d403ec11.png">

It looks like every word has the right amount of letters, just not the correct letters, which tells us that we're probably working with a shift cipher. Additionally, we found ourselves a crib (a piece known plaintext), so we now have a better idea of what the cleartext (the unciphered text) is supposed to look like. One shift cipher that employes a crib is the [Vigenère cipher](https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher). As luck would have it, [CyberChef](https://gchq.github.io/CyberChef/) has a *Vigenère Decode* tool!

![image](https://user-images.githubusercontent.com/99063625/157744937-f735dae9-7f46-4965-b536-3bcad08304b7.png)

It turns out that this kind of cipher requires a key to decode it. At this point, our two clues are the Declaration of Independence and the Preamble to the United States Constitution. Since we are already using the Preamble as our crib, we might want to try using the Declaration as our key.

![image](https://user-images.githubusercontent.com/99063625/157757811-f5c8d6f1-e5fd-46b2-adea-65a719bcc227.png)

### The flag is: ```gigem{C0nst1tut10n_0f_th3_Un1t3d_St4t3s}```

# Encoding (100 Points)
## I found some mysterious text. Can you find out what it means? Note: for these challenges, https://gchq.github.io/CyberChef/ is your best friend (it's a website that allows you to mix and match encodings on the fly).

```01001110 01101010 01100011 01100111 01001110 01101010 01101011 01100111 01001110 01101010 01100011 01100111 01001110 01101010 01010101 01100111 01001110 01101101 01010001 01100111 01001110 00110010 01001001 01100111 01001101 01111010 01001101 01100111 01001110 01101101 01010101 01100111 01001110 01101010 01001101 01100111 01001101 01111010 01000001 01100111 01001110 01101010 01010001 01100111 01001101 01111010 01000101 01100111 01001110 01101101 01010101 01100111 01001110 01101010 01100011 01100111 01001110 01010111 01011001 01100111 01001101 01111010 01000101 01100111 01001101 01111010 01010101 01100111 01001110 01010111 01011001 01100111 01001110 01101101 01010101 01100111 01001101 01111010 01000001 01100111 01001110 01111010 01010001 01100111 01001110 01010111 01011001 01100111 01001101 01111010 01001101 01100111 01001110 01101101 01010101 01100111 01001110 01101010 01001101 01100111 01001110 01111010 01001001 01100111 01001110 01111010 01101011 01100111 01001110 01111010 01000001 01100111 01001110 01111010 01010001 01100111 01001101 01111010 01000101 01100111 01001101 01111010 01000001 01100111 01001110 01101101 01010101 01100111 01001110 00110010 01010001 00111101```

<img width="371" alt="Screenshot 2022-02-05 003135" src="https://user-images.githubusercontent.com/99063625/152631455-6dba1dc9-8c8e-442d-ac75-15c2b405244e.png">

Visit the provided website, [CyberChef](https://gchq.github.io/CyberChef/), to take a crack at decrypting the ciphertext. You may already know that this ciphertext is a bunch of binary numbers, so you should probably get started with the *From Binary* tool CyberChef.

![image](https://user-images.githubusercontent.com/99063625/157507060-ee7a60a4-670a-4a3b-a3f7-c0eac20e208a.png)

This output looks a lot like Base64. However, if you ever unsure, you can always hover over a given Operation in CyberChef to reveal some documentation and examples.

![image](https://user-images.githubusercontent.com/99063625/157507259-4f46a499-dd29-443d-ba5d-58126d65d1e1.png)

An additional *Operation* dragged into the *Recipe* area will get chained together with the preceding *Recipe* items, so dragging the *From Base64* tool into the *Recipe* area converts the output from the previous *Operation*, and not the initial binary *Input*. 

![image](https://user-images.githubusercontent.com/99063625/157575984-be12a0d8-a499-46a7-adc7-e4eec26cf28b.png)

Decoding *From Base64* gives us an output that looks like a hexadecimal byte string, so it makes sense to try to decode *From Hex*.

![image](https://user-images.githubusercontent.com/99063625/157576260-cf30deda-ceb7-4e58-ace7-9c26e89196f8.png)

### The flag is: ```gigem{3nc0d1ng_15_n0t_3ncrypt10n}``` 

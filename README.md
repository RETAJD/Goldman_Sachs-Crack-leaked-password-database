# Goldman_Sachs-Crack-leaked-password-database
### EXERCISE 
As a governance analyst it is part of your duties to assess the level of protection offered by implemented controls and minimize the probability of a successful breach. You often need to know the techniques used by hackers to circumvent implemented controls and propose uplifts to increase the overall level of security in an organization. Gaining valid credentials gives the attackers access to the organization’s IT system, thus circumventing most of perimeter controls in place.

### TASK:
Your job is to crack as many passwords as possible with available tools (e.g. use Hashcat). Here are your Task instructions:

Review the links provided in the additional resources (section 4) below to gain a background understanding of password cracking
Try to crack the passwords provided in the 'password dump' file below using available tools
Assess the 5 questions in the task instructions below in relation to the passwords provided (type of hashing algorithm, level of protection, possible controls that could be implemented, password policy, changes in policy)
Draft an email/memo briefly explaining your findings in relation to controls used by the organization and your proposed uplifts. We recommend spending about 1.5 hours on this task and keeping it at 1 page in length. 
Your answer should be provided in the form of a draft email/memo explaining your findings and conclusions of controls currently used by an organization to prevent successful cracking of passwords and potential uplifts that you would propose to existing controls with justifications.

## CONSIDERATIONS:

After analysis, I found that the MD5 algorithm was used to protect the passwords. 

Reading about this algorithm, it is already old (1991) and it is popular cryptographically, so 
I would not use it because it offers very little protection in case of password leakage. 
Should not be used in collision tolerance situations. 

First of all, when assuming passwords, remember that they should be completely different than login. They were different than: 123456, 123456789, qwerty, password, 111111, 12345678, Marcin123, polska. -> these are typical passwords.

Use other password hashing algorithms (bcrypt, Argon2), newer, less popular that are more difficult to crack. Time is an important role of the algorithm. The better we encrypt the password, the longer the time to decrypt it, which is very important, as the required computational work will increase.

Increasing the length of the password, and the use of special characters.

Another point is the password manager that I discovered on my Iphone. There is a system developed there that automatically creates a strong password for us, consisting of many characters.
It is safe.

In my opinion, passwords should have something more when logging in, for example. A good solution is to confirm it via SMS, additional questions are good, for example, to enter a password and face verification.
You have to remember not to overdo verifications, because technology is for people and not for IT specialists. 



MD5 algorithm:
```
experthead:e10adc3949ba59abbe56e057f20f883e
interestec:25f9e794323b453885f5181f1b624d0b
ortspoon:d8578edf8458ce06fbc5bb76a58c5ca4
reallychel:5f4dcc3b5aa765d61d8327deb882cf99
simmson56:96e79218965eb72c92a549dd5a330112
bookma:25d55ad283aa400af464c76d713c07ad
popularkiya7:e99a18c428cb38d5f260853678922e03
eatingcake1994:fcea920f7412b5da7be0cf42b8c93759
heroanhart:7c6a180b36896a0a8c02787eeafb0e4c
edi_tesla89:6c569aabbf7775ef8fc570e228c16b98
liveltekah:3f230640b78d7e71ac5514e57935eb69
blikimore:917eb5e9d6d6bca820922a0c6f7cc28b
johnwick007:f6a0cb102c62879d397b12b62c092c06
flamesbria2001:9b3b269ad0a208090309f091b3aba9db
oranolio:16ced47d3fc931483e24933665cded6d
spuffyffet:1f5c5683982d7c3814d4d9e6d749b21e
moodie:8d763385e0476ae208f21bc63956f748
nabox:defebde7b6ab6f24d5824682a16c3ae4
bandalls:bdda5f03128bcbdfa78d8934529048cf
```

Cracked passwords (after using Hashcat): 
```
experthead:123456
interestec:123456789
ortspoon:qwerty
reallychel:password
simmson56:111111
bookma:12345678
popularkiya7:abc123
eatingcake1994:1234567
heroanhart:password1
edi_tesla89:password!
liveltekah:qazxsw
blikimore:Pa$$word1
johnwick007:bluered
flamesbria2001:Flamesbria2001
oranolio:Oranolio1994
spuffyffet:Spuffyffet12
moodie:moodie00
nabox:nAbox!1
bandalls:Banda11s
```

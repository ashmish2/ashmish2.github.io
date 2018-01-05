---
layout: post
title: Hashing Password
---
 As I mentioned in [my recent post](https://ashmish2.github.io/OilHack/), some big oil companies were hacked recently. 
 Linkedin also [got hacked recently](https://www.pcworld.com/article/257045/security/6-5m-linkedin-passwords-posted-online-after-apparent-hack.html) and millions of password were stolen.
 Now, you will think that big companies like linkedin will not store password in clear text and you are correct. 
 Then how crackers were able to extract so many passwords? From my previous post, we can be sure that we cannot rely on user
 to use strong password. Hence, it becomes easy for the hacker cracker to extract password knowing the hashing algorithm used. 
 Now the questions is if some cracker somehow got access to your server database, what can application developer do to protect 
 passwords and save users private data.
 
 
[Hashing algorithms](https://en.wikipedia.org/wiki/Cryptographic_hash_function) are strong enough if provided with right length and mixture (lower, upper, number etc) of alphabets in password. 
So to make it hard for cracker, multiple combination of password along with salt can be used. 
Salt is just a randomly generated string used along with password (suffix, prefix etc) to make it harder to crack.

Some of the possible combinations can be : 
sha1(password + salt)

sha1( sha1(password)  + sha1(salt)) 

sha1(sha1( sha1(password)  + sha1(salt)))

sha1 is hashing algorithm, password is password of user and salt is added random string.

Important thing to remember is the combination used for hashing which will be coded in software.
So, if only database is exposed to cracker, they cannot crack the passwords (even if user password is pass123 😛 )
assuming they don’t know the right combination of hashing used. 
For that they have to hack the software as well to get the salt and right combination of hashing used.


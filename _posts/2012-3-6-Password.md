---
layout: post
title: Password
---

  Internet is full of websites providing lots of interesting applications to the user. All these websites try to come up with numerous ways to provide security (for account hacking, data theft etc) to the user. But it turns out that you can provide 256 bit or 1024 bit encryption, Diffie Hellman or PGP; but there is a single point of failure which can be a very loose end – **THE USER**. This is very aptly put by this and this.  There are many ways by which your account can be hacked. Today, I am bringing up a very simple way to do this.

  All the websites currently requires you to register using your email id and password. As users enroll to so many websites, they usually end up using the same password again and again for their ease. So, a hacker can build a innocent looking website that asks you to register first and can get your email id and password. Then he can easily hack into your email, facebook or even your bank accounts if you are using the [same password](https://xkcd.com/792/)
 
  Now how to solve this problem. Ideal way is to keep separate password for each site and go crazy remembering all of them or don’t register to any site at all :-). But there can be some other way as well
1. Use tool to generate password for you like SuperGenPass. Its good but along with it comes issue of portability and ease of use. Also, should you trust this tool!
2. Go with [XKCD](https://xkcd.com/936/) way 🙂

Third and an easy way out is to have password in two parts :  Prefix and Suffix

a) **Prefix** : This part is constant made by combining 2-3 English words or your native language’s word or mix of both. Anything that suits you. But this has to be the one which you can remember very easily and shouldn’t be easily recognizable e.g catdog may not be a good prefix.
b) **Suffix** : Now, this is the variable part which you can generate for that particular site only. As this mostly has some relation with that site, you can easily recall this once you land on that page. e.g fb for facebook
Again, try not to make this so obvious, otherwise its easy to guess that you are using prefix suffix combination.

Also, you can keep prefix as suffix and vice versa for some sites. Even if you don’t remember what sites they are, you will end up entering right password in 2 iterations.

There is also a fourth solution used by some sites if not all (normally banks). This is called Two factor authentication or multifactor (> 2) authentication. This works even if your password is compromised. I will talk about this later.

Hope this article gives you a fair idea about the kind of attack that is possible and an easy yet effective precaution from your side. You can also come up with your own way of generating password, but the main idea is not to use same password again and again.

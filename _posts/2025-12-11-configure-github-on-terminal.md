---
title: Access Github Using Terminal
date: 2025-12-11 20:16:00 +60
image: https://i.postimg.cc/650Jvgr7/github-token.jpg
categories: [Tutorials, Programming]
tags: [git, github]
summary: Support for password authentication was removed on August 13, 2021. Error
lqip: https://i.postimg.cc/650Jvgr7/github-token.jpg
---

## Introduction

---
As a programmer using github, you might want to use the terminal to push and pull your code to github. 
To do so, you need to configure your terminal to be able to access your github account. 
Today, we take a look at how to make it possible and as easy as it gets.
Read along,  and as usual, we always help out with your questions.

> This tutorial is to help you configure your terminal access to github, not to teach you how to use git/github.
So we assume you are familiar with git and github already and just need how to configure access to your github account from the terminal. It's an advanced tutorial with lots of assumptions.
{: .prompt-info}

---

## Procedure
### How to configure your username and email for github on your terminal
1. To set your username
```
git config --global user.name "NAME"
```
2. To set your email
```
git config --global user.name "EMAIL@EMAIL.COM"
```

> These values above are the values of your github account, if you don't have an account already, you can create one on github.com for free.
{: .prompt-info}

---

### To check the values you have configured
You can use this command below to do so:
```
git config --list
```
> If you notice and error, you can repeat the very commands above and give in the correct values.
{: .prompt-info}

---

### Sign into Github on your browser
Clone the repository you want to work with. If there's no repository already, you can create one and use for your testing purpose.

---

### At this level you have completely configured the basics and have a repository to work with.
At this level if you try to do a git push it will ask for your password but after putting the password, you get an error. This is because the this method of authentication is no longer accepted by github. 
Below is what you need to do, which is the main purpose of this tutorial today.
> Support for password authentication was removed on August 13, 2021
{: .prompt-warning}

---

### Generate an access token from Github
1. Go to github on the browser that you sign in earlier
2. Click on your name
3. Click on settings 
4. Scroll down to developer settings
5. Click on Personal access token 
6. Click on Token (classic)
7. Next, Generate new token (classic)
8. Give a note/name for your token
9. Give an expiration date
10. Select the scope (all the things that token will be able to do)
11. Next click on "generate token"
12. Copy the generated token

---

### Adding the generated token to your terminal
Run the command below replacing the values in angled brackets and using the token you generated <>
```
git remote set-url origin https://<TOKEN>@github.com/<USERNAME>/<REPO>
```

If all is done well you can now push code to your github and do all the actions you selected in your scope in step 10 above. 
Also, the length of time was selected at step 7 above, so after that amount of time, it will expire.

---

> If it works for you, then that's great!
If it doesn't work for you then you are probably not respecting the sequence.
You can always get in touch with us with your further questions.
{: .prompt-tip}

---

Bye for now. 

---

Follow | [Telegram Channel](https://t.me/pcdrills/) | [Facebook Page](https://facebook.com/pcdrillsofficial/) | [Twitter Handle](https://twitter.com/pc_drills) | [Youtube Channel](https://youtube.com/pcdrills)


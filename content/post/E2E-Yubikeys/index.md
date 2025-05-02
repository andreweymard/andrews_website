---
title: How to send end-to-end PGP encrypted emails using Yubikeys
description: A step-by-step guide on sending a PGP encrypted email using PKI and a little extra security using Yubikeys
date: 2025-04-23
image: mailbox.jpg
tags: 
    - End-to-End
    - Yubikey
    - PKI
    - Guides
---

## What's wrong with regular email?

Answer? *Nothing*.
If you're here you don't want to send regular old email. You've got a keen interest in privacy and want to expand the borders further than what you are presented with. If you think of email encryption you'd want to start thinking about how your email is sent encrypted over the internet. Well, thanks to email providers like Outlook, Gmail and many others, they take care of sending your email for you making sure that no one unwanted snoops your private messages. But what if they are the ones to snoop on your email? For anyone that's worked at an IT dept at a SMEs know that accessing employee email is part of your job description this could be for various troubleshooting purposes and not for anything nefarious. But this access comes with responsibility to trust that said person is not going to use the information contained in the emails for personal gain.

So, whether it be Governments issuing subpoenas or your IT dept, you have a right to privacy and the tools to do so. Let's say Gmail for example. This email provider says that they will encrypt it and send it to the receiving party's provider/server and send it to the user from there. This is a perfectly **secure enough** way to send an email. But what if Gmail before sending it decides to have a quick little sneak peek before sending it off? Scrape just enough metadata and keywords to better target you with ads? The implications go on, what stops Gmail giving undemocratic governments access to an activist's emails? Potentially putting someone's life in danger? These reasons may not apply to you, but if like me you just want to learn about cool tech that some of the smartest minds of our generation has conceived, read on.

## Pretty Good Privacy?

Hailed as good as military-grade encryption by Bruce Schneier. This was developed in the 1990s by Phil Zimmermann. So how is a technology, at the time of writing, that is almost 35 years old still holding up to today's computational advances and prowess? This has has many iterations over the years and has moved through a lot of companies. vulnerabilities have been discovered and fixed and has stood the test of time. While there are positive and negative connotations around it, its still a highly secure way to send end-to-end encrypted emails.

## Public Key Infrastructure

This example starts with Alice, Bob and Chad. Chad is naughty so Alice and Bob try to play without him. But since he's always around they can't agree on a time to play without him butting in. So they need to devise a way to talk without him understanding what they're saying. They come up with 2 keys each. Alice's keys are mathematically linked in a way so that whatever padlock, key 1 locks, key 2 can unlock and vice-versa. Same goes for Bob's keys. So now they exchange one of those keys with each other. Now they both have the ability to lock something that the other can unlock. This is an ELI5 of how public/private key-pair works. So what we will be doing is creating a public/private key-pair and sharing the public one with the world so anyone can send us encrypted messages that we can unlock with our private key. 

## 

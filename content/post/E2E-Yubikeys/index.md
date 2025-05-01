---
title: Guide on end-to-end PGP encrypted emails using Yubikeys
description: A step-by-step guide on sending a PGP encrypted email using PKI and a little extra security using Yubikeys
date: 2025-04-23
image: mailbox.jpg
---

## What's wrong with regular email?

Answer? *Nothing*.
If you're here you don't want to send regular old email. You've got a keen interest in privacy and want to expand the borders further than what you are presented with online. If you think of email encryption you'd want to start thinking about how your email is sent encrypted over the internet? Well, thanks to email providers like Outlook, Gmail and many others, they take care of sending your email for you making sure that no one unwanted snoops your private messages. But what if they are the ones to snoop on your email? For anyone that's worked at an IT dept at a SMEs know that accessing employee email is part of your job description this could be for various troubleshooting purposes and not for anything nefarious. But this access comes with responsibility to trust that said person is not going to use the information contained in the emails for personal gain.

So whether it be Governments issuing subpoenas or your IT dept, you have a right to privacy and the tools to do so. How we achieve this is by encrypting our email before handing it to the email provider, let's say Gmail for example. This email provider says that they will encrypt it and send it to the receiving party's provider/server and send it to the user from there. This is a perfectly **secure enough** way to send an email. But what if Gmail before sending it decides to have a quick little sneak peek before sending it off? Scrape just enough metadata and keywords to better target you with ads? The implications go on, what stops Gmail giving undemocratic governments access to an activist's emails? Potentially putting someone's life in danger? These reasons may not apply to you, but if like me you just want to learn about cool tech that some of the smartest minds of our generation has conceived, read on.

##

This is **bold** text, and this is *emphasised* text.

Viit the [Hugo](https://gohugo.io) website!

{{< quote author="A famous person" source="The book they wrote" url="https://en.wikipedia.org/wiki/Book">}}
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Exepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
{{< /quote >}}

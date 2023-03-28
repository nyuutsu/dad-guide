# Background

## Context

When you sign into an online account, you show who you are (and so what information to show you) by entering two pieces of information: a username and a password. For various reasons[^note], using *only* a username and a password isn't secure enough for especially sensitive data.

This is why high-security online accounts (e.g. banks, retirement accounts, online pay statements) include *additional* checks when trying to log in. For example, your bank might send you a text message or email containing a code, and then ask you to provide that code. What they are doing is having you provide a second "factor", or "thing that proves who you are". That service "uses two-factor authentication" ("2FA").

## DAD & 2FA

[DAD](https://dad.ndrn.org/) has been updated to use two-factor authentication. Specifically: DAD uses codes produced by an "authenticator app".

DAD users need to

1. install an authenticator

2. tell the authenticator how to make codes for DAD by scanning a QR code ***or*** entering a password

2. log in to DAD at least one time

3. every 45 days or so, provide DAD a code from the authenticator

```admonish info
Steps 1 & 2 do not need to be done after initial setup. Once you've told the authenticator how to make the codes, it isn't going to forget and the codes are going to work fine. Just go in and get the current one if DAD asks for one.
```

Later sections of this guide cover what to do.

[^note]: Usernames are easy to discover. Often they can be guessed. In organizations, they often follow a pattern, so if you discover one username, you can deduce all of the usernames. Passwords are hard to remember, so people tend to use simple ones and then also re-use them across sites and services. Passwords are useful, but they can be compromised or guessed.

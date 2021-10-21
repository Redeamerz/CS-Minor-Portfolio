---
title: MFA Authentication
---

Two-factor authentication (also known as 2FA) is a security mechanism that
needs two different forms of identification to gain access to something.

Two-factor authentication can be used to make an online account, a
smartphone, or even a door more secure. Before anything that is being
secured may be accessed, 2FA requires two forms of information from the
user a password or personal identification number (PIN), a code given to
the user's smartphone, or a fingerprint.

## Pros and Cons of 2FA

### Pros

#### Second layer of security

This is a self-evident statement, but it is also the most obvious benefit
of using a two-factor authentication solution. While a password has been
the standard method of security for almost as long as accounts have been
required to be kept private in the digital age, it only provides one layer
of protection.

When a password is discovered, it is considered a security breach. Strong
passwords have been advised for a long time, typically comprising a
combination of letters, numbers, and special characters, but they are
still only one kind of security.

Furthermore, more secure methods of accessing personal information, such
as a speech recognition device, are only one layer that must be
compromised<sup>[(1)](#references)</sup>.

#### Variation

Only if you use a second password in the same way as the first will you
see a 100 percent increase in security levels. Two-factor authentication,
on the other hand, usually combines the authentication systems you use,
resulting in much higher security levels.

Other methods of achieving this, such as intrinsic authentication, which
uses a physical property to identify you, are available in addition to
using mobile devices to transmit on a security key (a tried-and-true
two-factor authentication approach).

#### Cost-effective

In general, two-factor authentication methods are not expensive. If you
add retinal scanning or voice recognition as a second step, the price will
rise, but advances in these techniques mean that you can now use these
types of hardware systems at relatively low costs.

### Cons

#### Time

Everything is relative when it comes to time. So, while the time it takes
to access accounts using a two-factor authentication process may be
negligible in terms of capacity for many, for others, such as using a card
reader each time, it would be a wasteful process that, when multiplied by
the number of employees, would equate to inefficient use of time.

Some two-factor authentication systems, such as SMS, are faster to
implement than others, so thorough research is advised if this is a
concern. A two-step process will always take longer for the second step,
so a two-step authentication system is unnecessary for data or accounts
that aren't important.

#### It's not foolproof

The reality is that no security system is foolproof – that is the nature
of the cyber landscape right now. Two-factor authentication processes are
certainly more effective than one-factor systems, that much is evident,
but determined hackers can still implement any number of devious schemes
and malware threats to undermine your system and access your sensitive
data.

That is not an easy feat to accomplish. The methods for circumventing or
breaching two-factor authentication systems will vary depending on several
factors, including the type of authentication system you use, as some are
more effective than others. But while a password, for example, can be
inadvertently shared, the same cannot be said of inherent recognition in
two-step authentication.

Cybercriminals have developed increasingly devious, underhand yet
sophisticated hardware to copy this information to steal data and access
accounts. Recent posts onh6ne show 2fa is far more secure than the
alternatives however nothing is foolproof when it comes to cybersecurity.

#### Cost

While relative to the organization, inevitably a two-factor authentication
system will involve some extra cost, and for smaller organizations that
can be restrictive. As there are so many options out there, the cost
increases can be minimised, however, so this need not rule out the
adoption of one of these systems. The cost of losing key personal data and
user accounts is often far higher than multifactor authentication will
ever cost.

## Types of 2FA

### Hardware Tokens

Hardware tokens are small, like a key fob, and generate a new numeric code
every 30-seconds, making them the most ancient form of 2FA. When a user
tries to access an account, they glance at the device and enter the
displayed 2FA code back into the site or app. Other versions of hardware
tokens automatically transfer the 2FA code when plugged into a computer’s
USB port.

They’ve got several downsides, however. For businesses, distributing these
units is costly. And users find their size makes them easy to lose or
misplace. Most importantly, they are not entirely safe from being hacked.

### SMS Text-Message and Voice-based tokens

SMS-based 2FA communicates with a user's phone directly. The site provides
the user a one-time passcode (OTP) through a text message after obtaining
their login and password. After that, much like with the hardware token,
the user must re-enter the OTP into the application to gain access.
Voice-based 2FA works similarly, automatically dialing a user and audibly
delivering the 2FA code. It is still used in nations where cellphones are
expensive or where cell connection is inadequate, despite its rarity.

For a low-risk online activity, text or voice authentication may be
sufficient. However, this degree of 2FA may not be sufficient for websites
that retain your personal information, such as utility providers, banks,
or email accounts. SMS is widely regarded as the least secure method of
user authentication. As a result, many businesses are strengthening their
security by shifting away from SMS-based two-factor authentication.

### Software Tokens

A software-generated time-based, one-time passcode (also known as TOTP, or
"soft-token") is the most popular kind of two-factor authentication (and a
preferred alternative to SMS and voice).

A user must first download and install a free two-factor authentication
program on their smartphone or computer. The app can then be used with any
site that accepts this type of authentication. The user first enters a
login and password, and then, when prompted, the code displayed on the app
is entered. Soft tokens, like hardware tokens, are often valid for less
than a minute. Soft-tokens further eliminate the possibility of hacker
eavesdropping because the code is created and shown on the same device.
With SMS or voice transmission techniques, this is a major worry.

### One Time Passwords

#### What is an OTP

A one-time password (OTP) is similar to a password, however, it can only
be used once. It is frequently used in conjunction with a conventional
password as a secondary authentication mechanism to provide additional
protection.

One-time passwords are exactly what they sound like one-time passwords.
Once you've used a password, it's dumped, and you'll have to enter a
different one the next time you need to access that application. This
improves security and makes it far more difficult for undesirable actors
to gain access to private accounts.
An OTP for a certain application or website can be accessed via smartphone
apps, text messages, or a proprietary token (such as a key fob). OneLogin
Protect is an example of an OTP generator that can be downloaded as a
mobile app. You're utilizing an OTP when you get an SMS text with a code
to assist you to log into a website or application.

OTPs are generated using a number of industry-standard methods, such as
SHA-1. To produce the OTP code, all of these methods require two inputs: a
seed and a moving factor. When you create a new account on the
authentication server, the seed is a static value (secret key).

The movement factor changes each time a new OTP is required, although the
seed does not. The method by which the moving factor is formed is a
significant difference between HOTP and TOTP.

#### HOTP

![HTOP-image](/image/article_img/hotp.webp 'HTOP process visualized')

HOTP stands for Hash-based Message Authentication Code, and the “H” in
HOTP stands for Hash-based Message Authentication Code (HMAC). In layman's
words, the HMAC-based One-time Password algorithm (HOTP) is an event-based
OTP with a counter as the moving factor in each code.

The movement factor is incremented based on a counter each time the HOTP
is requested and validated. The generated code is valid until you actively
request another one and the authentication server validates it. Each time
the code is validated and the user is granted access, the OTP generator
and the server are synchronized. Yubikey is an example of a HOTP-based OTP
generator.

#### TOTP

![TOTP-image](/image/article_img/totp.webp 'TOTP process visualized')

TOTP (Time-based One-time Password) is a time-based one-time password.
TOTP uses a static seed, similar to HOTP, but the movement factor is
time-based rather than counter-based.

A timestep refers to the length of time that each password is valid.
Timesteps are usually 30 seconds or 60 seconds in length. If you haven't
used your password within that time frame, it will expire, and you'll need
to request a new one in order to access your application.

### Push Notification

Instead of relying on the user receiving and entering a 2FA token,
websites and applications can now send a push notification to the user
when an authentication attempt is made. The owner of the device simply
views the information and can authorize or refuse access with a simple
tap. It's a passwordless authentication system that doesn't require any
codes or additional interaction.

Push notification removes phishing, man-in-the-middle attacks, and
unauthorized access by establishing a direct and secure connection between
the store, the 2FA service, and the device. However, it can only be used
with an internet-connected device that can run apps. SMS-based 2FA may
also be a preferable fallback in places where smartphone penetration is
low or the internet is intermittent. Push notifications, on the other
hand, are a more user-friendly and secure type of security when it is
available.

## References

1. OneLogin. (z.d.). OTP, TOTP, HOTP: What’s the difference? Geraadpleegd op 7 oktober 2021, van [https://www.onelogin.com/learn/otp-totp-hotp](https://www.onelogin.com/learn/otp-totp-hotp)
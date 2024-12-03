https://proton.me/support/encryption-lock-meaning

is thunderbird on firefox esr? 

https://addons.thunderbird.net/en-US/thunderbird/addon/importexporttools-ng/

proton mail + sender PGP >>> (subject subject not encrypted)

# thunderbird

![k9 privacy settings](/images/k9.jpg)

https://blog.thunderbird.net/2023/07/k-9-mail-collaborates-with-ostif-and-7asecurity-security-audit/

https://wiki.gnupg.org/EMailClients/Thunderbird

https://wiki.archlinux.org/title/thunderbird#Securing

https://forum.qubes-os.org/t/hardening-your-thunderbird-mail-vm-and-working-around-the-still-missing-qubes-attachments-plugin/1432

https://www.whonix.org/wiki/Encrypted_Email_with_Thunderbird

# IP

https://wiki.debian.org/TorBirdy

# Headers

https://lists.gnupg.org/pipermail/gnupg-devel/2015-July/030110.html

https://datatracker.ietf.org/doc/draft-ietf-lamps-header-protection/

https://modernpgp.org/memoryhole/guidance/

https://gist.github.com/leela52452/8470474b21efd0df6b2136ece829cd8c

https://www.ietf.org/archive/id/draft-autocrypt-lamps-protected-headers-02.html

https://attack.mitre.org/techniques/T1090/004/

## Subject lines

"Even though Proton Mail subject lines are not end-to end encrypted, it is exceptionally difficult for a third party to get access to them. Access would require breaching Swiss data privacy laws and getting a court order that is approved by a Swiss judge(new window).

You can also use generic subject lines that disclose minimal information about the message contents."

https://proton.me/support/does-protonmail-encrypt-email-subjects

# Spam?

https://simplelogin.io/docs/getting-started/anti-phishing/

https://security.stackexchange.com/questions/188654/protonmail-cannot-read-my-mail-but-can-detect-if-it-is-spam

"""

As you hint in your third point, it's a difference if the mail is from _and_ to a Protonmal account, or if one side is an third-party server.

For the cases where the sender or receiver (one of them) is not a Protonmail user, they DO read the mail, as they say themselves: [https://protonmail.com/blog/encrypted-email-spam-filtering/](https://protonmail.com/blog/encrypted-email-spam-filtering/)

Part of the text there:
> 
> 1. First, the IP address of the incoming SMTP server is checked against spam blacklists which contain IP addresses of servers we have previously received spam from. If we receive a hit, the message is rejected.
> 2. Secondly, the message is passed through our customized Bayesian filters which marks suspicious messages as spam.
> 3. Next, we generate checksums of incoming messages and check them against a database of known spam messages. If there is a match, we mark the message as spam. The checksums are done in such a way that it is also effective against mutating spam emails.
> 
> ...
> 
> All this is done in memory so that by the time anything is permanently stored to disk, the email is already un-readable to us. This gives us a very limited window to perform spam filtering on incoming messages.
> 
> ...

TL;DR. they encrypt the received mail after filtering it / filter after decrypting before sending.  
They still say they "can't read anything" despite anything running through their spam filter is not secure from admins and developers.

To be fair, even without filter the server must handle the unencrypted mail at some point, if the sender/receiver is external... but "they never can read it" is nonsense.

---

About internal mails from _and_ to Protonmail, I have not found a similar post - but there are (probably) some official statements on the internet.

* That they factor in if receivers mark something as spam.
* That they take care to block anyone over a treshold (unlike some mail providers who just don't care).
* And that there is a limit how many mails can be send in a certain time (making mass spam harder).

"""

https://support.mozilla.org/en-US/kb/thunderbirds-scam-detection

# Virus

https://support.mozilla.org/en-US/kb/security-panel-settings-in-thunderbird#w_antivirus-tab

https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-endpoint-linux

# User.js

(Note this is just a config file, javascript is not ran IN the emails)

https://github.com/HorlogeSkynet/thunderbird-user.js/blob/master/user.js

https://r-36.net/scm/privacy-haters/file/thunderbird/user.js.html

## user-overrides.js

https://codeberg.org/12bytes/thunderbird-user.js-supplement

# Aliasing

https://forwardemail.net/en

https://migadu.com/

# Self host?

port forward vpn

cgnet http://he.net/cgi-bin/ip_transit_quote

hetzner vps ip

# Annexure A

https://www.betterbird.eu/

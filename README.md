# matrixmail
Send messages to matrix rooms instead of email.

```bash
echo "the message" | mail -s "the subject" '!jEsUZKDJdhlrceRyVU:example.org'
```

Messages are send as plain text.

## Installation
Requires Python 3.6 or later and [matrix-nio](https://github.com/poljar/matrix-nio).

Copy or symlink to `/usr/bin/mail` and/or `/usr/bin/mailx`.
Also create a symlink `mail-setup` and run it to log in.
It will prompt for your login and save the session:
```shell
# ln -s mail mail-setup
# ./mail-setup
Homeserver (default: matrix.org): example.org
User: alice
Password: 
Device name (optional): Alice's Computer
```

## Compatibility
Only Send Mode, no Receive Mode or any interactive features.

Lines starting with `~` (tilde) are ignored.

# Reference
The mailx specification: https://pubs.opengroup.org/onlinepubs/9699919799/utilities/mailx.html

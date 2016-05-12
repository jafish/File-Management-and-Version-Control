# Version Control Class
## SSH Keys

### How do SSH keys work?

SSH keys are a way to authenticate without passwords. Instead, it uses "keys", which are always generated in pairs: one public, and one private key. The private key typically resides on your machine in your home folder, while the public key is intended for sharing widely, with any service or entity with which you would like to connect and authenticate through the protocol. For added protection, the private key can be locked with a passphrase, which then needs to be entered when attempting to use that key to authenticate.[^Wikipedia]

### How many keys do I need?

The jury seems to be out on whether or not multiple key pairs are necessary. Depending on where the private keys are stored, having multiple SSH key pairs may increase complexity with negligible increase in security. On the other hand, if a user connects to servers in different user roles and access levels, having multiple key pairs may make sense.[^MultipleKeys]

### Creating an SSH Key Pair

`ssh-keygen`

#### Passphrase

The passphrase guards against compromise of the private key. To login via SSH with my Lithium Host's CPanel account (for setting up SCP with Dropshare or WebDav with Transmit), I enter the public SSH key in CPanel. Then, when I go to login on the command line or in DropShare, a dialog pops up asking me to enter the password for my private SSH key, because at that point the process is attempting to access it in order to authenticate my login. This is an added layer of protection because without the passphrase, getting a hold of the private key file gets you nothing. 

##### Workaround for Not Being Able to Paste into SSH Passphrase Dialog

Run this command (`ssh-add ~/.ssh/id_rsa`), which requests a password on the command line, which does allow for pasting a passphrase copied from *1Password* or other password manager. This makes it easy to have non-human-readable (i.e. random, difficult, long, and a pain to type out) passwords.

### Should I Store My Private Key on Multiple Machines?

This answer suggests having a separate key "per origin"[^Separate-Key], but others suggest that having one pair shared across multiple machines with the same user is ok.[^Separate-Key-2] If one machine is a desktop and another a laptop, it's best to have a separate pair for the desktop since the laptop is easier to compromise. 

[^Wikipedia]: https://en.wikipedia.org/wiki/Secure_Shell#Key_management  
[^MultipleKeys]: http://serverfault.com/questions/80478/ssh-do-you-use-one-private-public-key-pair-for-each-remote-machine-or-a-single   
[^Separate-Key]: http://superuser.com/questions/189355/is-it-ok-to-share-private-key-file-between-multiple-computers-services  
[^Separate-Key-2]: http://serverfault.com/questions/170682/using-same-ssh-private-key-across-multiple-machines
======= <-- This was actually the separator git conflict marker - I just missed it!

Adding a small change to see what rebasing looks like.

One more change before the rebasing.

Another change.
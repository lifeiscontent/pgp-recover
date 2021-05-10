# pgp-recovery

### Steps for recovery

1. get a hold of your public key.
2. dearmor they public key `gpg --dearmor public-key.txt`
3. once you've got your paperkey on your machine, import your private key back to your keyring. `paperkey --pubring public-key.txt.gpg --secrets secret-key.txt | gpg --import`
4. delete `secret-key.txt` off your machine.

# Keybase 

## Install

Simply install and prove the device using the standard procedure. 

## Gpg

Install gpg using scoop `scoop install gpg4win`. 

Export the public and private key of keybase to the new computer.
```
keybase pgp export | gpg --import # Public key import 
keybase pgp export --secret | gpg --allow-secret-key-import --import
```

### Change trust of key 

Source: https://unix.stackexchange.com/questions/407062/gpg-list-keys-command-outputs-uid-unknown-after-importing-private-key-onto

```
gpg --edit-key <email>
trust
5 = I trust ultimately
```

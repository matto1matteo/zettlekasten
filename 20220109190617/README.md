# GPG issues

Recently arch is getting a lil bad with gpg key manipulation, so i found a
manual way to update certain needed key.

## Add gpg key manually

`gpg --keyserver keyserver.ubuntu.com --search-keys <key to search>`

where \<key to search\> is the actual number required by yay/pacman.

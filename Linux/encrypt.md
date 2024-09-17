to encrypt files you use `gpg`
```sh
gpg -c file
```
then write the password and done.

---
for folders it's a little bit different because this tool doesn't support folders so you have to compress it first.
```sh
tar -czf folder.tar.gz folder/
# then encrypt it
gpg -c folder.tar.gz
# to decrypt it
gpg folder.tar.gz.gpg
# extract it
tar -xzf folder.tar.gz
```

---
or you `zip`
```sh
zip -er folder.zip folder
unzip folder.zip
```
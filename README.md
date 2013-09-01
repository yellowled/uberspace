# Bash helper scripts

## Staging

Copy both `stage` and `unstage` to `~/bin/` and `mkdir ~/stage`. Configure the variables `UBERSPACE` (your Uberspace username) and `DOMAIN` (the domain associated with your Uberspace) in `~/bin/stage` **and** `~/bin/unstage`.

* `stage <STAGENAME>` creates `stagename.yourdomain.tld` (or rather the directory required for that) and a MySQL database named `username_stagename`. It also links the stage to your home dir, so you can access it through `~/stage/stagename/`.
* `unstage <STAGENAME>` removes stage, symlink and MySQL database.

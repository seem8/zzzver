# zzzver
Dumb version control script.
For those who don't need it,
but wants to have snapshot archives.

Dependencies are: bash, diff, gzip and md5sum.

1. Type 'chmod +x zzzver' and './zzzver' to run it.
2. If you don't add any parameter, it will echo a quick help:

Please specify:
zzzver init - to create new repository,
zzzver diff - to compare test and stable repo,
zzzver diff archive/name.tar.gz - to compare test and stable with specified archive,
zzzver merge - to copy test into stable,
zzzver save - to archive test and stable as date_time.tar.gz,
zzzver load archive/name.tar.gz - to replace test and stable with content of specified archive,
zzzver load archive/name.tar.gz test - to replace test with content of specified archive,
zzzver load archive/name.tar.gz stable - to replace stable with content of specified archive.
zzzver md5 - to make md5 hashes of files from testing and stable.

3. Init will create stable/, test/, archive/ subdirectories and zzzver log file. Zzzver is intended to run from directory, that is containing those three subdirs.

4. If you have bash executable in /bin, and not /usr/bin, edit the first line.

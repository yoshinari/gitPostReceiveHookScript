gitPostRecieveHookScript
========================

With this script, you can publish the files from the git bare repository automatically.

You can specify following actions to the ini file.

copy action:
   Checkout the files under destination directory.

scp action:
   Bad Logic.
    Copy all the files to taget server with scp command.
    Can not remove the "git removed files".

ftp action:
    Bad Logic.
    Copy all the files to target server with ncftpput command.
    Can not remove the "git removed files".

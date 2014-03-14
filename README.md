gitPostReceiveHookScript
========================

With this script, you can publish the files from the git bare repository automatically.

#### You can specify following actions to the ini file.

##### copy action
* Checkout the files under destination directory.

##### scp action
* Copy all the files to taget server with scp command.
* Erase the git removed files wich ssh command, but can not erase empty directory.

##### ftp action
* Copy all the files to target server with ncftpput command.
* Erase the git removed files with ftp command, but can not erase empty directory.

### Installation

* Make post-receive.ini file from post-receive.ini.sample file, then
update the definition to fit your bare repository.
* change file mode to 600: chmod 600 post-receive.ini
* Place etc/post-receive.ini and hooks/post-receive file under your bare repository.
* change file mode to runnable: chmod +x post-receive
* If you use ftp mode, the server must be installed ftp and ncftp program.

### Credits
This script uses the following open source component:

* [Drupal Deployment Skeleton](https://github.com/fluxsauce/DrupalDeploySkel) - cfg_parser function to read ini file.

gitPostReceiveHookScript
========================

With this script, you can publish the files from the git bare repository automatically.

#### You can specify following actions to the ini file.

##### copy action
* Checkout the files under destination directory.

##### scp action
* Bad Logic.
* Copy all the files to taget server with scp command.
* Can not remove the "git removed files".

##### ftp action
* Bad Logic.
* Copy all the files to target server with ncftpput command.
* Can not remove the "git removed files".

### Installation

* Make post-receive.ini file from post-receive.ini.sample file, then
update the definition to fit your bare repository.
* change file mode to 600: chmod 600 post-receive.ini
* Place etc/post-receive.ini and hooks/post-receive file under your bare repository.
* change file mode to runnable: chmod +x post-receive

### Credits
This extension uses the following open source component:

* [Drupal Deployment Skeleton](https://github.com/fluxsauce/DrupalDeploySkel) - cfg_parser function to read ini file.

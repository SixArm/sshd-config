# Secure Shell daemon (SSHd) configuration with sshd_config file


## Introduction

Our SSH configuration files are in two repos:

  * `sixarm-ssh-config` for the client configuration.

  * `sixarm-sshd-config` for the server configuration.

Take what you need. We welcome suggestions, feedback, and pull requests.


## Install

To install this system-wide on a typical Unix system, you must have root administration permissions, or similar kinds of sudo permissions.

Warning: doing this is dangerous and can seriously affect your systems, so if you don't understand the instructions below, then ask for help.

Create your SSH directory as needed:

    mkdir -p /etc/ssh

Do you already have an SSH config file?

    ls /etc/ssh/sshd_config

If so, then you may want to make a backup:

    cp /etc/ssh/sshd_config /etc/ssh/ssh_config.backup

Clone:

    git clone https://github.com/sixarm/sixarm-sshd-config

Appen this content to your own SSH config file:

    cat sixarm-sshd-config/sshd_config >> /etc/ssh/sshd_config

Edit as you like, using your own favorite editor:

    edit /etc/ssh/sshd_config


## Changes

* 2022-06-27 3.0.0 Rename repos
* 2016-04-03 2.0.0 Improve usability
* 2015-06-30 1.0.0 Publish


## License

You may choose any of these open source licenses:

  * Apache License
  * BSD License
  * CreativeCommons License, Non-commercial Share Alike
  * GNU General Public License Version 2 (GPL 2)
  * GNU Lesser General Public License (LGPL)
  * MIT License
  * Perl Artistic License
  * Ruby License

The software is provided "as is", without warranty of any kind,
express or implied, including but not limited to the warranties of
merchantability, fitness for a particular purpose and noninfringement.

In no event shall the authors or copyright holders be liable for any
claim, damages or other liability, whether in an action of contract,
tort or otherwise, arising from, out of or in connection with the
software or the use or other dealings in the software.

This license is for the included software that is created by SixArm;
some of the included software may have its own licenses, copyrights,
authors, etc. and these do take precedence over the SixArm license.

Copyright (c) 2015-Present Joel Parker Henderson

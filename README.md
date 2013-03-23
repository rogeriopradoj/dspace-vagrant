# DSpace VM

Configuration files for provisioning a virtual machine with DSpace using Vagrant and Chef Solo.

## Rough guide

Install [VirtualBox](http://virtualbox.org). Add VirtualBox to path e.g.:

    export PATH=$PATH:/Applications/VirtualBox.app/Contents/MacOS/

Install [Vagrant](http://vagrantup.com) from [package](http://downloads.vagrantup.com) as recommended by [Vagrant docs](http://docs.vagrantup.com/v1/docs/getting-started/index.html). Alternatively uncomment Vagrant gem dependency in Gemfile before running bundle install.

Download/clone [DSpace VM](https://github.com/lwalley/dspacevm):

    $ git clone git@github.com:rogeriopradoj/dspace-vagrant.git
    $ cd dspace-vagrant/

Create and provision virtual machine with Vagrant:

    $ vagrant up

SSH to virtual machine:

    $ vagrant ssh

Create dspace adminstrator for logging into the UI:

    vagrant@lucid64:~$ sudo /dspace/bin/dspace create-administrator



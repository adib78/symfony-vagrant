Symfony Standard Edition - Vagrant
==================================

Building a development environment with Symfony Standard Edition.

To use:

 1. install vagrant (www.vagrantup.com)
 2. install VirtualBox
 3. install the bindfs plugin => vagrant plugin install vagrant-bindfs
 4. fork this repo
 5. clone it => git clone git@github.com:...your-github.../...your-fork....git
 6. start the VM => vagrant up
 7. edit your hosts file => 192.168.56.101  symfony-vagrant.dev

Browse to symfony-vagrant.dev

Bower is installed, but has to be used as the www-data user

    vagrant ssh
    sudo su www-data
    cd /var/www
    bower install
    (etc)

Built using puPHPet

Edit details in the {project_home}/Vagrantfile and re-provision with "vagrant provision"

Connect to MySQL from the host to symfony-vagrant.dev via an SSH tunnel, using the symfony-vagrant/puphpet/files/dot/ssh/id_rsa key
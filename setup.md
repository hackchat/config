Install Virtual-Box http://download.virtualbox.org/virtualbox/4.1.16/VirtualBox-4.1.16-78094-OSX.dmg
gem install vagrant
vagrant box add lucid32 http://files.vagrantup.com/lucid32.box
vagrant init lucid32
vagrant up
vagrant ssh

# Install stuff
sudo apt-get install build-essential zlib1g-dev git-core sqlite3 libsqlite3-dev

## Install Ruby
cd
git clone git://github.com/sstephenson/rbenv.git .rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile
echo 'eval "$(rbenv init -)"' >> ~/.bash_profile
source .bash_profile 
$ git clone https://github.com/sstephenson/ruby-build.git
$ cd ruby-build
$ sudo ./install.sh
$ rbenv install 1.9.3-p125
rbenv global 1.9.3-p125

cd /vagrant/
gem install bundler

install gem 'therubyracer' inside of vagrant
uncomment this config.vm.forward_port inside of Vagrantfile
exit vagrant (exit)
vagrant reload

apt-get -y update
apt-get -y install curl git-core python-software-properties


# Node.js
add-apt-repository ppa:chris-lea/node.js
apt-get -y update
apt-get -y install nodejs



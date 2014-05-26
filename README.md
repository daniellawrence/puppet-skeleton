puppet-skeleton
==================

A simple puppet repo that can be used to bootstrap your adventures in puppet.

How to use?
--------------

You need to install puppet, puppet-lint & r10k to get the most out of this repo.

The basic setup and install.

    $ sudo apt-get install rubygems ruby-dev ruby
    $ sudo gem install puppet puppet-lint r10k

Install the default modules via *r10k*

	$ r10k puppetfile install
	$ ls -l modules

Installing on your puppet master

You will need to update the *tools/r10k_deployment.cfg* file before running this.
(unless you want this repo in its current state, landing on your puppetmaster)

	$ scp tools/r10k_deployment.cfg puppet:/tmp
	$ ssh puppet -t 'sudo cp /tmp/r10k_deployment.cfg /etc/r10k.cfg'
	$ ssh puppet -t 'sudo r10k deploy'

Why is modules/ empty ?
-----------------------------

This direction is populated by *r10k*, have a look at the *Puppetfile* for more information

Default modules
---------------

This are the default modules that are install from the forge via r10k.

* ntp
* apt

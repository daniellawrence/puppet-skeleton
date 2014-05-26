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

Why is modules/ empty ?
-----------------------------

This direction is populated by *r10k*, have a look at the *Puppetfile* for more information

Default modules
---------------

This are the default modules that are install from the forge via r10k.

* ntp
* apt

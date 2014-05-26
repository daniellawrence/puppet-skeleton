puppet-skeleton
==================

A simple puppet repo that can be used to bootstrap your adventures in puppet.

How to use?
--------------

You need to install puppet, puppet-lint & r10k to get the most out of this repo.

    $ sudo apt-get install rubygems ruby-dev ruby
    $ sudo gem install puppet puppet-lint r10k

Why is modules/ empty ?
-----------------------------

This direction is populated by *r10k*, have a look at the *Puppetfile* for more information

Default modules
---------------

This are the default modules that are install from the forge via r10k.

* ntp
* apt


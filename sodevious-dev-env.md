## Things to install

### install homebrew
`ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"`

### install rvm
`\curl -sSL https://get.rvm.io | bash
Downloading https://github.com/wayneeseguin/rvm/archive/master.tar.gz`
For using rvm in current shell: `source /Users/nicoledominguez/.rvm/scripts/rvm`

### add sublime text symlink
`ln -s "/Applications/Sublime Text 2.app/Contents/SharedSupport/bin/subl" ~/.rvm/bin/subl`

### add git config
* `git config --global user.name "Nicole Dominguez"`
* `git config --global user.email sodevious.net@gmail.com`

## Documentation & Instructions

### Python

Python demo
  /usr/local/share/python/Extras

Setuptools and Pip have been installed. To update them
  pip install --upgrade setuptools
  pip install --upgrade pip

To symlink "Idle" and the "Python Launcher" to ~/Applications
  `brew linkapps`

You can install Python packages with (the outdated easy_install or)
  `pip install <your_favorite_package>`

They will install into the site-package directory
  /usr/local/lib/python2.7/site-packages

See: https://github.com/Homebrew/homebrew/wiki/Homebrew-and-Python


### MySql

A "/etc/my.cnf" from another install may interfere with a Homebrew-built
server starting up correctly.

To connect:
    mysql -uroot

To have launchd start mysql at login:
    ln -sfv /usr/local/opt/mysql/*.plist ~/Library/LaunchAgents
Then to load mysql now:
    launchctl load ~/Library/LaunchAgents/homebrew.mxcl.mysql.plist
Or, if you don't want/need launchctl, you can just run:
    mysql.server start

### memcached

To have launchd start memcached at login:
    ln -sfv /usr/local/opt/memcached/*.plist ~/Library/LaunchAgents
Then to load memcached now:
    launchctl load ~/Library/LaunchAgents/homebrew.mxcl.memcached.plist
Or, if you don't want/need launchctl, you can just run:
    /usr/local/opt/memcached/bin/memcached

### rabbitmq

Management Plugin enabled by default at http://localhost:15672

Bash completion has been installed to:
  /usr/local/etc/bash_completion.d

To have launchd start rabbitmq at login:
    ln -sfv /usr/local/opt/rabbitmq/*.plist ~/Library/LaunchAgents
Then to load rabbitmq now:
    launchctl load ~/Library/LaunchAgents/homebrew.mxcl.rabbitmq.plist
Or, if you don't want/need launchctl, you can just run:
    rabbitmq-server

### phantomjs

### node 

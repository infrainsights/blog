# How to install Jekyll

Install rbenv:

    $ brew install rbenv ruby-build rbenv-default-gems rbenv-gemset
    $ mkdir ~/git/config/
    $ echo 'eval "$(rbenv init -)"' >> ~/git/config/env.sh

Install Ruby:

    $ rbenv install 3.1.3
    $ rbenv global 3.1.3

Install bundler:

    $ gem install bundler
    $ echo 'bundler' >> "$(brew --prefix rbenv)/default-gems"

Skip r-doc generation:

    $ echo 'gem: --no-document' >> ~/.gemrc

Install Jekyll:

    $ gem install jekyll

Start Jekyll:

    $ jekyll new blog
    $ cd blog
    ~/blog $ bundle exec jekyll server
    
Now browse to http://localhost:4000

---
title: EC2 for Ruby
layout: post
date: 2014-03-11
---

I forked a repo I already have for [launching a LAMP stack on EC2][1] NOTE: Link to public version of repo. 

I deploy this server, and collect the public IP address from the EC2 Management Console.

SSH into the server using `vagrant ssh`, and go to work 

check ruby
check rails
sudo apt-get install rails
sudo gem install bundler

download repo

sudo bundle install

_may be removed_ weird mysql thing, this worked for me
sudo apt-get install libmysql-ruby libmysqlclient-dev # http://stackoverflow.com/questions/7170722/mysql2-with-native-extensions-error-failed-to-build-gem-native-extension-gem

sudo apt-get install nodejs

{bundle exec} rake db:create:all
{bundle exec} rake db:migrate
rake db:migrate RAILS_ENV=production
rails server

[1]: https://github.com/AQDCT/bybh-vagrant-puppet-aws (link to real repo)


## Path B

Install passenger [2]


To install GNU C++ compiler:
   Please install it with apt-get install build-essential

 * To install Curl development headers with SSL support:
   Please run apt-get install libcurl4-openssl-dev or libcurl4-gnutls-dev, whichever you prefer.

 * To install Ruby development headers:
   Please install it with apt-get install ruby-dev

 * To install Apache 2 development headers:
   Please install it with apt-get install apache2-worker-dev

 * To install Apache Portable Runtime (APR) development headers:
   Please install it with apt-get install libapr1-dev

 * To install Apache Portable Runtime Utility (APU) development headers:
   Please install it with apt-get install libaprutil1-dev


[2]: http://www.modrails.com/documentation/Users%20guide%20Apache.html

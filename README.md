Twitter EgoSearch Skype
=======================
search on Twitter and notify with Skype.

- https://github.com/shokai/twitter-egosearch-skype

Requirements
------------
- Ruby 1.9.3~2.0.0
- MongoDB 2.0
- Skype
- Mac OSX or Linux


Install Dependencies
--------------------

    % gem install bundler
    % bundle install


Setup
-----

### Twitter
twitter-egosearch-skype uses [Tw](http://shokai.github.io/tw/) to use Twitter API.

    % tw --user:add
    % tw --user:list

### Skype
get ID of Chat.

    % bundle exec ruby bin/show_chat_list.rb


### config.yml

    % cp sample.config.yml config.yml


Run
---

    % MONGOID_ENV=production bundle exec ruby bin/egosearch.rb

<!--
# DEFAULT README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
 -->

# Ruby on Rails Guru

## Installation
Before you install Rails, you should check to make sure that your system has the proper prerequisites installed. These include:
- Ruby
- SQLite3
- Node.js
- Yarn

```
ruby --version
sqlite3 --version
node --version
yarn --version

gem install rails
rails --version
```

## Creating the Blog Application
```
rails new blog
```

## Hello, Rails!
We actually have a functional Rails application already. To see it, we need to start a web server on your development machine.

```bash
# mac, linux
bin/rails server

# window
ruby bin\rails server
```

## Generation
To define a model, we will use the model generator:
```
bin/rails generate model Article title:string body:text
```

## References
- [Getting Started with Rails](https://guides.rubyonrails.org/getting_started.html)
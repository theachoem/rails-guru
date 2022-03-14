# Ruby on Rails Guru

## Installation
Before you install Rails, you should check to make sure that your system has the proper prerequisites installed. These include:
- Ruby
- SQLite3
- Node.js
- Yarn

```shell
ruby --version
sqlite3 --version
node --version
yarn --version

gem install rails
rails --version
```

## Creating the Blog Application
```shell
rails new blog
```

## Hello, Rails!
We actually have a functional Rails application already. To see it, we need to start a web server on your development machine.

```shell
# mac, linux
bin/rails server

# window
ruby bin\rails server
```

## Generation
To define a model, we will use the model generator:
```shell
bin/rails generate model Article title:string body:text
```

## Database
Migrations are used to alter the structure of an application's database.

```shell
bin/rails db:migrate
```

### Interact with database

```shell
bin/rails console
```

```
> article = Article.new(title: "Hello Rails", body: "I am on Rails!")
> article.save
> article

> Article.find(1)
> Article.all
```

## Migrate to PostgreSQL
1. Install PostgreSQL `gem install postgresql`
2. Update to `gem "pg"` in Gemfile
3. Change adapter to postgresql in `database.yml`
4. Install [PostgreSQL app](https://postgresapp.com/downloads.html)
5. Run following commands:
```shell
bundle exec rake db:create
bundle exec rake db:migrate
bundle exec rake db:seed
```

## References
- [Getting Started with Rails](https://guides.rubyonrails.org/getting_started.html)
- [Migrate to PostgreSQL](https://medium.com/@virtual_khan/converting-rails-from-sqlite3-to-postgresql-d97023314a14)
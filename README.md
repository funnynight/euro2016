### https://euro2016-predictor.herokuapp.com/

# Betting Portal

Betting portal made in Ruby on Rails. Project was discontinued in 2016.

![](https://i.imgur.com/8nDQCBC.png)

## Functionality

1. Adding matches (CRUD)
2. Adding teams (CRUD)
3. Login & register
4. Last predictions (bets) view
5. Matches list view
6. User profile view with predictions history
7. Single match view with pie chart how users predicted

## Getting started

To get started with the app, clone the repo and then install the needed gems:

```
$ cd /path/to/repos
$ git clone https://github.com/karlosos/euro2016.git euro2016
$ cd euro2016
$ bundle install --without production
```

Next, migrate the database:

```
rake db:migrate
```

And run server:

```
rails server
```

## Update 2022

Added `Dockerfile` in 2022 as it's not possible to run this app on newer OS because of some old dependencies.


Managed to run this app and install dependencies on Debian 8 (jessie) with Ruby 2.1 and Node 12. See Dockerfile. To build the app using docker run:

```
docker compose build
docker­-compose run rails-app rake db:reset
docker­-compose run rails-app rake db:migrate
docker compose up
```

Open http://localhost:3000 to access the app.

## Screenshots

![](https://i.imgur.com/RGhew79.png)
![](https://i.imgur.com/upC9qOC.png)



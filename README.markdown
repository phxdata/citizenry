Citizenry
=========

Citizenry is a simple, friendly web application for communities to keep track of the people, companies, groups, and projects that make them great. It was built to power <http://epdx.org/>, a guide to the awesome tech community of Portland, Oregon.

This particular fork was created to run entirely on Heroku

Installation
------------

1. Clone the app

```
git clone git://github.com/phxdata/citizenry.git
```

2. Push to Heroku

```
heroku create citizenry-app -s cedar
git push heroku master
``` 

3. Heroku setup

```
heroku run rake db:migrate
heroku config:add S3_KEY=1fad......
heroku config:add S3_SECRET=44sfad......
heroku config:add S3_BUCKET=unique-snowflake-bucket
```

4. Local setup

Make changes in `config/settings.yml`


Colophon
--------

League Gothic from the Leage of Movable Type
http://www.theleagueofmoveabletype.com/fonts/7-league-gothic



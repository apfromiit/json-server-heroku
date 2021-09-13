# Deploy `json-server` to `heroku`

## Deploy to **Heroku**

Place your json in `db.json`

### Install Heroku

$ `heroku login`

$ `heroku create`

$ `git push heroku master`

#### How it works

Heroku will look for a startup-script, this is by default `npm start` so make sure you have that in your `package.json`
```json
 "scripts": {
    "start" : "node server.js"
 }
```

# Deploy `json-server` to `heroku`

## Deploy to **Heroku**

Place your json in `db.json`

$ `heroku login`

$ `heroku create`

$ `git push heroku master`

## How it works

Heroku will look for a startup-script, this is by default `npm start` so make sure you have that in your `package.json`
```json
 "scripts": {
    "start" : "node server.js"
 }
```

## Notes

The changes to db are non persistent.<br>
json-server runs as in-memory database.<br>
Heroku free dyno goes idle when there is no web traffic for 30 minutes.<br>
Heroku will cold start with original db on next API call.

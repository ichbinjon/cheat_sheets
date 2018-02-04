# Express Cheat Sheet

## Get started quickly

`express myapp` creates a new express skeleton app.

`express -h` shows the other arguments you can pass on. (help)

`npm install` cd into directory then run this command to install dependencies.

`DEBUG=myapp:* npm start` to run it with debugging options

## Using nodemon for auto restart

`npm install --save-dev nodemon` to install locally

Then add devstart to package.json
```
"scripts": {
    "start": "node ./bin/www",
    "devstart": "nodemon ./bin/www"
  },
```

Run server with `DEBUG=express-locallibrary-tutorial:* npm run devstart`

## Mongoose
- run `mongod` on local machine at start of dev!

Object IDs are created automatically and not included in the schema. `_id` field

- `killall mongod` if you forgot to control C out of mongod

## Postman

sending JSON to POST
```
    {
        "max_members": 10,
        "gameID": "5a5a1ba3aae36e3ee87e6cb7",
        "name": "my lobby for me",
        "userID":
            "5a5a1a7cbddf503edebc857b"
    }
```

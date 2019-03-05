# tinyurlclone

A tinyurl.com clone example, with user authentication. Makes heavy use of [json-server](https://github.com/typicode/json-server "Get a full fake REST API with zero coding in less than 30 seconds (seriously)")

## Usage

    http://localhost:3000/abc

Issues a redirect to a long url referenced by the hash "abc".

    http://localost:3000/signin

Sign in to a user account.

    http://localhost:3000/signup

Sign up for a new user account

    http://locslhost:3000/users/:id

View user id account page, add urls, etc.

## Installation

    git clone https://github.com/tamouse/tinyurlclone.git
    npm install

## Development

### database

Data for `json-server` is in `./db.json`


### Start up the app server

    npm start

### Getting data:

```bash
$ curl http://localhost:3000/users/?username=jandoe
[
  {
    "id": 12,
    "name": "Jane Doe",
    "username": "jandoe",
    "password": "password"
  }
]
```

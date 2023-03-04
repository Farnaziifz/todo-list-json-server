# JSONServer TODO List + JWT Auth

expose API using json-server

## Install

```bash
$ npm install
$ npm run start
```

## How to login/register?

You can login/register by sending a POST request to

```
POST http://localhost:8000/auth/login
POST http://localhost:8000/auth/register
```

with the following data

```
{
  "email": "farnaz@farnaz.dev",
  "password":"farnaz"
}
```

You should receive an access token with the following format

```
{
   "access_token": "<ACCESS_TOKEN>"
}
```

You should send this authorization with any request to the protected endpoints

```
Authorization: Bearer <ACCESS_TOKEN>
```

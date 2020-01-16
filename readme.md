# node-auth
basic auth example built with express, express-session, mongo, mongoose

## register api test

```sh
curl -v -X POST localhost:3000/register \
-H 'Content-Type: application/json' \
-d '{ "email": "example@gmail.com", "name": "Example", "password": "testpw", "passwordConfirmation": "testpw" }'
```

## mongo shell login
```sh
docker exec -it node-auth_db_1 mongo -u admin -p secret auth-example
```
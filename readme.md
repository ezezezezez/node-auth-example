# node-auth
simple node auth example built with express, express-session, mongo, mongoose

## test

```sh
curl -v -X POST localhost:3000/register \
-H 'Content-Type: application/json' \
-d '{ "email": "example@gmail.com", "name": "Example", "password": "Testpw12", "passwordConfirmation": "Testpw12" }'

curl -v -X POST localhost:3000/login -H 'Content-Type: application/json' -d '{"email":"example@gmail.com", "password":"Testpw12"}'

curl -v -X POST localhost:3000/logout
```

## mongo shell login
```sh
docker exec -it node-auth_db_1 mongo -u admin -p secret auth-example
```
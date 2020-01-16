# node-auth

## curl

```sh
curl -v -X POST localhost:3000/register \
-H 'Content-Type: application/json' \
-d '{ "email": "alex@gmail.com", "name": "Alex", "password": "secret12", "passwordConfirmation": "secret12" }'
```

### docker exec -it node-auth_db_1 mongo -u admin -p secret auth-example
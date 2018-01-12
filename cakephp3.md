## Migrations
### Create tables
```
bin/cake bake migration create_users username:string email:string created modified
```
### Add columns token to table users
```
bin/cake bake migration add_token_to_users token:string
```
### Run migrate
```
bin/cake migrations migrate
```
### Rollback migrate
```
bin/cake migrations rollback
```

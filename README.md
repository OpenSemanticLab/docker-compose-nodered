Customizable docker container for node red

# Add modules

`nano /container/Dockerfile`

# Add users

`docker-compose exec nodered /bin/bash`


## Flow-Admin

`node-red admin hash-pw`

`nano node-red/data/settings.js`

```js
    adminAuth: {
        type: "credentials",
        users: [{
            username: "nodered-admin",
            password: "<password-hash>",
            permissions: "*"
        }]
    },
```

## Dashboard Users

`node-red admin hash-pw`

`nano node-red/data/settings.js`

```js
    httpNodeAuth: {user:"user",pass:"<password-hash>"},
    httpStaticAuth: {user:"user",pass:"<password-hash>"},
```

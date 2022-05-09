# Code Review

## Tickets to complete.
### This is linked to backend more
1. Create folder for backend genereal layout
    - api (folder)
        - subtress (files)
    - frontend (folder)
        - subtress (files)

2. knexfile.js
    - use config file to import database values (make more secure)
    ```ruby
    const creds = require'../config/creds.js'
    module.exports = {
    development: {
        client: "pg",
        connection: {
        host: creds.DB_HOST,
        port: creds.DB_PORT,
        database: creds.DB_NAME,
        user: creds.DB_USER,
        password: creds.DB_PASS,
        },
        migrations: {
        directory: "./db/migrations",
        },
        seeds: {
        directory: "./db/seeds",
        },
    },
    };
    ```
3. Add .gitignore file

## Conclusion
Overall goodwork just that role based functions is such as isAdmin role is being reduntent when the middleware is attach to route `try running console.log(req.user)` and add to payload the isAdmin data.
    
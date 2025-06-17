# todo-api-expressjs

A simple Todo API with Express.js and Static page.

## Quickstart

(1) Install [NodeJS](https://nodejs.org/en/download) if not yet installed

(2) Install dependant packages

```bash
npm install
```

(3) Run the app

```
node app.js
```

Expected output would be like this

```
Server is running on port 8080
```

Now you're ready to access the app (static-page)

```
curl http://localhost:8080
```

You can access the backend API directory. See the next section

## Testing APIs

Post todo

```bash
curl --location 'localhost:8080/todos' \
--header 'Content-Type: application/json' \
--data '{
    "title": "District Brand Technician"
}'
```

Put todo

```bash
curl --location --request PUT 'localhost:8080/todos/<ID>' \
--header 'cache-control: no-cache' \
--header 'Content-Type: application/json' \
--data '{
    "completed": false
}'
```

Delete todo

```bash
curl --location --request DELETE 'localhost:8080/todos/<ID>' \
--header 'origin: http://localhost:8080'
```

Get todo

```bash
curl --location 'localhost:8080/todos/<ID>'
```

Get all todos

```bash
curl --location 'localhost:8080/todos'
```

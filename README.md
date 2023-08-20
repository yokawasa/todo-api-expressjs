# todo-app-expressjs
Todo application with Express.js and static page. The project is still WIP ...
Base code comes from [here](https://quickstarts.postman.com/guide/express/index.html#0)

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
Server is running on port 3000
```

Now you're ready to access the app (static-page)

```
curl http://localhost:3000
```

You can access the backend API directory. See the next section


## Testing APIs

Post todo

```bash
curl --location 'localhost:3000/todos' \
--header 'Content-Type: application/json' \
--data '{
    "title": "District Brand Technician"
}'
```

Put todo

```bash
curl --location --request PUT 'localhost:3000/todos/<ID>' \
--header 'cache-control: no-cache' \
--header 'Content-Type: application/json' \
--data '{
    "completed": false
}'
```

Delete todo

```bash
curl --location --request DELETE 'localhost:3000/todos/<ID>' \
--header 'origin: http://localhost:3000'
```

Get todo

```bash
curl --location 'localhost:3000/todos/<ID>'
```

Get all todos

```bash
curl --location 'localhost:3000/todos'
```

## Todo for the project

- add more docs
- store data in mongoDB

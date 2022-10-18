# Test Task Backend

## Setup

```bash
# install dependencies
$ npm install
```

```bash
# run backend
$ npm run start
```

## Documentation

### Authentication:

```js
POST /login

{
  "email": "test@email.com",
  "password": "qwerty"
}
```

### Registration:

_You can access data without registration using login endpoint with default credentials above_

```js
POST /register

{
  "email": "any@email.com",
  "password": "any_pass"
}
```

### Tasks:

*Requires authentication token\**

```js
GET /tasks
```

Example response:

```js
[
  {
    id: 1,
    text: 'Learn how to make a perfect scrambled egg'
  }
]
```

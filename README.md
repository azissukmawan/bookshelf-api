
# Bookshelf REST API

this project as my learning in basic learning to make a REST API using the Hapi javascript framework, this storage is still stored in an array, if you want to use this project follow the instruction description below




## Description

Fitur

- Add book
- Get all books
- Get all books by filter
- Get book by specific
- Update book
- Delete book

API Endpoint - Task

- GET /books => get all books (include filter query params) ✅
- GET /books/:id => get a book ✅
- POST /books => create a book ✅
- PUT /books/:id => update a book ✅
- DELETE /books/:id => delete a book ✅


## API Reference

#### Get all books

```http
  GET /books?name=
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name` | `string` | **Required**. Display all books that contain the name based on the value given in the query |


```http
  GET /books?reading=
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `reading`      | `string` | **Required**. If 0, then display the book that is not being read (reading: false). If 1, then display the book being read (reading: true). In addition, display the book whether it is being read or not. |

```http
  GET /books?finished=
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `finished`      | `string` | **Required**. If 0, then display books that have not been read (finished: false). If 1, then display books that have been read (finished: true). In addition, display books either finished or unread. |




## Run Locally

Clone the project

```bash
  git clone https://github.com/azissukmawan/bookshelf-api.git
```

Go to the project directory

```bash
  cd bookshelf
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  # for those who use hosting
  npm run start

  # for development
  npm run start-dev
```


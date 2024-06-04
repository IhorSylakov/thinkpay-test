# Thinkpay test

## Task

Using any modern frontend framework (Angular/Vue/React/other; Vue is preferred), develop a frontend application that will interact with the backend and perform the following tasks:

1. **Display product list**
   - Display the list of products in a table.
   - Provide filtering capability by `code`, `name`, or `price` of the product.

2. **Forms for creating/updating/deleting products**
   - Implement forms for creating, updating, and deleting products.
   - Display validation error messages.

3. **Product details**
   - Load data of a specific product via the `/products/{id}` endpoint.
   - Display a product detail card with detailed information.

4. **Upload to Git repository**
   - Upload the solution to a Git repository (e.g., GitHub).
   - Write a brief instruction on how to build and run the project (`npm install`, `npm run`, etc.).

## Endpoints

API - [https://thinkpay-test-backend-b206f7f709a4.herokuapp.com/](https://thinkpay-test-backend-b206f7f709a4.herokuapp.com/)

| Method  | URL             | Description                                |
|---------|-----------------|--------------------------------------------|
| GET     | /products       | Retrieve the list of products              |
| POST    | /products       | Create a new product                       |
| GET     | /products/{id}  | Retrieve a product by ID                   |
| PUT     | /products/{id}  | Update a product with the specified ID     |
| DELETE  | /products/{id}  | Delete a product with the specified ID     |

## Product's structure

```json
{
  "id": 2,
  "name": "Масло",
  "code": "1234-1235",
  "price": 5,
  "created_at": "2019-06-13 19:58:04",
  "updated_at": "2019-06-13 19:58:04"
}
```

- `name` - required, must be a string.
- `code` - required, must follow the format ####-####, where # is a digit from 1 to 9.
- `price` - required, must be a numeric value.

## Check working app

#### Link

[https://ihorsylakov.github.io/thinkpay-test/](https://ihorsylakov.github.io/thinkpay-test/)

#### Preview

![App preview](https://raw.githubusercontent.com/IhorSylakov/IhorSylakov/main/repo-previews/thinkpay-test.webp)

## Build and Run Instructions

#### Project setup
```sh
npm install
```

#### Compiles and hot-reloads for development
```sh
npm run serve
```

#### Compiles and minifies for production
```sh
npm run build
```

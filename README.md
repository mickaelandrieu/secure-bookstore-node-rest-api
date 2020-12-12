# Book (Secure) Store Node.js (Express.js) REST API for learning purposes only

## Installation

```
git clone https://github.com/mickaelandrieu/secure-bookstore-node-rest-api.git
cd secure-bookstore-node-rest-api
npm i
```

## Security

HTTP Basic Auth has been enabled on this app, with 2 allowed users :
* ``john:superSecret``
* ``elise:12345678``

## Endpoints

### Books

* `/books`
* `/books/<isbn>`

### Users

* `/users`
* `/users/<mail>`

### Book Store management

* `/borrow/<mail>/<isbn>`: borrow a book from the book store as an user
* `/bring-back/<mail>/<isbn>`: bring back a book to the book store as an user

## Deploy on Heroku

Create [an account on Heroku](https://signup.heroku.com/) (Free/Hobby tiers is enough) and install [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli).

Then, execute the following instruction in the `secure-bookstore-node-rest-api` folder:

```
heroku login
heroku create
git push heroku master
```

And "voila", the REST API is deployed and ready to be tested.

This project is licensed under the [MIT license](https://opensource.org/licenses/MIT).

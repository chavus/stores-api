# STORES API

A simple API to create stores and items and add items on each store.

## Framwework
- Flask - flask_restful, flask_jwt, flask_sqlalchemy

## Demo API URL: https://chavus-stores-api.herokuapp.com/

## API doc

- GET /items: Returns the list of itmes.
- GET /item/<name>: Return an specific item identified by its name. No duplicated items with same name should exist.
- POST /item/<name>: Add a new item. If item already exists, it will fail
  - Body Example {"price": 1.95, "store_id":1 }
- PUT /item/<name>: Create a new item or update an exisiting one.
  - Body Example: { "price": 19 , "store_id":1}








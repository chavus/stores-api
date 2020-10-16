# STORES API

A simple API to create stores and items and add items on each store.

## Framwework
- Flask - flask_restful, flask_jwt, flask_sqlalchemy

## Demo API URL: https://chavus-stores-api.herokuapp.com/

## API doc

### Authentication
- POST /register: Register a new user to create, update and delete items and stores
  - Body Example: { "username": "jose", "password": "asdf" }
- POST /auth: Authenticates a registered user. Returns an access_token
  - Body Example: { "username": "jose", "password": "asdf" }

### Stores
- GET /stores: Returns the list of stores
- POST /store/<name>: Add a new store
- GET /store/<name>: Return an specific store identified by its name. No duplicated stores with same name should exist
- DEL /store/<name>: Delete a store uniquely identified by name
  
### Items
- GET /items: Returns the list of itmes.
- POST /item/<name>: Add a new item. If item already exists, it will fail
  - Body Example {"price": 1.95, "store_id":1 }
- GET /item/<name>: Return an specific item identified by its name. No duplicated items with same name should exist.
- PUT /item/<name>: Create a new item or update an exisiting one.
  - Body Example: { "price": 19 , "store_id":1}
- DEL /item/<name>: Delete an item uniquely identified by name











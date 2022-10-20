# Install dependency 

- go get github.com/gin-gonic/gin

# To run this code 

- go run main_api.go

# Run this code after server is up.

## To view all books
- curl localhost:8080/books

## To update books
- curl localhost:8080/books --include --header  "Content-Type:application/json" -d @book.json --request "POST"

## To Checkout book
- curl localhost:8080/checkout?id=2 --request "PATCH"

## To Return book
- curl localhost:8080/return?id=2 --request "PATCH"

# gin-bun-contacts-api

A simple CRUD contacts API implemented in golang with [Gin](https://gin-gonic.com/) and [Bun](https://bun.uptrace.dev/)

## Architecture

### Why Gin?

It is more declarative and better to write `engine.GET("/path/to/return")` than the code incantations in Gorilla Mux or the built-in "net/http" package.

### Why Bun?

We have to be careful here - ORMs are notorious, but having an expression language for your selects, inserts, and 
updates means that your SQL is known to be good, and doesn't need as careful testing. Especially with a type safe
language like Go, you have less potential for runtime issues.  With a small database like this, it doesn't matter.
The point of using the Bun DML expression language here is to learn it for larger projects.

## Packages


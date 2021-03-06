# Node to Postgres Lecture

This expands upon the first node-books assignment.

---

Covers creating a CRUD application with Node/Express and PostgreSQL.

## Takeaways

* You can connect to your Postgres database using the `pg` module
* You need to know the URI for the database (see `connectionString` in server/routes/books.js)
* Use `pg.connect(...)` to connect to the database
* Use `client.query(...)` to query the database with SQL
* When creating queries with client-submitted data, always use the prepared statement pattern (see router.post in server/routes/books.js)
* Use optional paramaters with your Express routes. IE: `router.put('/:id', function(req, res) { ... });`

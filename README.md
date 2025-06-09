# go-dbpool-example
This is code sample for article : https://novrian.substack.com/publish/post/165523361

If we are talking application that is scalable and high performance, an Efficient database access is essential. One of the methods to improve database efficiency is through Database Connection Pooling, commonly referred to as DBPool. In this article, we will walkthrough what DBPool is, its value, and how to implement it in Go using the database/sql package and PostgreSQL.

What is DBPool?

DBPool is a technique used to manage and reuse a pool of database connections. In contrast with opening and closing a new connection for every request. In the later, each query creating a new connection (which is expensive), DBPool maintains a pool of open connections that can be reused across multiple database operations.

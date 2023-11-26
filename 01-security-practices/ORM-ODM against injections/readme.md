# ORM-ODM against injections

- There are chances that whenever we run database query using data from client like create user or update products there are chances that client inputs can have malicious code in it, And that malicious code can be sql injection or nosql injection.
- To prevent this we use ORM or ODM like `mongoose` or `sequlize` which makes database query simpler and also sanitize query to prevent any vulnerability.

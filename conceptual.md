### Conceptual Exercise

Answer the following questions below:

- What is RESTful routing?
- The client/server relationship is a prerequisite of a set of principles known as REST(representational state transfer) which provides a way of mapping HTTP verbs ( get, post, put, delete) and CRUD actions (create, read, update, delete) together

- What is a resource?
- A resource is an object sent by the server that correspoinds to a specific format to the client.

- When building a JSON API why do you not include routes to render a form that when submitted creates a new user?
- There is no reason to use render or redirect because building a JSON API passes the information from the route to a JSON dictionary in postgrSQL via POST.

- What does idempotent mean? Which HTTP verbs are idempotent?
- Idempotent means that the result is the same no matter how many times it is requested. However, the data requested CAN be changed. GET, PUT/PATCH, and DELETE are idempotent because the state of the server will always be the same after the HTTP verb occurs.

- What is the difference between PUT and PATCH?
- PUT updates the entire server while PATCH updates a small part of it.

- What is one way encryption?
- One way encryption is when only the user who created the account has access to the password itself non-reversibly. That way a company doesn't store the exact password in its database. However, a company can verify the password as the same input must always have the same output.

- What is the purpose of a `salt` when hashing a password?
- Adding a 'salt' when cryptographically hashing a password gives a user a unique starting sequence that unpredictably changes the output. Salt can be used by a company to look up a password in its database. But because the hashed password is different every time, there is no way of accessing what the hashed password actually translates to.


- What is the purpose of the Bcrypt module?
- Bcrypt is a way to cryptographically hash a password. It is intentionally designed to be slow so that it makes it tougher to hack. One tool utilized in Bcrypt is to designate a work factor, how many rounds of encryption you want.

- What is the difference between authorization and authentication?
- authentication is the process of verifying who someone is, whereas authorization is the process of verifying what specific applications, files, and data a user has access to.

# Endpoints

## Resources:
1. Books
2. Users
3. Admins

---

#### 1. Books

- `POST /books` -  create new book
- `GET /books/id` - find book by id
- `PUT /books/id` - update book by id
- `PATCH /books/id?query_param=` - patch book by id 
- `DELETE /books/id` - delete book by id
- `GET /books/filter?query_param=` - list of books after performing custom filters

---

#### 2. Users
- `POST /users` - creates new user
- `GET /users/id` - find user by id
- `PUT /users/id` - update user by id
- `PATCH /users/id?query_param=` - patch user by id
- `DELETE /users/id` - delete user by id
- `GET /users` - list of users
- `GET /users/id/issues` - list of borrowed books by user id
- `GET /users/id/notifications` - list of notifications by user id
- `GET /users/id/messages` - list of messages by user id
- `POST /users/id/notifications` - send new notification
- `POST /users/id/messages` - send new message 
- `GET /users/login` - returns user if exists
---

#### 3. Admins
- `POST /admins` - creates new admin
- `POST /admins/intimation` - creates live intimation of viewed books

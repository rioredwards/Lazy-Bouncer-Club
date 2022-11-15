# Lazy Bouncer Club

## Getting Started

Use [this template](https://github.com/alchemycodelab/backend-lazy-bouncer) to get started.

### Learning Objectives

- Use Express middleware to ensure requests are authenticated
- Use Express middleware to provide user-based authorization
- Use cookies to store user data
- Use JWTs for storing user data in cookies
- Sign & verify JWTs to ensure validity

### Description

A local underground dance club wants a service for managing memberships. They want their patrons to sign up using the service in order to gain access to the club.

Luckily for them, one of the club's bouncers knows a thing or two about software development and has built out an initial API. However, they are struggling with implementing authentication and didn't want to spend time learning how to do it.

Your task is to finish securing the API by building out the necessary middleware for authentication and authorization, as well as adding protection to the existing routes.

### Acceptance Criteria

- Only authenticated users can `GET` `/api/v1/users/me`
- Only the user with the `email` of `admin` can `GET` `/api/v1/users`
- `authenticate` middleware checks the session cookie for a valid JWT and assigns the payload to `req.user`

### Rubric

| Task                                                                          | Points |
| ----------------------------------------------------------------------------- | ------ |
| `authenticate` middleware implemented                                         | 2      |
| `authorize` middleware implemented                                            | 2      |
| GET `/api/v1/users/me` is only accessible to logged in users                  | 2      |
| GET `/api/v1/users` is only accessible to the user with a username of `admin` | 2      |
| Existing tests pass (remove .skip from each test)                             | 2      |

Prerequisites
Node.js and npm installed
MongoDB installed and running

Install dependencies
npm install

Fill in .env file

Usage
Endpoints
/user/register - Register a new user

/user/login - Log in to the application and receive an access token

/user/logout - Log out and clear the access token

/user/deleteAccount/:id - Delete a user account

/user/updateUsername/:id - Update a user's username

/user/updatePassword/:id - Update a user's password

/user/protected - A protected route that requires a valid access token

/post/posts - Get all posts

/post/posts/:id - Get a specific post

/post/posts - Create a new post (requires authentication)

/post/posts/:postId - Update a post (requires authentication)

/post/posts/:postId - Delete a post (requires authentication)

/comment/comment - Get all comments

/comment/comment/:id - Get comments for a specific post

/comment/comment/:postId - Create a new comment (requires authentication)

/comment/comment/:postId - Update a comment (requires authentication)

/comment/comment/:postId - Delete a comment (requires authentication)

Authentication
The application uses JSON Web Tokens (JWT) for authentication.
The access token is required for protected routes and should be included in the Authorization header.
Refresh tokens are not implemented in this example but can be added for a more secure authentication flow.

Running
npm run start or npm run dev
# JWT blacklisting

- If we have banking system or any highly vulnerable system then we need to implement JWT blacklisting.
- JWT lives in client any there is no way to revoke this in server. i.e. if any of our jwt is compromised and we don't want to use that same jwt again we blacklist that jwt token.
- It hand to do this, there is one way to do this is by storing jwt in our database. if jwt built in expiration get expired we revoke that jwt from database.

- So to do this we have to store 2 token into client side.

  - Access token
  - Refresh token

- Here access token is short lived token and refresh token is long lived token.
- When access token get expired we use refresh token to get new access token.
- We store that refresh token in our database and we match that whenever we get request from client.

What is a token?

A token is a temporary digital key that proves you are authenticated.

Instead of sending email + password on every request, the server gives you a token after login.

You then use that token to access protected endpoints.

Why we need it:

• Security — password is not sent repeatedly

• Performance — no need to re-check credentials every time

• Stateless architecture — server doesn’t store session in memory

---

Basic flow

1. User logs in with email/password
    
2. Server validates credentials
    
3. Server generates token(s)
    
4. Client stores token
    
5. Client sends token in Authorization header for protected requests
    

  

Example header:

  

Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9…

---

Main token types (what you must know as QA)

1. Access Token
    
    Short-lived (e.g. 5–15 minutes)
    
    Used to access protected APIs
    
2. Refresh Token
    
    Longer-lived (days/weeks)
    
    Used only to request a new access token
    

  

Access token = enter the building

Refresh token = get a new badge without showing passport again

---

Why 2 tokens?

  

If access token is stolen → damage is limited because it expires quickly.

Refresh token is usually stored more securely and validated strictly.

---

Where tokens live

  

Web:

• LocalStorage or SessionStorage

• HttpOnly secure cookie (more secure)

  

Mobile:

• Secure storage (Keychain / Keystore)

---

What is inside a token?

  

Often JWT (JSON Web Token). It contains:

  

• user id

• roles

• expiration time

• signature

  

Server verifies signature to ensure token was not modified.

---

What you must understand as manual QA:

  

• Token has expiration

• Token can be invalid

• Token can be missing

• Token can be malformed

• Token can belong to another user

• Token must not give access after logout
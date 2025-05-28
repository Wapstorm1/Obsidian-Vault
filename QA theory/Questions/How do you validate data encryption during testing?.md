To ensure data encryption is implemented correctly and securely, follow these steps:

**1. Understand the Encryption Requirements**
• Identify sensitive data to be encrypted (e.g., passwords, credit card details).
• Understand encryption methods used (e.g., AES, RSA, hashing).


**2. Verify Data in Transit**
• Use tools like **Wireshark** or **Fiddler** to capture network traffic.
• Ensure sensitive data is transmitted over secure protocols (e.g., HTTPS, TLS).
• Verify the data is encrypted and cannot be read in plain text.

**3. Validate Data at Rest**
• Query the database directly to check that sensitive fields (e.g., password, credit_card) are encrypted.
• Look for unreadable values (e.g., hashed or ciphertext).
• Example Query:


```
SELECT password FROM users WHERE id = 1;
Expect hashed/encrypted value like: $2a$10$... instead of 'mypassword'

```


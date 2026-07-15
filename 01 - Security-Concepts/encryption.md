# Encryption

## Overview

Encryption is the process of converting information into a coded format to prevent unauthorized access. It is a fundamental security control used to protect sensitive data both at rest and in transit.

In a Zero Trust security model, encryption helps ensure that even if an attacker gains access to a network, device, or storage system, the protected data remains unreadable without the appropriate decryption keys.

---

## Why Encryption Matters

Organizations use encryption to:

- Protect sensitive data from unauthorized access.
- Secure communications between systems and services.
- Reduce the impact of data breaches.
- Support regulatory and compliance requirements.
- Strengthen defense-in-depth security strategies.

---

## Encryption in Zero Trust

One of the core principles of Zero Trust is **Assume Breach**.

Rather than trusting internal networks automatically, organizations operate under the assumption that attackers may already be present. Because of this, sensitive information should remain protected regardless of where it is stored or transmitted.

Examples include:

- Encrypting files stored in databases and storage accounts.
- Encrypting communications between services.
- Protecting data even when it moves within the same datacenter. 

---

## Hashing

Hashing uses cryptographic algorithms to generate a fixed-length value from input data.

Unlike encryption, hashing is a **one-way operation**, meaning the original data cannot be recovered from the resulting hash.

Hashing is commonly used to:

- Verify data integrity.
- Detect unauthorized changes.
- Securely store passwords. 

### Example

```text
Password: MySecurePassword

Hash:
8f434346648f6b96df89dda901c5176b10a6d83961fca836c48cb41557cf50a9
```

### Hashing Workflow

```text
Plain Text
    ↓
Hash Function
    ↓
Hash Value
```

---

## Salting

A **salt** is a unique random value added to a password before hashing.

Using salts ensures that identical passwords generate different hash values, making password attacks significantly more difficult.

### Benefits

- Prevents the use of precomputed rainbow tables.
- Protects users with identical passwords.
- Increases password storage security. 【1-ca0de4】

### Salting Workflow

```text
Password
    +
Unique Salt
        ↓
      Hash
        ↓
Store Hash + Salt
```

---

## Peppering

A **pepper** is a secret value added during the hashing process.

Unlike salts, peppers are not stored alongside user records. Instead, they are kept in a secure location such as a secrets vault or protected configuration store.

### Benefits

- Adds an extra layer of protection.
- Helps protect credentials even if a database is compromised.
- Reduces the effectiveness of offline password attacks.

### Peppering Workflow

```text
Password
    +
Salt
    +
Pepper
        ↓
      Hash
```

---

## Work Factors

A **work factor** increases the computational effort required to generate a hash.

This is achieved by performing additional hashing iterations, making brute-force and dictionary attacks more expensive and time-consuming.

### Benefits

- Slows down password-cracking attempts.
- Increases resistance against automated attacks.
- Improves overall credential security. 

---

## Security Best Practices

### Recommended

- Encrypt sensitive data at rest and in transit.
- Use strong cryptographic algorithms.
- Store passwords using hashing, not encryption.
- Generate a unique salt for every password.
- Store peppers separately from the database.
- Apply appropriate work factors to password hashes. 

### Avoid

- Storing passwords in plain text.
- Reusing salts across multiple users.
- Keeping peppers inside the same database.
- Using weak or outdated cryptographic algorithms. 

---

## Key Takeaways

- Encryption protects data from unauthorized access.
- Hashing provides integrity verification and secure password storage.
- Salting prevents identical passwords from producing identical hashes.
- Peppering introduces an additional secret layer of protection.
- Work factors increase the cost of password attacks.
- Encryption is a critical component of the Zero Trust security model.
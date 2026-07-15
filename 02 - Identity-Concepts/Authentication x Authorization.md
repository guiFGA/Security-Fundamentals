# Authentication vs Authorization

## Overview

Authentication and Authorization are two fundamental concepts in identity and access management (IAM). Although they are closely related, they serve different purposes.

- **Authentication (AuthN)** verifies who a user is.
- **Authorization (AuthZ)** determines what an authenticated user is allowed to do. 

A simple way to remember the difference:

> Authentication answers **"Who are you?"**
>
> Authorization answers **"What are you allowed to do?"** 

---

# Authentication (AuthN)

## What is Authentication?

Authentication is the process of verifying the identity of a user, device, or application before granting access to a system.

The goal is to prove that the entity requesting access is really who it claims to be. 

### Common Authentication Methods

- Username and password
- Multi-Factor Authentication (MFA)
- Biometrics
- PIN codes
- Security tokens
- Windows Hello
- Authenticator applications 


### Example

When you sign in to Microsoft 365 using your email address and password, the system verifies your identity before allowing access.

Another example is signing into a third-party application using your Google or Microsoft account. 

---

# Authorization (AuthZ)

## What is Authorization?

Authorization is the process of determining what resources and actions an authenticated user can access.

Authorization occurs **after authentication**.

Once the identity has been verified, the system evaluates permissions, roles, and policies to determine the appropriate level of access. 


### Example

A user successfully signs in to an application:

- An employee can view reports.
- A manager can approve requests.
- An administrator can manage users.

All three users are authenticated, but each receives different permissions based on authorization rules. 【1-8c0634】

---

# Authentication vs Authorization

| Authentication | Authorization |
|---------------|--------------|
| Verifies identity | Determines permissions |
| Answers "Who are you?" | Answers "What can you do?" |
| Happens first | Happens after authentication |
| Uses credentials | Uses roles, permissions, and policies |
| Focuses on identity | Focuses on access control |

---

# Key Takeaways

- Authentication verifies an identity.
- Authorization determines permissions.
- Authentication always occurs before authorization.
- MFA strengthens authentication security.
- RBAC simplifies authorization management.
- Least Privilege reduces security risks.
- Both Authentication and Authorization are essential components of the Zero Trust security model. 【1-8c0634】
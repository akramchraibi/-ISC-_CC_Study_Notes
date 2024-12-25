
## Access control process
Triple-A (AAA) -> Identification, Authentification, Authorization + Accounting.


### Identification 
During this first step, an individual makes a claim about their identity (Might be false)

### Authentification
Once the claim is made, the second step is to prove it (by providing ID for example)

### Authorization
Proving who you are doesn't mean u have access to systems, u need to be *ALLOWED* to have access to that system/data/place.

### Accounting
Logging of activity and access to data/systems/places.

___
### Digital Access Control
In the electronic world, authorization takes form as **Access Listes** that give access to a person or a group of people once a ressource is solicited. 

It also does the logging and the tracking (Privacy laws still have to apply)

___
## Password Policies
Requirement for users to follow to choose and maintain their passwords.

### Password length
### Password complexity
### Password expiration
A policy that requires a change of password every time a set amount of time has passed.
### Password History
A history of a user's previous passwords is used to prevent them from reusing the same password multiple times.
### Password Reset
A way to let users reset their password as will or if it compromised. If not implemented well, it could be a way an attacker can gain access.
### Password Reuse
When a user has the same password on multiple sites. hard to enforce but if an attacker gets access to that other site that shares the password, they can use it on yours and gain access.
### Password Managers

___
## Authentification Factors
Ways to prove identity : 
- **Something you Know**
- **Something you Are**
- **Something you Have**

### Something you Know
Most common. eg; Password, pin, security questions...
### Something you Are
Biometrics
### Something you Have
A badge, a Smartphone with an electronic Token, key fob...

### Multi-Factor Authentification
Combining between the ones above (2 or more) because none of them are fool proof.
___
## Summary
1. The access control process consists of three major steps. Identification is when a user makes a claim of identity. Authentication is when the user proves that identity claim. Authorization is when the system determines whether the user is allowed to perform a requested action.
2. Accounting processes create a record of who performed which actions on a system and are useful when investigating security incidents. 
3. Multi-factor authentication combines at least two of the three factors: something you know, something you have, and something you are.
4. Password length requirements set a minimum number of characters that must be in a user’s password, whereas password complexity requirements mandate the use of different character types.
5. Password history requirements prevent the reuse of old passwords, whereas pass- word expiration requirements force the periodic reset of existing passwords. Users should be permitted to reset their passwords whenever they wish.
6. Users should be encouraged not to reuse passwords across multiple sites, as this increases the risk of compromise. Password managers provide a convenient tool for managing many unique, strong passwords.
--- 
# Exam tip
When you take the CC exam, you’ll likely find a question about multi-factor
authentication. Be careful to ensure that the authentication techniques come
from two different factors. Mistaking two “something you know” techniques for
multi-factor authentication is a common exam mistake!
 
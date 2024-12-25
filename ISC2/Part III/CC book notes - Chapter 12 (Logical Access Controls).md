## Authorization
### Least Privilege
It limits internal attacks if an employee turns malicious, it also protects against external attacks in the sense of if someone's system gets compromised the attacker can't get too far.
### Segregation of duties
The segregation of duties principle says that no single person should possess two permissions that, in combination, allow them to perform a sensitive operation. Instead, those permissions should be segregated and held by two different people. Account reviews and audits should inspect permissions to ensure that segregation of duties is properly enforced.
Segregation of duties is a key control in accounting to prevent fraud, such as creating fake vendors and issuing unauthorized payments. By separating the responsibilities of creating vendors and authorizing payments, no single employee can commit fraud alone, reducing the risk of embezzlement without collusion. Information security professionals play a role in enforcing these controls by configuring access systems.
In IT, segregation of duties applies to software development, where developers are not allowed to deploy their own code. Instead, code is submitted for testing and evaluation, and only a separate individual can move it into production after it passes security and functionality checks.
### Authorization model
#### Mandatory Access control (MAC)
Most restrictive, the permissions are managed by the OS based on labels on users and objects, not even system admins can change the permissions. They're rarely fully implemented besides on highly secured facilities.
#### Discretionary Access control (DAC)
Most Common. Users who own files / equipment have the discretion to allow other user to use/modify their property.
![[Pasted image 20241209203935.png]]
#### Role-Based Access Control (RBAC) 
IT admin assigns permissions to roles and those roles can then be distributed to people based on what kind of work they do.

> [!note]
> When designing an access control system, you need to select the approaches that best balance security requirements and business needs in your organization. On the one hand, if you choose a system that is not strict enough, you might unintentionally jeopardize your security. On the other hand, however, if you choose a system that is too strict, you might make it too difficult for people to get their work done.

> [!important] Concept not covered by the book
> ***Role explosion***
> If one employee requires access to ten applications or services with two roles per application, the number of roles being managed for this single employee is twenty. As the number of applications and systems used in enterprises grows across the organization the number of roles can reach hundreds or thousands.
> ***Attribute-based access control***
> Attribute-based access control, also known as policy-based access control for IAM, defines an access control paradigm whereby a subject's authorization to perform a set of operations is determined by evaluating attributes associated with the subject, object, requested operations, and, in some cases, environment attributes.
> ***Dynamic access control***
> Dynamic access control refers to the ability of an access control system to automatically adjust permissions based on certain triggers or changes in context. An employee's access being automatically revoked upon their transfer to a different department exemplifies this, as the system dynamically responds to changes in the user's role or status within the organization
> ***Role mining***
> Role mining involves analyzing user behavior patterns and access logs to define new roles that accurately reflect actual access needs and operational practices. This process can help optimize the RBAC system by ensuring that roles are both efficient and aligned with real-world usage.

## Account Type
### User Account
Typical user account for like all employees from receptionist to CEO. They might have different permissions though.
### Admin Account
Highly sensitive, you can break stuff with it unintentionally that's why most IT admins have regular account that they used and only elevate their privileges when needed. Also very bad if it gets compromised. Also a lot of logging and detection of potential threats on these and we use ***privileged account management (PAM)***.
### Guest Account
Give to guest for example when they want WIFI.
### Shared / Generic Account
Bad idea, no use.
### Service Account
Used by a service or an app, typically has elevated privileges and must therefore be monitored constantly.

## Non Repudiation
Non-­repudiation is a security goal that prevents someone from falsely denying that something is true.
We use *digital signatures*. Digital signatures use encryption technology to provide non­repudiation for electronic documents.
There are other ways that you can provide non-­repudiation as well. You might use bio-
metric security controls, such as a fingerprint or facial recognition, to prove that someone
was in a facility or performed an action. You might also use video surveillance for that same
purpose.

# Exam Essentials
- Non-­repudiation uses technical measures to ensure that a user is not able to later deny that they took some action.
- The principle of least privilege says that users should have only the minimum set of privileges necessary to carry out their job responsibilities.
- the segregation of duties principle says that no single person should possess two permissions that, in combination, allow them to perform a sensitive operation.
- Mandatory access control (MAC) systems are the most stringent type of access control. In MAC systems, the operating system itself restricts the permissions that may be granted to users and processes on system resources.
- Discretionary access control (DAC) systems allow users to assign access permissions to other users—­the owners of files, computers, and other resources have the discretion to configure permissions as they see fit.
- In role-­based access control (RBAC) systems, administrators assign users to roles based upon their job responsibilities and assign the permissions necessary to carry out different jobs to those roles.
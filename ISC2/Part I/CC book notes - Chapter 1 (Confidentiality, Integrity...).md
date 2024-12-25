## Three primary objectives
- Confidentiality 
- availability
- integritycours
![[Pasted image 20241126103652.png]] 

### Confidentiality 
Confidentiality ensures that only authorised individuals have access to information and resources.

#### Confidentiality risks
- Snooping : when someone can wander around the office and can access information left by mistake on desks or elsewhere public.
	- Protection : Clean desk policy
- Dumpster Diving : When someone goes through the trash to find documents.
	- Protection : shredder
- Eavesdropping : Overhearing conversations or wiretapping.
	- Protection : Encryption for Wiretapping and limiting where confidential convos can have place.
- Social Engineering : Psychological tricks to get access to data.
	- Protection : Educate employees about this kind of attack.

### Integrity
Protecting the data from being altered by unauthorised people.

#### Integrity Risks
- Unauthorised Modification of Information : When an attacker gains access to a system and makes changes that violate the security policy
- Impersonation : When an attacker pretends to be someone else to have access and change data.
	- This is an extension of social engineering and the best way to mitigate it is to educate people.
- Man-in-the-Middle Attacks : When someone positions themselves between a user and a system and can gather or change information.
- Relay Attacks : An attacker finds a way to record or observe an employee logging into the network, captures and replays that process for them to get access.
	- For both Relay and Man-in-the-Middle attacks, best way defence is encryption.


### Availability
Availability controls ensure that information and systems remain available to authorized
users when needed.

#### Availability Risks
- DOS : Attacks that occur when a malicious individual bombards a system with an overwhelming amount of network traffic.
	- Protect using a firewall or partnering with ISP to block malicious trafic before reaching our network.
- Power Outages : Power = No more
	- remediate using redundant power sources and backup generators.
- Hardware Failure : when an equipment fails.
	- protect using redundancy
- Destruction of Equipement : when hardware is destroyed intentionally or unintentionally.
	- small scale : redundancy ; large scale : a backup data center in a remote location.
- Service Outages : This is due to programming errors or failure of equipment...
	- Buying / building resilient systems.

## Non-Repudiation
Non-repudiation is a security goal that prevents someone from falsely denying that something is true.
You can provide this by using Digital Signatures, bio-metrics, video surveillance... 

---
## SUMMARY
1. The CIA triad references the three main goals of information security: confidentiality, integrity, and availability.
2. Confidentiality protects sensitive information from unauthorized access. The major threats to confidentiality include snooping, dumpster diving, eavesdropping, wiretapping, and social engineering.
3. Integrity protects information and systems from unauthorized modification. The major threats to integrity include the unauthorized modification of information, impersonation attacks, man-in-the-middle attacks, and replay attacks.
4. Availability ensures that authorized users have access to information when they need it. The major threats to availability include denial-of-service attacks, power outages, hardware failures, destruction of equipment, and service outages.
5. Non-repudiation uses technical measures to ensure that a user is not able to later deny that they took some action.

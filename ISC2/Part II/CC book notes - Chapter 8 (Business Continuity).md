## Definition
Business Continuity planning is the discipline of planning for an eventual small scale catastrophe (either natural or human made) and ways to keep the business running in the meanwhile.
The focus of business continuity is keeping operations running, so BCP is sometimes
referred to as continuity of operations planning (COOP).

## BCP Scope
Can't plan for everything so must define a scope.
- **Which business activities will the plan cover?**
- **What types of systems will the plan cover?**
- **What types of controls will the plan consider?**

## Business impact analysis
It's a backwards process that helps security professionals identify the most important IT infrastructure. We start by identifying the core missions of the company and then we retrace our steps to get to the IT infrastructure that supports these core missions.
We then do a risk assessment and we list it in descending order as so :

| Risk                                | Annualized risk assessment |
| ----------------------------------- | -------------------------- |
| Hurricane damage to the data center | $145,000                   |
| Fire in data center                 | $18,000                    |
| Power outage                        | $12,000                    |
| Theft of equipment                  | $3,400                     |
in a cloud centric environment, collaboration between companies to achieve this sort of things is important
## Business Continuity Controls
Just make sure stuff is redondant and fault tolerant.

### Single point of failure analysis
just see where you can do redondant stuff and do it (Links, tools, machines...)

### Other continuity risks
- Sudden bankruptcy of a key vendor
- Inability to provide the requisite computing or storage capacity
- Utility service failures
- Any other risk that IT management believes may disrupt operations
- Personnel succession to the IT professionals that take care of your systems

## High Availability and Fault Tolerance
### High Availability
The core concept of high availability is having operationally redundant systems, sometimes at different sites.

### Fault Tolerance
Protect systems against failure by using redondant devices especially : 
- Power supply
- Storage media
- Networking components
#### Power Supply
![[Pasted image 20241208125848.png]]

You plug both and when fails the other continues to power the server uninterrupted.
Data centers use *uninterruptible power supplies (UPS)* to provide battery power to systems in the event of a brief disruption.
![[Pasted image 20241208130243.png]]
*power distribution units (PDUs)* are used to manage the power within the rack, making sure clean and well managed.

#### Storage
This is achieved through the use of a technology known as redundant arrays of inexpensive disks (RAID).
##### RAID level 1
Disk replication
![[Pasted image 20241208130541.png]]

##### Disk Striping with Parity (RAID 5)
segmentation and replication on different disk.
![[Pasted image 20241208130857.png]]
P one has parity information, it knows where everything is.

> [!note] Exam Tip
> One important thing to remember: RAID is a fault tolerance strategy designed to protect against a single or double disk failure, depending on the RAID level. It is not a backup strategy. You should still perform regular data backups to protect your organization’s information in the event of a more catastrophic failure, such as the physical destruction of the entire server.

#### Networking Component
Just make everything redondant from ISPs to cables.

#### Redundancy Through Diversity

# Exam Essentials
- Business continuity efforts are activities designed to keep a business running in the face of adversity. The business impact analysis (BIA) is an impact assessment that begins by identifying the organization’s mission-­essential functions and then tracing those backward to identify the critical IT systems that support those processes.
- Single point of failure analyses identify places where the failure of one component could cause an entire system or service to become unavailable.
- High availability (HA) uses multiple systems to protect against failures. Fault tolerance (FT) helps to protect a single system from failing in the first place by making it resilient in the face of technical failures.
- Three of the components most likely to fail in a computer system are the power supply, storage, and network connection.
## Disaster recovery planning
Disaster recovery plans (DRPs) may include immediate measures that get operations working again temporarily, but the disaster recovery efforts are not finished until the organization is completely back to normal.

### Types of Disasters
The disaster recovery plan can be triggered by an environmental natural disaster, such as a hurricane, a technological failure, such as a power outage, a health emergency, such as a pandemic, or a hazard caused by humans, such as a ransomware attack.
The source of a disaster or hazard may be internal to the organization, such as a data center failure, or external, such as a supply chain disruption. In any case, the organization must quickly recognize the circumstances and activate its corresponding disaster recovery plan.

### Initial response
#### Staffing
During a disaster recovery effort, organizations shift focus from regular operations to restoring functionality quickly. Employees often take on temporary roles different from their usual duties, emphasizing the need for flexibility. To prepare for such situations, organizations should assign disaster recovery responsibilities in advance and provide appropriate training to ensure readiness.

#### Communication
Employees must have secure and reliable mean to communicate with the hierarchy even after hours and especially is a disaster occurs.

### Assessment
Once the immediate danger passes, the disaster recovery team shifts to identifying the extent of the damage and start putting in place a plan for remediation.

### Disaster recovery Metrics
- ***The recovery time objective (RTO)*** is the targeted amount of time that it will take to restore a service to operation following a disruption.
- ***The recovery point objective (RPO)*** is the maximum time period from which data may be lost as a result of a disaster.
- ***The recovery service level (RSL)*** is the percentage of a service that must be available during a disaster.

> [!note] Exam Tip
> Remember, disaster recovery efforts conclude only when the organization is back to normal operations in its primary operating environment.

### Training and Awareness
Training and awareness are essential for an effective disaster recovery plan. Personnel involved should receive regular training on their roles, along with frequent awareness programs to keep their responsibilities fresh in mind.

## Backups
### Backup Media
#### Tape Backups
Linear Tape-­Open (LTO) tapes, Old stuff, still used but really not so much because other means got cheaper and cheaper also they're hard to manage.
![[Pasted image 20241208135235.png]]
#### Disk Backup
On site or outside it, just disks where we backup data. also NAS and SAN stuff.
#### Cloud Backups
AWS and stuff, great geographical diversity and great prices.

### Backup Types
#### Full Backups
#### Differential and Incremental Backups
Differential just makes copies of files that changed since the last full backup. Incremental They include only those files that have changed since the most recent full or incremental backup.
### Backup Scenario
In this example, Joe, a storage administrator, performs full backups every Sunday and differential backups on weekdays. If the system fails on Friday, Joe would first restore the last full backup from Sunday and then the most recent differential backup from Thursday, which contains all changes since Sunday.
If Joe switches to incremental backups, he would still start with the full backup from Sunday but would need to apply each incremental backup (from Monday to Thursday) in sequence. While incremental backups save storage space, the restoration process takes longer since multiple backups must be applied.

## Disaster Recovery Sites
#### Hot Sites
Full on backup Data center, fully equiped, SO EXPENSIVE, but basically the holly grail of disaster recovery sites.
#### Cold Sites
Just a empty space with data center racks that can get operations running after A LOT OF TIME. Cold sites are far less expensive than hot sites, but activating them can take weeks or even months.
#### Warm Sites
Equipped data center but not active, so BIG price for equipment but no IT staff necessary.
#### Offsite Storage
Disaster recovery sites serve as both operational facilities and offsite storage for business data. Storing backups at a secure, geographically distant location ensures protection against local disasters. This is part of site resiliency planning. Data can be physically transported or digitally transferred through site replication. When planning offsite backups, organizations must decide between online backups, which are quickly accessible but costly, and offline backups, which are cheaper but require manual restoration.
#### Alternate Business Processes
We can also change how we work. For example switching to paper based processing when systems are down.

## Testing disaster recovery plans
1. To validate that the plan functions correctly and that the technology will work in the event of a disaster
2. To provide an opportunity to identify necessary updates to the plan due to technology or business process changes
There's 5 types of tests :
#### Read-­Throughs
Read-throughs, or checklist reviews, are the simplest form of disaster recovery testing. In this method, disaster recovery staff distribute the current plan to all involved personnel, who then review their specific procedures. Team members provide feedback on necessary updates to ensure the plan remains up-to-date.
#### Walk-Throughs
Walk-throughs, also known as tabletop exercises, are a more advanced form of disaster recovery testing. They bring the team together to review and discuss the plan collectively. This approach is more effective than read-throughs, as it encourages interaction and collaboration, allowing for a deeper review of the plan.
#### Simulations
The test planners design a simulation of an emergency situation and then the disaster recovery team describes how they would react.
#### Parallel tests
The 3 before were theoretical, In this one we activate the DR response and it runs parallel to the normal one, so that we don't disturb operations.
#### Full Interruption Tests
This one, we really shut down normal operations and try to run on the DR environment.

# Exam Essentials
- Disaster recovery (DR) is a subset of business continuity activities designed to restore a business to normal operations as quickly as possible following a disruption.
- ***The recovery time objective (RTO)*** is the targeted amount of time that it will take to restore a service to operation following a disruption. ***The recovery point objective (RPO)*** is the maximum time period from which data may be lost as a result of a disaster. ***The recovery service level (RSL)*** is the percentage of a service that must be available during a disaster.
- Full backups include everything on the media being backed up. They make a complete copy of the data. Snapshots are a form of full backup created using specialized functionality of the hardware platform. Differential backups supple- ment full backups and create a copy of only the data that has changed since the last full backup. Incremental backups include only those files that have changed since the most recent full or incremental backup.
- Hot sites are fully operational data centers that have all the equipment and data required to handle operations ready to run. Cold sites are facilities that can be used to restore operations eventually, but they are essentially empty office spaces. Warm sites have the hardware and software necessary to support the company’s operations, but they are not kept running in a parallel fashion.
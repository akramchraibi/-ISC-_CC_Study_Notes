## Creating an incident response program
- **Preparation** : Activities that put in place an incident response plan and team.
- **Detection and Analysis** : Incident determination and identification of its scope.
- **Containment, eradication and recovery** : Stop further damage, removal of the effect of previous damage and restoration of normal operations.
- **Post-Incident Activity** : Analysis and identification of lessons leanred in order ro improve down the line.
This process can be described in the NIST incident response life cycle :
![[Pasted image 20241208212424.png]]
An incident response plan should follow :
- ***Statement of purpose*** : eg: Do we only care about cyber security incident or do we extend the plan to loses of important information.
- ***Clear strategy and goal*** : What's the upmost priority for the people handling the crisis at a strategic level.
- ***Organization’s approach to incident response*** : Who has the authority to do what during a crisis?
- It should also cover ***communication*** within the team, with other groups within the organization, and with third parties.
- ***Approval of senior management*** : helps with stubborn middle managers when you wanna halt all their operations.
```NIST SP 800-­61``` - Source

## Building an incident response team
### Team composition :
- Management
- Information security personnel
- Physical security personnel 
- Technical subject matter experts
- Legal counsel 
- Public relations and marketing staff
- Human ressources team members

You won't need all of them during a crisis but you got to have them trained and ready 24/7 for any eventualities and get backups for them also.
If you lack any abilities, such as a forensics expert, you might want to have them as an external hire. Although you don't want to be negotiating any contracts in the middle of a crisis so be sure to prepare for this in advance.
### Training and testing
Provide your team with the incident response plan and make sure they work together well before a crisis occurs.

## Incident communications plan
### Internal communications
***Incident notification and escalation procedures*** help ensure that the appropriate people within your organization know about an incident at the right time and are provided with the right information.
### External communications
You don't want any kind of incident to be disclosed before senior management approval and before your public relations personnel has the time to make a statement.
You are not always required to disclose the incident and you shouldn't if you feel like it would jeopardise the organization's reputation or would alerts the attackers. Nut you should of you have a legal obligation to do so especially in some case where user data is concerned.
### Secure Communications
We shouldn't *only* be concerned who we communicate with but how. Having secure communications channels ensures that there are no leaks.

## Incident identification and response
### Security data ressources
- Intrusion detection and prevention systems
- Firewalls
- Authentication systems
- System integrity monitors
- Vulnerability scanners
- System event logs
- NetFlow connection records
- Anti-malware Packages

### Correlating security information
***Security information and event management (SIEM)*** systems act as centralized log repository and analysis solutions. SIEM systems can detect possible incidents based on rules and algorithms, bringing them to the attention of security administrators for further review. They also provide a critical centralized information source to investigators pursuing a security incident.

### Receiving Incident reports
While we get notified of crisis from internal information, if our systems fail, we receive a notice of breach from elsewhere (employee, contractor, another organization...) we must handle these incident reports with a consistent and well planned manner.

### Responding to incidents
The person on duty or the one who first notices the incident has tremendous power when it comes to a successful incident response. They are called first responders.
They start by isolating the system and containing the damage, either by isolating the affected part from the network or by keeping it running for evidence collecting all the while preventing it from communicating with other systems.

> [!note] Exam Tip
> This is a favorite topic for exam questions. Remember that a first responder’s highest priority should be containing the damage by isolating affected systems.

While we build incident response capabilities we should also think about threat intelligence and conter intelligence capabilities as our adversaries are always watching.

# Exam Essentials
- The four stages of the NIST incident response process are preparation, detection & analysis, containment, eradication & recovery, and post-­incident activity.
- Incident response teams commonly include members from management, information security, physical security, legal counsel, public relations, human resources, along with technical subject matter experts.
- The highest priority of a first responder during incident response is to quickly contain the damage caused by the security incident.
- Security information and event management (SIEM) systems act as centralized log repository and analysis solutions.
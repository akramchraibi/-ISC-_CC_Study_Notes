## Risk
It's the job of the Cyber Security professional to identify, assess and manage risks in an organization.

## Type of Risk

### Internal and External risks
#### Internal Risks
Originates from within the organization and can be addressed by adding internal controls.

> If, for example, our process lets accounting members to commit fraud we failed to protect from this internal risk and a way to mitigate it would be to add a two person control (So that operations need to be supervised by two people at a time). 

#### External risks

>A Ransomware attack for example, can't do much about it besides building controls to limit the damage or the likelihood of an attack (2-factor authentification, backups...).

### Multiparty attack
When risk is shared among multiple organisations.

>If a SaaS provider is compromised all the customers are subject to this risk. 

### Specific Risks

#### Legacy Systems
Hard to secure especially if no longer maintained by the manufacturer.

>Either replace them or set up controls to mitigate any kind of risk.

#### Intellectual Property
business need to IP === business should consider it as a risk and protect it.

#### Software licence Compliance
Use Third party licensed software? Pay for it and use licence monitoring software to remember to pay for it.

## Risk Identification and Assessement
### The language of Risk
#### Threats
forces that jeopardise the security of your information and systems. Natural or human-made, you can't really control them.

#### Vulnerabilities
Things that the threats exploit to undermine your systems, data integrity... You spend much of your time on chasing them.

#### Risk
When both of the above are present. eg; when you have a patch missing and there is an exploit for the unpatched system

![[Pasted image 20241203222009.png]]
Both a threat and a Vulnerability must be present to establish risk.

> [!note] Exam Tip
> There is one related term that you should know for the exam. A threat vector is the method that an attacker uses to get to a target. This might be a hacker toolkit, social engineering, or physical intrusion.

### Ranking risks
#### Risk likelihood
Probability of occurrence of the risk, if  my operations are in Fès, i won't be trying to protect against a Tsunami.

#### Risk impact
How much damage will the risk do if it occurs.

#### Risk Assessment techniques
- Qualitative techniques : subjective measure; High, medium and low ranking for likelihood and impact.
![[Pasted image 20241203222705.png]]
- Quantitative techniques : math and stuff.

> [!note] Exam Tip
> You don’t need to know how to do the math for a quantitative risk assessment on the CC exam, but you’ll learn it if you move on to prepare for the CISSP or other advanced cybersecurity certifications.


## RISK TREATMENT STRATEGIES

Risk assessment done ->
- Avoid the risk.
- Transfer the risk.
- Mitigate the risk.
- Accept the risk.

### Risk Avoidance
Change the operations to not be affected by a risk. Transfert your operations from Casa to Fès to avoid Tsunamis.

### Risk Transference
insurance -> The risk no longer falls on you but it can harm reputation

### Risk Mitigation
take action to avoid risk -> a Firewall for example

### Risk Acceptance
If it costs too much to mitigate a risk that won't cause that much damage. might as well accept it.

## Risk Profile and Tolerance
The combination of risks that affect an organization are known as its **risk profile**.
The initial level of risk that exists in an organization before any controls are put in place is the organization’s **inherent risk**.
risk that results from adding controls is known as **control risk**.
The risk that remains after the inherent risk is reduced by controls is known as the **residual risk**.
The reality is that the organization will need to accept some ongoing risk in order to continue operations. Business leaders must decide how much risk they choose to accept. This is a process known as determining the organization’s **risk tolerance**.

![[Pasted image 20241203224150.png]]

> [!note] Exam Tip
> The goal of risk management is to make sure that the combination of the residual risk and the control risk is below the organization’s risk tolerance.

# Exam Tips
- Internal risks are those that arise from within the organization. External risks are those where the threat originates outside of the organization. Multiparty risks are shared among many different organizations.
- Threats are external forces that jeopardize the security of your information and systems. Vulnerabilities are weaknesses in your security controls that a threat might exploit to undermine the confidentiality, integrity, or availability of your information or systems. Risks occur when your environment contains both a vulnerability and a corresponding threat that might exploit that vulnerability.
- Risks are prioritized based on their likelihood and impact. The likelihood of a risk is the probability that it will actually occur. The impact of a risk is the amount of damage that will occur if the risk materializes.
- Qualitative risk assessment techniques use subjective judgments to assess risks, typically categorizing them as low, medium, or high on both the likelihood and impact scales. Quantitative risk assessment techniques use objective numeric ratings to assess the likelihood and impact of a risk.
- The four risk treatment options are avoiding a risk, transferring a risk, mitigating a risk, and accepting a risk.
- An organization’s risk profile begins with its inherent risk. Security professionals then apply controls to reduce that inherent risk, leaving the remaining residual risk. Controls may introduce new control risks.
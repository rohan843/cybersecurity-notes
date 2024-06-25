# Cybersecurity Notes

## Contents

- [Cybersecurity Notes](#cybersecurity-notes)
  - [Contents](#contents)
  - [Cybersecurity](#cybersecurity)
    - [Common Terms](#common-terms)
  - [Historic Cybersecurity Attacks](#historic-cybersecurity-attacks)
    - [Brain Virus](#brain-virus)
    - [Morris Worm](#morris-worm)
  - [Modern Cybersecurity Attacks](#modern-cybersecurity-attacks)
    - [LoveLetter Attack (aka ILOVEYOU virus)](#loveletter-attack-aka-iloveyou-virus)
    - [Equifax Breach](#equifax-breach)
  - [Common Cybersecurity Attacks](#common-cybersecurity-attacks)
    - [Phishing](#phishing)
    - [Malware](#malware)
    - [Social Engineering](#social-engineering)
      - [Social Engineering Principles](#social-engineering-principles)
    - [Data Breaches: Maintain your cool](#data-breaches-maintain-your-cool)
  - [CISSP (Certified Information Systems Security Professional) Security Domains](#cissp-certified-information-systems-security-professional-security-domains)
  - [Determining the Type of Attack](#determining-the-type-of-attack)
    - [Password Attack](#password-attack)
    - [Social Engineering Attack](#social-engineering-attack)
    - [Physical Attack](#physical-attack)
    - [Adversarial Artificial Intelligence](#adversarial-artificial-intelligence)
    - [Supply Chain Attack](#supply-chain-attack)
    - [Cryptographic Attack](#cryptographic-attack)
  - [Understanding Attackers](#understanding-attackers)
    - [Threat Actor Types](#threat-actor-types)
      - [Advanced Persistent Threats](#advanced-persistent-threats)
      - [Insider Threat](#insider-threat)
      - [Hacktivists](#hacktivists)
    - [Hacker Types](#hacker-types)
  - [Frameworks and Controls](#frameworks-and-controls)
  - [Secure Design](#secure-design)
  - [Ethics in Cybersecurity](#ethics-in-cybersecurity)
    - [Ethical Principles in Security](#ethical-principles-in-security)
    - [Ethical Concerns and Laws Related to Counterattacks](#ethical-concerns-and-laws-related-to-counterattacks)
      - [US's Standpoint on Counterattacks](#uss-standpoint-on-counterattacks)
      - [ICJ's Standpoint on Counterattacks](#icjs-standpoint-on-counterattacks)
  - [Common Cybersecurity Tools](#common-cybersecurity-tools)
    - [Security Information and Event Management (SIEM) Tools](#security-information-and-event-management-siem-tools)
    - [Other Tools](#other-tools)
    - [General Purpose Tools](#general-purpose-tools)
  - [8 CISSP Domains](#8-cissp-domains)
    - [Dom. 1: Security and Risk Management](#dom-1-security-and-risk-management)
    - [Dom. 2: Asset Security](#dom-2-asset-security)
    - [Dom. 3: Security Architecture and Engineering](#dom-3-security-architecture-and-engineering)
    - [Dom. 4: Communication and Network Security](#dom-4-communication-and-network-security)
    - [Dom. 5: Identity and Access Management](#dom-5-identity-and-access-management)
    - [Dom. 6: Security Assessment and Testing](#dom-6-security-assessment-and-testing)
    - [Dom. 7: Security Operations](#dom-7-security-operations)
    - [Dom. 8: Software Development Security](#dom-8-software-development-security)
  - [Threats, Risks and Vulnerabilities](#threats-risks-and-vulnerabilities)
    - [Impact study of Ransomware](#impact-study-of-ransomware)
    - [Key Impacts of Threats, Risk and Vulnerabilities](#key-impacts-of-threats-risk-and-vulnerabilities)
  - [Layers of the Web](#layers-of-the-web)
  - [NIST's Risk Management Framework](#nists-risk-management-framework)
  - [Common Risk Management Strategies](#common-risk-management-strategies)
  - [Frameworks](#frameworks)
  - [Controls](#controls)
  - [The CIA Triad](#the-cia-triad)

## Cybersecurity

It is the practice of ensuring **confidentiality, integrity and availability** of information by protecting network, devices, people and data from unauthorized access and criminal exploitation.

A **threat actor** is any person or group that presents a security risk.

Security protects us from _internal_ and _external_ threats. An **internal threat** is posed by current or former employees, external vendors or trusted partners (basically, from anyone associated with the organization). An **external threat** is from someone outside the organization trying to gain access to private information, networks, or devices.

Often, the internal threats are accidental, such as an employee clicking on a compromized link in an email. Nonetheless, they may be intentional as well, such as an internal actor trying to gain unauthorized access to some data or abusing systems for personal use.

Security teams also ensure compliance with regulations and laws that may require implementation of certain security standards. This prevents organizations from fines and other charges, while allowing them to satisfy their ethical obligation to protect their users.

Security teams also maintain and improve business productivity, by establishing business continuity plans. This allows employees to do their jobs even in the case of an event such as a data breach.

Upholding security reduces expenses because of downtime, breaches and fines. It also helps in maintaining brand trust.

### Common Terms

1. **Compliance**: The process of adhering to internal standards and external regulations. It enables organizations to avoid fines and security breaches.
2. **Security Frameworks**: These are guidelines used for building plans to help mitigate risks and threats to data and privacy.
3. **Security Controls**: They are safeguards designed to reduce _specific_ security risks. They are used with security frameworks to establish a strong security posture.
4. **Security Posture**: It is an organization's ability to manage its defence of critical assets and data and react to change. A strong security posture leads to lower risk for the organization.
5. **Threat**: Any circumstance or event that can negatively impact assets.
6. **Threat Actor**: [aka **malicious attacker**] Any person or group that poses a security risk. The risk may relate to computers, applications, networks and data.
7. **Network Security**: It is the practice of keeping an organization's network infrastructure secure from unauthorized access. This includes services, data, systems and devices that are stored in an organization's network.
8. **Cloud Security**: It is the process of ensuring that assets stored in the cloud are properly configured, or set up correctly and access to those assets is limited to authorized users.
9. **Programming**: The process to create a specific set of instructions for a computer to execute tasks such as:
   1. Automation of repetitive tasks (e.g., searching a list of malicious domains)
   2. Reviewing web traffic
   3. Alerting suspicious activity
10. **Personally Identifiable Information (PII)**: Any information used to infer an individual's identity.
11. **Sensitive Personally Identifiable Information (SPII)**: A specific type of PII that falls under stricter handling guidelines, such as AadharID or biometric data. SPII theft poses a significantly larger threat to an individual as compared to PII theft.

> PII and SPII are major targets for actors engaging in identity theft (the act of stealing personal information to commit fraud while impersonating a victim; its primary objective is financial gain).

More information of cybersecurity terms is available at the [NIST Glossary](https://csrc.nist.gov/glossary).

## Historic Cybersecurity Attacks

Often, attackers use modifications of past attacks, and therefore understanding the past attacks can help create a secure system and organization.

**Computer Virus**: Malicious code written to interfere with computer operations and cause damage to data and software. A virus often attaches itself to programs or data on a computer, then spreads and infects one or more computers in a network.

**Malware**: This is any software designed to harm devices or networks. Viruses are often refered to as malware, but malware includes many other kinds of software as well.

We will examine 2 early malware attacks: **Brain virus** and **Morris worm**. These were developed to accomplish specific tasks, but their developers underestimated the amount of damage and the number of infected computers these would cause.

### Brain Virus

It was created by the Alvi brothers in 1986, with the intention to track illegal copies of medical software and prevent pirated licenses. However, the actual effect of the virus was unexpected.

Once a person used a pirated copy of the software, the virus infected that computer. _Any_ disk that was connected to that computer also got infected.

Each time someone used an infected disk, the virus moved to a new computer. Thus undetected, the virus spread globally within a couple of months.

While the intention behind the virus was not to cause harm to data and software, it slowed productivity and significantly affected business operations.

This virus presents an important event in the field of software, demonstrating the need for security and maintaining productivity.

### Morris Worm

Developed by Robert Morris in 1988, its original objective was to assess the size of the Internet. The program would crawl the web, and install itself onto other computers to tally the number of computers that were connected to the Internet.

However, the worm failed to keep track of the computers it had already compromized, and continued to re-install itself, **untill the computers ran out of memory and crashed.**

About 6000 computers were affected, representing _10%_ of the Internet at the time.

This attack cost millions of dollars in damages due to business disruptions and the efforts required to remove the worm.

> After the Morris worm, **Computer Emergency Response Teams** (CERTs) were established to respond to computer security incidents. These continue to exist today.

## Modern Cybersecurity Attacks

With the spread of the Internet, lots of computers are accessible without the need for physical access to hardware devices or data transfer devices.

We will examine 2 notable attacks that relied on the Internet: the **LoveLetter Attack** and the **Equifax Breach**.

### LoveLetter Attack (aka ILOVEYOU virus)

In the year 2000, Onel de Guzman created the LoveLetter malware to steal Internet login credentials. This attack spread rapidly. The people who weren't yet suspicious of unsolicited emails were especially affected.

Victims recieved an email with the subject line `I Love You`, and an attachment labelled `Love Letter For You`. When the attachment was opened, the malware scanned the user's address book. Then, it automatically sent itself to each person on the list, and installed a program to collect user information and passwords.

Recipients would think that they are recieving an email from a friend, but it would actually be malware.

This malware ended up affecting **45 million computers** globally, and is believed to have caused over **$10 billion** in damages.

This attack is also an example of social engineering.

**Social Engineering**: A manipulation technique that exploits human error to gain private information, access or valuables.

This attack showed attackers the power of social engineering. The number of social engineering attacks increases with every new social media.

Its common now for employees to recieve training in how to identify social engineering attacks, specifically, phishing.

**Phishing**: The use of digital communications to trick people into revealing sensitive data or deploy malicious software.

### Equifax Breach

In 2017, attackers successfully infiltrated the credit reporting agency, Equifax. This was one of the **largest known data breaches of sensitive information**. During the breach, over 143 million customer records (that included PII) were stolen, and the breach affected approximately 40% of all Americans.

The breach occurred due to multiple failures on Equifax's part. The company failed to take action to fix multiple known vulnerabilities in the months leading up to the data breach.

The company had to pay over $575 million to resolve customer complaints and cover required fines.

This large fine alerted other companies to take measures to prevent such a breach on their systems.

## Common Cybersecurity Attacks

### Phishing

Phishing is the use of digital communications to trick people into revealing sensitive data or deploying malicious software.

Some common types of these attacks are:

1. **Business Email Compromise (BEC)**: A threat actor sends an email message that seems to be from a known source to make a seemingly legitimate request for information in order to obtain a financial advantage.
2. **Spear Phishing**: A malicious email attack that targets a specific user or group of users. The email seems to originate from a trusted source.
3. **Whaling**: It is a form of spear phishing, where threat actors target company executives to gain access to sensitive data.
4. **Vishing**: The exploitation of electronic voice communication to obtain sensitive information or to impersonate a known source.
5. **Smishing**: The use of text messages to trick users, in order to obtain sensitive information or to impersonate a known source.

### Malware

Malware is software designed to harm devices or networks. There are many types of malware. The primary purpose of malware is to obtain money, or in some cases, an intelligence advantage that can be used against a person, an organization, or a territory.

Some common types of malware are:

1. **Viruses**: Malicious code written to interfere with computer operations and cause damage to data and software.
   1. A virus **needs to be _initiated_ by a user** (i.e., _this user is the threat actor here, not necessarily the virus developer_), who transmits the virus via a malicious attachment or file download.
   2. When someone opens the malicious attachment or download, the virus hides itself in other files in the now infected system.
   3. When the infected files are opened, it allows the virus to insert its own code to damage and/or destroy data in the system.
2. **Worms**: Malware that can _duplicate and spread itself across systems on its own_. Unlike a virus, a worm does not need to be downloaded by the user. Instead, it self-replicates and spreads from an already infected computer to other devices on the same network.
3. **Ransomware**: A malicious attack, where the threat actors _encrypt_ an organization's data and demand payment to restore access.
4. **Spyware**: A malware that is used to gather and sell information without consent. Spyware can be used to access devices. This allows threat actors to collect personal data such as private emails, texts, voice and image recordings, and locations.

### Social Engineering

Social engineering is a manipulation technique that exploits human error to gain private information, access, or valuables. **Human error** is usually a result of trusting someone without question. _It's the mission of a threat actor, acting as a social engineer, to create an environment of **false trust** and lies to exploit as many people as possible._

Some of the most common social engineering attacks today are:

1. **Social media phishing**: A threat actor collects detailed information about their target from social media sites. Then, they initiate an attack.
2. **Watering hole attack**: A threat actor attacks a website frequently visited by a specific group of users.
3. **USB baiting**: A threat actor strategically leaves a malware USB stick for an employee to find and install, to unknowingly affect a network.
4. **Physical social engineering**: A threat actor impersonates an employee, customer or vendor to obtain unauthorized access to a physical location.

#### Social Engineering Principles

Social engineering is incredibly effective. This is because people are generally trusting and conditioned to respect authority. The number of social engineering attacks is increasing with every new social media application that allows public access to people's data.

Reasons why social engineering attacks are so effective include:

- **Authority**: Threat actors impersonate individuals with power. This is because people, in general, have been conditioned to respect and follow authority figures.
- **Intimidation**: Threat actors use bullying tactics. This includes persuading and intimidating victims into doing what they are told.
- **Consensus/Social Proof**: Because people sometimes do things that they believe many others are doing, threat actors use others' trust to pretend they are legitimate. For example, a threat actor might try to gain access to private data by telling an employee that other people at the company have given them access to that data in the past.
- **Scarcity**: A tactic used to imply that goods or services are in limited supply.
- **Familiarity**: Threat actors establish a fake emotional connection with users that can be exploited.
- **Trust**: Threat actors establish an emotional relationship with users that can be exploited _over time_. They use this relationship to develop trust and gain personal information.
- **Urgency**: A threat actor persuades others to respond quickly and without questioning.

### Data Breaches: Maintain your cool

If we are on the security team and responding to a data breach incident, we have to remain calm and composed. Others in the "room" may be upset and worried, but we have to be reassuring and remain calm.

The first thing we should do is to contain the breach. This means that **if we are still losing data, we should do everything in our power to stop the loss.** This may involve _shutting down the server, shutting down the data center or the data center communications_. Stopping the data loss is the first priority.

> First stop the breach, and then investigate the breach.

Executing the incident management plan is the most important thing we should keep in mind as an entry level analyst.

## CISSP (Certified Information Systems Security Professional) Security Domains

There are 8 security domains defined by CISSP to assist and organize the work of security professionals. **Security roles may focus on one domain or include several domains**.

Gaps in any of these can harm an organization.

The domains are:

1. **Security and Risk Management**: It defines security goals and objectives, risk mitigation, compliance, business continuity and the law. For e.g., updating company policies about some PII storage as the laws change.
2. **Asset Security**: It secures digital and physical assets. It's also related to the storage, maintenance, retention and destruction of data. For e.g., ensuring older equipment is properly destroyed, including any kind of sensitive information.
3. **Security Architecture and Engineering**: It optimizes data security by ensuring effective tools, systems, and processes are in place. For e.g., setting up a firewall.
4. **Communications and Network Security**: Manage and secure physical networks and wireless communications. For e.g., analysing user behaviour within the organization for suspicious activity or unsecured connections.
5. **Identity and Access Management**: It keeps data secure, by ensuring users follow established policies to control and manage physical assets, like office spaces, and logical assets, such as networks and applications. This includes validating employees' identities and documenting their access roles. For e.g., setting up employees' key card access to buildings.
6. **Security Assessment and Testing**: It involves conducting security control testing, collecting and analysing data and conducting security audits to monitor for risks, threats and vulnerabilities. For e.g., conducting audits to ensure access to payroll data is only given to those employees who require it.
7. **Security Operations**: Conducting investigations and implementing preventative measures. E.g., addressing an alert that an unknown device has connected to the network.
8. **Software Development Security**: Uses secure coding practices, which are a set of recommended guidelines that are used to create secure applications and services. For e.g., working with software teams to ensure that secure coding practices are involved in the SDLC.

## Determining the Type of Attack

### Password Attack

These attacks try to access password-secured devices, systems, networks or data. For e.g., brute force attacks and rainbow table attacks.

These fall under the communication and network security domain.

### Social Engineering Attack

Social engineering is a manipulation technique that exploits human error to gain private information, access, or valuables. For e.g., phishing, smishing, vishing, spear phishing, whaling, social media phishing, business Email Compromise (BEC), watering hole attack, usb (Universal Serial Bus) baiting, physical social engineering.

These fall under the security and risk management domain.

### Physical Attack

A physical attack is a security incident that affects not only digital but also physical environments where the incident is deployed. For e.g., malicious USB cable, malicious flash drive, and card cloning and skimming.

These attacks fall under the asset security domain.

### Adversarial Artificial Intelligence

Adversarial AI uses AI and ML techniques (described [here](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2023.pdf)) to conduct attacks more efficiently.

Adversarial AI falls under both the communication and network security and the identity and access management domains.

### Supply Chain Attack

These attacks target systems, applications, hardware and/or software to locate a vulnerability where malware can be deployed.

These attacks cause a breach at any point in the supply chain. They are costly as they can affect multiple organizations and the individuals who work for them.

They fall under several CISSP domains, including but not limited to security and risk management, security architecture and engineering, security operations.

### Cryptographic Attack

These attacks affect secure forms of communications between a sender and an intended recipient. For e.g., birthday attacks, collision attacks and downgrade attacks.

They fall under the communication and network security domains.

## Understanding Attackers

A **threat actor** is any person or group that presents a security risk.

### Threat Actor Types

#### Advanced Persistent Threats

Advanced persistent threats (APTs) have significant expertise accessing an organization's network without authorization.

They tend to **research their targets** (which include government entities and large corporations) in advance and can **remain undetected** for an extended period of time.

Their intentions and motivations can include:

1. Damaging critical infrastructure such as the power grid and natural resources.
2. Gaining access to intellectual property such as trade secrets or patents.

#### Insider Threat

Insider threats abuse their authorized access to obtain data that may harm an organization.

Their intentions and motivations can include:

1. Sabotage
2. Corruption
3. Espionage
4. Unauthorized data access or leaks

#### Hacktivists

These are threat actors driven by political agenda.

Their goals may include:

1. Demonstrations
2. Propaganda
3. Social change campaigns
4. Fame

### Hacker Types

**Hacker**: Any person who uses computers to gain access to computer systems, networks or data.

Hackers can be beginner or advanced technology professionals who use their skills for a variety of reasons.

There are 3 main **categories of hackers**:

1. **Authorized Hackers**: [aka Ethical Hackers] They follow a code of ethics and adhere to the law to conduct organizational risk evaluations. They are motivated to safeguard people and organizations from malicious threat actors.
2. **Semi-authorized Hackers**: They are considered researchers. They search for vulnerabilities but don't take advantage of the vulnerabilities they find.
3. **Unauthorized Hackers**: [aka Unethical Hackers] They are malicious threat actors who do not follow or respect the law. Their goal is to collect and sell confidential data for financial gain.

> There are multiple hacker types that fall into one or more of these categories.

New and unskilled actors have various goals including:

1. To learn and enhance their hacking skills.
2. To seek revenge.
3. To exploit security weaknesses by using existing malware, programming scripts and other tactics.

Other types of hackers are not motivated by any particular agenda other than completing the job they were contracted to do. These types of hackers can be considered unethical or ethical hackers. They have been known to work on both illegal and legal tasks for pay.

There are also hackers who consider themselves vigilantes. Their main goal is to protect the world from unethical hackers.

## Frameworks and Controls

To secure our organization from threats, we start with identifying critical assets and risks. Then, we implement the necessary frameworks and controls.

**Security Frameworks**: These are guidelines used for building plans to help mitigate risk and threats to data and privacy. They essentially provide a structured approach to document and implement a security lifecycle.

**Security Lifecycle**: A constantly evolving set of policies and standards that define how an organization manages risks, follows established guidelines, and meets regulatory compliance and laws.

The following are the purposes of security frameworks:

1. Protecting PII
2. Securing financial information
3. Identifying security weaknesses
4. Managing organizational risks
5. Aligning security with business goals

Frameworks have **4 core components**:

1. **Identifying and documenting security goals** (for e.g., an organization may have a goal to align with the E.U.'s GDPR. Consequently, a security analyst may be asked to identify and document areas where the organization is out of compliance with GDPR.)
2. **Setting guidelines to acheive security goals** (for e.g., when implementing guidelines to acheive GDPR compliance, an organization may have to develop new policies on how to handle data requests from individual users.)
3. **Implementing strong security processes** (for e.g., in case of GDPR, a security analyst working for a social media company may help design procedures to ensure the organization complies with verified user data requests. Such a request could be when a user attempts to update or delete their profile information.)
4. **Monitoring and communicating results** (for e.g., we may monitor our organization's internal network and report a potential security issue affecting GDPR to a manager or to a regulatory compliance officer.)

**Security controls**: They are safeguards designed to reduce specific security risks. For e.g., a guideline requiring all employees to complete a privacy training to reduce the risk of data breaches.

## Secure Design

**CIA Triad**: It is a foundational model that helps inform how organizations consider risk when setting up systems and security policies.

***C*onfidentiality**: Only authorized users can access specific assets or data. For e.g., strict access controls.

***I*ntegrity**: Data is correct, authentic and reliable. For e.g., encryption to protect data from tampering.

***A*vailability**: Data is available to those who are authorized to access it.

**Asset**: An item percieved as having value to an organization. The value is generally determined by the cost associated with the asset.

**Cybersecurity Framework: NIST CSF**: It is a voluntary framework that consists of standards, guidelines and best practices to manage cybersecurity risk.

Some other controls, frameworks, and compliance standards are:

1. **NIST RMF (Risk Management Framework)**
2. **The Federal Energy Regulatory Commission - North American Electric Reliability Corporation (FERC-NERC)**
   1. This is a _regulation_.
   2. It applies to organizations that work with electricity or that are involved with the U.S. and North American power grid.
   3. It defines some _Critical Infrastructure Protection (CIP) Reliability Standards_ the orgs must adhere to.
3. **The Federal Risk and Authorization Management Program (FedRAMP®)**
   1. This is a _U.S. federal government program_.
   2. It standardizes security assessment, authorization, monitoring, and handling of cloud services and product offerings to provide consistency across the government sector and third-party cloud providers.
4. **Center for Internet Security (CIS®)**
   1. This is a _nonprofit with multiple areas of emphasis_.
   2. It _provides a set of controls_ that can be used to safeguard systems and networks against attacks. Its purpose is to help organizations establish a better plan of defense.
   3. It also provides actionable controls that security professionals may follow if a security incident occurs.
5. **General Data Protection Regulation (GDPR)**
   1. It is a _European Union (E.U.) general data regulation_.
   2. It protects the processing of E.U. residents' data and their right to privacy in and out of E.U. territory.
6. **Payment Card Industry Data Security Standard (PCI DSS)**
   1. It is an _international security standard_.
   2. It ensures that organizations storing, accepting, processing, and transmitting credit card information do so in a secure environment.
   3. Its objective is to reduce credit card fraud.
7. **The Health Insurance Portability and Accountability Act (HIPAA)**
   1. It is a _U.S. federal law_.
   2. It prohibits patient information from being shared without their consent.
   3. It has 3 rules: Privacy, Security and Breach notification.
   4. **Protected Health Information (PHI)**: It relates to the past, present, or future physical or mental health or condition of an individual, whether it's a plan of care or payments for care.
   5. **Health Information Trust Alliance (HITRUST®)**: It is a security framework and assurance program that helps institutions meet HIPAA compliance.
8. **International Organization for Standardization (ISO)**
   1. It is a _standards' organization_.
   2. It was created to establish international standards related to technology, manufacturing, and management across borders. It helps organizations improve their processes and procedures for staff retention, planning, waste, and services.
9. **System and Organizations Controls (SOC type 1, SOC type 2)**
   1. This is a _standard_.
   2. It was developed by American Institute of Certified Public Accountants® (AICPA) auditing standards board.
   3. SOC1 and SOC2 are a series of reports that focus on an organization's user access policies at different organizational levels such as Associate, Supervisor, Manager, Executive, Vendor and Others.
   4. SOC1 and SOC2 are used to assess an organization's financial compliance and levels of risk. They also cover confidentiality, privacy, integrity, availability, security, and overall data safety. Control failures in these areas can lead to fraud.

> One of the most dangerous threat actors are disgruntled employees, as they have access to sensitive information and know where to find it. To reduce this type of risk, we would use the principle of availability and the organizational guidelines based on frameworks, to ensure staff members only access the data they need to perform their jobs.

## Ethics in Cybersecurity

Ethically, our job is to remain unbiased and maintain security and confidentiality.

**Security Ethics**: Guidelines for making appropriate decisions as a security professional.

### Ethical Principles in Security

1. Confidentiality: Proprietary or private information such as PII must be kept confidential and safe. There needs to be a high level of respect for privacy to safeguard private assets and data.
2. Privacy Protections: Safeguarding personal information from unauthorized use.
3. Laws: The rules that are recognized by a community and enforced by a governing entity.

As a security professional, we must:

1. Remain unbiased and conduct our work honestly, responsibly, and with the highest respect for the law.
2. Be transparent and just, and rely on evidence.
3. Ensure that we are consistently invested in the work we are doing, so we can appropriately and ethically address issues that arise.
4. Stay informed and strive to advance our skills, so we can contribute to the betterment of the cyber landscape.

### Ethical Concerns and Laws Related to Counterattacks

#### US's Standpoint on Counterattacks

In the US, deploying a counterattack on a threat actor is illegal and only defence is allowed. Counterattacks are seen as acts of vigilantism. (A vigilante is a person who is not a member of law enforcement who decides to stop a crime on their own.)

Counterattacks can lead to further escalation, leading to more damage and harm. Furthermore, if the attack was undertaken by a state-sponsored hacktivist (from another country), it could lead to serious international implications.

#### ICJ's Standpoint on Counterattacks

ICJ says that a person or group can counterattack if:

1. The counterattack will only affect the party that attacked first.
2. The counterattack is a direct communication asking the initial attacker to stop.
3. The counterattack does not escalate the situation.
4. The counterattack effects can be reversed.

Typically, organizations do not counterattack as the above scenarios are hard to measure.

## Common Cybersecurity Tools

**Log**: It is a record of events that occur within an organization's systems, such as employees signing into their computers or accessing web based services.

### Security Information and Event Management (SIEM) Tools

These are applications that collect and analyse log data to monitor critical activities in an organization. These tools collect real time information, allowing security analysts to identify potential breached as they happen.

SIEM tools have a dashboard like interface that visually organizes data into categories. Users can then select the data they wish to analyse.

Splunk and Chronicle are two commonly used SIEM tools.

**Splunk** is a data analysis platform. It is provided by the Splunk Enterprise as a self-hosted tool.

**Chronicle** is a cloud based SIEM tool provided by Google.

These tools collect data from multiple sources, and then analyse the data to identify potential security threats.

### Other Tools

**Playbook**: A manual that provides details about any operational action. They essentially guide security analysts on how to respond to a security incident before, during and after it has occurred. Different organizations have different playbooks, but the idea is to provide a step by step guide to the security analysts to complete specific tasks.

Consider as an example a forensic team investigating a security breach at a medical company for insurance purposes. In a forensic investigation, we may follow one of 2 playbooks:

1. **Chain of Custody Playbook**: **Chain of custody** is the process of documenting evidence possession and control during an incident lifecycle. We'll need to document who, what, where, and why we have the collected evidence. Evidence must be kept safe and tracked. Every time evidence is moved, it should be reported. This allows all parties involved to know exactly where the evidence is at all times.
2. **Protecting and Preserving Evidence Playbook**: Protecting and preserving evidence is the process of properly working with fragile and volatile digital evidence. In this playbook, we consult the **order of volatility**, which is a sequence outlining the order of data that must be preserved from first to last. It prioritizes volatile data, which is data that may be lost if the device in question powers off, regardless of the reason. While conducting an investigation, improper management of digital evidence can compromise and alter that evidence. _When evidence is improperly managed during an investigation, it can no longer be used._ For this reason, the first priority in any investigation is to properly preserve the data. We can preserve the data by making copies and conducting your investigation using those copies.

**Network Protocol Analyser**: [aka Packet Sniffer] This is a tool designed to capture and analyse data traffic within a network. These tools therefore keep a record of all the data that a computer within an organization's network encounters. For e.g., tcpdump and Wireshark.

### General Purpose Tools

Linux, SQL and Python are commonly used in cybersecurity.

**Web Vulnerability**: This is any unique flaw in a web application that a threat actor could exploit by using malicious code or behaviour to allow unauthorized access, data theft and malware deployment.

**Antivirus Software**: [aka anti-malware] This is a program used to prevent, detect and eliminate malware and viruses. Some antivirus softwares can scan the mamory of a device to find patterns that indicate the presence of malware.

**Intrusion Detection System (IDS)**: An IDS is an application that monitors system activity and alerts on possible intrusions. The system scans and analyzes network packets, which carry small amounts of data through a network. The small amount of data makes the detection process easier for an IDS to identify potential threats to sensitive data. Other occurrences an IDS might detect can include theft and unauthorized access.

**Penetration Testing**: [aka Pen-testing] It is the act of participating in a simulated attack that helps identify vulnerabilities in systems, networks, websites, applications and processes. It is a thorough risk assessment that can evaluate and identify external and internal threats, and weaknesses.

**Encryption**: It makes data unreadable and difficult to decode for an unauthorized user. Its main goal is to ensure confidentiality of private data. _Encryption_ is the process of converting data from a readable format to a cryptographically encoded format. _Cryptographic encoding_ means converting plaintext into secure ciphertext. _Plaintext_ is unencrypted information and _secure ciphertext_ is the result of encryption.

> Encoding and encryption serve different purposes. Encoding uses a public conversion algorithm to enable systems that use different data representations to share information, for example, string data can be ASCII encoded or UTF-8 encoded, but neither of these qualifies as encrypted as these are well known string encodings.

## 8 CISSP Domains

**Security Posture**: An organization's ability to manage its defence of critical assets and data, and react to change.

### Dom. 1: Security and Risk Management

It is focussed on defining security goals and objectives, risk mitigation, compliance, business continuity, and legal regulations.

**Defining security goals and objectives**: By doing so, organizations can reduce risks to critical assets and data, such as PII.

**Risk Mitigation**: It is the process of having the right procedures and rules in place to quickly reduce the impact of a risk, like a breach.

**Compliance**: It is the primary method used to develop an organization's internal security policies, regulatory requirements, and independent standards.

**Business Continuity**: An organization's ability to maintain their everyday productivity by establishing risk disaster recovery plans.

**Legal regulations** and **professional and organizational ethics** are other important components of this domain.

**Information security**, or InfoSec, is also related to this domain and refers to a set of processes established to secure information. An organization may use playbooks and implement training as a part of their security and risk management program, based on their needs and perceived risk. There are many InfoSec design processes, such as:

1. Incident response
2. Vulnerability management
3. Application security
4. Cloud security
5. Infrastructure security

As an example, a security team may need to alter how personally identifiable information (PII) is treated in order to adhere to the European Union's General Data Protection Regulation (GDPR).

### Dom. 2: Asset Security

It is focussed on securing digital and physical assets. It's also related to the storage, maintenance, retention and destruction of data.

There should be proper security in place for critical data such as PII and SPII, when stored or moved over a network. Moreover, there should be proper rules in place to decide how to store, maintain and destroy data.

For example, proper destruction of old hard drives.

Conducting a security impact analysis, establishing a recovery plan, and managing data exposure will depend on the level of risk associated with each asset. Security analysts may need to store, maintain, and retain data by creating backups to ensure they are able to restore the environment if a security incident places the organization's data at risk.

### Dom. 3: Security Architecture and Engineering

It is focussed on optimizing data security by ensuring effective tools, systems, and processes are in place to protect an organizations assets and data.

One core concept of shared design architecture is **shared responsibility**. It means all individuals within an organization take an active role in lowering risk and maintaining both physical and virtual security. This involves having policies to allow users to identify and report security concerns. Additional design principles related to this domain include:

1. Threat modeling
2. Least privilege
3. Defense in depth
4. Fail securely
5. Separation of duties
6. Keep it simple
7. Zero trust
8. Trust but verify

An example of managing data is the use of a security information and event management (SIEM) tool to monitor for flags related to unusual login or user activity that could indicate a threat actor is attempting to access private data.

### Dom. 4: Communication and Network Security

It is focussed on managing and securing physical networks and wireless communications. This includes on-site, remote, and cloud communications. For example, globally disallowing employees' laptops from connecting to public networks.

Organizations with remote, hybrid, and on-site work environments must ensure data remains secure, but managing external connections to make certain that remote workers are securely accessing an organization's networks is a challenge. Designing network security controls-such as restricted network access-can help protect users and ensure an organization's network remains secure when employees travel or work outside of the main office.

### Dom. 5: Identity and Access Management

It is focussed on access and authorization to keep data secure, by making sure users follow established policies to control and manage assets. It does this by ensuring user identities are trusted and authenticated and that access to physical and logical assets is authorized.

We should ensure the access to data is limited to what employees need. The goal of IAM is to reduce the overall risk to systems and data. IAM uses **the principle of least privilege**, which is the concept of granting only the minimal access and authorization required to complete a task. As an example, a cybersecurity analyst might be asked to ensure that customer service representatives can only view the private data of a customer, such as their phone number, while working to resolve the customer's issue; then remove access when the customer's issue is resolved.

Consider if all users used the same admin account. It would be very difficult to identify which user performed what activity.

There are **4 main components to IAM**:

1. **Identification**: When a user verifies who they are by providing a username, an access card, or biometric data such as a fingerprint.
2. **Authentication**: It is a verification process to prove a person's identity such as entering a password or PIN.
3. **Authorization**: It takes place once a user's identity has been confirmed. It relates to the level of access of the user, which depends on the role of the user in the organization.
4. **Accountability**: It refers to monitoring and recording user actions such as login attempts to prove systems and data are used properly.

### Dom. 6: Security Assessment and Testing

It is focussed on conducting security control testing, collecting and analysing data, and conducting security audits to monitor for risks, threats and vulnerabilities.

This domain usually involves examining organizational goals and objectives, and evaluating if the controls being used actually achieve those goals.

This involves collecting and analysing security data regularly. Analysts might use security control testing evaluations and security assessment reports to improve existing controls or implement new controls.

Security assessments help organizations determine whether their internal systems are secure or at risk. Organizations might employ penetration testers, often referred to as "pen testers," to find vulnerabilities that could be exploited by a threat actor.

An example of implementing new controls could be the introduction of multi-factor authentication to better protect the organization from threats and risks.

Additionally, this domain emphasizes the importance of conducting security audits to monitor for and reduce the probability of a data breach. To contribute to these types of tasks, cybersecurity professionals may be tasked with auditing user permissions to validate that users have the correct levels of access to internal systems.

### Dom. 7: Security Operations

This domain is focussed on conducting investigations and implementing preventative measures.

Investigations begin once a security incident has been identified. These processes require a heightened sense of urgency in order to minimize potential risks to the organization.

If there is an active attack, mitigating it and preventing it from escalating further is essential for ensuring that private information is protected from threat actors.

Once a threat is neutralized, the collection of digital and physical evidence to conduct a forensic investigation will begin.

A digital forensic investigation must take place to determine when, how and why the breach occurred. This helps security teams to identify areas for improvement and preventative measures that can be taken to mitigate future attacks.

This domain includes using strategies, processes, and tools such as:

1. Training and awareness
2. Reporting and documentation
3. Intrusion detection and prevention
4. SIEM tools
5. Log management
6. Incident management
7. Playbooks
8. Post-breach forensics
9. Reflecting on lessons learned

### Dom. 8: Software Development Security

It is focussed on using secure coding practices. Secure coding practices are recommended guidelines that are used to create secure applications and services.

Security is an additional step in the SDLC. By ensuring that each phase of the SDLC undergoes security reviews, security can be fully integrated into the software product.

For example, performing a secure design review during the design phase, secure code reviews during the development and testing phases, and penetration testing during the deployment and implementation phase.

Performing application security tests can help ensure vulnerabilities are identified and mitigated accordingly. Having a system in place to test the programming conventions, software executables, and security measures embedded in the software is necessary. Having quality assurance and pen tester professionals ensure the software has met security and performance standards is also an essential part of the software development process. For example, an entry-level analyst working for a pharmaceutical company might be asked to make sure encryption is properly configured for a new medical device that will store private patient data.

## Threats, Risks and Vulnerabilities

**Threat**: Any circumstance or event that can negatively impact assets. An example is a social engineering attack (a manipulation technique exploiting human error to gain private information, access or valuables). Another example is phishing (a type of social engineering). Some common threats nowadays are:

1. **Insider Threats**: Staff members or vendors may abuse their authorized access to obtain data that may harm an organization.
2. **Advanced Persistent Threats (APTs)**: These occur when a threat actor maintains unauthorized access to a system for an extended period of time.

**Risks**: They are different from threats. A risk is anything that can impact the confidentiality, integrity or availability of an asset. Risks can be thought of as the _likelihood_ of a threat. An example of risk to an organization is the lack of backup protocols that would allow recovery of stored information in case of any accident or security incident. Another way to understand risks is that `being late to work` is a risk, while `traffic`, `an accident`, `a flat tire`, etc. are threats. Risks are commonly rated on 3 levels: **low risk asset, medium risk asset and high risk asset** depending on possible threats and value of an asset.

**Low-risk asset**: It is information that would not harm the organization's reputation or ongoing operations, and would not cause financial damage if compromized. This includes public information such as website content, published research data.

**Medium-risk asset**: Information that's not available to the public and may cause some damage to the organization's finances, reputation or ongoing operations. For example, the early release of a company's quaterly earnings could impact the value of their stock.

**High-risk asset**: Information protected by regulations or laws, which if compromized would have a severe negative impact on an organization's finances, ongoing operations or reputation. This could include assets containing SPII, PII or intellectual property.

There are different factors that affect the likelihood of a risk to an organization's assets. These include:

1. **External Risk**: Anything outside an organization that has the potential to harm organizational assets, such as threat actors attempting to gain access to private information.
2. **Internal Risk**: A current or former employee, vendor, or trusted partner who poses a security risk.
3. **Legacy Systems**: These are old systems that might not be accounted for or updated, but can still impact assets, such as workstations or old mainframe systems. For example, an organization might have an old vending machine that takes credit card payments or a workstation that is still connected to the legacy accounting system.
4. **Multiparty Risk**: Outsourcing work to third-party vendors can give them access to intellectual property, such as trade secrets, software designs, and inventions.
5. **Software Compliance/Licensing**: Software that is not updated or in compliance, or patches that are not installed in a timely manner pose security risks.

> The [OWASP Top 10](https://owasp.org/www-project-top-ten/) list presents the top 10 risks posed to web applications. The [NIST Cybersecurity Risks List](https://www.nist.gov/itl/smallbusinesscyber/cybersecurity-basics/cybersecurity-risks) presents various common risks posed to software.

**As a security analyst, it is important to stay up-to-date on the most recent risks.**

**Vulnerability**: A weakness that can be exploited by a threat. For example, an outdated firewall, software or application, weak passwords, or unprotected confidential data. _People_ (client, external vendor or employee) can also be considered a vulnerability. People's actions can significantly affect an organization's internal network. Therefore, maintaining security has to be a united effort. This requires training people to act in a secure manner. Organizations must regularly inspect for vulnerabilities within their systems. Some common vulnerabilities are:

1. **ProxyLogon**: A pre-authenticated vulnerability that affects the Microsoft Exchange server. This means a threat actor can complete a user authentication process to deploy malicious code from a remote location.
2. **ZeroLogon**: A vulnerability in Microsoft's Netlogon authentication protocol. An authentication protocol is a way to verify a person's identity. Netlogon is a service that ensures a user's identity before allowing access to a website's location.
3. **Log4Shell**: Allows attackers to run Java code on someone else's computer or leak sensitive information. It does this by enabling a remote attacker to take control of devices connected to the internet and run malicious code.
4. **PetitPotam**: Affects Windows New Technology Local Area Network (LAN) Manager (NTLM). It is a theft technique that allows a LAN-based attacker to initiate an authentication request.
5. **Security logging and monitoring failures**: Insufficient logging and monitoring capabilities that result in attackers exploiting vulnerabilities without the organization knowing it.
6. **Server-side request forgery**: Allows attackers to manipulate a server-side application into accessing and updating backend resources. It can also allow threat actors to steal data.

> For there to be a risk, _both_ threat _and_ vulnerability must be present.

Various lists such as [CISA's Known Exploited Vulnerabilities Catalog](https://www.cisa.gov/known-exploited-vulnerabilities-catalog) and [NIST's National Vulnerability Database](https://nvd.nist.gov/vuln) present various new vulnerabilities.

### Impact study of Ransomware

**Ransomware** is a malicious attack where threat actors encrypt an organization's data and demand payment to restore access.

After deployment, ransomware can freeze network systems, make devices unusable and lock confidential data, making devices inaccessible. The threat actor then demands a ransom before providing a decryption key to allow organizations to return to their normal business operations.

When ransom negotiations occur or data is leaked by a threat actor, these eventa can occur through the dark web.

### Key Impacts of Threats, Risk and Vulnerabilities

1. **Financial Impact**: When an organization's assets are compromized in an attack, the financial consequences can be significant. These can include interrupted production and services, the cost to correct the issue, and fines if assets are compromized because of non-compliance with laws and regulations.
2. **Identity Theft**: Storing any kind of personal data poses a risk to an organization. Sensitive data can include PII, which can be sold or leaked through the dark web. This is because the dark web provides a sense of secrecy, and threat actors may be able to sell data there without legal consequences.
3. **Reputational Damage**: A solid customer base supports an organization's mission, vision and financial goals. An exploited vulnerability can lead customers to seek new business relationships with competitors or create bad press that causes permanent damage to an organization's reputation.
4. There may also be **legal penalties and fines** on the loss of personal data.

## Layers of the Web

The Web is an interlinked network of online content made up of **3 layers**:

1. **Surface Web**: It is the layer that most people use. It's content can be accessed by a web browser.
2. **Deep Web**: The content of the deep web requires authorization to access it. For example, an intranet of an organization, only accessible to individuals with access specifically provided by the organization.
3. **Dark Web**: It can only be accessed using special software. It generally carries a negative connotation since it is the preferred web layer for criminals because of the secrecy it provides.

## NIST's Risk Management Framework

There are **7 steps** in the RMF:

1. **Prepare**: The activities that are necessary to manage security and privacy risks, before a breach occurs. This involves monitoring for risks, and identifying controls that can be used to reduce those risks.
2. **Categorize**: It is used to develop risk management processes and tasks. The risk management processes are used to develop tasks by thinking how the confidentiality, integrity and availability of systems and information can be impacted by risk.
3. **Select**: It involves choosing, customizing and capturing documentation of the controls that protect an organization. For example, keeping the playbook up to date, or helping to manage other documentation that helps the security team manage issues more efficiently.
4. **Implement**: It involves implementing security and privacy plans for the organization. Good plans when implemented minimize the impact of ongoing security risks. For example, if employees constantly require password resets, implementing a change to password requirements may help solve the issue.
5. **Assess**: In this step, we determine if the established controls are implemented correctly. Analysts identify potential weaknesses and determine whether the organization's tools, procedures, controls and protocols should be changed to better manage potential risks.
6. **Authorize**: It involves being accountable for the security and privacy risks that may exist in an organization. It could involve generating reports, developing plans of action, and establishing project milestones that are aligned to the organization's security goals.
7. **Monitor**: It involves being aware of how the systems are operating. Assessing and maintaining technical operations are common tasks for analysts. We should know how the current systems support organizational security goals, and of any need of changes to the systems to better support those goals.

## Common Risk Management Strategies

The following are some common strategies used to manage risks:

1. **Acceptance**: This is accepting a risk to avoid disrupting business continuity.
2. **Avoidance**: It involves creating a plan to avoid the risk altogether.
3. **Transference**: Transferring a risk to a third party to manage.
4. **Mitigation**: Lessening the impact of a known risk.

## Frameworks

Security frameworks are guidelines used for building plans to help mitigate risk and threats to data and privacy.

Security involves not just the virtual space, but also the physical space. Therefore, many organizations have plans to maintain safety in the work environment.

Other security frameworks provide guidance for how to prevent, detect and respond to security breaches.

An especially dangerous attack is social engineering, where employees of an organization are directly attacked. _People are the biggest threat to security._ So, frameworks can be used to create plans to increase employee awareness, and educate them about how they can protect the organization, their co-workers and themselves. An important part of this training is how to detect red flags, and how to promptly report security issues.

**Cyber threat framework** is a framework developed by the U.S. government to provide a common language for describing and communicating information about cyber threat activity. It helps cybersecurity professionals analyze and share information more efficiently. This allows organizations to improve their response to the constantly evolving cybersecurity landscape and threat actors' many tactics and techniques.

**ISO/IEC 27001** is an internationally recognized and used framework. The ISO 27000 family of standards enables organizations of all sectors and sizes to manage the security of assets, such as financial information, intellectual property, employee data, and information entrusted to third parties. This framework outlines requirements for an information security management system, best practices, and controls that support an organization’s ability to manage risks. Although the ISO/IEC 27001 framework does not require the use of specific controls, it does provide a collection of controls that organizations can use to improve their security posture.

## Controls

Security controls are used to reduce specific security risks. Three common controls are:

1. **Encryption**: The process of converting data from a readable into an encoded format. This ensures confidentiality of sensitive data.
2. **Authentication**: The process of verifying who someone or something is. For example, passwords, multi-factor authentication, biometrics, etc.

> **Vishing** is the exploitation of electronic voice communication (biometric data) to obtain sensitive information or to impersonate a known source.

3. **Authorization**: It is the concept of granting access to specific resources within a system.

There are various kinds of controls:

1. Examples of **physical controls**: Gates, fences, and locks, Security guards, Closed-circuit television (CCTV), surveillance cameras, and motion detectors, Access cards or badges to enter office spaces.
2. Examples of **technical controls**: Firewalls, MFA, Antivirus software.
3. Examples of **administrative controls**: Separation of duties, Authorization, Asset classification.

## The CIA Triad

It is a model that helps inform how organizations consider risk when setting up systems and security policies.

**Confidentiality**: Only authorized users can access specific assets or data. For e.g., strict access controls and access provisioning on a need-to-know basis.

**Integrity**: Data is correct, authentic and reliable. For e.g., encryption to protect data from tampering.

**Availability**: Data is available to those who are authorized to access it.

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
- **Consensus/Social Proof**: Because people sometimes do things that they believe many others are doing, threat actors use others’ trust to pretend they are legitimate. For example, a threat actor might try to gain access to private data by telling an employee that other people at the company have given them access to that data in the past.
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
2. **Asset Security**: It secures digital and physical assets. It's also related to the storage, maintenence, retention and destruction of data. For e.g., ensuring older equipment is properly destroyed, including any kind of sensitive information.
3. **Security Architecture and Engineering**: It optimizes data security by ensuring effective tools, systems, and processes are in place. For e.g., setting up a firewall.
4. **Communications and Network Security**: Manage and secure physical networks and wireless communications. For e.g., analysing user behaviour within the organization for suspicious activity or unsecured connections.
5. **Identity and Access Management**: It keeps data secure, by ensuring users follow established policies to control and manage physical assets, like office spaces, and logical assets, such as networks and applications. This includes validating employees' identities and documenting their access roles. For e.g., setting up employees' key card access to buildings.
6. **Security Assessment and Testing**: It involves conducting security control testing, collecting and analysing data and conducting security audits to monitor for risks, threats and vulnerabilities. For e.g., conducting audits to ensure access to payroll data is only given to those emplyees who require it.
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

1. **Identifying and documenting security goals** (for e.g., an organization may have a goal to aligh with the E.U.'s GDPR. Consequently, a security analyst may be asked to identify and document areas where the organization is out of compliance with GDPR.)
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

> One of the most dangerous threat actors are disgruntled employees, as they have access to sensitive information and know where to find it. To reduce this type of risk, we would use the principle of availability and the organizational guidelines based on frameworks, to ensure staff members only access the data they need to perform their jobs.

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

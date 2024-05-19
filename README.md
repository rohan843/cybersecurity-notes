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
    - [LoveLetter Attack](#loveletter-attack)

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

### LoveLetter Attack

In the year 2000, Onel de Guzman created the LoveLetter malware to steal Internet login credentials. This attack spread rapidly. The people who weren't yet suspicious of unsolicited emails were especially affected.

Victims recieved an email with the subject line `I Love You`, and an attachment labelled `Love Letter For You`. When the attachment was opened, the malware scanned the user's address book. Then, it automatically sent itself to each person on the list, and installed a program to collect user information and passwords.

Recipients would think that they are recieving an email from a friend, but it would actually be malware.

This malware ended up affecting **45 million computers** globally, and is believed to have caused over **$10 billion** in damages.

This attack is also an example of social engineering.

**Social Engineering**: A manipulation technique that exploits human error to gain private information, access or valuables.

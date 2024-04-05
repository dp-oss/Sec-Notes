---
id: 1712243286-OESL
aliases:
  - Exam Objectives
tags: []
---

# Exam Objectives

## 1.0 Threats, attacks and Vulnerabilities
### 1.1 Compare and contrast different types of social engineering techniques
- Phishing:
    - Social engineering attack where the threat actor posing as something benign manipulates the target to take a certain action
- Smishing:
    - Phishing over SMS 
- Vishing: 
    - voice Phishing usually over the phone 
- Spam: 
    - Unsolicited messaging sent to users, not necessariliy mailicious but cetrainly can be
- Spam over instant messaging (SPIM)
    - spam sent through SMS or other messengers 
- Spear Phishing: 
    - Targeted phishing attacks usually aimed at higher up people in an organization 
- Dumpster Diving: 
    - digging through garbage or anything discarded to find out more information on a target 
- Shoulder Surfing: 
    - Finding out information by looking over someone's shoulder and looking at their screen 
- Pharming: 
    - creating a fake version of a real website to harvest credentials usually sent through phishing
- Tailgating: 
    - entering a secure area without authorization by following somebody inside 
- Eliciting information: 
    =  
- Whaling: 
    - Phishing that targets a specific high up individual such as the ceo 
- Prepending:   
    = 
- Identity Fraud: 
    =
    - Using someone's Personal information to benefit yourself 
- Invoice Scams:
    - Sending a fake bill to a company to try and get them to pay it
- Credential Harvesting: 
    =
    - taking login credentials to access services without authorization
- Reconnaissance:
    - finding out information about a target, frequently done before pen testing but can also be done by attackers
- Hoax: 
    - a fake event used in social engineering to get people to act without thinking
- Impersonation:
    - social engineering technique where you pretend to be someone else 
- Watering Hole attack:
    - compromising a resource usually a website that is outside of a target but frequently used by the target in order to gain access to the target itself 
- Typosquatting: 
    - registering domains that are similar to the domain a user would want to go to in order to carry out malicious activities such as credential harvesting
- Pretexting
    = 
- Influence Campaigns:
    - a targeted exrcise used to manipulate peoples thinking
    - Hybrid Warfare: 
        =
    - Social media:
        - influence campaigns using public social media platforms can be wide reaching 
- **Principles(Reasons for Effectiveness)**
    - Authority:
        - convincing social engineering target that you have authority over them to encourage certain action
    - Intimidation: 
        - technique to scare a target into action
    - Consensus: 
        - convincing target that others agree with the actions you want them to take 
    - Scarcity: 
        - convincing someone to act quickly something finite is going to run out 
    - Trust: 
        - convincing target that you are trustworthyin order to encourage the action 
    - Urgency: 
        - convincing target that the action needs to be taken as soon as possible to prevent them from analyzing the request

### Given a scenario, analyze potential indicators to determine the type of attack
- **Malware**: 
    - malicious software, not installed intentionally
    - Trojans: 
        - malware prentending to be something else 
    - Worms:
        - malware that can propogate itself and spread to other machines 
    - Potentially unwanted programs (PUPs): 
        - software not installed intentionally could be benign or malicious 
    - Fileless virus: 
        = 
        - virus that lives in memory 
    - Command and control: 
        - server used to control infected machines known as bots somtimes called a C2 
    - Bots: 
        - infected computers that can be controlled by an attacker
    - Cryptomalware: 
        - malware that uses cryptography to encrypt user data making it unreadable 
    - Logic bombs: 
        - software or scripts that execute when specified conditions are met such as at a certain time
    - Spyware: 
        - malware that is designed to steal user data
    - Keyloggers:
        - software that captures users keystrokes, usually to steal credentials and spy 
    - Remote Access Trojan(RAT): 
        - malware designed to look benign but actually provides the attacker with remote control over a users system
    - Rootkit: 
        - malware that hides itself in low level operating system files to avoid detection, can be hard to find 
    - Backdoor: 
        - an opening in a piece of software intentially left to provide access to those who know about it, can be left by the dev or an attacker
- **Password attacks**:
    - attacks designed to break find out a password
    - Dictionary:
        - a password attack that uses a long word list trying every single one to see if it's the password
    - Bruteforce: 
        - Password attack that tries every single password possible to guess the password
        - Offline: 
            - offline bruteforce uses the hashed passwords and compares hashes of every possible password against the known password's hash
        - Online: 
            - sometimes known as spraying trying every possible password to authenticate directly with the service 
    - Rainbow table: 
        - a premade list of common passwords along with their hashes to compare directly with the hashed password 
    - Plaintext/unencrypted:
        - passwords typically are stored in a hashed format, unhashed or plaintext password storage is unsafe because if compromised the attacker has the exact password needed to authenticate 
- **Physical attacks**: 
    - malicious Universal Serial Bus (USB) cable:
        - USB cable designed to look benign but actually steals data from the connected device 
    - malicious flash drive:
        - flash drive that appears to be benign but actually can infect or execute commands on a system
    - Card cloning:
        - taking stolen card information and writing it to another card to be used by the attacker 
    - Skimming: 
        - devices planted on card readers to steal information off of cards to be cloned later

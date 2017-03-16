---
<!-- .slide: data-autoslide="10000" -->

### Vulnerabilty Management
<br>
<span style="color:#e49436">Play VM</span>
<br>
<span style="color:gray">-</span>
<br>
<span style="color:#e49436">Dr.B.Muthukumaran</span>

---

<!-- .slide: data-autoslide="2000" -->

## Agenda <span style="color: #666666">Sessions</span>
### <span class="fragment" data-fragment-index="1" data-autoslide="2000">Vulnerability Management <span style="color: #666666">.</span>
<br>
### <span class="fragment" data-fragment-index="2" data-autoslide="3500">Network Forensics<span style="color: #e49436">Security</span>. and <span style="color: #e49436">Guidelines</span>.</li>

---
<!-- .slide: data-autoslide="2000" -->

## Agenda
- Network
  + Vulnerability analysis
- Email Forensics 
  + Email Forensics - email spoofing – 
  + Phishing – mail header analysiw

---
<!-- .slide: data-autoslide="2000" -->
## Agenda
- Malware Concetps 
  + Virus - Components - Function of replicator, 
  + concealer and dispatcher- Trigger Mechanisms- Virus families  
  + worms - Types - Families - sandboxing
  + Trojans and Backdoors, Types of Trojans - 

---
<!-- .slide: data-autoslide="2000" -->

## Agenda
- Botnets
  + Botnets - types of botnet- Structure of bots – 
  + Crime bots - Spamming bots - 
  + DoS – DDoS Attacks – types - Honey Pots

---
<!-- .slide: data-autoslide="2000" -->

## Agenda
- Network forensics  
  + Key Loggers - Port Scans – SYN flood - 
  + Protocols Susceptible to Sniffing - Active and Passive Sniffing- 
  + Wireshark – Capture and Display Filters - pcap analysis – Problems -  
  + Forensic evidences - log analysis & evidence collection. 
  
---
<!-- .slide: data-autoslide="11000" -->

### <span style="color: #e49436">What is network?</span>

- NW - Group or system of interconnected people or things.
- Is a set of computers connected together for sharing resources.
- Is a telecommunications network allowing computers to exchange data.
- Computing devices exchange data with each other through data link.
- Computers are connected with cable media and / or wireless media

---
<!-- .slide: data-autoslide="11000" -->

### <span style="color: #e49436">What is Protocol?</span>

- The official procedure or system of rules
- Rules for governing affairs of state or diplomatic occasion
- Protocol - set of rules and guidelines for communicating data
- Rules defined for each step of computer communication 
- Networks follow these rules to successfully transmit data.

---
<!-- .slide: data-autoslide="11000" -->

### <span style="color: #e49436">What is TOPOLOGY?</span>

- Shape of a local-area network (LAN) or other communications system
- Four principal topologies used in LANs.
   + *Bus topology*: Devices are connected to a central cable, called bus.
   + *Ring topology*: Devices are connected to one another (closed Ring).
   + *Star topology*: Devices are connected to a central hub (star).
   + *Tree topology*: Combines bus and star topologies.


---
### What is a <span style="color: #e49436">vulnerability</span>? 

- Vulnerability represents a weak point though in the system
- Security of a computer can be breached through vulnerability.  
- Vulnerability  is  a  programming  error  in  an  application  
- Is exploited to gain access to the computer.

---

### <span style="color: #e49436"> Vulnerability detection.</span>

- Vulnerability detection is  
   + a continuously monitoring, always-on system  
   + that can detect and alert administrators  
   + to the presence of vulnerabilities as they appear.  


---
### What is <span style="color: #e49436"> V.Scan.</span>

- Scanning refers to the use of a scanning computer program 
  + to evaluate a connected network and gather vulnerability information.
- Scanning is the process of understand the vulnerability Risk and threat

---

### <span style="color: #e49436"> Vulnerability scanner.</span>

- Vulnerability scanner 
  + is a computer program  
  + specifically designed to search a given target 
  + for weaknesses.  
- Scanner systematically engages the target in an attempt to assess 
  + where  the  target  is vulnerable to “attack”. 
- Used either with good intention or maliciously.

---
### <span style="color: #e49436"> Vulnerability scanner.</span>

- Examples - Vulnerability scanner 
  + Nessus 
  + OpenVAS 
  + NexPose  

---
### Types of<span style="color: #e49436"> V.Scanning.</span>
- Random Scanning
- Hitlist scanning
- Signpost scanning
- Vertical, Horizontal scanning
- Permutation scanning
- Local subnet scanning

---
### <span style="color: #e49436"> Random Scan</span>

- Each compromised host probes random addresses in the IP address space.  
- Code Red (CRv2) performed random scanning. 
- Random scanning potentially creates a high traffic volume. 
- Scanned addresses are in different networks, 
- Disadvantage
  + High amount of traffic leads to attack detection

---
### <span style="color: #e49436"> Hitlist Scan</span>

- Machine probes all addresses from an externally supplied list.  
- Detects a vulnerable machine, sends a portion of the initial hitlist to the recipient and keeps the rest. 
- Allows for great propagation speed and no collisions during the scanning phase. 
- Disadvantage 
  + Hitlist needs to be assembled in advance. 
  + Portion of the hitlist needs to be transmitted to machines that are being infected. 
  + Large, lists leads to attack detection.

---
### <span style="color: #e49436"> Signpost Scan</span>
 - Also called topological scanning 
 - takes advantage of habitual communication patterns of the compromised host to select new targets. 
 - Does not generate a high traffic load and thus reduces chances of attack detection.
 - Disadvantage 
   + spreading speed depends on agent machines and their user behavior,
   + Recruitment is slower.
   
---
### <span style="color: #e49436"> Permutation Scan </span>(1/2)
- All compromised machines share a common pseudo-random permutation of the IP address space
- Each IP address is mapped to an index in this permutation.  
- Is preceded by small hitlist scanning 
- Machine infected during initial phase begins scanning through the permutation 
- Uses the index computed from its IP address as a starting point. 
- Always starts from a random point in the permutation. 

---
### <span style="color: #e49436"> Permutation Scan </span> (2/2)
- Seeing an already-infected machine, chooses a new random starting point. 
- At threshold  a worm copy becomes dormant to minimize collisions. 
- Disadvantage
- As infection progresses, a large percentage of infected machines become dormant. 
- This results in a very low number of duplicated scans and hinders detection.

---
### <span style="color: #e49436">Local Subnet Scan</span>

- Local subnet scanning scans for targets that reside on the same subnet as the compromised host. 
- A single copy of the scanning program can compromise many vulnerable machines behind a firewall. 
- The Code Red II and the Nimda Worm used local subnet scanning.

---
### <span style="color: #e49436"> Horizontal Scanning </span>

- This is the common type of the scan for worms. 
- Scanning machines are looking for a specific vulnerability, 
- Scans the same destination port on all machines from the list, 
- List assembled through host scanning techniques

---
### <span style="color: #e49436">Vertical Scanning </span>

- This is the common type of the scan for intrusions and multiple vector worms. 
- Scanning machines probe multiple ports at a single destination, looking for any way to break in.


---
### What is <span style="color: #e49436">Risk</span>


---
### What is <span style="color: #e49436">Risk classification</span>



---
### What is <span style="color: #e49436">Risk evaluation</span>



---
### What is <span style="color: #e49436">Risk Matrix</span>



---
### What is <span style="color: #e49436">Risk Mitigation</span>



---
### What is <span style="color: #e49436">W.Risk</span>



---
### What is <span style="color: #e49436">Threat</span>






---
<!-- .slide: data-autoslide="2000" -->
## Agenda
- Malware Concetps 
  + Virus - Components - Function of replicator, 
  + concealer and dispatcher- Trigger Mechanisms- Virus families  
  + worms - Types - Families - sandboxing
  + Trojans and Backdoors, Types of Trojans - 

---
<!-- .slide: data-autoslide="15000" -->

### What is <span style="color: #e49436">Malware </span>

- Malware, short for malicious software
- Is an umbrella term used to refer forms of hostile software
- Is any software used to disrupt computer or mobile operations
- Used to gather sensitive information and gain access to private computer systems
- Used to display unwanted advertising
- Includes computer viruses, worms, trojan horses, ransomware, spyware, adware, scareware, and other malicious programs

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Virus </span>

- A computer virus is a malicious software program
- When executed, replicates by reproducing itself
- Infects other computer programs by modifying them.
- Infecting computer programs includes, data files, or “boot” sector of the hard drive.
- Viruses use different stealth strategies to avoid detection


---
<!-- .slide: data-autoslide="15000" -->
### Virus <span style="color: #e49436"> Components </span>


---
<!-- .slide: data-autoslide="15000" -->
### Function of <span style="color: #e49436"> replicator </span>

- helps in multiplication of the virus
- Job to ensure survival of the virus 
- Achieved by appending  themselves  to  legitimate  programs  in  the  machine. 
- Program is run then the virus will 'wake up' and start to reproduce.

---
<!-- .slide: data-autoslide="15000" -->
### Function of <span style="color: #e49436"> Concealer </span>

- Job  of  hiding  the  virus.  
- Uses  a  number  of  methods  to  do  this    
- Today's  viruses  use  advance  techniques to stop being caught from Antivirus software

---
<!-- .slide: data-autoslide="15000" -->
### Function of <span style="color: #e49436">Payload</span>

- Payload  of  a  virus  can  be  practically  anything, 
in fact if it can be programmed then it can be the payload.  
If  an  obvious  payload  gets  delivered  soon  after infection then the user is soon going to notice and will go 
virus  hunting.  This  does  not  help  the  long  life  or  wide spread of a virus


---
<!-- .slide: data-autoslide="15000" -->
### Function of <span style="color: #e49436"> Trigger</span>


---
<!-- .slide: data-autoslide="15000" -->
### Virus <span style="color: #e49436"> Types </span>



---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> Mutation engine</span>
- Heart of a metamorphic virus is a mutation engine,
- Responsible for transforming its program. 
- takes an input program and morphs it to a structurally different but semantically equivalent program
- Three modules of any mutation engine: 
  + disassembly module, reverse engineering module, transformation module
  
---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Worm</span>

- Computer worm is a standalone malware computer program
- Replicates itself in order to spread to other computers
- Worms spread by exploiting vulnerabilities in operating systems.
- Worm searches a vulnerable host to replicate itself 

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Worm</span> Types

-  *Email-Worms*: Spreads via email messages.
-  *Instant-Messaging* Worms: Spread useing instant messaging applications
-  *File-sharing* worms copies itself into a shared folder
-  *Internet-worms* target low level TCP/IP ports directly

---
<!-- .slide: data-autoslide="15000" -->

### Difference <span style="color: #e49436">Worm - virus?</span>

- Both are malware and can perform the same malicious actions.  
- Viruses typically don’t self-propagate, and rely on users  to activate and transport the virus to a new destination.  
- Worms are generally self-propagating, 
 
---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436"> Trojan </span>

- Trojan Horse is a destructive program that has been disguised
- Looks like an innocuous software.
- Worms / virus programs concealed in a Trojan Horse.
- Trojan Horses are not viruses
- They do not reproduce themselves and spread as viruses do


---
<!-- .slide: data-autoslide="15000" -->

### Types of <span style="color: #e49436"> Trojan</span>

Joke Trojans
NVP Trojan
IconDance Trojan
Destructive Trojans

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436"> Joke Trojans </span>
- Joke Trojan causes no damage 
- Play an annoying sound from your computer's speaker, 
- Warp the appearance or display a taunting message on the screen, 
- Msg is "Now formatting hard drive!" 
- are harmless and easily deleted.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> NVP Trojan</span>

- Is a Macintosh Trojan horse 
- Modifies the system file  
- User types any text, the vowels (a, e, i, o, and u) fail to appear. 
- Trojan masquerades as a utility program 

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> IconDance Trojan</span>

- IconDance Trojan minimizes all application windows 
- Starts rapidly scrambling all the desktop icons. 
- It does nothing more than make you take the time to reorganize your Windows desktop.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> Destructive Trojan </span>

- Can either wipe out your hard drive or selectively delete or modify certain files. 
- Although these are the most dangerous Trojans, their very nature tends to limit their spread: In the process of attacking your computer, they reveal their presence, often by displaying a taunting message on the screen. And, if they reformat your hard drive, they also wipe themselves out.


---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436"> Spyware</span>

- Spyware is a type of malware
- Aims to gather information about a person or organization
- Info gathered without their knowledge,
- Information sent to another entity without the consumer’s consent,
- Variety of Spyware in circulation


---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Spyware-Types </span>(1/2)

- Browser Hijack: Control web browser and display unsolicited advertisements.
- Adware: Monitors online activities for targeted Pop-Up advertising.
- Trojans: Make your computer vulnerable ti remote controll by hackers.
- Profiling Cookies: Track your web surfing habits.
- Keyboard Loggers and Trackware Programs: Capture and record your every keystroke, inlcuding personal information and passwords.


---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Spyware-Types.. </span> (2/2)

- Dialers Auto-dial toll calls without your permission.
- Droneware Control your PC, to send spam or to host offense web images.
- Web Bugs: A graphics designed to monitor the reader. Often invisible because they are typically only 1-by-1 pixel in size. They are represented as HTML IMG tags.


---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436"> Grayware </span>

- Browser hijacker - software that modifies the default browser behavior.
- Homepage hijacker - modifies the default home page
- Search hijacker modifies the default search engine of the browser.
- Error page hijacker causes the browser to display a particular web site whenever a misspelled URL is entered into the address bar.



---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Zeus Trojan </span>

- First spotted in 2007, 
- specifically designed to create a botnet of compromised computers 
- To be recruited for information stealing and financial fraud activities. 
- Spreads through phishing and drive-by attacks 
- collects information using various techniques like form grabbing and key-stroke monitoring.  

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Zeus Trojan </span>

- Estimate Zeus botnet had infected more than 3.6  million computers
- toolkit comes with an easy installation procedure and customization mechanisms 
- Zeus  uses  complicated  multilevel  obfuscation  mechanisms  
- this is to avoid  detection and hinder any analysis procedure. 


---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Stuxnet worm</span>
- Designed to specifically target SCADA systems   
- Employ  PLC  rootkit technology that  allowed  PLC code  modifications. 
- initially  found  to  target  Iranian  facilities.
- quickly  spread  to various other countries. 
- position as  one  of  the  most dangerous cyber weapons.

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Stuxnet worm</span>
- Designed to propagate through various zero day vulnerabilities,   
- Unknown  exploits on  print spooler service, Microsoft Windows Server services used  
- features include 
  + stolen component certificates, 
  + complicated injection and hooking mechanisms, 
  + dynamic updates  and specific antivirus evasion utilities. 

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Dugu worm</span>

- 2011 a  new  sophisticated  worm  attack  was  identified.  
- Dugu was specifically designed  to  
  + steal  passwords,  
  + collect computer screenshots located on the infected machine. 
- Dugu spreads through a previously unknown vulnerability in MS word documents
- main purpose is to conduct industrial espionage.

---
<!-- .slide: data-autoslide="2000" -->

### <span style="color: #e49436">Recap</span>

---
<!-- .slide: data-autoslide="2000" -->

## Agenda
- Botnets
  + Botnets - types of botnet- Structure of bots – 
  + Crime bots - Spamming bots - 
  + DoS – DDoS Attacks – types - Honey Pots
---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">BotNet</span>

- Term “botnet” coined from “robot networks.” 
- Robot” has a Czech derivation from the word “robotovat,” which means “to work.” 
- Botnet, therefore, is an apt definition: 
- bots are highly adaptable worker bees that do their master’s bidding

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">BotNet</span>
- The overall architecture and implementation of botnets is complex
- Evolving toward the use of common software engineering techniques such as modularity
- The predominant remote control mechanism for botnets remains Internet Relay Chat (IRC) 
- IRC includes a rich set of commands enabling a wide range of use

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">BotNet</span>

- Wide diversity of exploits for infecting target systems written into botnet codebases.
- All botnets include denial of service (DoS) attack capability.
- Shell encoding and packing mechanisms that can enable attacks to circumvent defensive systems are common
- All botnets include a variety of sophisticated mechanisms for avoiding detection

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">BotNet</span>

- New botnets use different organizational techniques, including:
- Decentralized Naming Resolution. 
  + Using techniques pioneered by spammers botnets now act as their own DNS cloud, 
  + avoid centralized name resolution. 
  + Victims are instructed to use existing botnets for DNS resolution, avoiding the centralized use of naming services.

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">BotNet</span>

- Tor botnets. 
  + IRC operators have reported botnets on the Undernet network connecting from TOR exit nodes. 
  + Tor is a proxy network 
  + Uses a type of MIX-net routing to anonymize traffic. 
  + Botnets using Tor therefore pose difficult detection and response problems

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">BotNet</span>

- Tunneling bots. 
  + Increase in the number of bots that tunnel through existing protocols.
  + Bots potentially use net news, web blogs, and other resources. 
  + Fundamentally, these sorts of bots pose more of a problem for detection.


---
<!-- .slide: data-autoslide="2000" -->

### <span style="color: #e49436">Recap</span>
---

<!-- .slide: data-autoslide="2000" -->

## Agenda
- Network forensics  
  + Key Loggers - Port Scans – SYN flood - 
  + Protocols Susceptible to Sniffing - Active and Passive Sniffing- 
  + Wireshark – Capture and Display Filters - pcap analysis – Problems -  
  + Forensic evidences - log analysis & evidence collection. 


---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Key Loggers</span>


---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Key Loggers</span>


---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Port Scan</span>



---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">SYN flood</span>


---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Sniffing</span>
- Sniffing is the electronic form of eavesdropping 
- Carried out on communications, computers transmit across networks
- Sniffing involves 
  + capturing, decoding, inspecting and interpreting 
  + information inside a network packet on a TCP/IP network. 
- Acts as network probes for examining network traffic.


---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Packer Sniffer</span>

- Packet sniffer is a utility 
- used since the original release of Ethernet. 
- Allows individuals to capture data as it is transmitted over a network 
- Used by network professionals to diagnose network issues, 
- Malicious capture unencrypted data, like passwords and usernames.

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Active Sniffing</span>

- Sniffing is performed on a switched network, known as active sniffing.
- Relies on injecting packets into the network that causes traffic. 
- Is required to bypass the segmentation that switches provided. 
- Sniffers operate at the Data Link layer of the OSI model.  
- Grab whatever they see on the wire and record it for later review. 

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Passive Sniffing</span>

- Hubs see all traffic in the collision domain. 
- Sniffing performed on a hub is known as passive sniffing.
- Collision domain is a logical area of the network in which one or more data packets can collide with each other.
- Passive sniffing worked well during the days that hubs were used. 

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Protocols - Sniffing</span>
- Telnet and Re-login: 
- HTTP: Passwords and data sent 
- SNMP: SNMPv1 no good security. SNMP passwords sent in clear text.
- NNTP: Passwords and data sent.
- POP, IMAP: Passwords and data sent.
- FTP: Passwords and data sent.

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Sniffing Tools</span>

- Wireshark.
- Tcpdump.
- Dsniff.
- NetStumbler.
- Ettercap.
- Ntop.

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Wireshark</span>



---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">PCAP Analysis</span>


---




![Thanks](images/thanks.png)





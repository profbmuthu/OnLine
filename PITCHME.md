---
<!-- .slide: data-autoslide="10000" -->

![LOGO](https://d1z75bzl1vljy2.cloudfront.net/img/gp-logo.png)

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
### <span class="fragment" data-fragment-index="1" data-autoslide="2000">Vulnerability <span style="color: #666666">.</span>
<br>
### <span class="fragment" data-fragment-index="2" data-autoslide="3500">Vulnerability Management<span style="color: #e49436">Security</span>. and <span style="color: #e49436">Guidelines</span>.</li>

---
<!-- .slide: data-autoslide="2000" -->

## Agenda
- Network
  + Network, protocol, topology, IP Addresses.
- Cyber Crime
  + IP Spoofing, email spoofing, piggybacking, masquerading
  + 419 Nigerian frauds, Advance Fee Frauds
  + data theft, Man-in-the-Middle Attacks, Session Hijacking,
  + Social engineering, Scavenging
  + Virus / worms - Dos Attacks - DDoS Attacks

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
## What is a <span style="color: #e49436">vulnerability</span>? 

- Vulnerability represents a weak point though in the system
- Security of a computer can be breached through vulnerability.  
- Vulnerability  is  a  programming  error  in  an  application  
- Is exploited to gain access to the computer.

---

## <span style="color: #e49436"> Vulnerabilities detection system.</span>

- Vulnerability  detection  system is  
   + a continuously  monitoring, always-on system  
   + that can detect and alert administrators  
   + to the presence of vulnerabilities as they appear.  
   
---

## <span style="color: #e49436"> Vulnerability scanner.</span>

- Vulnerability scanner 
  + is a computer program  
  + specifically designed to search a given target 
  + for weaknesses.  
- Scanner systematically engages the target in an attempt to assess 
  + where  the  target  is vulnerable to “attack”. 
- Used either with good intention or maliciously.



---
## <span style="color: #e49436"> Random Scanning</span>

- Each compromised host probes random addresses in the IP address space.  
- Code Red (CRv2) performed random scanning. 
- Random scanning potentially creates a high traffic volume. 
- Scanned addresses are in different networks, 
- Disadvantage
  + High amount of traffic leads to attack detection

---
## <span style="color: #e49436"> Hitlist Scanning </span>

- Machine probes all addresses from an externally supplied list.  
- Detects a vulnerable machine, sends a portion of the initial hitlist to the recipient and keeps the rest. 
- Allows for great propagation speed and no collisions during the scanning phase. 
- Disadvantage 
  + Hitlist needs to be assembled in advance. 
  + Portion of the hitlist needs to be transmitted to machines that are being infected. 
  + Large, lists leads to attack detection.

---
## <span style="color: #e49436"> Signpost Scanning </span>
 - Also called topological scanning 
 - takes advantage of habitual communication patterns of the compromised host to select new targets. 
 - Does not generate a high traffic load and thus reduces chances of attack detection.
 - Disadvantage 
   + spreading speed depends on agent machines and their user behavior,
   + Recruitment is slower.
   
---
## <span style="color: #e49436"> Permutation Scanning </span>(1/2)
- All compromised machines share a common pseudo-random permutation of the IP address space
- Each IP address is mapped to an index in this permutation.  
- Is preceded by small hitlist scanning 
- Machine infected during initial phase begins scanning through the permutation 
- Uses the index computed from its IP address as a starting point. 
- Always starts from a random point in the permutation. 

---
## <span style="color: #e49436"> Permutation Scanning </span> (2/2)
- Seeing an already-infected machine, chooses a new random starting point. 
- At threshold  a worm copy becomes dormant to minimize collisions. 
- Disadvantage
- As infection progresses, a large percentage of infected machines become dormant. 
- This results in a very low number of duplicated scans and hinders detection.


---
## <span style="color: #e49436">Local Subnet Scanning </span>

- Local subnet scanning scans for targets that reside on the same subnet as the compromised host. 
- A single copy of the scanning program can compromise many vulnerable machines behind a firewall. 
- The Code Red II and the Nimda Worm used local subnet scanning.


---

![Thanks](images/thanks.png)


---
## <span style="color: #e49436"> Horizontal Scanning </span>

- This is the common type of the scan for worms. 
- Scanning machines are looking for a specific vulnerability, 
- Scans the same destination port on all machines from the list, 
- List assembled through host scanning techniques

---
## <span style="color: #e49436">Vertical Scanning </span>

- This is the common type of the scan for intrusions and multiple vector worms. 
- Scanning machines probe multiple ports at a single destination, looking for any way to break in.

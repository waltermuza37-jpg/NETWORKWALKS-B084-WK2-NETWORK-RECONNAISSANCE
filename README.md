# NETWORKWALKS-B084-WK2-NETWORK-RECONNAISSANCE
Networkwalks Week 2 practical cybersecurity project focused on network reconnaissance, host discovery and network scanning using Kali Linux, Nmap and Zenmap.


# NETWORKWALKS B084 – WEEK 2
## Network Reconnaissance, Footprinting and Configuration

### 1. Project Overview

This repository documents my Week 2 practical activities as part of the Networkwalks Cybersecurity Internship (Batch B084).

The practical covered network configuration, background reconnaissance (footprinting), DNS investigation, website technology fingerprinting and network discovery using Kali Linux, Nmap and Zenmap.

The exercises focused on understanding how publicly available information can reveal an organisation's digital footprint and how network scanning tools can identify active devices within a local network.

### 2. Lab Environment and Tools

**Operating System:** Kali Linux

**Virtualisation:** Oracle VirtualBox

**Tools Used:**
- WHOIS
- WhatWeb
- Nslookup
- cURL
- WAFW00F
- DNSRecon
- Nmap
- Zenmap

**Reconnaissance Target:** networkwalks.com

### 3. Practical 1: Background Reconnaissance (Footprinting)

The first practical focused on collecting publicly available information about networkwalks.com.

#### Task 1: WHOIS – Domain Registration Lookup

Command:
```bash
whois networkwalks.com
```

Purpose: Investigate domain registration details, registrar information, registration and expiry dates, and name servers.

#### Task 2: WhatWeb – Website Technology Fingerprinting

Command:
```bash
whatweb networkwalks.com
```

Purpose: Identify publicly detectable website technologies, web server information, CMS platforms and frameworks.

#### Task 3: Nslookup – DNS Resolution

Command:
```bash
nslookup networkwalks.com
```

Purpose: Resolve the domain name to its corresponding IP address and examine DNS responses.

#### Task 4: cURL – HTTP Response Header Analysis

Command:
```bash
curl -I https://networkwalks.com
```

Purpose: Examine HTTP response headers, server information, response status and other exposed metadata.

#### Task 5: WAFW00F – Web Application Firewall Detection

Command:
```bash
wafw00f networkwalks.com
```

Purpose: Identify whether a Web Application Firewall is protecting the website and whether its technology can be detected.

#### Task 6: DNSRecon – DNS Enumeration

Command:
```bash
dnsrecon -d networkwalks.com
```

Purpose: Investigate DNS records, including name servers, mail servers, TXT, SPF and other available records.

### 4. Practical 2: Network Reconnaissance Using Nmap and Zenmap

The second practical focused on identifying devices within a local network using Nmap and its graphical interface, Zenmap.

#### Task 1: Install Zenmap

Download and install Zenmap from its official source to provide a graphical interface for network scanning.

#### Task 2: Identify Local Network Configuration

Determine the local IP address and LAN subnet to establish the network range for the reconnaissance exercise.

#### Task 3: Network Host Discovery

Use Nmap and Zenmap to examine the local subnet and identify active hosts.

Example Nmap host discovery command:

```bash
nmap -sn <LAN-subnet>
```

#### Task 4: Identify Live Hosts

Examine scan results to establish how many hosts are active within the scanned subnet.

#### Task 5: Identify IP Addresses

Record the IP addresses of the discovered live hosts.

#### Task 6: Identify MAC Addresses

Examine available scan results to identify the MAC addresses associated with discovered devices.

### 5. Key Learning Outcomes

Through these practical exercises, I developed hands-on experience in:

- Linux command-line operations.
- Domain registration intelligence gathering.
- Website technology fingerprinting.
- DNS resolution and enumeration.
- HTTP response header analysis.
- Web Application Firewall detection.
- Network configuration and subnet identification.
- Network reconnaissance and host discovery.
- Using Nmap and Zenmap for network scanning.
- Identifying IP and MAC addresses of active network devices.

### 6. Security Relevance

Reconnaissance is an important stage in cybersecurity assessments because it helps establish what information and services are exposed by a target.

From a defensive security perspective, these techniques help security professionals understand external attack surfaces, identify information disclosure and investigate network exposure.

### 7. Practical Evidence

This repository contains practical screenshots, command outputs and observations from the Week 2 exercises.

### 8. Conclusion

Week 2 provided practical exposure to two important areas of cybersecurity reconnaissance: background footprinting and network discovery.

By working with Kali Linux, Nmap and Zenmap, I gained a better understanding of how reconnaissance tools collect information about websites, domains and network devices.

These skills provide a foundation for further learning in vulnerability assessment, network security and defensive security operations.

---

**Programme:** Networkwalks Cybersecurity Internship  
**Batch:** B084  
**Week:** 2  
**Practical Focus:** Background Reconnaissance and Network Discovery  
**Operating System:** Kali Linux

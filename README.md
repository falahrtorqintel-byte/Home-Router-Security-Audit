# home-network-scanning-device-mapping
his project demonstrates a simple, ethical, and beginner-friendly approach to identifying devices connected to a home network. The goal is to improve visibility, security awareness, and basic network hygiene for non-technical users.

This project is part of KaredokNet, an independent initiative focused on practical WiFi and home network security.

# Environment
Network type: Home / Lab network
Scope: Local subnet only (192.168.1.0/24)
Authorization: Network owned and managed by me
OS: Linux
Tools Used
Nmap
What Was Done
Identified the active network interface and subnet
Performed host discovery to list active devices
Conducted a light service scan on the router (non-intrusive)
Classified devices based on role and behavior
Interpreted risks using clear, human-readable explanations
Key Findings
Multiple active devices were identified on the local network
The router exposed several common services (FTP, HTTP, SMB)
Some services may be unnecessary in a home environment
Device visibility helps reduce unknown or unmanaged risks
Risk Interpretation (Plain Language)
FTP (Port 21)
Legacy service that is not encrypted. If unused, it increases unnecessary exposure.

HTTP (Port 80)
Indicates an unencrypted management interface. Credentials may be exposed on local networks.

SMB (Port 445)
Common in LAN environments but should never be exposed beyond the local network.

# Recommendations
Disable unused router services (e.g., FTP)
Use HTTPS for router management if available
Regularly review connected devices
Isolate IoT devices when possible
Keep router firmware up to date
Screenshots
Sensitive IP addresses and identifiers have been anonymized.

# Ethical Note
All scanning activities were performed on a network I own or manage. No intrusive, aggressive, or illegal actions were conducted. This project focuses on awareness, visibility, and basic security hygiene.

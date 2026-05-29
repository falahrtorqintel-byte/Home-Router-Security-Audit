#  Home Router Security Audit

Project Type:Cybersecurity / Network Security
Device: ZTE F663NV3a (ISP Firmware)
Status: Completed

Overview This project documents a full security audit and hardening process performed on a home router after encountering a real connection error on a Windows laptop.
The issue led to a deeper investigation into the router’s configuration, revealing several common security weaknesses found in ISP-provided routers.

The goal of this project:

Improve the security of the home Wi-Fi network
Close high-risk vulnerabilities (WPS, UPnP, weak encryption, default admin access)
Understand router configuration at a technical level
Build strong cybersecurity documentation for a professional portfolio
Background The audit began with a simple problem:
Windows reported an “unencrypted DNS” status and failed to connect to Wi-Fi.

This triggered a step-by-step investigation that uncovered:

Weak default router configurations left by the ISP
Hidden menus and locked-down settings
Disabled firewall
Mixed WPA modes and outdated TKIP encryption
Default admin password
No user education from the ISP regarding security
This project became a real-world learning experience in securing an actual network environment.

🛠️ Hardening Steps Performed
✅ 1. Upgraded Wi-Fi Security Mode
Before: WPA/WPA2 Mixed Mode + TKIP
After: WPA2-PSK + AES
Reason: AES is modern, secure, and immune to legacy attacks targeting TKIP.
✅ 2. Strengthened Wi-Fi Password
Replaced the short password with a long passphrase (3–4 random words + numbers + symbols).
Improves resistance against brute-force and dictionary attacks.

✅ 3. Changed the Router Admin Password
Removed default “admin/admin” credential
Set a strong, long administrator password
Prevents unauthorized access to router configuration
✅ 4. Enabled Firewall (HIGH Mode)
Firewall previously disabled by ISP.
HIGH mode protects the network from:

External port scanning
Ping/ICMP probing
Unwanted inbound traffic
Internal LAN-to-LAN communication remains allowed for testing and learning.
✅ 5. Checked and Disabled Risky Features
Verified through hidden pages:

WPS: Not available → likely disabled by firmware (safe)
UPnP: Not available → router returns 404 (safe)
Checked manually using: Both returned 404 Not Found, confirming that dangerous features are disabled.

✅ 6. Limited Maximum Wi-Fi Clients
Default: 32 devices
Updated to: 10 devices
Benefits:

Prevents unauthorized users from connecting
Reduces network congestion
Helps detect unknown devices more easily
Adjusted Transmit Power
Reduced from maximum → 80%
Minimizes Wi-Fi signal leakage outside the home
Helps reduce wireless attack surface
Additional Monitoring & Analysis
Checked SSID Information
Reviewed Device Information (WLAN/LAN status, packet counters)
Analyzed basic traffic (ARP, DHCP broadcast)
Observed network stability and packet errors
🖼️ Included Screenshots (Suggested)
Screenshot	Status
Router Login Page	✔
WPA2 + AES Security Settings	✔
Firewall set to HIGH	✔
Admin Password Change Page	✔
Maximum Clients = 10	✔
WPS/UPnP 404 Not Found	✔
SSID Information Page	✔
Transmit Power = 80%	✔
🧪 Results & Security Improvements
All major vulnerabilities have been closed:
Default admin password → secured
Mixed WPA mode / TKIP → AES only
Firewall OFF → HIGH enabled
Unlimited Wi-Fi clients → limited
Overpowered transmission → optimized
WPS/UPnP → *disabled / inaccessible
No unknown devices detected
This router is now significantly more secure than standard ISP installations.

🧠 Lessons Learned

A small technical issue can lead to deep cybersecurity learning.
ISP routers often ship with unsafe default configurations.
Security awareness is essential for all network users.
Real-world auditing experience is extremely valuable for cybersecurity careers.
Documentation and analysis make the project strong for a portfolio.
🎓 Skills Gained

Wireless security (WPA2, AES, WPS, UPnP)
Router hardening techniques
Basic network traffic analysis
ARP, DHCP behavior understanding
Firewall configuration
Password entropy & security design

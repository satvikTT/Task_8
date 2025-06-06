# Working and Understanding VPN - Virtual Private Network (Task_8)

---
## Objective

Understand the role of VPNs (Virtual Private Networks) in enhancing online privacy, protecting communication, and masking IP addresses through practical experience.
---
## Tools used:

- **Free VPN Clients**: ProtonVPN (Free Tier), Windscribe (Free)
- **Websites Used**:
  - ```bash
    https://whatismyipaddress.com
    ```
  - ```bash
    https://dnsleaktest.com
    ```
  - ```bash
    https://ipleak.net
    ```
---
## Steps Followed

1. **Signup and Installation**
   - Create a free account on ProtonVPN / Windscribe.
   - Downlaod and Install the VPN client. 
2. **Connecting to VPN**
   - Launch the Client and log into it.
   - Select a VPN server (try to choose the closest for better perfromance).
3. **IP Address verification**
   - Check original IP address using :
     ```bash
     whatismyipaddress.com
     ```
   - After VPN connection, note the changed IP address and new location.
4. **Encryption Verification** & **Performance Comparison**
   - Access secure websites (HTTPS).
   - Verify VPN encryption using DNS Leak Test and IP Leak Test.
   - Run DNS leak test to ensure DNS queries are encrypted.
     ```bash
     dnsleaktest.com
     ```
   - Disconnect VPN and repeat the IP test for comparison.
   - Observe differences in speed and location visibility.
---
## VPN vs Actual IP Test:

### Without VPN (Real IP):
- **Public IP**: 49.36.187.191
- **ISP**: Reliance Jio (India)
- **DNS Servers**: Multiple from Reliance Jio (India)
- **Location**: Delhi, India
- **DNS Leak**: DNS servers reveal real ISP & region (No protection)

### With VPN (ProtonVPN connected):
- **Public IP**: 2.58.44.251
- **ISP**: M247 Europe SRL (Netherlands)
- **DNS Servers**: Netherlands & Sweden
- **Location**: Amsterdam, Netherlands
- **DNS Leak Test**: DNS requests are routed through encrypted VPN DNS servers.
- **Result**: Real IP hidden, traffic encrypted, no DNS leak.
---
## Summary: VPN and real IP difference

| Feature                    | Without VPN                     | With VPN                              |
|----------------------------|---------------------------------|---------------------------------------|
| **Public IP**              | Real ISP IP shown               | VPN-assigned IP shown                 |
| **Location**               | Actual location visible         | Masked (e.g., Netherlands)            |
| **DNS Servers**            | From actual ISP                 | From VPN or third-party               |
| **Privacy Risk**           | High (identity exposed)         | Low (identity and traffic protected)  |
| **Encryption**             | No                              | Yes                                   |
| **ISP Visibility**         | Sees all browsing traffic       | Only sees encrypted VPN tunnel        |
---
## Benefits and Limitations:

###Benefits of VPNs
1. Privacy Protection
- Hides your real IP address from websites and ISPs.
- Prevents tracking of your online activities.
2. Data Encryption
- Encrypts your internet traffic, securing it from hackers, especially on public Wi-Fi.
3. Bypass Geo-Restrictions & Censorship
- Access content/services (e.g., Netflix, YouTube, news sites) restricted in your region.
4. Secure Remote Access
- Allows employees to access company networks securely from anywhere.
5. Improved Online Security
- Reduces risk of man-in-the-middle attacks and eavesdropping.
6. Safe File Sharing
- Makes it safer to share large files over long distances or insecure networks.
###Limitations of VPNs
1. Reduced Internet Speed
- Encryption and routing through remote servers can slow down browsing and downloads.
2. Cost
- Reliable VPN services usually require a paid subscription.
3. Not 100% Anonymous
- VPN providers may still log your activity. True anonymity often requires additional tools like Tor.
4. Incompatibility with Some Services
- Some websites and apps block VPN traffic (e.g., banking apps, streaming services).
5. Legal Restrictions
- VPN usage is restricted or illegal in some countries (e.g., China, Iran, North Korea).
6. Potential Trust Issues
- Free or unknown VPN providers might sell user data or lack proper security protocols.

---
## Outcome:

Haivng hands-on experience with VPN tools and a better understanding of:
- How VPNs mask your IP address
- How DNS leak tests work
- The significance of encrypted tunnels
- Benefits and limitations of using a VPN
---
## Learning

- VPNs mask your actual IP and replace it with that of a remote server.
- They encrypt your internet traffic, making it unreadable to ISPs and hackers.
- Using VPN protects against DNS and WebRTC leaks that can expose your identity.
- VPNs change geographic location digitally, enabling access to region-restricted content.
- Free VPNs have limitations (limited speed, servers, logs policy) compared to premium ones.

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
## Summary: VPN Privacy Benefits

| Feature                    | Without VPN                     | With VPN                              |
|----------------------------|---------------------------------|---------------------------------------|
| **Public IP**              | Real ISP IP shown               | VPN-assigned IP shown                 |
| **Location**               | Actual location visible         | Masked (e.g., Netherlands)            |
| **DNS Servers**            | From actual ISP                 | From VPN or third-party               |
| **Privacy Risk**           | High (identity exposed)         | Low (identity and traffic protected)  |
| **Encryption**             | No                              | Yes                                   |
| **ISP Visibility**         | Sees all browsing traffic       | Only sees encrypted VPN tunnel        |
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

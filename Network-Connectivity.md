# Network Connectivity Troubleshooting Guide

## Purpose
Provide a structured workflow for diagnosing and resolving network connectivity issues in a help desk environment.

---

## Step 1: Identify the Scope of the Issue

Ask the user:

• Can you access any websites?  
• Are other users affected?  
• Is the issue limited to one application?  
• Are you connected via Wi-Fi or Ethernet?  

Determine whether the issue is:

• User-specific  
• Device-specific  
• Network-wide  

---

## Step 2: Check Physical Connections

Verify:

• Ethernet cable is securely connected  
• Network port lights are active  
• Wi-Fi is enabled on the device  

If wireless:

• Confirm connection to correct SSID  

---

## Step 3: Check IP Configuration

Run:

ipconfig /all

Verify:

• Device has a valid IP address  
• Correct subnet mask and gateway  
• DNS server is assigned  

Common issue:

169.254.x.x address → Indicates DHCP failure

---

## Step 4: Test Connectivity Using Ping

Follow troubleshooting sequence:

1. Ping localhost:
ping 127.0.0.1

2. Ping default gateway:
ping <gateway IP>

3. Ping external address:
ping 8.8.8.8

4. Ping domain name:
ping google.com

Results help determine whether issue is:

• Local device problem  
• Network issue  
• Internet connectivity problem  
• DNS resolution failure  

---

## Step 5: Check Network Adapter Status

Verify:

• Adapter is enabled  
• No driver errors in Device Manager  

Try:

Disable and re-enable adapter

---

## Step 6: Renew IP Address

Run:

ipconfig /release  
ipconfig /renew  

This resolves many DHCP-related issues.

---

## Step 7: Flush DNS Cache

Run:

ipconfig /flushdns

Useful when:

• Websites do not load correctly  
• DNS records are outdated  

---

## Step 8: Test Internet Access via Browser

Check if:

• Only specific sites fail  
• VPN connection is causing issues  
• Proxy settings are enabled incorrectly  

---

## Common Issues and Fixes

| Issue | Likely Cause | Solution |
|------|-------------|----------|
| No IP address | DHCP failure | Renew IP or check DHCP server |
| Can ping IP but not website | DNS issue | Flush DNS or update DNS settings |
| Cannot reach gateway | Network cable or switch issue | Check physical connection |
| Wi-Fi connected but no internet | Router or ISP problem | Restart router |

---

## Escalation Criteria

Escalate if:

• Network switch or router failure suspected  
• Multiple users affected  
• VLAN configuration issues present  
• Firewall blocking connectivity  

---

## Best Practices

• Document troubleshooting steps in ticket  
• Record IP configuration details  
• Confirm resolution with user before closing ticket  

---

*This guide demonstrates real-world help desk network troubleshooting procedures.*

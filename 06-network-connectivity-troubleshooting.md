# Ticket 006 — Network Connectivity Troubleshooting

## Ticket Summary
Performed network connectivity troubleshooting on a Windows computer to diagnose and verify local network, internet, and DNS connectivity.

## Environment
- Windows PC
- Command Prompt
- Wi-Fi Network
- TCP/IP
- DNS
- DHCP

## Issue
Simulated a help desk scenario in which a user was connected to Wi-Fi but reported problems accessing the internet.

## Troubleshooting Steps
1. Opened Command Prompt.
2. Ran `ipconfig` to review the computer's network configuration and verify that an IPv4 address and default gateway were assigned.
3. Pinged the default gateway to test communication between the computer and local network/router.
4. Received 4 of 4 packets with 0% packet loss, confirming local network connectivity.
5. Ran `ping 8.8.8.8` to test external internet connectivity.
6. Received 4 of 4 packets with 0% packet loss, confirming internet connectivity.
7. Ran `ping google.com` to test DNS name resolution and external connectivity.
8. Successfully resolved the domain and received responses with 0% packet loss.
9. Ran `ipconfig /flushdns` to clear the DNS resolver cache.
10. Ran `ipconfig /release` to release the current DHCP-assigned IPv4 configuration.
11. Ran `ipconfig /renew` to request network configuration from the DHCP server again.
12. Ran `ping google.com` again to verify connectivity after the troubleshooting steps.

## Resolution
Local network, internet, and DNS connectivity were successfully verified. The DNS cache was cleared and the computer's DHCP configuration was renewed. A final connectivity test returned 0% packet loss.

## Commands Used
- `ipconfig`
- `ping`
- `ipconfig /flushdns`
- `ipconfig /release`
- `ipconfig /renew`

## Skills Demonstrated
- Network Troubleshooting
- Windows Command Prompt
- TCP/IP Fundamentals
- DNS Troubleshooting
- DHCP Troubleshooting
- IP Configuration
- Connectivity Testing
- Help Desk Ticket Documentation

## Lab Note
This ticket was completed as a simulated help desk scenario in a hands-on IT support lab environment.

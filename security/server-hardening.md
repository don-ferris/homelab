## Server Hardening

- Remove or disable unnecessary services and open ports.
- Enforce strong password policies; disable accounts with empty passwords.
- Always enable firewalls and restrict network traffic to trusted IP ranges.
- **Run CrowdSec:** Deploy CrowdSec on every server to monitor, detect, and block suspicious network and service activity using community-based intelligence.
- Use Fail2ban for targeted brute-force protection (e.g., SSH, web login).
- Use SELinux, AppArmor, or similar kernel security features in enforcing mode.
- Regularly update system packages (OS and kernel).
- Limit physical access to servers (BIOS password, disable USB/Thunderbolt boot if appropriate).
- Turn off unnecessary system protocols (disable ICMP/Ping if not needed).
- Implement system logging and auditing (central logging to monitor for unwanted changes).
- Remove unnecessary packages and users from each server.

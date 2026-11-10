```text
██╗  ██╗ █████╗ ██╗    ██╗██╗  ██╗ ██████╗ ██████╗ ███████╗
██║  ██║██╔══██╗██║    ██║██║ ██╔╝██╔═══██╗██╔══██╗██╔════╝
███████║███████║██║ █╗ ██║█████╔╝ ██║   ██║██║  ██║█████╗
██╔══██║██╔══██║██║███╗██║██╔═██╗ ██║   ██║██║  ██║██╔══╝
██║  ██║██║  ██║╚███╔███╔╝██║  ██╗╚██████╔╝██████╔╝███████╗
╚═╝  ╚═╝╚═╝  ╚═╝ ╚══╝╚══╝ ╚═╝  ╚═╝ ╚═════╝ ╚═════╝ ╚══════╝
```

```powershell
PS C:\> Get-ADUser hawkode -Properties Description, info, MemberOf, AdminCount

DistinguishedName : CN=hawkode,OU=Tinkerers,DC=homelab,DC=internal
Enabled           : True
Description       : Builds it. Hardens it. Breaks it. Writes down what happened.
info              : AD, Entra ID, networks, logs, and how all of them get attacked.
MemberOf          : {Protected Users}
AdminCount        : 0
```

#### ~/main_quest
```diff
+ [*] Mapping AD and Entra ID attack paths, then closing them
+ [*] Splitting the homelab into VLANs that actually mean something
+ [*] Writing Splunk detections that fire before the damage is done
```

#### ~/crafted
- `[+]` [entra-iam-automation](https://github.com/Hawkode/entra-iam-automation) - one line on what it does.
- `[+]` [MailGuard](https://github.com/Hawkode/MailGuard) - one line on what it does.
- `[+]` [Windows-Health-Monitor](https://github.com/Hawkode/Windows-Health-Monitor) - one line on what it does.

#### ~/training_grounds
- `[+]` [splunk-security-logs](https://github.com/Hawkode/splunk-security-logs) - log analysis and detection in Splunk.
- `[+]` [OpenVAS-Vulnerability-Scanning](https://github.com/Hawkode/OpenVAS-Vulnerability-Scanning) - vulnerability scanning and triage.
- `[+]` [Snort-Lab](https://github.com/Hawkode/Snort-Lab) - IDS rules. Packets that don't match shall not pass.
- `[+]` [nmap-security-assessment](https://github.com/Hawkode/nmap-security-assessment) - network discovery and service enumeration.
- `[+]` [Metasploitable 2 pentest](https://github.com/Hawkode/Penetration-testing-techniques-Metasploitable-2-) - breaking a box built to be broken.
- `[+]` [Windows-Defender-Firewall-Lab](https://github.com/Hawkode/Windows-Defender-Firewall-Lab) - host firewall rules and hardening.

#### ~/inventory
```text
┌──(hawkode㉿kali)-[~/inventory]
└─$ ls
bloodhound  burpsuite  hashcat  metasploit  nmap  openvas  powershell  python  snort  splunk  wireshark
```

```diff
- [-] Meterpreter session 1 closed.  Reason: User exit
```

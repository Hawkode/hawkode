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

DistinguishedName : CN=hawkode,OU=SuperUser 😎,DC=homelab,DC=internal
Enabled           : True
Description       : One does not simply walk into Domain Admin. Usually. 🙃
info              : Entra ID, AD, Kerberos, privesc, phishing, and the logs that catch them.
MemberOf          : {Protected Users}
AdminCount        : 0
```

#### ~/main_quest
```diff
+ [*] Automating joiners, movers, leavers and access reviews across AD and Entra ID
+ [*] Hunting standing admins, risky app consents and stale accounts
+ [*] Splitting networks into VLANs that actually mean something
+ [*] Closing patch gaps before a scanner finds them
+ [*] Taking Windows from low-priv to SYSTEM, then catching it in Splunk
```

#### ~/crafted
- `[+]` [entra-iam-automation](https://github.com/Hawkode/entra-iam-automation) - joiner, mover, leaver and access reviews for Entra ID and hybrid AD.
- `[+]` [MailGuard](https://github.com/Hawkode/MailGuard) - phishing triage CLI: headers, links, attachments and SPF/DKIM/DMARC, scored.
- `[+]` [Windows-Health-Monitor](https://github.com/Hawkode/Windows-Health-Monitor) - endpoint posture checks (Defender, firewall, patching, BitLocker, log clearing) that report to Splunk. Tested on PowerShell 5.1 and 7.
- `[+]` [PasswordAnalyzer](https://github.com/Hawkode/PasswordAnalyzer) - password auditor: entropy, Have I Been Pwned k-anonymity check, zxcvbn strength.

#### ~/prod
- `[+]` [Two-site domain consolidation](https://hawkode.github.io/projects/windows-server-2022-domain-migration/) - two office domains merged into one on Windows Server 2022, 60+ users moved, Entra ID identities matched.
- `[+]` [Snipe-IT asset inventory](https://hawkode.github.io/projects/snipe-it-asset-inventory/) - every device tracked to a site, a desk and a lifecycle stage.
- `[+]` [Network cabling & port mapping](https://hawkode.github.io/projects/network-cabling-port-mapping/) - patch panel to wall socket: traced, labelled, documented.

#### ~/training_grounds
- `[+]` [IAM Lab in Entra ID](https://hawkode.github.io/projects/entra-iam-lab/) - RBAC, Conditional Access, PIM and access reviews from an empty tenant.
- `[+]` [Windows Privilege Escalation](https://hawkode.github.io/projects/windows-privilege-escalation/) - low-priv to SYSTEM, and the event IDs that expose it.
- `[+]` [Splunk privesc detection](https://hawkode.github.io/projects/splunk-privesc-detection/) - Sysmon, SPL and alerts mapped to MITRE ATT&CK.
- `[+]` [Windows Health Monitor](https://hawkode.github.io/projects/windows-health-monitor/) - part 3: harden the host, and alert when the monitor goes quiet.
- `[+]` [Metasploitable 2 pentest](https://github.com/Hawkode/Penetration-testing-techniques-Metasploitable-2-) - breaking a box built to be broken.
- `[+]` [Hydra](https://hawkode.github.io/guides/hydra-online-password-attacks/) - online password attacks, and how to spot and stop them.
- `[+]` [John the Ripper](https://hawkode.github.io/guides/john-the-ripper-password-cracking/) - offline cracking, and why the hash is the real defence.
- `[+]` [Home network](https://hawkode.github.io/projects/home-network-udr7/) - VLANs and zone firewall rules. Untrusted traffic shall not pass.

#### ~/inventory
```text
┌──(hawkode㉿kali)-[~/inventory]
└─$ ls
active-directory  entra-connect    john             powershell    snort           wireshark
burpsuite         exchange-online  metasploit       privesccheck  splunk
dhcp              group-policy     microsoft.graph  python        unifi
dns               hashcat          nmap             robocopy      windows-server
endpoint-central  hydra            openvas          snipe-it      wireguard
```

```diff
- [-] Meterpreter session 1 closed.  Reason: User exit 👋
```

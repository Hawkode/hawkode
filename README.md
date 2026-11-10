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
Description       : Finds the path to Domain Admin. Then closes it.
info              : Entra ID, AD, Kerberos, privesc, phishing, and the logs that catch them.
MemberOf          : {Protected Users}
AdminCount        : 0
```

#### ~/main_quest
```diff
+ [*] Automating joiners, movers, leavers and access reviews across AD and Entra ID
+ [*] Hunting standing admins, risky app consents and stale accounts
+ [*] Taking Windows from low-priv to SYSTEM, then catching it in Splunk
+ [*] Pulling phishing emails apart, header by header
```

#### ~/crafted
- `[+]` [entra-iam-automation](https://github.com/Hawkode/entra-iam-automation) - joiner, mover, leaver and access reviews for Entra ID and hybrid AD.
- `[+]` [MailGuard](https://github.com/Hawkode/MailGuard) - phishing triage CLI: headers, links, attachments and SPF/DKIM/DMARC, scored.
- `[+]` [PasswordAnalyzer](https://github.com/Hawkode/PasswordAnalyzer) - password entropy, Have I Been Pwned check and a John the Ripper wrapper.

#### ~/training_grounds
- `[+]` [IAM Lab in Entra ID](https://hawkode.github.io/projects/entra-iam-lab/) - RBAC, Conditional Access, PIM and access reviews from an empty tenant.
- `[+]` [Windows Privilege Escalation](https://hawkode.github.io/projects/windows-privilege-escalation/) - low-priv to SYSTEM, and the event IDs that expose it.
- `[+]` [Splunk privesc detection](https://hawkode.github.io/projects/splunk-privesc-detection/) - Sysmon, SPL and alerts mapped to MITRE ATT&CK.
- `[+]` [Metasploitable 2 pentest](https://github.com/Hawkode/Penetration-testing-techniques-Metasploitable-2-) - breaking a box built to be broken.
- `[+]` [Hydra](https://hawkode.github.io/guides/hydra-online-password-attacks/) - online password attacks, and how to spot and stop them.
- `[+]` [John the Ripper](https://hawkode.github.io/guides/john-the-ripper-password-cracking/) - offline cracking, and why the hash is the real defence.
- `[+]` [Home network](https://hawkode.github.io/projects/home-network-udr7/) - VLANs and zone firewall rules. Untrusted traffic shall not pass.

#### ~/inventory
```text
┌──(hawkode㉿kali)-[~/inventory]
└─$ ls
burpsuite      hydra       microsoft.graph  powershell    seatbelt  sysmon
entra-connect  john        nmap             privesccheck  snort     winpeas
hashcat        metasploit  openvas          python        splunk    wireshark
```

```diff
- [-] Meterpreter session 1 closed.  Reason: User exit
```

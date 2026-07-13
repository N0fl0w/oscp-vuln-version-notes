# 👣 Foothold / Ports

## 🐧 Linux

### Port 25 — SMTP

#### ▸ Sendmail + clamav-milter

- **Service:** Mail server filtering system

- **Vulnerability:** Command Injection → RCE

- **Version:** clamav-milter < 0.91.2

- **Exploit:** [https://www.exploit-db.com/exploits/4761](https://www.exploit-db.com/exploits/4761)

#### ▸ OpenSMPTD

- **Service:** OpenSMTPD

- **Vulnerability:** RCE as root

- **Version:** 5.7.1 through 6.6.3

- **Exploit:** [https://www.exploit-db.com/exploits/47984](https://www.exploit-db.com/exploits/47984) or can use metasploit

### Port 80 — HTTP (Web Applications )

#### ▸ ZoneMinder Web Console

- **Service:** CCTV monitoring web interface

- **Vulnerability:** SQL Injection → RCE

- **Version:** ZoneMinder 1.29.0

- **Exploit:** [https://www.exploit-db.com/exploits/41239](https://www.exploit-db.com/exploits/41239)

#### ▸ Generic Web App (Login / Panel)

- **Service:** Custom web application

- **Vulnerability:** Command Injection

- **Version:** Varies

- **Exploit:** Manual

#### ▸ PHP Photo Gallery

- **Service:** Simple PHP Photo Gallery

- **Vulnerability:** SQL Injection

- **Version:** v8.0

- **Exploit:** sqlmap

- [https://www.exploit-db.com/exploits/48424](https://www.exploit-db.com/exploits/48424)

#### ▸ CS CART Web

- **Service:** CS CART eCommerce Platform

- **Vulnerability:** Unrestricted File Upload → RCE

- **Version:** 1.3.3

- **Exploit:** Manual (webshell upload )

- [https://gist.github.com/momenbasel/ccb91523f86714edb96c871d4cf1d05c](https://gist.github.com/momenbasel/ccb91523f86714edb96c871d4cf1d05c)

#### ▸ Zenphoto Web

- **Service:** ZenPhoto in /test folder

- **Vulnerability:** RCE

- **Version:** 1.4.1.4

- **Exploit:** [https://www.exploit-db.com/exploits/18083](https://www.exploit-db.com/exploits/18083)

#### ▸ WordPress

- **Service:** Simple-File-List plugin

- **Vulnerability:** File upload

- **Version:** 4.2.2

- **Exploit:** [https://www.exploit-db.com/exploits/48979](https://www.exploit-db.com/exploits/48979)

- **Service:** Site-Editor plugin

- **Vulnerability:** Local file inclusions

- **Version:** v1.1

- **Exploit:** [https://www.exploit-db.com/exploits/44340](https://www.exploit-db.com/exploits/44340)

- This attack allows also to run webshells or reverse shells if uploaded

- **Service:** Wp-Advanced-search plugin

- **Vulnerability:** Unauthenticated SQL Injection

- **Version:** < 3.3.9.2

- **Exploit:** [https://wpscan.com/vulnerability/2ddd6839-6bcb-4bb8-97e0-1516b8c2b99b/](https://wpscan.com/vulnerability/2ddd6839-6bcb-4bb8-97e0-1516b8c2b99b/)

#### ▸ GravCMS RCE

- **Service:** GravCMS

- **Vulnerability:** Arbitrary YAML Write/Update (Unauthenticated ) RCE

- **Version:** 1.10.7

- **Exploit:** [https://www.exploit-db.com/exploits/49973](https://www.exploit-db.com/exploits/49973)

#### ▸ BoxBilling

- **Service:** BoxBilling

- **Vulnerability:** Remote Code Execution (RCE )

- **Prerequisites:** Needed admin / administrator account with one order

- **Version:** 4.22.1.5

- **Exploit:** [https://github.com/0xk4b1r/CVE-2022-3552](https://github.com/0xk4b1r/CVE-2022-3552)

#### ▸ Subrion CMS

- **Service:** Subrion CMS at `/panel`

- **Vulnerability:** Arbitrary File Upload to RCE

- **Prerequisites:** Needed admin / administrator account

- **Version:** 4.2.1

- **Exploit:** [https://www.exploit-db.com/exploits/49876](https://www.exploit-db.com/exploits/49876)

- Note: Make sure to include /panel/

#### ▸ Laravel

- **Service:** Laravel

- **Vulnerability:** debug mode - Remote code execution

- **Prerequisites:** Needed admin / administrator account

- **Version:** 8.4.2

- **Exploit:** [https://github.com/zhzyker/CVE-2021-3129](https://github.com/zhzyker/CVE-2021-3129)

- Try this too [https://github.com/khanhnv-2091/laravel-8.4.2-rce](https://github.com/khanhnv-2091/laravel-8.4.2-rce)

#### ▸ Filemanager

- **Service:** Responsive FileManager

- **Vulnerability:** 'path' Path Traversal

- **Version:** 9.13.4

- **Exploit:** [https://www.exploit-db.com/exploits/49359](https://www.exploit-db.com/exploits/49359)


#### ▸ OpenEMR

- **Service:** OpenEMR

- **Vulnerability:** RCE (AUTHENTICATED )

- **Version:** v5.0.1.3

- **Exploit:** [https://www.exploit-db.com/exploits/45161](https://www.exploit-db.com/exploits/45161)


#### ▸ pgAdmin

- **Service:** pgAdmin

- **Vulnerability:** Path Traversal in Session Handling Leads to Unsafe Deserialization and RCE

- **Version:** <=8.3

- **Exploit**: Automate way [https://www.rapid7.com/db/modules/exploit/multi/http/pgadmin_session_deserialization/](https://www.rapid7.com/db/modules/exploit/multi/http/pgadmin_session_deserialization/)**

- **Exploit:** Manual way [https://www.shielder.com/advisories/pgadmin-path-traversal_leads_to_unsafe_deserialization_and_rce/](https://www.shielder.com/advisories/pgadmin-path-traversal_leads_to_unsafe_deserialization_and_rce/)

#### ▸ LimeSurvey

- **Service:** LimeSurvey

- **Vulnerability:** A Remote Code Execution

- **Version:** 5.2.4

- **Exploit:** [https://github.com/D3Ext/CVE-2021-44967/tree/main](https://github.com/D3Ext/CVE-2021-44967/tree/main)

- Manual way: [https://github.com/Y1LD1R1M-1337/Limesurvey-RCE](https://github.com/Y1LD1R1M-1337/Limesurvey-RCE)

#### ▸ JetBrains TeamCity

- **Service:** JetBrains TeamCity

- **Vulnerability:** Authentication Bypass

- **Version:** 2023.11.4

- **Exploit:** [https://www.exploit-db.com/exploits/52411](https://www.exploit-db.com/exploits/52411)

#### ▸ php-spx

- **Service:** php-spx

- **Vulnerability:** path traversal vulnerability

- **Version:** 0.4.15

- **Exploit:** [https://www.exploit-db.com/exploits/52411](https://www.exploit-db.com/exploits/52411)

#### ▸ MantisBT

- **Service:** MantisBT

- **Vulnerability:** Arbitrary File Read inside install.php script

- **Version:** Install.php being exposed

- **Exploit:** [https://mantisbt.org/bugs/view.php?id=23173](https://mantisbt.org/bugs/view.php?id=23173)

- **Service:** MantisBT

- **Vulnerability:** Command Execution / Injection Vulnerability

- **Version:** 2.5.2

- **Exploit:** [https://mantisbt.org/bugs/view.php?id=26091](https://mantisbt.org/bugs/view.php?id=26091)

#### ▸ Simple Online Planning Tool

- **Service:** SOPlanning

- **Vulnerability:** Remote Code Execution (RCE ) (Authenticated)

- **Version:** 1.52.01

- **Exploit:** [https://www.exploit-db.com/exploits/52082](https://www.exploit-db.com/exploits/52082)

---

### Port 3000

#### ▸ Cassandra Web

- **Service:** Cassandra web

- **Vulnerability:** Remote File disclosure

- **Version:** 0.5.0

- **Exploit:** [https://www.exploit-db.com/exploits/49362](https://www.exploit-db.com/exploits/49362)

- Note: Read the exploit and the file to check

#### ▸ Grafana

- **Service:** Grafana web

- **Vulnerability:** Directory Traversal and Arbitrary File Read

- **Version:** 8.3.0

- **Exploit:** [https://www.exploit-db.com/exploits/50581](https://www.exploit-db.com/exploits/50581)


#### ▸ Gitea

- **Service:** Gitea / Like github

- **Vulnerability:** Remote Code Execution

- **Version:** 1.7.5

- **Exploit:** [https://www.exploit-db.com/exploits/49383](https://www.exploit-db.com/exploits/49383)

#### ▸ CodoLogic

- **Service:** CodoForum

- **Vulnerability:** Remote Code Execution

- **Version:** v.5.1

- **Exploit:** [https://www.exploit-db.com/exploits/50978](https://www.exploit-db.com/exploits/50978)

#### ▸ SuiteCRM

- **Service:** SuiteCRM

- **Vulnerability:** Remote Code Execution

- **Version:** <= 7.12.4

- **Exploit:** [https://github.com/manuelz120/CVE-2022-23940](https://github.com/manuelz120/CVE-2022-23940)

#### ▸ FuguHub

- **Service:** FuguHub

- **Vulnerability:** Remote Code Execution

- **Version:** 8.4

- **Exploit:** [https://github.com/SanjinDedic/FuguHub-8.4-Authenticated-RCE-CVE-2024-27697](https://github.com/SanjinDedic/FuguHub-8.4-Authenticated-RCE-CVE-2024-27697)

#### ▸ ImageMagick

- **Service:** ImageMagick

- **Vulnerability:** Remote Code Execution

- **Version:** 6.9.6-4

- **Exploit:** [https://github.com/SudoIndividual/CVE-2023-34152/](https://github.com/SudoIndividual/CVE-2023-34152/)

#### ▸ HTMLAWED

- **Service:** HTMLAWED Test

- **Vulnerability:** **File upload bypass to RCE**

- **Version:** 1.2.1

- **Exploit:** [https://github.com/flatpressblog/flatpress/issues/152](https://github.com/flatpressblog/flatpress/issues/152)

#### ▸ FlatPress

- **Service:** HTMLAWED Test

- **Vulnerability:** Remote Code Execution

- **Version:** 1.2.5

- **Exploit:** [https://github.com/cosad3s/CVE-2022-35914-poc](https://github.com/cosad3s/CVE-2022-35914-poc)

#### ▸ RubyDome HTML TO PDF

- **Service:** pdfkit

- **Vulnerability:** Remote Code Execution

- **Version:** < 0.8.7.2

- **Exploit:** [https://github.com/UNICORDev/exploit-CVE-2022-25765](https://github.com/UNICORDev/exploit-CVE-2022-25765)

#### ▸ RubyDome HTML TO PDF

- **Service:** pdfkit

- **Vulnerability:** Remote Code Execution

- **Version:** < 0.8.7.2

- **Exploit:** [https://github.com/UNICORDev/exploit-CVE-2022-25765](https://github.com/UNICORDev/exploit-CVE-2022-25765)

#### ▸ PluXml

- **Service:** PluXml

- **Vulnerability:** Remote Code Execution

- **Version:** 5.8.7

- **Exploit:** [https://github.com/erlaplante/pluxml-rce](https://github.com/erlaplante/pluxml-rce)

#### ▸ Jorani

- **Service:** PluXml

- **Vulnerability:** Unrestricted File Upload → Remote Code Execution Exploit

- **Version:** 1.0.0

- **Exploit:** [https://github.com/samipmainali/Jorani-Reverse-Shell-v1.0.0](https://github.com/samipmainali/Jorani-Reverse-Shell-v1.0.0)

#### ▸ SeaCMS

- **Service:** SeaCMS

- **Vulnerability:** 'file' Local File Inclusion

- **Version:** 11.1

- **Exploit:** [https://www.exploit-db.com/exploits/49250](https://www.exploit-db.com/exploits/49250)

---

### Port 4506

#### ▸ ZeroMQ ZMTP 2.0

- **Service:** Saltstack 3000.1

- **Vulnerability:** RCE

- **Version:** 2.0

- **Exploit:** [https://github.com/jasperla/CVE-2020-11651-poc](https://github.com/jasperla/CVE-2020-11651-poc)

---

### Port 5437

#### ▸ PostgreSQL

- **Service:** postgresql

- **Vulnerability:** RCE to a shell using default creds

- **Version:** 9.3-11.7

- **Exploit:** [https://www.exploit-db.com/exploits/50847](https://www.exploit-db.com/exploits/50847)

---

### Port 6379

#### ▸ Redis

- **Service:** Redis

- **Vulnerability:** RCE

- **Version:** 4.x / 5.x ) and (5.0.14) and (4.0.14) the last exploit works well

- **Exploit:** [https://github.com/Dliv3/redis-rogue-server](https://github.com/Dliv3/redis-rogue-server) and this one is also good [https://github.com/jas502n/Redis-RCE](https://github.com/jas502n/Redis-RCE)


---

### Port 8000

#### ▸ Gerapy Web Application

- **Service:** Gerapy

- **Vulnerability:** RCE

- **Version:** 0.9.7

- **Exploit:** [https://github.com/terribledactyl/Gerapy_RCE_0.9.7/blob/main/gerapy_rce.py](https://github.com/terribledactyl/Gerapy_RCE_0.9.7/blob/main/gerapy_rce.py)

### Port 8021

#### ▸ FreeSWITCH

- **Service:** freeswitch-event

- **Vulnerability:** Command Execution

- **Version:** 1.10.1

- **Exploit:** [https://www.exploit-db.com/exploits/47799](https://www.exploit-db.com/exploits/47799)

#### ▸ rConfig

- **Service:** rConfig

- **Vulnerability**: SQL INJECTION + Remote Command Injection

- **Version:** 3.9.4

- **Exploit 1:** rConfig 3.9 - SQL Injection [https://www.exploit-db.com/exploits/48208](https://www.exploit-db.com/exploits/48208)

- **Exploit 2**: rConfig 3.9.4 - 'search.crud.php' RCE [https://www.exploit-db.com/exploits/48241](https://www.exploit-db.com/exploits/48241)

- Exploit 3: rConfig 3.9.x Metasploit module [https://www.rapid7.com/db/modules/exploit/linux/http/rconfig_ajaxarchivefiles_rce/](https://www.rapid7.com/db/modules/exploit/linux/http/rconfig_ajaxarchivefiles_rce/) (THIS ONE AUTOMATES ONLY NEED THIS EXPLOIT )

### Port 8080

#### ▸ Exhibitor (ZooKeeper UI)

- **Service:** Web-based management console

- **Vulnerability:** OS Command Injection

- **Version:** Exhibitor 1.0

- **Exploit:** [https://www.exploit-db.com/exploits/48654](https://www.exploit-db.com/exploits/48654)

#### ▸ Jenkins

- **Service:** Jenkins

- **Vulnerability:** File disclosure

- **Version:** <= version 2.441

- **Exploit:** [https://github.com/godylockz/CVE-2024-23897](https://github.com/godylockz/CVE-2024-23897)

### Port 8090

#### ▸ Confluence

- **Service:** Atlassian Confluence

- **Vulnerability:** OGNL injection vulnerability which can get you a shell!

- **Version:** versions <= 7.13.6 LTS and <= 7.18.0

- **Exploit:** [https://github.com/jbaines-r7/through_the_wire](https://github.com/jbaines-r7/through_the_wire)

---

### Port 9000

#### ▸ tar-fs tool being Used on Web

- **Tool:** tar-fs

- **Vulnerability:** Arbitrary File Write/Overwrite

- **Version:** 3.0.0

- **Exploit:** [https://www.exploit-db.com/exploits/52268](https://www.exploit-db.com/exploits/52268)

#### ▸ Ray OS

- **Tool:** Ray OS

- **Vulnerability:** Command Injection RCE(Unauthorized )

- **Version:** v2.6.3

- **Exploit:** [https://www.exploit-db.com/exploits/51978](https://www.exploit-db.com/exploits/51978)

### Port 9443

#### ▸ Prison Management System

- **Service:** Prison Management System

- **Vulnerability:** Sql Injection + Authenticated RCE via Unrestricted File Upload


- **Exploit:** SQL to authenticate [https://www.exploit-db.com/exploits/52017](https://www.exploit-db.com/exploits/52017)

- After authenticating can perform this [https://www.rapid7.com/db/modules/exploit/linux/http/prison_management_rce/](https://www.rapid7.com/db/modules/exploit/linux/http/prison_management_rce/) (Metasploit module )

### Port 9666

#### ▸ Pyload

- **Service:** Pyload

- **Vulnerability:** Pre-auth Remote Code Execution (RCE)

- **Version:** 0.5.0

- **Exploit:** [https://github.com/overgrowncarrot1/CVE-2023-0297](https://github.com/overgrowncarrot1/CVE-2023-0297)

### Port 9090

#### ▸ OpenFire

- **Service:** Openfire

- **Vulnerability:** Openfire Console Authentication Bypass Vulnerability with RCE plugin

- **Version:** 3.10.0<=Openfire<4.6.8 and 4.7.0 <=Openfire<4.7.5 

- **Exploit:** [https://github.com/miko550/CVE-2023-32315](https://github.com/miko550/CVE-2023-32315)

- This is only to create the admin user [https://github.com/K3ysTr0K3R/CVE-2023-32315-EXPLOIT](https://github.com/K3ysTr0K3R/CVE-2023-32315-EXPLOIT)

## 🪟 Windows

### Port 80

#### ▸ PHP Power Management

- **Service:** PHP power Management

- **Vulnerability:** # Universal Buffer Overflow Lead to an RCE as Administrator

- **Version:** 


- Metasploit module: `windows/http/hp_power_manager_filename`

#### ▸ Monstra

- **Service:** Monstra CMS

- **Vulnerability:** Authenticated RCE

- **Version:** 3.0.4

- **Exploit:** [https://github.com/wcheng729/Monstra-3.0.4-RCE/](https://github.com/wcheng729/Monstra-3.0.4-RCE/)

### Port 445

#### ▸ SMB

- **Service:** SMB ms09-050

- **Vulnerability:** 'srv2.sys' SMB Code Execution

- **Version:** Ran a Vuln script and detected


- Metasploit module: [https://www.rapid7.com/db/modules/exploit/windows/smb/ms09_050_smb2_negotiate_func_index/](https://www.rapid7.com/db/modules/exploit/windows/smb/ms09_050_smb2_negotiate_func_index/)

### Port 1978

#### ▸ Remote Mouse

- **Service:** RemoteMouse

- **Vulnerability:** Arbitrary Remote Command Execution

- **Version:** 3.008

- **Exploit:** Python exploit: [https://github.com/p0dalirius/RemoteMouse-3.008-Exploit/](https://github.com/p0dalirius/RemoteMouse-3.008-Exploit/)

### Port 4848

#### ▸ Oracle GlassFish Server

- **Service:** Oracle GlassFish Server

- **Vulnerability:** Directory Traversal

- **Version:** 4.1

- **Exploit:** [https://www.exploit-db.com/exploits/39441](https://www.exploit-db.com/exploits/39441)

### Port 8080

#### ▸ Argus Surveillance

- **Service:** Argus Surveillance

- **Vulnerability:** Directory Traversal and Password Descriptor (2 more for privilege escalation )

- **Version:** 4.0.0.0 and 4.0

- **Exploit 1:** [https://www.exploit-db.com/exploits/45296](https://www.exploit-db.com/exploits/45296) (Directory Traversal )

- Automated way: [https://github.com/Jasurbek-Masimov/CVE-2018-15745/](https://github.com/Jasurbek-Masimov/CVE-2018-15745/)

- **Exploit 2**: [https://github.com/s3l33/CVE-2022-25012/](https://github.com/s3l33/CVE-2022-25012/) (Hash Decryptor )

### Port 8081

#### ▸ Sonatype Nexus

- **Service:** H2 Database

- **Vulnerability:** Remote Code Execution (Authenticated)

- **Version:** 3.21.1

- **Exploit:** [https://www.exploit-db.com/exploits/49385](https://www.exploit-db.com/exploits/49385)

### Port 8082

#### ▸ H2 Database

- **Service:** H2 Database

- **Vulnerability:** JNI Code execution

- **Version:** 1.4.199

- **Exploit:** [https://www.exploit-db.com/exploits/49384](https://www.exploit-db.com/exploits/49384)

### Port 9998

#### ▸ SmarterMail

- **Service:** SmarterMail Build 6985

- **Vulnerability:** RCE

- **Version:** Build 6985 (Tetsed on 6191 )


---

# 🚨 Privilege Escalation

## 🐧 Linux

### Kernel Exploits

#### ▸ Linux Kernel 2.6.36-rc8 - 'RDS Protocol'

- **Service:** Kernel RDS PROTOCOL

- **Vulnerability:** Kernel exploit

- **Version:** Linux 2.6.32-21-generic 32 bit system

- **Exploit:** [https://www.exploit-db.com/exploits/15285](https://www.exploit-db.com/exploits/15285)

### Vulnerable Programs

#### ▸ PKEXEC / Pwnkit

- **Service:** Pkexec

- **Vulnerability:** polkit pkexec utilitiy

- **Version:** `pkexec version 0.96`

- **Exploit:** [https://github.com/ly4k/PwnKit](https://github.com/ly4k/PwnKit)

#### RPC.py

- **Service:** Remote Procedure Call (RPC ) framework library

- **Vulnerability:** Remote Code Execution (RCE) (if running as root)

- **Version:** 0.6.0

- **Exploit:** [https://github.com/ehtec/rpcpy-exploit/blob/main/rpcpy-exploit.py](https://github.com/ehtec/rpcpy-exploit/blob/main/rpcpy-exploit.py)

### Tools / Packages

#### Exiftool

- **Tool:** Exiftool

- **Vulnerability:** code execution vulnerability

- **Version:** 7.44 and up

- **Exploit:** [https://github.com/UNICORDev/exploit-CVE-2021-22204](https://github.com/UNICORDev/exploit-CVE-2021-22204) or follow this [https://www.exploit-db.com/docs/49881](https://www.exploit-db.com/docs/49881)

- **Note**: This escalated privs because of cron job running as root

#### Happy-dom

- **Tool:** Happy-dom

- **Vulnerability:** Arbitrary Code Injection

- **Version:** *<15.10.2

- **Exploit:** [https://security.snyk.io/vuln/SNYK-JS-HAPPYDOM-8350065](https://security.snyk.io/vuln/SNYK-JS-HAPPYDOM-8350065)

## 🪟 Windows

### Vulnerable Programs

#### ▸ PaperStream IP (TWAIN )

- **Service:** PaperStream IP

- **Vulnerability:** Local Privilege Escalation

- **Version:** 1.42.0.5685

- **Exploit:** [https://www.exploit-db.com/exploits/49382](https://www.exploit-db.com/exploits/49382) Changes are needed and make sure to use the right msfvenom payload

#### ▸ BarracudaDrive

- **Service:** BarracudaDrive

- **Vulnerability:** Insecure Folder Permissions Lead to Local Privilege Escalation

- **Version:** v6.5

- **Exploit:** [https://www.exploit-db.com/exploits/48789](https://www.exploit-db.com/exploits/48789)

#### ▸ TotalAV

- **Service:** BarracudaDrive

- **Vulnerability:** Privilege Escalation

- **Version:** 2020 4.14.31

- **Exploit:** [https://www.exploit-db.com/exploits/47897](https://www.exploit-db.com/exploits/47897) (THEIR IS A VIDEO TOO )

#### ▸ Remote Mouse GUI

- **Service:** Remote Mouse

- **Vulnerability:** Privilege Escalation

- **Version:** 3.008


#### ▸ Veyon

- **Service:** VeyonService

- **Vulnerability:** Unquoted Service Path

- **Version:** 4.3.4

- **Exploit:** [https://www.exploit-db.com/exploits/48246](https://www.exploit-db.com/exploits/48246)

#### ▸ Xampp

- **Service:** VeyonService

- **Vulnerability:** Local Privilege Escalation

- **Version:** 7.4.3

- **Exploit:** [https://www.exploit-db.com/exploits/50337](https://www.exploit-db.com/exploits/50337)

### Kernel Exploits

#### ▸ MS11-046

- **Version:** `Microsoft Windows [Version 6.0.6001 Service Pack 1 Build 6001]`

- **Vulnerability:** 'afd.sys' Local Privilege Escalatio

- **Exploit:** [https://www.exploit-db.com/exploits/40564](https://www.exploit-db.com/exploits/40564)

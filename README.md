# Enumeration-of-system-info
Enumeration of system info
# What's system info enumeration?
System info enumeration is a process of gathering information about a system, such as its operating system, network infrastructure, usernames, machine names, and other details. It can be used for ethical hacking, penetration testing, or system administration. System info enumeration can be performed using various tools and techniques, such as command-line utilities, network scanners, or web crawlers.

# My list of command for enumerating system info

## Usefull command shell Windows
	• hostname (hostname del sistema)
	• systeminfo (informazioni di sistema, versione OS, Os build number, hardware configuration, windows hotfix installed)
	• wmic qfe get Caption,Description,HotFixID,InstalledOn (hotfix installati con vari dettagli)
	• whoami
	• whoami /priv (enumera l'utente e i suoi privilegi)
	• net users (lista gli user accounts)
	• net user administrator (mostra le informazioni di configurazione di tale account)
	• net localgroup (enumera i gruppi che ci sono nel sistema)
	• net localgroup administrators (mostro quali sono gli utenti che sono nel gruppo administrators)
	• ip a s (mostra le network interfaces connesse al computer)
	• cat /etc/networks (lista le network configurate)
	• cat /etc/hosts (enumera i domini mappati localmente e i rispettivi ip)
	• cat /etc/resolv.conf (mostra il DNS nameserver ip)
	• net start (enumera la lista dei servizi in running)
	• wmic service list brief (uguale al comando di sopra, ma da anche informazioni dettagliate)
	• tasklist /SVC (mostra la lista dei task in running e il corrispettivo servizio)
	• schtasks /query /fo LIST (enumera la lista dei task schedulati)
	• Get-ChildItem -Path C:\Users -Recurse -filter *flag*.txt (cerca il flag nel punto che dici tu)
	• cd /
	• dir
  • type flag.txt

## Usefull command bash Linux
	• hostname (hostname del sistema)
	• cat /etc/issue (trova il nome distro di linux)
	• cat /etc/*release (trova la versione di linux)
	• uname -a (trova la versione del kernel di linux)
	• lscpu (trova le informazioni hardware del sistema)
	• df -h (trova la list degli storage con le varie informazioni tra cui dove sono montate)
	• whoami (ti dice in quale user account sei)
	• groups root (enumera i gruppi di cui fa parte root)
	• cat /etc/passwd (lista gli user and service accounts)
	• groups (enumera i gruppi che ci sono)
	• who (mostra gli utenti connessi ora)
	• lastlog (lista tutti gli utenti con l'ultimo accesso fatto)
	• ip a s (mostra le varie interfaccie connesse)
	• cat /etc/networks (enumera la lista delle network configurate e i loro subnet)
	• cat /etc/hosts (enumera la lista dei domini mappati localmente e i rispettivi ip)
	• cat /etc/resolv.conf (trova l'ip del default DNS server name)
  • cat /etc/cron* (enumera la lista dei cron job)

## Usefull command meterpreter Windows and Linux
	• sysinfo (informazioni di sistema)
	• shell (apre una shell)
	• getuid (NT-WINDOWS)
	• getprivs (enumera i privilegi che ha l'utente)
	• background (mette in background la sessione meterpreter = ctrl+z)
	• ifconfig (le interfaccie)
	• netstat (ottieni la lista delle porte aperte)
	• route (ottieni la routing table)
	• ps (mostra i processi che runnano su windows)
	• pgrep explorer.exe (cerca il suo pid)
	• migrate 2176 (migra nel pid)
	• lpwd (mostra la cartella locale di kali)
	• download flag5.zip (scarica il zip)
	• checksum md5 /bin/bash (tira fuori il checksum di un file)
	• getenv PATH (ti dà il path di dove sono le variabili d'ambiente)
	• search -d /usr/bin -f *flag* -r (-d cerca dalla directory che indichi, -f indichi cosa cerchi e metti -r se vuoi cercare nelle sue sottocartelle)
	• upload /usr/share/webshells/php/php-backdoor.php (carica una webshell nel target)

For more information about the enumeration, I direct you to my nmap github repository.<br> 
**https://github.com/SavioFengGit/Nmap-Active-Information-Gathering** <br>


#Author
<b>Xiao Li Savio Feng</b>




# Methodology

## Network Scanning

- [ ] nmap -sn 10.11.1.0/24
- [ ] nmap -sL 10.11.1.0/24
- [ ] nbtscan -r 10.11.1.0/24
- [ ] smbtree

## Individual Host Scanning

- [ ] nmap  --top-ports 20 --open ipaddress
- [ ] nmap -sS -A -sV -O -p- ipaddress -oA nmap
- [ ] nmap -sU ipaddress
- [ ] searchsploit -x --nmap nmap.xml
- [ ] dig axfr @ipaddress dc

## Service Scanning

### WebApp
- [ ]   Nikto
- [ ]   gobuster -u http://ipaddress -w /usr/share/wordlists/common.txt -s 200,204,301,302,307,403 -r -t 15 -o gobuster.txt
- [ ]   wpscan
- [ ]   dotdotpwn
- [ ]   view source 
- [ ]   davtest\cadevar
- [ ]   droopscan
- [ ]   joomscan
- [ ]   LFI\RFI Test
      
### Linux\Windows
- [ ]   snmpwalk -c public -v1 ipaddress 1
- [ ]   smbclient -L //ipaddress
- [ ]   showmount -e ipaddress port
- [ ]   rpcinfo
- [ ]   Enum4Linux

### Anything Else
- [ ]   nmap scripts (locate *nse* | grep servicename)
- [ ]   hydra
- [ ]   MSF Aux Modules
- [ ]   Download the software

### Exploitation
- [ ]   Gather Version Numbers
- [ ]   Searchsploit
- [ ]   Default Creds
- [ ]   Creds Previously Gathered
- [ ]   Download the software

## Post Exploitation

## Linux
- [ ]   linux-local-enum.sh
- [ ]   linuxprivchecker.py
- [ ]   linux-exploit-suggestor.sh
- [ ]   unix-privesc-check.py
- [ ]   find / -perm -4000 2>/dev/null | xargs ls -la

## Windows
- [ ]   wpc.exe
- [ ]   windows-exploit-suggestor.py
- [ ]   windows_privesc_check.py
- [ ]  	windows-privesc-check2.exe

## Priv Escalation
- [ ]  acesss internal services (portfwd)
- [ ]  add account

## Windows
- [ ]  List of exploits

## Linux
- [ ]  sudo su 
- [ ]  KernelDB
- [ ]  Searchsploit

## Final
- [ ]  Screenshot of IPConfig\WhoamI
- [ ]  Copy proof.txt
- [ ]  Dump hashes 
- [ ]  Dump SSH Keys
- [ ]  Delete files

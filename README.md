# nmap-cheat-sheet
A collection of useful Nmap commands

## Banner grabbing
```Bash
nmap -sS -sV -p 80 -v -n -Pn --script banner [host/IP]
```

## Vulnerability scanning
```Bash
nmap -sV --script=exploit,external,vuln,auth,default -oX nmap-metasploitable-test2.xml --webxml [host/IP]
```

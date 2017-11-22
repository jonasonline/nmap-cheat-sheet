# nmap-cheat-sheet
A collection of useful Nmap commands

## Updating scripts
nmap --script-updatedb

## Banner grabbing
```Bash
nmap -sS -sV -p [Port number] -v -n -Pn --script banner [host/IP]
```

## Vulnerability scanning
```Bash
nmap -sV --script=exploit,external,vuln,auth,default -oX nmap-output.xml --webxml [host/IP]
```

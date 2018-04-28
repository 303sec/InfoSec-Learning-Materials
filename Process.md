# Pentest Process

## Initial Enumeration

### Port scanning:
nmap -F $TARGET

{Check web services/anything obvious)

nmap -p- $TARGET -oA fullPortSweep

nmap -p<open ports> -A $TARGET -oA scriptsVersionsOS

nmap -p<open ports> --script=vuln $TARGET -oA vulnScripts

nmap -p- -sU Full UDP Scan -oA UDPSweep


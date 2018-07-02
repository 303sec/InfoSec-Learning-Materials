# OSCP Methodology

## Vaguely Important Things (Higher Abstraction PoV)
- Try Harder = Enumerate Harder
- Nmap -> Gobuster / Wfuzz -> Nikto -> Searchsploit
- [Useful OSCP Notes](https://github.com/dostoevskylabs/dostoevsky-pentest-notes)

## Note taking / Reporting

[OffSec's Reporting Template](https://www.offensive-security.com/pwk-online/PWKv1-REPORT.doc)

- Read up on what specific requirements there are for extra points
- Over the next week of study, refine note-taking & screenshotting to make life easier
- Use OneNote, seems to be recommended a bunch


## Things to do that will be *very* useful
- Compiling exploits for various operating systems so I don't need to later down the line... github might be best here for finding & checking these.
- Making the most of the labs whilst they are available. Try to get through as much as possible, because it's the only limited resource.
- Look at Penetration Testing book for good methodology



## Initial Enumeration

### Port scanning:
nmap -F $TARGET

{Check web services/anything obvious)

nmap -p- $TARGET -oA fullPortSweep

nmap -p<open ports> -A $TARGET -oA scriptsVersionsOS

nmap -p<open ports> --script=vuln $TARGET -oA vulnScripts

nmap -p- -sU Full UDP Scan -oA UDPSweep


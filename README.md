##### This is a basic script i have made for just harden my skill on python. Python is a great language for automating your Pentest Engaments. It's worth it for learning.



## Installation
```
git clone https://github.com/sl4x0/whois-and-portscan.git
cd whois-and-portscan
pip3 install -r requirments.txt
chmod u+x main.py
./main.sh --help
```

## Showing help
```bash
┌─[]─[slax@Parrot]─[~/whois-and-portscan]
└──╼ $./main.py --help
                                                                        
 Usage: main.py [OPTIONS] COMMAND [ARGS]...                             
                                                                        
╭─ Options ────────────────────────────────────────────────────────────╮
│ --install-completion          Install completion for the current     │
│                               shell.                                 │
│ --show-completion             Show completion for the current shell, │
│                               to copy it or customize the            │
│                               installation.                          │
│ --help                        Show this message and exit.            │
╰──────────────────────────────────────────────────────────────────────╯
╭─ Commands ───────────────────────────────────────────────────────────╮
│ domain    Print the domain registrant's name and organization.       │
│ portscan  Perform a portscan against a target on the top TOP ports,  │
│           and print the open ports and services.                     │
╰──────────────────────────────────────────────────────────────────────╯


```

## For WHOIS Scanning
```bash
┌─[slax@Parrot]─[~/whois-and-portscan]
└──╼ $./main.py domain --help
                                                                        
 Usage: main.py domain [OPTIONS] NAME                                   
                                                                        
 Print the domain registrant's name and organization.                   
                                                                        
╭─ Arguments ──────────────────────────────────────────────────────────╮
│ *    name      TEXT  [default: None] [required]                      │
╰──────────────────────────────────────────────────────────────────────╯
╭─ Options ────────────────────────────────────────────────────────────╮
│ --help          Show this message and exit.                          │
╰──────────────────────────────────────────────────────────────────────╯

```
## For PortScanning 
```bash
┌─[slax@Parrot]─[~/whois-and-portscan]
└──╼ $./main.py portscan --help
                                                                        
 Usage: main.py portscan [OPTIONS] TARGET                               
                                                                        
 Perform a portscan against a target on the top TOP ports, and print    
 the open ports and services.                                           
                                                                        
╭─ Arguments ──────────────────────────────────────────────────────────╮
│ *    target      TEXT  [default: None] [required]                    │
╰──────────────────────────────────────────────────────────────────────╯
╭─ Options ────────────────────────────────────────────────────────────╮
│ --top         INTEGER  [default: 10]                                 │
│ --help                 Show this message and exit.                   │
╰──────────────────────────────────────────────────────────────────────╯


```

## Basic Usage
```
┌─[slax@Parrot]─[~/whois-and-portscan]
└──╼ $./main.py domain testphp.vulnweb.com
testphp.vulnweb.com is registered by Acunetix Acunetix - Acunetix Ltd
```
```
┌─[slax@Parrot]─[~/whois-and-portscan]
└──╼ $./main.py portscan testphp.vulnweb.com
25 smtp
80 http
```
by [Sl4X0](https://www.twitter.com/sl4x0)

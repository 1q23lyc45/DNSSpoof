# DNSSpoof

A DNS spoofer tool written in Python3.

## How to use it?

    usage: dnsspoof.py [-h] [-d DOMAIN] [-i INTERFACE] [-t TARGET] [-r IP]
    
    optional arguments:
      -h, --help    show this help message and exit
      -d DOMAIN     Domain to spoof (default: all)
      -i INTERFACE  Interface to listen on (default: default)
      -t TARGET     Target's IP. If not specified (default: all)
      -r IP         IP to redirect the target to (default: local IP)

## Requirements

This script uses the following modules:

 - Argparse
 - Scapy
 - Threading

## How does it work?

The script will sniff the network traffic and intercept all the DNS queries matching a given domain name from the victim. Once this query is intercepted, it will forge and send a valid response with a malicious RR holding a given IP.

# Additional License and Disclaimer

This software is provided “as is” and the author makes no representations or warranties of any kind, express or implied, including, but not limited to, the implied warranties of merchantability, fitness for a particular purpose and non-infringement. In no event shall the author be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the software.

Use of this software is strictly limited to legitimate security testing purposes. Any use of this software for illegal activities is strictly prohibited and the author is not responsible for any consequences resulting from its use.

Before using this software, ensure that your behavior complies with local laws and regulations, and that you have obtained sufficient authorization. Do not scan unauthorized targets.

By using this software, you agree to the terms of this license agreement.

Please use this software responsibly and ethically. It is important to understand that using this software without proper authorization can have serious legal consequences. 

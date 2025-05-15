#### check if site IP is exposed or hidden behind CDN

#### check to which resources belongs server via Shodan, whois, dig etc.

#### check if ports are open via nmap

#### check if any directories are open via gobuster
- download list from ``https://github.com/danielmiessler/SecLists``
- ``gobuster -u https://example.com -w directory-list-lowercase-2.3-small.txt -t 1 -a "Mozilla/5.0 (SafeSecurityTest)" -k -m dir``

#### check for any custom open endpoints/controllers


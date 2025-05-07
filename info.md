#### For checking IP
- ``https://www.shodan.io/``

#### Get dns by domain name
- ``whois example.com``
- ``dig example.com``

#### For getting records for subdomains
- ``https://crt.sh/``
- ``curl -s "https://crt.sh/?q=%25.example.com&output=json" | jq '.[] | .name_value'`` (list of subdomain for scripts)

#### DNS history
- ``https://viewdns.info/iphistory/?domain=example.pt``

#### Whatweb
- ``whatweb -v farmacia.pt``

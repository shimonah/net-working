#for checking IP
https://www.shodan.io/

#get dns by domain name
whois example.com
dig example.com

#for getting records for subdomains
https://crt.sh/

#list of sub domains for script usage
curl -s "https://crt.sh/?q=%25.example.com&output=json" | jq '.[] | .name_value'

#DNS history
https://viewdns.info/iphistory/?domain=example.pt

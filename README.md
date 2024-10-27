# nahamsec_bbt_tutorial
crt sub-domain scan
```
curl -s https://crt.sh/\?q\=\%.$1\&output\=json | jq -r '.[].name_value' | sed 's/\*\.//g' | sort -u
```
Domain scan
```
./domainscan.sh media.yahoo.com | cut -d "."  -f 1,2,3 | sort -u
```

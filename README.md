# praia-arp
Cross-platform ARP table access for [Praia](https://praia.sh)

## Install
```praia
sand install github.com/viggou/praia-arp
```

## Usage
```praia
use "arp"

let entries = arp.table()            // all entries
let entry = arp.lookup("10.0.0.1")   // single IP
let entry = arp.refresh("10.0.0.1")  // ping to populate, then lookup
```
Each entry is a map: `{ip, mac, interface, hostname, state}`

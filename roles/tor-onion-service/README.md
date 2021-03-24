TOR Onion Node
==============

Connects the server into a TOR network, then the server gets an *.onion address. Everybody who knows the
onion address can reach exposed services of the server in TOR network.

Second function - optionally contribute to TOR network by setting up at least a bridge relay.

```yaml
role_tor_onion_service:
    # left side - port exposed on the *.onion domain
    # right side - local service address to be forwarded to left side
    service_ports:
        "22": "127.0.0.1:22"
        "80": "127.0.0.1:80"

    # be a bridge relay? please contribute to TOR network at least in this way :)
    bridge_relay: false
```

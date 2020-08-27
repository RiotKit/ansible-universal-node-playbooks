Port multiplexer
================

Sets up multiple protocols like VPN, SSH, HTTPS on single port.

- Additional layer of security by hiding services behind regular 443 port, no one would expect it
- Misleads the eavesdropping by mixing different services on one port (privacy)
- Proxies transparently, so the source IP address is preserved and fail2ban can be still used together to provide maximum security

**Before using this role make sure that nothing is listening on 443 port on 0.0.0.0 (does not collide with 127.0.0.1:443)**


Read more:
https://confluence.jaytaala.com/display/TKB/Transparent+SSLH%3A+using+a+single+port+to+transparently+route+incoming+traffic+for+Apache%2C+OpenVPN%2C+and+SSH



Alternative solutions
---------------------

- Port knocking

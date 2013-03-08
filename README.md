# config4hypedns

A script to configure Dnsmasq or BIND 9 to handle HypeDNS resolution.

### Overview

One of the current problems with HypeDNS is that users need to set the HypeDNS name server as their primary name server for it to work. This rsults in all the users DNS requests going through Hyperboria to the HypeDNS name server, which is generally going to be slower and less reliable, and is also a privacy concern for some.

The config4hypedns script is designed to correct this by allowing the use of Dnsmasq (or BIND 9 for those who need it) to selectively redirect ONLY HypeDNS host names to the HypeDNS name server, while still allowing normal DNS operation for all other requests. Additionally, these services can provide local caching, which can improve DNS performce significantly.

### Notes

This is a Python script, so users will need to ensure they have Python installed. It should work with either Python 2 or 3 at this time.

Feedback, good or bad, is encouraged. Seek Grundy on IRC, uppit, or socialnode. Email: grundy@hyperboria.name

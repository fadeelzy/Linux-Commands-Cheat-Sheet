# 🌐 Networking Commands Cheat Sheet

A list of essential Linux networking commands to test connectivity, resolve hosts, and download resources.

# 🔎 Host Resolution

nslookup <hostname>
Looks up the IP address of a hostname.

dig <hostname>
Performs detailed DNS lookups.

# 📡 Connectivity Testing

ping <hostname or IP>
Tests if a host is reachable and measures round-trip time.

traceroute <hostname>
Traces the path packets take to a destination, showing each hop.

# 🌍 Downloading Files

wget <URL>
Downloads files from the internet via HTTP, HTTPS, or FTP.

curl <URL>
Transfers data from or to a server. Can fetch, upload, or interact with APIs.

# 📄 Searching in Logs & Network Context

grep "pattern" <file>
Searches for specific text within a file. Often used in log analysis.

# 📊 Network Interface & IP Info

ifconfig (deprecated, use ip)
Displays network interface details.

ip addr
Shows IP addresses assigned to interfaces.

ip route
Displays routing table information.

✅ With these commands, you can test connectivity, resolve hostnames, trace routes, and download resources directly from your Linux system.
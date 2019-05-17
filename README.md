# scripts
A collection of useful scripts that I use. Bash and Batch

## netsh-tool.bat

Quickly change your network config to any of the following:

1. DHCP (automatic DNS)
2. DHCP (custom DNS)
3. Static (interactive)
4. Static (predefined)

**DHCP with auto DNS** resets the selected network interface to use DHCP for IP, Subnet, Gateway, and DNS servers.

**DHCP with custom DNS** makes the interface use DHCP for IP, Subnet, and Gateway, but static DNS servers.

**Static interactive mode** asks for input on IP, Subnet, Gateway, and DNS servers.

**Static predefined mode** uses hardcoded values that can be changed by editing the script.

## resolved-tool.sh

I use this for restarting the `systemd-resolved` service on my DigitalOcean Ubuntu 18.04 droplet. For some reason, it doesn't do this automatically, so I just run this after a reboot to solve DNS resolution issues. Run as `sudo`.
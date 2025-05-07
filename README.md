Discord Traffic Tunneling with WireGuard
This setup allows users to route only Discord traffic through a WireGuard tunnel, while keeping the rest of the traffic unaffected. It is ideal for users who want to use Discord securely over a VPN while maintaining normal internet usage for other applications.

Prerequisites
WireGuard installed and configured on your system.

Basic understanding of WireGuard configuration and networking.



AllowedIPs = 3.233.0.0/16, 20.54.0.0/16, 199.232.0.0/16, 172.64.0.0/16, 162.159.0.0/16, 142.250.0.0/16, 104.18.0.0/16, 10.13.0.0/16
This ensures that only the specified IP ranges for Discord traffic will be routed through the WireGuard tunnel.

Apply the Configuration:
After editing the configuration, apply the changes:

Use the wg-quick up <your-config> command to bring up the tunnel.

Connect to Your VPN:
Connect to your WireGuard VPN. At this point, only Discord traffic will be routed through the VPN while other traffic will be routed normally.

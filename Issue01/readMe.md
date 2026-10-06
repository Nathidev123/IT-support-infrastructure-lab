# Issue 1 — Connected, but No Internet

## User Complaint

> "My laptop says it is connected to Wi-Fi, but I cannot access the Internet."

## Initial Hypothesis

The issue may be related to the Wi-Fi connection, network configuration, or Internet connectivity.

## Investigation

The following checks were performed to identify where connectivity may be failing:

* `ipconfig /all` — reviewed network configuration, IP addressing, DHCP, DNS, and default gateway.
* `ping 127.0.0.1` — tested the local TCP/IP stack.
* `ping 192.168.0.1` — tested connectivity to the default gateway.
* `ping google.com` — tested DNS resolution and connectivity to an Internet destination.

## Evidence

# Issue 01 — Connected, but No Internet

## Evidence

### Network Configuration
![IP Configuration](https://github.com/Nathidev123/IT-support-infrastructure-lab/blob/main/ipconfig.png?raw=true)

### Local TCP/IP Stack
![Loopback Ping](https://github.com/Nathidev123/IT-support-infrastructure-lab/blob/main/loopback-ping.png?raw=true)

### Default Gateway Connectivity
![Gateway Ping](gateway-ping.png)

### Internet Connectivity & DNS
![Google Ping](google-ping.png)

## Findings

* The workstation has a valid IPv4 configuration.
* A default gateway is configured.
* The local TCP/IP stack responded successfully.
* The default gateway responded successfully with 0% packet loss.
* `google.com` successfully resolved to an IP address and responded with 0% packet loss.
* Basic local network connectivity, DNS resolution, and Internet connectivity are functioning.

## Diagnosis

The reported issue could not be reproduced during testing.

The workstation demonstrated working local network connectivity, DNS resolution, and Internet connectivity at the time of investigation.

## Recommended Resolution / Next Step

No network configuration changes are recommended at this stage.

If the user continues experiencing the issue, further investigation should determine whether the problem is intermittent, application-specific, or limited to particular websites or services.


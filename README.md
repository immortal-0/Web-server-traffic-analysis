# Web-server-traffic-analysis
Wireshark-based analysis of web server traffic containing reconnaissance, scanning, probing, and Log4j-related exploitation attempts.
This project focuses on analyzing network traffic captured from a web
server environment using Wireshark.

The traffic included normal web activity as well as reconnaissance,
scanning, probing, and suspected Log4j exploitation attempts.

The goal was to identify suspicious network behavior, analyze packet
details, and understand how malicious web traffic appears at the
network level.

## Tools

- Wireshark
- PCAP traffic capture
- TCP/IP protocol analysis
- HTTP traffic analysis

## Analysis Areas

The investigation focused on:

- Source and destination IP addresses
- TCP connections
- HTTP requests
- Destination ports
- Repeated connection attempts
- Scanning behavior
- Web application probing
- Suspicious request patterns
- Log4j-related exploit attempts

## Wireshark Filters Used

Examples:

tcp

http

ip.addr == <target-ip>

tcp.port == 80

http.request

tcp.flags.syn == 1 && tcp.flags.ack == 0

## Investigation Process

1. Identified the web server traffic.
2. Filtered HTTP and TCP sessions.
3. Reviewed repeated connection attempts and unusual requests.
4. Investigated traffic associated with scanning and probing.
5. Examined suspicious HTTP payloads for exploitation indicators.
6. Compared suspicious traffic with normal client activity.
7. Documented notable findings.

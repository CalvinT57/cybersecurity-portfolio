# Network Traffic Analysis and Threat Detection Using Wireshark

## Objective
The objective of this project was to capture and analyze live network traffic in order to identify common protocols, observe normal network behavior, and practice traffic filtering techniques used by SOC analysts.

## Tools Used
- Wireshark
- macOS network interface (Wi-Fi)

## Environment
- Operating System: macOS
- Capture Interface: Wi-Fi
- Traffic Type: Normal user browsing activity

## Methodology
1. Captured live network traffic using Wireshark on the active Wi-Fi interface.
2. Generated realistic traffic by visiting common websites.
3. Applied protocol-based filters to isolate DNS, HTTP, and TCP traffic.
4. Analyzed TCP handshake behavior and connection attempts.
5. Identified notable patterns within the captured traffic.

## Observed Traffic
- DNS queries were observed resolving domain names to IP addresses.
- HTTP traffic was minimal due to encrypted HTTPS usage.
- TCP traffic showed normal connection establishment using SYN, SYN-ACK, and ACK packets.
- Repeated outbound connections were observed to common domains associated with normal browsing behavior.

## Indicators and Patterns
| Type | Description |
|-----|------------|
| DNS | Domain resolution requests and responses |
| TCP | Connection establishment and handshake behavior |
| HTTP | Limited unencrypted traffic observed |
| SYN Packets | Initial connection attempts |

## Security Relevance
This analysis demonstrates how SOC analysts monitor network traffic to distinguish normal behavior from potentially suspicious activity. Understanding protocol behavior and connection patterns is critical for detecting anomalies, scanning activity, and potential intrusions.

## Limitations
- Traffic analyzed was limited to normal browsing activity.
- Encrypted HTTPS traffic limited visibility into application-layer content.

## Lessons Learned
- Network traffic analysisTCP-based protocols form the foundation of most network communication.
- Encryption reduces visibility but does not eliminate metadata analysis.
- Traffic filtering is essential for efficient investigation.


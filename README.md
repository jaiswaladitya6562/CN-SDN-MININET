# CN-SDN-MININET
# SDN Traffic Monitoring using Mininet and POX

## Problem Statement
Implement an SDN-based traffic monitoring system using Mininet and POX controller to observe network behavior and flow statistics.

## Setup
1. Run POX controller:
   ./pox.py monitor

2. Run Mininet:
   sudo mn --topo single,2 --controller remote

## Testing

### Test Case 1: Ping
pingall

### Test Case 2: Traffic Generation
iperf h1 h2

## Output
- Controller logs packet and byte count
- Flow rules visible using:
  sudo ovs-ofctl dump-flows s1

## Features
- PacketIn handling
- MAC learning
- Flow rule installation (match-action)
- Traffic monitoring

## Proof

<img width="674" height="167" alt="Screenshot from 2026-04-22 22-30-11" src="https://github.com/user-attachments/assets/bd52e7e9-d927-4d8f-904d-c9e4862a87ae" />

<img width="730" height="431" alt="Screenshot from 2026-04-22 22-29-28" src="https://github.com/user-attachments/assets/891be438-25d7-425b-bc28-ccd29124edf0" />

<img width="672" height="74" alt="Screenshot from 2026-04-22 22-30-55" src="https://github.com/user-attachments/assets/c239b3a4-32c2-432e-9d1b-17465a9d60de" />

<img width="728" height="119" alt="Screenshot from 2026-04-22 22-31-26" src="https://github.com/user-attachments/assets/eff39e0c-1fb8-4b05-b206-effaee024f3e" />

Scapy is a powerful interactive packet manipulation program. It is able to forge or decode packets of a wide number of protocols, send them on the wire, capture them, match requests and replies, and much more. It can easily handle most classical tasks like scanning, tracerouting, probing, unit tests, attacks or network discovery (it can replace hping, 85% of nmap, arpspoof, arp-sk, arping, tcpdump, tethereal, p0f, etc.). It also performs very well at a lot of other specific tasks that most other tools can’t handle, like sending invalid frames, injecting your own 802.11 frames, combining technics (VLAN hopping+ARP cache poisoning, VOIP decoding on WEP encrypted channel, …),

Scapy is a packet manipulation tool for computer networks,[1][2] written in Python by Philippe Biondi. It can forge or decode packets, send them on the wire, capture them, and match requests and replies. It can also handle tasks like scanning, tracerouting, probing, unit tests, attacks, and network discovery.

What is ARP poisoning
Machines on a TCP/IP local area network identify each other and communicate using the physical addresses of their network adapters (MAC address). Every machine keeps a list (cache) of neighboring machines and their MAC addresses, if that list is contaminated, i.e a machine on that list will have the wrong MAC address. All communication to that machine will be directed to the wrong machine.
ARP poisoning is the method of tricking a machine to save data on about an IP address with the wrong MAC address in it’s ARP table.

How the script works
The following script gets two arguments
HOST_TO_ATTACK – The machine we want to poison
HOST_TO_IMPERSONATE – The machine we want the poisoned machine to think we are, so when it want to communicate with that machine, it will actually communicate with us.

The script queries the target machine for it’s mac address by sending an who-has packet to broadcast.
The who-has packet has fake source IP address coupled with the attacker MAC address.
When the target gets the who-has packet the target will store the false IP and MAC address data in it’s ARP table.

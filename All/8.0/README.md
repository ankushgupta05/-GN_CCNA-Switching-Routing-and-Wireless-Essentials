Here are your **IPv6 GUA Assignment** quiz questions with options and **correct answers marked with ✔️**:

---

### Question 1

Which address type is automatically created by default on a host interface when no RAs are received?

* ⬜ Global unicast address
* ✔️ Link-local address
* ⬜ MAC address

---

### Question 2

Which method best describes stateless DHCP?

* ⬜ SLAAC only
* ✔️ SLAAC with stateless DHCPv6 Server
* ⬜ Stateful DHCPv6 Server

---

If you want me to continue with more questions or explain any concept, just ask!



Got it! Here’s **8.2.7 SLAAC Check Your Understanding** with **all options** and the **correct answers marked** by ✔️:

---

### Question 1

Which two ICMPv6 messages are used in the SLAAC process? (Choose two.)

* ⬜ Neighbor Advertisements (NA)
* ⬜ Neighbor Solicitation (NS)
* ✔️ Router Solicitation (RS)
* ✔️ Router Advertisements (RA)

---

### Question 2

Which command must be configured on a router to enable it to join the IPv6 all-routers multicast address ff02::2?

* ⬜ ip routing
* ✔️ ipv6 unicast-routing
* ⬜ ipv6 address ipv6-address/prefix-length
* ⬜ ipv6 address ipv6-address link-local

---

### Question 3

What are the flag settings when a host should use the SLAAC only option?

* ✔️ A=1, M=0, O=0
* ⬜ A=1, M=1, O=0
* ⬜ A=1, M=0, O=1
* ⬜ A=0, M=1, O=1

---

### Question 4

Which ICMPv6 message is sent by a host in an attempt to locate an online IPv6 enabled router to obtain IPv6 addressing information?

* ⬜ Neighbor Advertisements (NA)
* ⬜ Neighbor Solicitation (NS)
* ✔️ Router Solicitation (RS)
* ⬜ Router Advertisements (RA)

---

### Question 5

What method is used by a host to verify an IPv6 address is unique on the local network before assigning that address to an interface?

* ⬜ ARP
* ✔️ DAD
* ⬜ PING
* ⬜ SLAAC

---

If you want me to do the same for any other quiz or question set, just ask!



Here’s the **8.3.6 Check Your Understanding - DHCPv6** quiz with **all options and correct answers marked with ✔️**:

---

### Question 1

What destination UDP port do DHCPv6 clients use to send DHCPv6 messages?

* ⬜ 67
* ⬜ 68
* ✔️ 546
* ⬜ 547

---

### Question 2

What DHCPv6 message does a host send to look for a DHCPv6 server?

* ⬜ ADVERTISE
* ✔️ SOLICIT
* ⬜ INFORMATION-REQUEST
* ⬜ REQUEST

---

### Question 3

What DHCPv6 message does a host send to the DHCPv6 server if it is using stateful DHCPv6?

* ⬜ ADVERTISE
* ⬜ SOLICIT
* ⬜ INFORMATION-REQUEST
* ✔️ REQUEST

---

### Question 4

What flag settings combination is used for stateless DHCP?

* ✔️ A=1, M=0, O=1
* ⬜ A=1, M=0, O=0
* ⬜ A=0, M=1, O=0
* ⬜ A=0, M=1, O=1

---

### Question 5

What M flag setting indicates that stateful DHCPv6 is used?

* ⬜ M=0
* ✔️ M=1

---

If you want me to continue or format more quizzes, just say!





Here’s **8.4.9 Check Your Understanding - Configure DHCPv6 Server** quiz with **all options and correct answers marked with ✔️**:

---

### Question 1

Which three DHCPv6 roles can a router perform? (Choose all that apply.)

* ✔️ DHCPv6 client
* ✔️ DHCPv6 relay agent
* ✔️ DHCPv6 server
* ⬜ DHCPv6 pool

---

### Question 2

Which command is **not** configured in stateless DHCPv6?

* ⬜ address prefix ipv6-address/prefix
* ⬜ domain-name name
* ⬜ dns-server server-address
* ✔️ ipv6 dhcp server pool-name

---

### Question 3

An IPv6-enabled router is to acquire its IPv6 GUA from another IPv6 router using SLAAC. Which interface configuration command should be configured on the client router?

* ✔️ ipv6 address autoconfig
* ⬜ ipv6 address auto config
* ⬜ ipv6 address dhcp
* ⬜ ipv6 address dhcpv6

---

### Question 4

A router is to provide DHCPv6 server services. Which command should be configured on the client facing interface?

* ⬜ ipv6 enable
* ⬜ ipv6 dhcp pool POOL-NAME
* ✔️ ipv6 dhcp server POOL-NAME
* ⬜ ipv6 nd other-config-flag

---

### Question 5

An IPv6-enabled router is to acquire its IPv6 GUA from a DHCPv6 server. Which interface configuration command should be configured on client router?

* ⬜ ipv6 address autoconfig
* ⬜ ipv6 address auto config
* ✔️ ipv6 address dhcp
* ⬜ ipv6 address dhcpv6

---

### Question 6

Which DHCPv6 verification command would display the link-local and GUA assigned address for each active client?

* ⬜ show ip dhcp pool
* ✔️ show ipv6 dhcp binding
* ⬜ show ipv6 dhcp interface
* ⬜ show ipv6 dhcp pool

---

### Question 7

Which command is configured on the client LAN interface of the DHCPv6 relay agent?

* ⬜ ip helper-address
* ✔️ ipv6 dhcp relay destination
* ⬜ ipv6 enable
* ⬜ ipv6 helper-address

---

If you want me to keep going or want explanations, just ask!













Here is your **8.5.3 Module Quiz - SLAAC and DHCPv6** with **all options** and the **correct answers marked with ✔️**:

---

### Question 1

How does an IPv6 client ensure that it has a unique address after it configures its IPv6 address using the SLAAC allocation method?

* ⬜ It sends an ARP message with the IPv6 address as the destination IPv6 address.
* ⬜ It checks with the IPv6 address database that is hosted by the SLAAC server.
* ⬜ It contacts the DHCPv6 server via a special formed ICMPv6 message.
* ✔️ It sends an ICMPv6 Neighbor Solicitation message with the IPv6 address as the target IPv6 address.

---

### Question 2

Which method would an IPv6-enabled host using SLAAC employ to learn the address of the default gateway?

* ✔️ Router advertisements that are received from the link router
* ⬜ Advertise messages that are received from the DHCPv6 server
* ⬜ Neighbor advertisements that are received from link neighbors
* ⬜ Reply messages that are received from the DHCPv6 server

---

### Question 3

What two methods can be used to generate an interface ID by an IPv6 host that is using SLAAC? (Choose two.)

* ✔️ EUI-64
* ✔️ Random generation
* ⬜ Stateful DHCPv6
* ⬜ DAD
* ⬜ ARP

---

### Question 4

A client is using SLAAC to obtain an IPv6 address for its interface. After an address has been generated and applied to the interface, what must the client do before it can begin to use this IPv6 address?

* ⬜ It must send a DHCPv6 INFORMATION-REQUEST message to request the address of the DNS server.
* ⬜ It must send an ICMPv6 Router Solicitation message to determine what default gateway it should use.
* ⬜ It must send a DHCPv6 REQUEST message to the DHCPv6 server to request permission to use this address.
* ✔️ It must send an ICMPv6 Neighbor Solicitation message to ensure that the address is not already in use on the network.

---

### Question 5

Which command should be configured on a router interface to set the router as a stateful DHCPv6 client?

* ⬜ ipv6 enable
* ✔️ ipv6 address dhcp
* ⬜ ipv6 address autoconfigure
* ⬜ ipv6 dhcp server stateful

---

### Question 6

What message informs IPv6 enabled interfaces to use stateful DHCPv6 for obtaining an IPv6 address?

* ✔️ The ICMPv6 Router Advertisement
* ⬜ The ICMPv6 Router Solicitation
* ⬜ The DHCPv6 Reply message
* ⬜ The DHCPv6 Advertise message

---

### Question 7

Which destination IP address is used when an IPv6 host sends a DHCPv6 SOLICIT message to locate a DHCPv6 server?

* ⬜ FF02::2
* ⬜ FF02::1
* ⬜ FE80::1
* ✔️ FF02::1:2

---

### Question 8

In which alternative to DHCPv6 does a router dynamically provide IPv6 configuration information to hosts?

* ⬜ ARP
* ⬜ EUI-64
* ⬜ ICMPv6
* ✔️ SLAAC

---

### Question 9

A company implements the stateless DHCPv6 method for configuring IPv6 addresses on employee workstations. After a workstation receives messages from multiple DHCPv6 servers to indicate their availability for DHCPv6 service, which message does it send to a server for configuration information?

* ⬜ DHCPv6 SOLICIT
* ⬜ DHCPv6 REQUEST
* ⬜ DHCPv6 ADVERTISE
* ✔️ DHCPv6 INFORMATION-REQUEST

---

### Question 10

What process is used in ICMPv6 for a host to verify that an IPv6 address is unique before configuring it on an interface?

* ✔️ DAD
* ⬜ SLAAC
* ⬜ EUI-64
* ⬜ ARP

---

If you'd like explanations or want more questions, just say!






Here are the questions 11 to 13 with all options and the correct answers marked with ✔️:

---

### Question 11

What are two characteristics of the SLAAC method for IPv6 address configuration? (Choose two.)

* ✔️ The default gateway of an IPv6 client on a LAN will be the link-local address of the router interface attached to the LAN.
* ⬜ This stateful method of acquiring an IPv6 address requires at least one DHCPv6 server.
* ⬜ Clients send router advertisement messages to routers to request IPv6 addressing.
* ✔️ IPv6 addressing is dynamically assigned to clients through the use of ICMPv6.
* ⬜ Router solicitation messages are sent by the router to offer IPv6 addressing to clients.

---

### Question 12

After booting, a client receives an ICMPv6 RA message with the M flag set to 0 and the O flag set to 1. What does this indicate?

* ⬜ The client should request an IPv6 address directly from a DHCPv6 server.
* ⬜ The client should automatically configure an IPv6 address without contacting a DHCPv6 server.
* ✔️ The client should automatically configure an IPv6 address and then contact a DHCPv6 server for more information.
* ⬜ The client should be statically configured with an IPv6 address because the local router does not support autoconfiguration.

---

### Question 13

A network administrator is entering the command `ipv6 unicast-routing` to start configuring DHCPv6 operation on a router. Which statement describes the function of this command?

* ✔️ It is required for sending ICMPv6 RA messages.
* ⬜ It is required to configure stateful DHCPv6 server on the router.
* ⬜ It is required to configure stateless DHCPv6 server on the router.
* ⬜ It is required for enabling DNS service in DHCPv6 configurations.

---

Let me know if you want me to continue or explain any answers!

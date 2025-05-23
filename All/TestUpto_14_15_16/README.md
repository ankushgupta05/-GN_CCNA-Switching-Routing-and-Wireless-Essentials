# accuracy 85 hai

Here are the answers and explanations for your questions:

---

### Question 1

*Match the characteristic to the corresponding type of routing.*

| Characteristic                                                     | Routing Type        |
| ------------------------------------------------------------------ | ------------------- |
| typically used on stub networks                                    | *Static Routing*  |
| less routing overhead                                              | *Static Routing*  |
| new networks are added automatically to the routing table          | *Dynamic Routing* |
| best choice for large networks                                     | *Dynamic Routing* |
| not suitable for topologies where more than one router is required | *Static Routing*  |

---

### Question 2

*Which route would be used to forward a packet with a source IP 192.168.10.1 and destination IP 10.1.1.1?*

* The destination is *10.1.1.1*, so the route to 10.1.1.0/24 or 10.1.0.0/16 will be used.
* Among the options:

  * O 10.1.1.0/24 [110/65] via 192.168.200.2, 00:01:20, Serial0/1/0 — OSPF learned route, more specific
  * S 10.1.0.0/16 is directly connected, GigabitEthernet0/0 — static connected larger subnet
  * C 192.168.10.0/30 — not related to destination 10.1.1.1
  * S* 0.0.0.0/0 [1/0] via 172.16.1.1 — default route (used if no other match)

*Answer:*

* *O 10.1.1.0/24 \[110/65] via 192.168.200.2, 00:01:20, Serial0/1/0*

---

### Question 3

*What happens to a static route when the outgoing interface goes down?*

* For static routes configured with an exit interface (not next-hop IP), the static route is removed if interface is down.
* For static routes with next-hop IP, the route remains but will be invalid if next-hop is unreachable.

*Answer:*

* *The static route is removed from the routing table.*

---

### Question 4

*What does R1 use as the MAC address of the destination when constructing a frame to Server B?*

* R1 is directly connected to Server B through switch S1.
* When sending a frame to a host on the same subnet, the router uses the destination host's MAC address.
* If not in ARP cache, R1 sends an ARP request to resolve the MAC address.

*Answer:*

* *If the destination MAC address that corresponds to the IPv4 address is not in the ARP cache, R1 sends an ARP request.*

---

### Question 5

*Match routing table entry to function:*

| Category                | Function                                                      |
| ----------------------- | ------------------------------------------------------------- |
| Administrative distance | *D* Identifies the trustworthiness of a route source        |
| Route source            | *C* Identifies how a route was learned                      |
| Destination network     | *B* Identifies the address of the remote network            |
| Metric                  | *A* Identifies the value assigned to reach a remote network |

---

### Question 6

*When is it more beneficial to use dynamic routing instead of static?*

*Answer:*

* *on a network where there is a lot of topology changes*

---

If you want, I can help explain any of these in more detail!




Here are Questions *7 to 11* with *all options*, highlighting the correct answer along with an explanation:

---

### *Question 7*

*What will the router do with a packet destined for 192.168.12.227?*

A. Drop the packet because it is not a valid IPv4 address
B. Drop the packet because it has no match in the routing table
C. Forward the packet via FastEthernet0/0
*D. Send the packet out the Serial0/0/0 interface.* ✅

*Explanation:*
192.168.12.227 does not match any specific route, so the router uses the default route (0.0.0.0/0) via next-hop 209.165.200.226, which is reachable through interface Serial0/0/0.

---

### *Question 8*

*Which static route command would configure a route from R1 to the LAN on R2 that is connected to R2 G0/1 interface?*

A. ipv6 route 2001:db8:1:4::/64 fe80::2
B. ipv6 route 2001:db8:1:4::/64 S0/0/0
C. ipv6 route 2001:db8:1:4::/64 2001:db8:1:2::2
**D. ipv6 route 2001:db8:1:4::/64 2001:db8:1:3::1** ✅

*Explanation:*
R2’s G0/1 connects to 2001\:db8:1:4::/64. From R1, the path to that LAN goes through 2001\:db8:1:3::1, which is R2’s G0/0 interface. This is the correct next-hop IPv6 address.

---

### *Question 9*

*Which command would create a fully specified static route on R1 to reach the PC B network?*

A. ipv6 route 2001:db8:1:4::/64 fe80::2
B. ipv6 route 2001:db8:1:4::/64 S0/0/0
C. ipv6 route 2001:db8:1:4::/64 2001:db8:1:2::2
D. ipv6 route 2001:db8:1:4::/64 G0/1
**E. ipv6 route ::/0 G0/1 fe80::2** ✅

*Explanation:*
A *fully specified static route* in IPv6 uses both an *exit interface* and a *next-hop link-local address*. Option E is correct because it defines both, creating a reliable path to the destination.

---

### *Question 10*

*What is the best configuration for a static route on R1 to reach PC2 and avoid a recursive route lookup?*

A. ip route 192.168.2.0 255.255.255.0 10.1.1.2 90
B. ip route 192.168.2.0 255.255.255.0 10.1.1.1 90
C. ip route 192.168.2.0 255.255.255.0 S0/0/0
D. ip route 192.168.2.0 255.255.255.0 Fa0/0 10.1.1.1
**E. ip route 192.168.2.0 255.255.255.0 Fa0/0 10.1.1.2 95** ✅

*Explanation:*
To avoid a recursive lookup, specify both *interface* and *next-hop. A **floating static route* uses an administrative distance (AD > 1). Option E does all this with AD 95.

---

### *Question 11*

*What does the number 5 represent in the following command?*

ip route 172.16.100.128 255.255.255.128 209.165.200.226 5

*A. administrative distance* ✅
B. metric
C. hop count
D. number of equal cost paths
E. maximum bandwidth

*Explanation:*
The *last number in a static route* defines the *administrative distance (AD). Lower ADs are more preferred. AD of 5 makes it a **floating static route* used only if another route fails.

---

Would you like me to continue with *questions 12–15* in the same format?








Here’s a detailed table for *Questions 12 to 20, listing **all options* with the *correct answers marked and explained*:

---

### ✅ = Correct Answer

### ❌ = Incorrect Answer

| Q#     | Option                                                                                                 | Answer | Explanation                                                                                      |
| ------ | ------------------------------------------------------------------------------------------------------ | ------ | ------------------------------------------------------------------------------------------------ |
| *12* | A(config)# no ip route 10.0.0.0 255.0.0.0 172.16.40.2                                                  | ✅      | This removes the old static route with the old next-hop.                                         |
|        | A(config)# no network 10.0.0.0 255.0.0.0 172.16.40.2                                                   | ❌      | Incorrect syntax; network is for routing protocols like RIP, not static routes.                |
|        | A(config)# no ip address 10.0.0.1 255.0.0.0 172.16.40.2                                                | ❌      | ip address is used to configure interface IPs, not routes.                                     |
|        | A(config)# ip route 10.0.0.0 255.0.0.0 192.168.1.2                                                     | ✅      | This adds the new static route with the correct next-hop.                                        |
|        | A(config)# ip route 10.0.0.0 255.0.0.0 s0/0/0                                                          | ❌      | This uses an exit interface, not the updated next-hop IP.                                        |
| *13* | Ping from the 192.168.10.0 network to the 10.10.10.2 address.                                          | ❌      | This does not validate the route; tests from source subnets don’t confirm next-hop reachability. |
|        | Ping any valid address on the 192.168.10.0/24 network.                                                 | ✅      | Valid way to verify that packets are routed correctly to that network.                           |
|        | Delete the default gateway route on the router.                                                        | ❌      | Irrelevant to testing a specific static route.                                                   |
|        | Manually shut down the router interface used as a primary route.                                       | ❌      | Unnecessary for testing; disruptive and not a test method.                                       |
| *14* | any router running an IOS prior to 12.0                                                                | ❌      | Irrelevant to static routing.                                                                    |
|        | edge router connection to the ISP                                                                      | ✅      | Default static routes are typically used at the network edge to reach external networks.         |
|        | any router where a backup route to dynamic routing is needed for reliability                           | ❌      | Describes floating static route, not default route necessarily.                                  |
|        | the router that serves as the gateway of last resort                                                   | ✅      | Default static route defines the gateway of last resort.                                         |
|        | stub router connection to the rest of the corporate or campus network                                  | ✅      | Stub routers use default static routes to reach all external networks.                           |
| *15* | send the packet out interface Serial0/0/0                                                              | ❌      | This connects back to R1 and doesn’t reach 192.168.10.128.                                       |
|        | send the packet out interface Serial0/0/1                                                              | ✅      | Matches static route for 192.168.10.128/26 via 10.0.0.6.                                         |
|        | send the packet out interface FastEthernet0/0                                                          | ❌      | That interface is for 192.168.10.64/26, not 128/26.                                              |
|        | drop the packet                                                                                        | ❌      | A valid route exists; it won’t be dropped.                                                       |
| *16* | ::/0                                                                                                   | ✅      | This is the correct default route in IPv6.                                                       |
|        | ::/128                                                                                                 | ❌      | This matches only the specific host address ::.                                                  |
|        | ::1/64                                                                                                 | ❌      | ::1 is the loopback address, and /64 is an invalid prefix here.                                  |
|        | FFFF::/128                                                                                             | ❌      | Not a valid default or common routing prefix.                                                    |
| *17* | fully specified static route                                                                           | ❌      | No exit interface is mentioned.                                                                  |
|        | recursive static route                                                                                 | ✅      | Next-hop address must be resolved recursively in the routing table.                              |
|        | directly attached static route                                                                         | ❌      | Not used here; no interface specified.                                                           |
|        | floating static route                                                                                  | ❌      | No administrative distance higher than default (1) is specified.                                 |
| *18* | It is simply a static route with 0.0.0.0/0 as the destination IPv4 address.                            | ❌      | That’s a default static route, not floating.                                                     |
|        | It is configured with a higher administrative distance than the original dynamic routing protocol has. | ✅      | Floating routes "float" because they are less preferred unless the primary route fails.          |
|        | When it is configured, it creates a gateway of last resort.                                            | ❌      | This describes a default route, not a floating one.                                              |
|        | It is used to provide load balancing between static routes.                                            | ❌      | Load balancing is not the purpose of floating routes.                                            |
| *19* | The netmask is incorrect.                                                                              | ❌      | 0.0.0.0 0.0.0.0 is the correct default netmask.                                                  |
|        | The next hop address is incorrect.                                                                     | ✅      | The next hop should be a host IP address, not a network address (172.16.2.0 is a network).       |
|        | The destination network is incorrect.                                                                  | ❌      | It’s a default route; the destination is correctly 0.0.0.0.                                      |
|        | The exit interface is missing.                                                                         | ❌      | You can use next-hop IP instead of exit interface.                                               |
| *20* | The route was dynamically learned from another router.                                                 | ❌      | Static (S) routes are manually configured.                                                       |
|        | The route was automatically installed when an IP address was configured on an active interface.        | ❌      | That only installs *connected* or *local* routes, not static ones.                           |
|        | The route was dynamically created by router R1.                                                        | ❌      | R1 doesn’t create static routes automatically.                                                   |
|        | The route was manually entered by an administrator.                                                    | ✅      | A static (S) route must be manually configured.                                                  |

---

Let me know if you'd like this in Markdown or PDF format!


Here are the correct answers and explanations for *Questions 21 to 27*, including all options:

---

### *Question 21*

*What error has been made in the static route configuration?*

*Correct Answer:* ✅ *The interface is incorrect.*

| Option                                  | Description                                                                                                                  |
| --------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| ❌ The next hop address is incorrect.    | The next-hop 2001:db8:a:1::2 is correct for reaching R2.                                                                   |
| ❌ The network prefix is incorrect.      | The destination network 2001:db8:1:2000::/64 is correct for R2’s LAN.                                                      |
| ✅ The interface is incorrect.           | The configured interface s0/0/1 might be incorrect or not up. Using the *next-hop address alone* is preferred with IPv6. |
| ❌ The destination network is incorrect. | The destination prefix is correct.                                                                                           |

---

### *Question 22*

*What is the cause of this problem?*

*Correct Answer:* ✅ *The static route for 192.168.2.0 is incorrectly configured.*

| Option                                                        | Description                                                                                     |
| ------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| ✅ The static route for 192.168.2.0 is incorrectly configured. | The static route points to 192.168.3.0 which is a *network, not a **next-hop IP address*. |
| ❌ The serial interface between the two routers is down.       | The serial link is working (ping to 10.1.1.2 is successful).                                  |
| ❌ A default route is not configured on R1.                    | A default route isn't required here; a correct static route is.                                 |
| ❌ There is no gateway of last resort at R1.                   | Not needed unless default routing is required.                                                  |

---

### *Question 23*

*What is the issue?*

*Correct Answer:* ✅ *R1 needs a static route to the R2 LAN.*

| Option                                           | Description                                                                  |
| ------------------------------------------------ | ---------------------------------------------------------------------------- |
| ✅ R1 needs a static route to the R2 LAN.         | R1 has no route to 10.0.60.0/24. This route must be added manually.        |
| ❌ R2 needs a static route to the R1 LANs.        | R2 doesn’t need it to reach the internet; R1 has a default route to the ISP. |
| ❌ R1 needs a default route to R2.                | R1 already has a default route to the ISP.                                   |
| ❌ R1 and R2 must use a dynamic routing protocol. | Static routing is acceptable and intended.                                   |
| ❌ R2 needs a static route to the Internet.       | R2 already uses R1 as a default gateway to the Internet.                     |

---

### *Question 24*

*Which change should be made to the static route command so that traffic will only use the OSPF link when it is up?*

*Correct Answer:* ✅ *Change the administrative distance to 120.*

| Option                                             | Description                                                                                             |
| -------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| ❌ Change the destination network to 198.51.0.5.    | That’s the next-hop, not the destination network.                                                       |
| ❌ Change the administrative distance to 1.         | That would make it *preferable* over OSPF (not desired).                                              |
| ✅ Change the administrative distance to 120.       | OSPF has an AD of 110. Setting static to 120 makes it a *floating route* (used only when OSPF fails). |
| ❌ Add the next hop neighbor address of 198.51.0.8. | Not relevant; AD value is the key fix.                                                                  |

---

### *Question 25*

*Which two statements correctly describe the addressing that HostA will generate in the process?*

*Correct Answers:* ✅ *A packet with the destination IP address of ServerB.*
✅ *A frame with the destination MAC address of RouterA.*

| Option                                                 | Description                                         |
| ------------------------------------------------------ | --------------------------------------------------- |
| ✅ A packet with the destination IP address of ServerB. | IP destination is ServerB.                          |
| ❌ A frame with the destination MAC address of SwitchA. | Switches don’t have MACs for end-device addressing. |
| ❌ A packet with the destination IP address of RouterB. | The IP packet still targets ServerB.                |
| ✅ A frame with the destination MAC address of RouterA. | First-hop router MAC is used in the frame.          |
| ❌ A frame with the destination MAC address of ServerB. | Not in the same local network.                      |
| ❌ A packet with the destination IP address of RouterA. | IP destination is not changed.                      |

---

### *Question 26*

*What characteristic completes the statement?*

*Correct Answer:* ✅ *the "show ipv6 route static" command.*

| Option                                                    | Description                                           |
| --------------------------------------------------------- | ----------------------------------------------------- |
| ✅ the "show ipv6 route static" command.                   | Correct way to verify static IPv6 route.              |
| ❌ the "ipv6 unicast-routing" command.                     | Enables routing; does not verify routes.              |
| ❌ the interface type and interface number.                | Needed during configuration but not for verification. |
| ❌ the next-hop address of two different adjacent routers. | Not required for static route verification.           |

---

### *Question 27*

This question seems to be incomplete — please provide the full question prompt for accurate analysis and response.

---

Let me know when you're ready to continue with more questions or need the final table format for the README!



Here are the correct answers with *all options* for Questions 27 to 33, including explanations:

---

### *Question 27*

*Refer to the exhibit. Which interface will be the exit interface to forward a data packet that has the destination IP address 192.168.71.52?*

| Option                                             | Answer | Explanation                                                                                       |
| -------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------- |
| ❌ None, the packet will be dropped.                |        | There *is* a static route to the 192.168.71.0/26 network, so the packet will not be dropped.    |
| ❌ GigabitEthernet0/1                               |        | This interface connects to 192.168.139.224/27; it’s unrelated to 192.168.71.52.                   |
| ✅ *Serial0/0/0*                                  | ✔      | There is a static route: S 192.168.71.0/26 via 192.168.70.1 which is reachable via Serial0/0/0. |
| ❌ The packet will take the gateway of last resort. |        | Gateway of last resort is *not set*, so this is incorrect.                                      |

---

### *Question 28*

*What two pieces of information are needed in a fully specified static route to eliminate recursive lookups? (Choose two.)*

| Option                                                    | Answer | Explanation                                                       |
| --------------------------------------------------------- | ------ | ----------------------------------------------------------------- |
| ❌ the administrative distance for the destination network |        | Admin distance is not needed for eliminating recursive lookups.   |
| ✅ *the interface ID exit interface*                     | ✔      | Specifying the exit interface helps eliminate recursion.          |
| ✅ *the IP address of the next-hop neighbor*             | ✔      | Providing the next-hop IP also avoids recursive lookups.          |
| ❌ the interface ID of the next-hop neighbor               |        | There's no such concept. Only the *exit* interface is relevant. |
| ❌ the IP address of the exit interface                    |        | This is not a valid requirement in static route syntax.           |

---

### *Question 29*

*What routing solution will allow both PC A and PC B to access the Internet with minimum router CPU and bandwidth use?*

| Option                                                                                                                                 | Answer | Explanation                                                                       |
| -------------------------------------------------------------------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------- |
| ❌ Configure a static route from R1 to Edge and a dynamic route from Edge to R1.                                                        |        | This increases Edge's resource usage.                                             |
| ❌ Configure a dynamic routing protocol between R1 and Edge and advertise all routes.                                                   |        | Dynamic protocols increase CPU and bandwidth.                                     |
| ✅ *Configure a static default route from R1 to Edge, a default route from Edge to the Internet, and a static route from Edge to R1.* | ✔      | This uses static routing which is CPU-efficient and meets all connectivity needs. |
| ❌ Configure a dynamic route from R1 to Edge and a static route from Edge to R1.                                                        |        | Still involves dynamic routing, which uses more resources.                        |

---

### *Question 30*

*What is the cause of the problem with PC0 not reaching [www.server.com](http://www.server.com)?* (PT Activity required for full verification)

| Option                                                                 | Answer | Explanation                                                                                  |
| ---------------------------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- |
| ❌ A serial interface on Branch is configured incorrectly.              |        | Not enough info to confirm this as the issue.                                                |
| ✅ *The DNS server address on PC0 is configured incorrectly.*         | ✔      | This is a common misconfiguration leading to web access issues despite network connectivity. |
| ❌ Routing between HQ and Branch is configured incorrectly.             |        | If that were the case, *all communication* would fail.                                     |
| ❌ The clock rate on one of the serial links is configured incorrectly. |        | That would disrupt the entire link, not just DNS resolution.                                 |

---

### *Question 31*

**What would happen after the IT administrator enters ip route 172.16.1.0 255.255.255.0 s0/0/0?**

| Option                                                                                                     | Answer | Explanation                                                                |
| ---------------------------------------------------------------------------------------------------------- | ------ | -------------------------------------------------------------------------- |
| ❌ The 172.16.1.0 static route would be entered into the running-config but not shown in the routing table. |        | It would be shown and override the RIP route.                              |
| ❌ The 172.16.1.0 static route is added to the existing routes in the routing table.                        |        | Static routes override dynamic routes with the same prefix.                |
| ❌ The 0.0.0.0 default route would be replaced with the 172.16.1.0 static route.                            |        | These are *separate* routes.                                             |
| ✅ *The 172.16.1.0 route learned from RIP would be replaced with the 172.16.1.0 static route.*            | ✔      | Static routes have lower admin distance than RIP, so they take precedence. |

---

### *Question 32*

*Which static route would be used to create a backup route to 172.16.1.0 that activates only if RIP fails?*

| Option                                             | Answer | Explanation                                                          |
| -------------------------------------------------- | ------ | -------------------------------------------------------------------- |
| ❌ ip route 172.16.1.0 255.255.255.0 s0/0/0 91      |        | Admin distance 91 < RIP (120), so it would override RIP immediately. |
| ✅ *ip route 172.16.1.0 255.255.255.0 s0/0/0 121* | ✔      | This makes it a *backup* because its AD > RIP's 120.               |
| ❌ ip route 172.16.1.0 255.255.255.0 s0/0/0         |        | Default AD is 1, so it overrides RIP.                                |
| ❌ ip route 172.16.1.0 255.255.255.0 s0/0/0 111     |        | Still lower than RIP's AD; it will replace it.                       |

---

### *Question 33*

*Which command configures an IPv6 static route on R2 to reach PC1 without recursive lookup?*

| Option                                                        | Answer | Explanation                                                     |
| ------------------------------------------------------------- | ------ | --------------------------------------------------------------- |
| ❌ R2(config)# ipv6 route 2001\:db8:10:12::/64 S0/0/1          |        | S0/0/1 is on *R1*, not R2.                                    |
| ✅ *R2(config)# ipv6 route 2001\:db8:10:12::/64 S0/0/0*      | ✔      | This uses *R2’s own interface*, eliminating recursive lookup. |
| ❌ R2(config)# ipv6 route ::/0 2001\:db8:32::1                 |        | This sets a *default route*, not specific to PC1’s subnet.    |
| ❌ R2(config)# ipv6 route 2001\:db8:10:12::/64 2001\:db8:32::1 |        | This causes a recursive lookup to resolve the next-hop.         |

---

Let me know if you want the answers summarized in a table format for your notes or README!

* Connectionless (no call set up at the network layer) and unreliable designed to be used in a packet switched network like the Internet.
* There is no state about end-to-end connections
* **Best effort Services** meaning no guarantee about bandwith, timing, loss, error, order. 
* No congestion indicators present, the internet depends on TCP for that. 
## IPv4 Datagram Format
![[Pasted image 20260331152313.png]]
## Classful IP Addressing 
![[Pasted image 20260331163957.png]]
![[Pasted image 20260331164016.png]]

## Special IP Addresses (Classful)
* Network Addresses: (specific netid) (all 0s hostid) => 75.0.0.0 
* Direct Broadcast Access: (specific) (all 1s) => 75.255.255.255 (source sends to all hosts in this network)
* Limited Broadcast Access: (all 1s) (all 1s) => 255.255.255.255 (source to all hosts in the SAME network)
* This host on this network: (all 0s) (all 0s) => 0.0.0.0
* Specific host on this network: (all 0s) (specific) => 0.3.1.28 (same network, specific host)
* Loopback Address (127) (any) => packets dont leave node

## Private Addressing in Classful IP addresses 

| Range                         | Total    | Type              |
| ----------------------------- | -------- | ----------------- |
| 10.0.0.0 - 10.255.255.255     | $2^{24}$ | Commercial        |
| 172.16.0.0 - 172.31.255.255   | $2^{20}$ | Mostly Commercial |
| 192.168.0.0 - 192.168.255.255 | $2^{16}$ | Residential Usage |
> Private IP addresses are non-routable

## CIDR (Classless InterDomain Routing)
* subnet portion of address of arbitrary length
* address format: a.b.c.d/x, where x is the bits in subnet portion of address
>[!example] Example
>![[Pasted image 20260331192416.png]]

>[!important] Total Usable Hosts
> Assuming a /24 for CIDR (24 bits for network, 8 for hosts). There will ALWAYS be 2 special unusable addresses (all bit 0 -> for network, all bit 1 -> for all hosts)
> i.e. `192.168.1.0` & `192.168.1.255`
> Therefore total usable hosts would be $2^{8} = 256 \Rightarrow 256-2=254$ usable host addresses

## Subnetting Example 
assume someone sends data to 200.10.2.45   (a device in IT department)

* External Router knows `200.10.0.0/16` -> company gateway. So it sends it there.
* Company Gateway (edge router) now knows `200.10.2.0/24` so it forwards it to IT subnet.
* Now internal router in that subnet will send it to destination.
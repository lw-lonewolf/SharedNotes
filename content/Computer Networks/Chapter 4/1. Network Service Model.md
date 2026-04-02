What service model shall be followed for data travel? 

For **individual datagrams** example services may be: 
* guaranteed delivery
* guaranteed delivery with less than 40ms delay 

For **a flow of datagrams**:
* in-order datagram delivery
* guaranteed minimum bandwidth to flow
* restrictions on changes in inter-packet spacing (jitter)

The most common network architecture in use is the Internet (no shit sherlock.)

### Quality of Service Guarantees Provided

| **Network Architecture**                      | Service Model                 | Bandwith           | Loss     | Order    | Timing |
| --------------------------------------------- | ----------------------------- | ------------------ | -------- | -------- | ------ |
| Internet                                      | best effort                   | none               | no       | no       | no     |
| ATM                                           | Constant Bit Rate             | Constant Rate      | yes      | yes      | yes    |
| ATM                                           | Available Bit Rate            | Guaranteed Minimum | no       | yes      | no     |
| Internet (*Proposed Service Model Extension*) | Intserv Guaranteed (RFC 1633) | yes                | yes      | yes      | yes    |
| Internet (Proposed Service Model Extension)   | DiffServ (RFC 2475)           | possible           | possibly | possibly | no     |
### Best Effort Services
* simplicity has allowed for wide deployment and adoption of the Internet.
* sufficient provisioning of bandwidth allows performance of real-time applications (e.g. interactive voice, video) to be "good enough" for "most of the time")
* replicated, application-layer distributed services allow services to be provided from various locations 
* congestion control of "elastic" services helps 
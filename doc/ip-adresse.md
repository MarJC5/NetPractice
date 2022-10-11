# IP adresse

## IPv4

An Internet Protocol address (IP address) is a numerical label such as 192.0.2.1 that is connected to a computer network that uses the Internet Protocol for communication.

An IP address serves two main functions: network interface identification and location addressing.

An IPv4-adress is a 32-bit number divided into 4 "blocks", each 8 bits.

i.e.: `192.168.100.1` turns into `11000000.10101000.01100100.00000001`

So the min. value of one "block" is 0 and the max. value is 255.

The same logic applies to the network-mask:
`255.255.255.0` turns into `11111111.11111111.11111111.00000000`
Special to the mask is, after one bit was 0 there can't be any 1 bit's anymore.
so the only available numbers are:

- `255 (binary: 11111111)`
- `254 (binary: 11111110)`
- `252 (binary: 11111100)`
- `248 (binary: 11111000)`
- `240 (binary: 11110000)`
- `224 (binary: 11100000)`
- `192 (binary: 11000000)`
- `128 (binary: 10000000)`
- `0 (binary: 00000000)`

Through which `255.255.255.0` is a valid mask
and `255.255.128.128` is not a valid mask.

In order to have the ability to send packages between two IP-addresses they either need to be part of the same network or they need to be connected by a router which is part of both subnets.

## Special IP Address Ranges

`10.0.0.0/8` (10.0.0.0 – 10.255.255.255)

- Scope: Private network
- Description: Used for local communications within a private network.
- Number of addresse: 16'777'216

`127.0.0.0/8` (127.0.0.0 – 127.255.255.255)

- Scope: Host
- Description: Used for loopback addresses to the local host.
- Number of addresse: 16'777'216

`172.16.0.0/12` (172.16.0.0 – 172.31.255.255)

- Scope: Private network
- Description: Used for loopback addresses to the local host.
- Number of addresse: 1'048'576

`192.168.0.0/16` (192.168.0.0 – 192.168.255.255)

- Scope: Private network
- Description: Used for local communications within a private network.
- Number of addresse: 65'536
  
[<- back to summary](/README.md)

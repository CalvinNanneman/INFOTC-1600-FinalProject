# How to determine the number of hosts on a subnet

When working with computer networks it is often necessary to know the size of a network and how many usable IP addresses are available in a given network. The goal of this tutorial is to explain how to calculate the number of availalbe IP addresses there are on a given subnet.

## Broadcast Addresses and Network Addresses

Every IPv4 network, no matter the size, has both a network address and a broadcast address. The network address is used as an 'ID' for the network and is the first IP address in the given range of IP addresses. 

For more info on network addresses click [here](https://en.wikipedia.org/wiki/Network_address)

Every IPv4 network also has a broadcast address. This address is used to transmit to every single address in the network. The broadcast address is the last IP address of the network's given range of IP addresses. 

For more info on broadcast addresses click [here](https://en.wikipedia.org/wiki/Broadcast_address)

The range of addresses between the network address and the broadcast are 'usable' addresses and can be assigned to devices. 

## What determines a networks size?

Each IPv4 network has something called a subnet mask. The subnet mask is much like an IP address and consists of four octets of bits. The subnet mask is what ultimatly determines a network's number and range of usable IP addresses. Continue to the tutorial to see how the subnet mask is used to calculate the nubmer of usable addresses.

[Tutorial - How to calculate usable IP addresses](calculate.md)

[About](README.md)

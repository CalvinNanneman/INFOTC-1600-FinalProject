# How to calculate number of usable IP addresses based on Subnet mask


## Example Network address 192.168.5.0 
## Example Subnet mask 255.255.255.0


### How to determine the number and range of usable IP addresses of the example network address and subnet mask

First, we need to convert both the IP address and subnet mask into binary

If you unfamilar with how to do this click [here](https://www.computernetworkingnotes.com/ccna-study-guide/convert-decimal-ip-address-in-binary-and-binary-in-decimal.html)

<span style="color: cyan"> 192.168.5.0 = <span style="color: red"> 11000000.10101000.00000101.00000000

<span style="color: cyan"> 255.255.255.0 = <span style="color: red"> 11111111.11111111.11111111.00000000

Notice, on the subnet mask there are 8 unused bits (the zeros at the end)

To calculate the total number of IP addresses on this subent we simply have to put 2 to the power of n, where n is equal to the number of unused bits at the end of the subnet mask. In this case that nubmer is 8, so we will calculate 2<sup>8</sup>

2<sup>8</sup> = 256

This means that there are 256 total IP addresses on this example network. Remember, each network has both a network address and broadcast address that cannot be used. To find the number of usable addresses we simply need to subract two from 256. 
 256 - 2 = 254 usable addresses. 

 This process can be stated in a formula 
  
 ## h = 2<sup>n</sup> - 2
 
 Where h is the number of usable addresses and n is the number of zeros in the subnet mask. 

 In this example, the network address is given and we can easily determine the range of IPs for this network. 

To find the broadcast address we have to add 8 1's to the end of the network address
<span style="color: red"> 11000000.10101000.00000101.00000000 --> 11000000.10101000.00000101.11111111

Then convert back to decimal

<span style="color: red"> 11000000.10101000.00000101.11111111 = 192.168.5.255

Thus the Broadcast address is 192.168.5.255

The range of usable IP addresses is everything between the Network address and Broacast address

<span style="color: green"> Range = 192.168.5.1 to 192.168.5.254

[Home](home.md)
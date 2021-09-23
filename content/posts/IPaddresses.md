{
  "title": "IP Addresses",
  "date": "2021-08-31T10:19:51-05:00",
  "draft": false,
  "author": "Said Neder",
  "tags": ["Networking"]
}

This is in the third layer of the OSI model that is Network, related to routing.

Inet = IPv4, decimal notation
Inet6 = IPv6, hexadecimal notation

## IPv4
`192.168.57.139`
Each group before the dot is an octect, made by 8 bits, representing 1 and 0, and made all up together conforms 32 bits and that is equivalent to 4 bytes.

With that said, there isn't enough ipv4 for the world itself so now we use ipv6.

## IPv6
`2800:bf0:8040:11c4:dd55:372d:7329:176a`
The IPv6 is made up of 128 bits that is 16 bytes. is made of the hexadecimal numbers (1,2,3,4,5,6,7,8,9,a,b,c,d,e,f)

the quantity of ipv6 that are out there are endless, but still no one uses ipv6, thanks to NAT that is Network Address translation, we are assiging private ip addresses.

And private ip addresses are ip addresses that are only known to you, in your lan, not on the interweb (WAN)

 So natting works because all of this privates ip addresses comes out as just one public ip address that is the one that your ISP is renting you.

### Classes of private ip addresses

![Private ip addresses chart](https://slideplayer.com/slide/3366765/12/images/9/PRIVATE+IP+ADDRESS+%28are+not+used+anywhere+on+public+internet%2C+reserved+for+private+LANs%29.jpg)

***Class A:***
This is for a large corporation that their address starts with `10.0.0.0` that lets you have a lot of hosts.

***Class B:***
This are used for medium-large size corporations, they support up to 65,000 hosts.

***Class C:***
Is the common household, small business use, it always starts with `192.168.0.0` and its subnet is /24 (255.255) and it has a number of hosts that is maximun till 254.

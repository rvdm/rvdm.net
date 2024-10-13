---
title: "bgp"
date: 2024-10-13T17:50:35+02:00
draft: false
menu: "main"
---
---

This page is about AS57048 and how to peer with me. AS57048 is an ipv6-only hobby-ASN with no other purpose than to learn as well as to provide me with ipv6 connectivity in places where I don't have it.

## General info
AS57048 runs on a VM on a [proxmox](https://www.proxmox.com) server co-located at [coloclue](https://coloclue.net/) in Amsterdam. I run a mix of physical interconnects as well as tunneled connections for transit and peering.

General information on AS57048 can be found in a couple of places:
[peeringdb](https://www.peeringdb.com/asn/57048)
[bgp.tools](https://bgp.tools/as/57048)
[bgp.he.net](https://bgp.he.net/AS57048)

I announce only a single prefix ( 2a0e:f7c0::/29 ). I do strict RPKI ROV validation.

## Peering locations

You can directly peer with me in the following locations:
| Network/Exchange                  | Location          | IP on peering lan       |
| ----------------------------------|-------------------|-------------------------|
| [Frys-IX](https://frys-ix.net/)   | NIKHEF Amsterdam  | 2001:7f8:10f::ded8:1629 |
| [ColoClue](https://coloclue.net/) | Qupra Amsterdam   | 2a02:898::60:2          |
| [4ixp](https://www.4ixp.com/)     | Zurich via tunnel | 2001:7f8:d0::ded8:1     |

In all locations where a route server is available, I peer with it.

## Upstreams
I use transit from a few (free) transit providers and friends:
| Network       | ASN     |
| --------------|---------|
| [ColoClue](https://coloclue.net) | AS8283 |
| [Hurricane Electric](https://he.net) | AS6939 | 
| [FreeTransit](https://freetransit.ch/) | AS41051 |
| [NetOne](https://noc.netone.nl) | AS200132 |
| [BGPTunnel](https://bgptunnel.com/) | AS209533 |

## Policies
- Open peering policy
- No contract
- RPKI ROV strict
- PeeringDB and IRR up to date
- No SLA, no funny business :smiley:

Should you want to contact me to set up a peering session at any of the available locations, *peering [at] [this domain name]* can be used to get in touch.

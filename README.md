

    ██╗ ██████╗ ████████╗    ██████╗ ██████╗  ██████╗ ████████╗ ██████╗  ██████╗ ██████╗ ██╗     ███████╗
    ██║██╔═══██╗╚══██╔══╝    ██╔══██╗██╔══██╗██╔═══██╗╚══██╔══╝██╔═══██╗██╔════╝██╔═══██╗██║     ██╔════╝
    ██║██║   ██║   ██║       ██████╔╝██████╔╝██║   ██║   ██║   ██║   ██║██║     ██║   ██║██║     ███████╗
    ██║██║   ██║   ██║       ██╔═══╝ ██╔══██╗██║   ██║   ██║   ██║   ██║██║     ██║   ██║██║     ╚════██║
    ██║╚██████╔╝   ██║       ██║     ██║  ██║╚██████╔╝   ██║   ╚██████╔╝╚██████╗╚██████╔╝███████╗███████║
        

* [PHY/MAC](#phymac)
 * [IEEE 802.15.4](#ieee-802154)
    * [Network topologies](#network-topologies)
 * [IEEE 802.11](#ieee-80211)
 * [Bluetooth](#bluetooth)
 * [Bluetooth 4.0 Low Energy](#bluetooth-40-low-energy)
 * [Others](#others)
* [Application Layer](#application-layer)
* [References](#references)

# PHY/MAC

## IEEE 802.15.4

This prototocol is part of IEEE 802.15™: Wireless Personal Area Networks (PANs)

Telecommunications and information exchange between systems for local and metropolitan area networks. 
This standard defines the physical layer (PHY) and medium access control (MAC) sublayer specifications
for low-data-rate wireless connectivity with fixed, portable, and moving devices with no battery or very
limited battery consumption requirements. In addition, the standard provides modes that allow for precision
ranging. PHYs are defined for devices operating various license-free bands in a variety of geographic
regions.

Two different device types can participate in an IEEE 802.15.4 network: a full-function device (FFD) and a
reduced-function device (RFD).

A system conforming to this standard consists of several components. The most basic is the device. A device
has a single radio interface that implements an IEEE Std 802.15.4 MAC and PHY. Two or more devices
communicating on the same physical channel constitute a wireless personal area network (WPAN). A
WPAN includes at least one FFD, operating as the PAN coordinator.
 
### Network topologies

Depending on the application requirements, an IEEE 802.15.4 low-rate WPAN (LR-WPAN) operates in either of two
topologies: the star topology or the peer-to-peer topology.

 ● - Full Function Device

 ○ - Reduce Function Device


#### Star topology

                ○
                ▲
                │
                │
                ▼
        ●◀─────▶●◀─────▶○
              ╱ ▲
             ╱  │
          PAN   │
     Coordinator▼
                ●

After an FFD is activated, it can establish its
own network and become the PAN coordinator. All star networks operate independently from all other star
networks currently in operation. This is achieved by choosing a PAN ID that is not currently used by any
other network within the radio communications range. Once the PAN ID is chosen, the PAN coordinator
allows other devices, potentially both FFDs and RFDs, to join its network.

#### Peer-to-peer topology

       ┌───────▶●◀─────┐
       │        ▲      │
       │        │      │
       │        │      │
       ▼        │      ▼
       ●◀───────┼──────●◀───────▶○
       ▲        │      ▲╲
       │        │      │ ╲
       │        ▼      │  PAN
       └───────▶●◀─────┘ Coordinator

In a peer-to-peer topology, each device is capable of communicating with any other device within its radio
communications range. One device is nominated as the PAN coordinator, for instance, by virtue of being the
first device to communicate on the channel. Further network structures are constructed out of the peer-to-
peer topology, and it is possible to impose topological restrictions on the formation of the network.

## IEEE 802.11

## Bluetooth

## Bluetooth 4.0 Low Energy

## Others

# Application Layer

## CoAP

The Constrained Application Protocol (CoAP) is a specialized web
transfer protocol for use with constrained nodes and constrained
(e.g., low-power, lossy) networks.

CoAP provides a request/response interaction model between
application endpoints, supports built-in discovery of services and
resources, and includes key concepts of the Web such as URIs and
Internet media types.  CoAP is designed to easily interface with HTTP
for integration with the Web while meeting specialized requirements
such as multicast support, very low overhead, and simplicity for
constrained environments.

# References

1. [IEEE 802.15™: Wireless Personal Area Networks (PANs)][1]
2. [IEEE Std 802.15.4TM-2015][2]
3. [The Constrained Application Protocol (CoAP)][3]


[1]: http://standards.ieee.org/about/get/802/802.15.html "IEEE 802.15™: WIRELESS PERSONAL AREA NETWORKS (PANs)"
[2]: http://standards.ieee.org/getieee802/download/802.15.4-2015.pdf " IEEE 802®: LOCAL AND METROPOLITAN AREA NETWORK STANDARDS"
[3]: https://tools.ietf.org/html/rfc7252 "The Constrained Application Protocol (CoAP)"

                                                             

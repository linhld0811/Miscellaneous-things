# WebRTC Connection Process:
1. ICE Gathering: Both devices gather ICE candidates (network addresses) and exchange them to find the best network path.
2. Connectivity Checks: Devices perform connectivity checks to determine the best route for communication, using STUN/TURN servers if needed.
3. Peer-to-Peer Connection: Once the best network path is identified, a direct peer-to-peer connection is established for media streaming.
4. SDP offer: Device A sends an SDP offer, describing the media streams (the type of codec, transport protocol, 
and other related information) and connection parameters.
5. SDP Answer: Device B responds with an SDP answer, agreeing on the media format and other parameters.
# References:
1. **ICE Protocol** (Interactive Connectivity Establishment protocol): establish connections between devices over the Internet
  - ICE helps WebRTC traverse NATs and firewalls by allowing devices to find and use the most efficient network path between them, regardless of how the network is configured.
2. **ICE gathering**: devices exchange ICE candidates
3. **ICE Candidates**: addresses that devices use to connect with each other over the internet.
 - A device can have multiple ICE candidates, each containing information such as IP addresses, port numbers, and transport protocols
4. **NAT** (Network Address Translators) technique deployed by routers to conserve,
    hide and add an extra layer of security to the internal IP addresses of devices in its network.
    Routers achieve this by allowing multiple devices on their local network to share a single public IP address
    that they can use to communicate with other devices, this could be DNS servers or other devices.
    NATs make networks safer, they also present a significant obstacle to establishing peer-2-peer communication between devices.
5. **STUN servers** (Session Traversal Utilities NAT)

# Tutorials:
1. [Create STUN/TURN Server](https://ourcodeworld.com/articles/read/1175/how-to-create-and-configure-your-own-stun-turn-server-with-coturn-in-ubuntu-18-04)
2. [Check ICE Server](https://webrtc.github.io/samples/src/content/peerconnection/trickle-ice/)
3. [ICE Explained](https://www.digitalsamba.com/blog/ice-and-sdp-in-webrtc)
4. [Webrtc Ports Explained](https://bloggeek.me/webrtc-ports-ip-addresses/)

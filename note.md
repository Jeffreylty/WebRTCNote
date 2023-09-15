ICE (Interactive Connectivity Establishment):

Used to find the best way to route media.
Uses STUN (Session Traversal Utilities for NAT) and TURN (Traversal Using Relays around NAT) servers to resolve NAT/firewall issues and establish a connection between peers.
SDP (Session Description Protocol):

Describes multimedia sessions. It doesn't transport any media by itself, but is used in the signaling process to agree on the type of media, formats, codecs, etc.
Signaling:

Not specifically defined by WebRTC; applications can use any protocol.
The process where peers exchange metadata to coordinate communication. This includes exchanging SDP offers/answers, ICE candidates, etc.
Many WebRTC apps use protocols like SIP (Session Initiation Protocol) or simple WebSocket-based signaling.
SRTP (Secure Real-time Transport Protocol):

Used to transport audio and video securely.
Ensures that the media streams are encrypted and authenticated.
DTLS (Datagram Transport Layer Security):

Used to secure the connection and validate the integrity and origin of data.
Ensures that the connection between peers is secure, and the data exchanged is authentic.
RTP (Real-time Transport Protocol):

Used for transporting real-time media like audio and video.
RTCP (Real-Time Control Protocol):

Works alongside RTP.
Provides out-of-band control information for an RTP flow. This includes feedback about QoS, jitter, latency, etc.
SCTP (Stream Control Transmission Protocol):

Transport protocol used by data channels for sending arbitrary data between peers.
Data Channels:

Allow bidirectional communication of any type of data. This is built on top of SCTP and is part of the WebRTC specification.
TURN (Traversal Using Relays around NAT):

When direct peer-to-peer communication is blocked due to NAT or firewall constraints, TURN servers can be used to relay the traffic.
STUN (Session Traversal Utilities for NAT):

Used to discover the public IP address of the client when behind a NAT.

# Spring

## Websockets:
 is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C. WebSocket is distinct from HTTP.

 The WebSocket protocol enables **interaction** between a web browser (or other client application) and a web server with lower overhead than half-duplex alternatives such as HTTP polling, facilitating real-time data transfer from and to the server. This is made possible by providing a standardized way for the server to send content to the client without being first requested by the client, and allowing messages to be passed back and forth while keeping the connection open.

 WebSockets keeps a unique connection open while eliminating latency problems that arise with Long Polling.

 WebSockets generally do not use XMLHttpRequest, and as such, headers are not sent every-time we need to get more information from the server. This, in turn, reduces the expensive data loads being sent to the server.

 Some problems with Websockets:
 1. WebSockets don’t automatically recover when connections are terminated.
 2. Browsers older than 2011 aren’t able to support WebSocket connections.
 

 ## Polling:
 It is implemented on the back of XMLHttpRequest, which is near-universally supported by devices so there’s usually little need to support further fallback layers. In cases where exceptions must be handled though, or where a server can be queried for new data but does not support long polling (let alone other more modern technology standards), basic polling can sometimes still be of limited use, and can be implemented using XMLHttpRequest, or via JSONP through simple HTML script tags.

 Some problems with polling:
 1. polling is a lot more intensive on the server.
 2. Reliable messaging ordering can be an issue with long polling because it is possible for multiple HTTP requests from the same client to be in flight simultaneously.
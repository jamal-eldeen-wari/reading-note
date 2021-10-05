# The HTTP Request Lifecycle:
HTTP 1.1 request, not a persistent connection as HTTP/2 and persistent connection requests.

Lifecycle has number of steps:
1. Local Processing: this request is being made by a browser, as opposed to cURL, an API client like Postman, or some other app:
 1. Your browser extracts the "scheme"/protocol (we have established
that this will be HTTP).
 2. The browser will then look through its own cache of recently requested URLs, the operating system’s cache of recent queries, your router’s cache, and your DNS cache.

2. Resolve an IP:
If the cache lookup fails (we will assume it does), your browser fires off a DNS request using UDP3. The DNS request contains the preconfigured IP for your DNS server and your return IP in its header.
Your request will now have to travel many network devices to reach its target DNS server.
Once your request arrives at your configured DNS server, the server looks for the address associated with the requested hostname. If it finds one, it sends a response. If, on the other hand, the DNS server you have targeted cannot locate the given hostname, it passes the request along to another DNS server it is configured to defer to. This happens recursively until the address is found, or an "authoritative" nameserver is hit. If an address for the given domain cannot be resolved, the server responds with a failure and your browser returns an error.
We will assume the request is successful though, given that all of this is still a precursor. If the response makes it back the requesting client now has a target IP. It will also have received a piece of information as part of the answer that will let it know how long the returned answer can be cached for.

3. Establish a TCP Connection:
since the request is sent over TCP 6, which is a transport layer protocol like UDP, the client must open a TCP connection.
Important to note the difference between TCP and UDP is that TCP ensures delivery and ordered data transmission. as a sequence number for every byte sent.This allows the receiver to re-order received packets back into their original order, and allows the sender to retransmit any packet that does not get acknowledged by the receiver.

 three-way handshake: Where the server must already be "listening" on a port, performing a passive open, after which the client can initiate an active open, and the handshake works as folows:
 1. The client initiates the active open by sending a SYN7 "control"8 packet to the server. 
 2. The server responds with a SYN-ACK9 message.
 3. the client sends an ACK10 message back to the server with a sequence number equal to x+1, which should match the SYN-ACK message’s acknowledgment number and ensure that our data is being delivered reliably.

 4. Send an HTTP Request:
 The request is made up of a "request line", request header, and a body. The "request line" is simply a line that indicates the HTTP method, the resource being requested, and the protocol version. The header of the request is made up of pairs in the form name:value CR LF. Two consecutive CR LF pairs indicate the end of the header section. 
 Once the HTTP request is sent, it follows a similar routing procedure as the one discussed earlier, with the difference being that using TCPs magic sequence number powers, the server can ensure it receives the whole request, in the correct order.

Once the server receives the request, processes it, and finds the resource being requested, it generates an HTTP response. An HTTP response has a similar structure to an HTTP request, containing a "status line", response header fields, and an optional body. 
Once the response is generated, the server responds to the request. At the TCP layer, the client receives the first data packet, the first byte of which should contain the HTTP response header. More packets start coming in, and at the TCP layer they are re-ordered as needed. For every two packets that the client receives at the TCP layer, it sends an ACK message to the server. This goes on until the response is (hopefully) fully loaded.

5. Tearing Down and Cleaning Up:
Once the response has been fully delivered, the client sends a FIN packet at the TCP level, to which the server responds with an ACK, and then generally sends a FIN of its own, which the client responds to with its own ACK signal.

At this point, your browser begins processing what it has received. If it is an image, data, or other media file that is being consumed by some application inside the browser, a variety of things can happen.

## Way of performing HTTP requests in Java:
HttpUrlConnection class allows us to perform basic HTTP requests without the use of any additional libraries. All the classes that we need are part of the java.net package.

### How Can We Create Request?
We can create an HttpUrlConnection instance using the openConnection() method of the URL class.

### How to add request parameter from java?
we have to set the doOutput property to true, then write a String of the form param1=value¶m2=value to the OutputStream of the HttpUrlConnection instance.

### How can we set Request Headers?
We can add  headers to a request can be achieved by using the setRequestProperty() method.

### How can we handle coockies?
The java.net package contains classes that ease working with cookies such as CookieManager and HttpCookie.

### How can we Read a Response?
It can be done by parsing the InputStream of the HttpUrlConnection instance.


### How can we Build a Full Response?
It's not possible to get the full response representation using the HttpUrlConnection instance.
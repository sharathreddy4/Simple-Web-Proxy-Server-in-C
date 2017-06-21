# Simple-Web-Proxy-Server-in-C
This repo is an assignment to create a HTTP based web proxy server that handles requests from clients, pass them to	HTTP server and handle returning traffic from the	HTTP server back to clients. This is done as part of Network Systems course at CU boulder.

## Execution sequence(commands to be typed for compiling and running).
*Server:
Compiling: cc -o p proxy_server.c
Execution: ./p <port number>

*Client:
Initiating telnet:  telnet localhost <port number>
giving command:
			
			<method> <url> <http version>
			ex: GET http://www.google.com HTTP/1.0
			    GET http://www.yahoo.com HTTP/1.1
		
## Testing sequence
*Simple proxy testing: 
		a. Open 2 terminals in the same directory that contains the proxy_server object file
		b. In one terminal execute the server program using the above given execution sequence.
		c. In another terminal perform the telnet ping and give the necessary command as shown above.
		
*Caching testing
		a. During execution, when a basic URL is requested  for the first time, the server displayes a message saying the unavailability of CACHE. But if the same
			URL is again requested this time server displayes a message to saying the availablity of CACHE and a file with the same
			name as URL will be present in the Directory. This acts as the cache. 
		b.The cached pages are displayed even after disconnecting from the internet.
	
	
	

# Assignment--1-


Q - Discuss TCP & UDP Protocols and mention the difference between the two along with examples where they are used?

A - TCP (Transmission Control Protocol) - Connection oriented protocol, reliable as it delivers the bytes stream        (data ko binary format me transfer kiya jata hai I.e 0 & 1) without error from one machine to another. Eg - Email and Online games
 UDP (User Datagram Protocol) - Connectionless protocol;, Unreliable and user where prompt/fast delivery is more important than accuracy. Eg - Live streaming, Video call and Online Games (Multiplayer)

Q - List the TCP Flags along with their use/function?

A - TCP uses flag to manage the communication between/w sender and receiver which helps in connection establishments, data transfer & connection termination

          								  Types of Flag
	1)  URG (Urgent) - Indicates that the data should be processed immediately 
	2)  ACK (Acknowledgement) - Used to confirm the receipt of data. Once the ACK is received then further action are performed.
	3)  PSH (Push) - Force data to be sent immediately instead of waiting for a buffer to be filled Eg. Voice call, Gaming
	4)  RST (Reset) -  Reset a connection incase of an error or unexpected termination
	5)  SYN (Synchronise) - Initiate a connection between/w two devices.
	6)  FIN  (Finish) - Terminates the connection b/w sender and receiver.
					
									   Usage
         1)  3-way Handshake (Connection Establishment)

			. Client - Server ( SYN)
			. Server - Client (SYN-ACK)
			. Client- Server ( ACK)

	2)  Data transfer 
			
			. PSH flag ensues data is sent imminently 
			. ACK flag confirms receipt  of packets 

	3) Connection Termination 
			. Client - Server (FIN)
			. Server - Client (ACK)
			. Server - Client (FIN)
			. Client - Server (ACK)

Q - What is the difference in executing Nmap as root user and as normal user? Give the flags in Nmap which require root permission to be performed?

A - The difference is about the access level to the Nmap function & capabilities. 
	Following are the flag which require root access
		. SYN Scan (-sS)
		. Connect Scan (-sT)
		. Service & OS detection (-sV, -o)
		. Aggressive scanning (-A)
		. Idel Scan (-sl)
		. Fragmented Packets (-f)
		. Spoofing (IP/MAC) (-S,  - - spoof - Mac)

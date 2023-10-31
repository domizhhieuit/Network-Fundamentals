# Everything hosts do to speak on the internet 

### Host connect through other internet

![Alt text](image-1.png)

Host A,Host C and Router have MAC router address

/24 is a subnet of Mac - 255.255.255.0

- Host A has some data to sent to host c
 - Host A knows host c' IP address
    - Provided by the user or the application 
 - Host A knows host C's IP address is on a foreign network

 - Host A creates a L3 header 

  - Layer 3 - End to End 
- Host A need create a L2 header 
  - Hop To Hop 
  Next Hop is Router 

Host A uses ARP to reslove the MAC address of the Router's IP
- If anyone out there has the IP 10.1.1.1 send me your MAC

- Host A create L2 header 
 
    - Layer 2 - Hop to Hop

- Data is sent to the router
    - L2 header is discarded 
    - Router takes over from this point
    - Host A's job is done
- ARP mapping can be used for any host in foreign networks
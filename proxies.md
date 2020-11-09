# Proxies


### Proxy vs Reverse Proxy
A `proxy` is a server that accepts connections from clients, which **actively configured** the proxy server on their machines, in their network settings.  
This practice has several uses. Companies and organizations can set up proxy servers to filter connections, provide more security, and log traffic. Without using the proxy, clients can’t reach the outside network. Proxy servers are also useful to provide privacy and avoid network restrictions imposed by countries governments.  
  
A `reverse proxy` on the other hand is **set up by the server**. It’s completely transparent to clients, they don’t know this `middleman` exists, but it does a very useful job on the servers, filtering requests and sending them to the appropriate service that handles them.
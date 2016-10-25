#I2P Hidden RetroShare Nodes  
I2P is an anonymous overlay network - a network within a network. 
It is intended to protect communication from dragnet surveillance and 
monitoring by third parties such as ISPs. 
I2P can run Hidden Services similar to [Tor Hidden Serives](../tutorial/tor-hidden-rs-node/). 
to route encrypted traffic inside the network to anonymize the Client and the Server.  

RetroShare can be run behind an I2P Hidden Service for incoming connections. 
The outgoing connections are sent through a local I2P Socks Proxy. 
This makes it possible to obfuscate your metadata which could disclose 
your Network Friend Graph. The hidden service address 
(e.g. ld5...2z3p.b32.i2p) is replacing the IPv4 address 
(e.g. 192.168.1.216) as the listening address for incoming connections. 

I2P allows clients and relays to offer hidden services. That is, you can 
offer a web server, SSH server, etc., without revealing your IP address 
to its users. In fact, because you don't use any public address, you can 
run a hidden service from behind your firewall.  

##Hidden Service Setup  
###I2P Installation  
This Guide requires to have Tor already installed on your System.  
If not, please refer to the offical [I2P Documentation](https://geti2p.net/en/docs) 
on how to install I2P.  

Download I2P for various operating systems: [I2P Download](https://geti2p.net/en/download)  

###Outgoing I2P Proxy  
For this we have to create a “Local tunnel” in the I2P Router Console. If 
you have it running on your local computer, Hidden Service Manager should be located 
at [http://127.0.0.1:7657/i2ptunnelmgr](http://127.0.0.1:7657/i2ptunnelmgr)  
![i2p hidden service manager](../img/tutorial/i2p/hidden_service_manager.png "i2p hidden service manager")  

Click on Tunnel Wizard  
![i2p Tunnel Wizard](../img/tutorial/i2p/tunnel_wizard.png "i2p Tunnel Wizard")  

If you need to connect to a remote service, such as an IRC server inside 
I2P or a code repository, then you will require a CLIENT tunnel. 
![i2p Client Tunnel](../img/tutorial/i2p/client_tunnel.png "i2p Client Tunnel")  

Select SOCKS 4/4a/5 - A tunnel that implements the SOCKS protocol. 
This enables both TCP and UDP connections to be made through a SOCKS 
outproxy within I2P. 
<a href="../../img/tutorial/i2p/socks_proxy.png" target="_blank">![i2p Socks Proxy](../img/tutorial/i2p/socks_proxy.png "i2p Socks Proxy")</a>  

Choose a name and description for your tunnel. These can be anything you 
want - they are just for ease of identifying the tunnel in the routerconsole. 
![i2p Tunnel Name](../img/tutorial/i2p/socks_name.png "i2p Tunnel Name")  

Leave *Outproxies* empty
![i2p Outproxy](../img/tutorial/i2p/outproxy.png "i2p Outproxy")  

This is the port that the client tunnel will be accessed from locally. 
This is also the client port for the HTTPBidir server tunnel.  

 - Select **4447** as RetroShare and I2P use this as the default  
 
How do you want this tunnel to be accessed? By just this machine, 
your entire subnet, or external internet? You will most likely want 
to just allow 127.0.0.1  

 - let I2P Proxy bind to **localhost/127.0.0.1** only  
 
![i2p Port Binding](../img/tutorial/i2p/port_binding.png "i2p Port Binding")   

The I2P router can automatically start this tunnel for you when the 
router is started. This can be useful for frequently-used tunnels 
(especially server tunnels), but for tunnels that are only used 
occassionally it would mean that the I2P router is creating and 
maintaining unnecessary tunnels.  
![i2p Auto Start](../img/tutorial/i2p/auto_start.png "i2p Auto Start")  

The wizard has now collected enough information to create your tunnel.  
<a href="../../img/tutorial/i2p/wizard_completed.png" target="_blank">![i2p Wizard Completed](../img/tutorial/i2p/wizard_completed.png "i2p Wizard Completed")</a>  

###Configure your hidden service  



##RetroShare I2P Setup  



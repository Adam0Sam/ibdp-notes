### Secure VPN Technologies

All traffic on the VPN must be encrypted, authenticated and then sent along virtual tunnels. This is done with either **IPsec** or **SSL/TLS**

1. Internet Protocol Security Protocol (IPSsec) functions in both transport and tunnel mode: secure transmission of encrypted data over public IP-based networks *and* authentication via digital certificates
2. Secure Socket Layer (SSL) or Transport Layer Security (TLS). SSL/TLS based VPNs are much simpler than IPSec based VPNs. The use of this technology does not require special client software because all Web browsers/servers support SSL/TLS

### Trusted VPN Technologies

1. Layer 2 VPNs
	- Asynchronous Transfer Mode (ATM) circuits
	- Frame relay circuits
	- Transport of layer 2 frames over MultiProtocol Label Switching (MPLS)
2. Layer 3 VPNs
	- MultiProtocol Label Switching (MPLS) with constrained distribution of routing information through Border Gateway Protocol (BGP)


> [!tip] Hybrid VPNs
> Hybrid VPN technologies combine both [[#Secure VPN Technologies"|secure]] and [[#Trusted VPN Technologies|trusted]] technologies of VPNs
> #todo wtf does this mean


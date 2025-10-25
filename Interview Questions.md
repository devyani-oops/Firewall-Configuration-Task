## Interview Questions Preparation

1. What is a firewall?
   
  A firewall is a network security system that monitors and controls incoming and outgoing network traffic based on predetermined security rules. It acts as a barrier between trusted internal networks and untrusted external networks.

2. Difference between stateful and stateless firewall?
   
  Stateful Firewall: Tracks the state of network connections (like TCP handshakes), maintains context about active sessions, and makes decisions based on the connection state.
  
  Stateless Firewall: Filters packets based on static information like source/destination IP and ports without tracking connection state. Less secure but faster.

3. What are inbound and outbound rules?
   
  Inbound Rules: Control incoming traffic to your computer from external sources
  
  Outbound Rules: Control outgoing traffic from your computer to external destinations

4. How does UFW simplify firewall management?
   
  UFW (Uncomplicated Firewall) provides a user-friendly interface for iptables, using simple commands like ufw allow ssh instead of complex iptables syntax, making firewall management accessible to beginners.

5. Why block port 23 (Telnet)?
   
  Telnet transmits data in plain text, including passwords, making it vulnerable to eavesdropping. It's an insecure protocol that should be replaced with SSH (port 22) which encrypts all communication.

6. What are common firewall mistakes?
   
  Blocking all ports including SSH (locking yourself out)
  
  Not regularly updating firewall rules
  
  Allowing unnecessary services
  
  Forgetting to configure both inbound and outbound rules
  
  Not testing rules after implementation

7. How does a firewall improve network security?
   
    Prevents unauthorized access to network resources
    
    Blocks malicious traffic and attacks
    
    Controls data flow between network segments
    
    Logs network activity for monitoring
    
    Enforces security policies

8. What is NAT in firewalls?
   
  NAT (Network Address Translation) allows multiple devices on a private network to share a single public IP address. Firewalls often perform NAT to hide internal network structure and conserve IP addresses.


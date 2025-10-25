### Quick start

# Commands Used for Kali Linux Firewall Task

# 1. Installation and Initial Setup
                              sudo apt update
                              sudo apt install ufw
                              sudo ufw status

# 2. Checking Current State
                              sudo ufw status verbose
                              sudo netstat -tulpn
                              sudo iptables -L

# 3. Setting Default Policies
                              sudo ufw default deny incoming
                              sudo ufw default allow outgoing

# 4. Allowing SSH (Critical)
                              sudo ufw allow 22/tcp
                              sudo ufw allow ssh

# 5. Blocking Telnet
                              sudo ufw deny 23/tcp

# 6. Verification
                              sudo ufw status numbered

# 7. Enabling Firewall
                              sudo ufw enable

# 8. Testing
                              telnet localhost 23
                              nc -zv localhost 23
                              ssh localhost

# 9. Cleanup
                              sudo ufw delete deny 23/tcp
                              sudo ufw disable
                              sudo ufw reset

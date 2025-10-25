### Results and Verification

Rule Configuration Summary
Rule	                Action         	Port          	Protocol	      Status
Default Incoming	    Deny	          All	            All         	  Active
Default Outgoing    	Allow	          All           	All	            Active
SSH	                  Allow	          22	            TCP	            Active
Telnet	              Deny	          23            	TCP 	          Tested

### Test Results

 -Telnet Block: Connection attempts to port 23 were refused

- SSH Allow: SSH connections to port 22 worked normally

- Rule Persistence: Rules maintained after firewall enable

- Clean Removal: Test rules successfully removed during cleanup

### Key Learnings

**Technical Insights**
UFW Simplification: UFW provides user-friendly interface over complex iptables

Order Matters: Rule order affects processing sequence

Default Policies: Critical to set deny incoming as default

Testing Essential: Must verify both allowed and blocked connections

**Security Best Practices**
Always Allow SSH First: Prevent remote access lockout

Principle of Least Privilege: Only allow necessary services

Regular Audits: Periodically review firewall rules

Documentation: Maintain records of all changes

![image alt]()
![image alt]()
![image alt]()
![image alt]()

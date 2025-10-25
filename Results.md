### Results and Verification

Rule Configuration Summary
Rule	                Action         	Port          	Protocol	      Status
Default Incoming	    Deny	          All	            All         	  Active
Default Outgoing    	Allow	         All            	All	           Active
SSH	                 Allow	         22	             TCP	           Active
Telnet	              Deny	          23             	TCP 	          Tested

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

![image alt](https://github.com/devyani-oops/Firewall-Configuration-Task/blob/5d2225df1a6fd9065b6e2c91ba51a4fae3aa3d71/Screenshot%202025-10-25%20105029.png)
![image alt](https://github.com/devyani-oops/Firewall-Configuration-Task/blob/7aede9825ef729372fa39fe235c994b21a460cfe/Screenshot%202025-10-25%20105047.png)
![image alt](https://github.com/devyani-oops/Firewall-Configuration-Task/blob/5cfddf4bbc8fd7d7fbeb5c9115fae3766f65134d/Screenshot%202025-10-25%20105102.png)
![image alt]()

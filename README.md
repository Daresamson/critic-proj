Here's a table summarizing CIDR, subnetting, and key factors for the organization's subnetting plan:
Department	Current Hosts	Future Hosts	CIDR Notation	Subnet Mask	IP Address Range
![Screenshot (116)](https://github.com/user-attachments/assets/8ea00883-9ae8-48d8-adf0-72c27d98e5a0)

# Key Factors
•	Current Hosts: Number of hosts currently required.
•	Future Hosts: Anticipated number of hosts accounting for growth (50% increase).
•	CIDR Notation: Classless Inter-Domain Routing representation.
•	Subnet Mask: Standard subnet mask corresponding to CIDR notation.
•	IP Address Range: The usable range of IP addresses for each department.

# Subnetting Plan for Growing Organization
1. Identify Subnet Requirements
•	Departments and Current Hosts:
o	Finance: 50 hosts
o	Human Resources: 30 hosts
o	Sales: 70 hosts
o	Marketing: 40 hosts
o	IT: 100 hosts
o	Operations: 80 hosts
•	Future Growth: Plan for at least 50% growth in each department over the next five years.
2. Allocate IP Addresses
•	Total Hosts Required (with growth):
o	Finance: 75 hosts (requires 128 addresses)
o	Human Resources: 45 hosts (requires 64 addresses)
o	Sales: 105 hosts (requires 128 addresses)
o	Marketing: 60 hosts (requires 64 addresses)
o	IT: 150 hosts (requires 256 addresses)
o	Operations: 120 hosts (requires 128 addresses)
•	Total Subnets Required: 6
3. Subnet Masking
•	Subnet Masks:
o	Finance: /25 (255.255.255.128)
o	Human Resources: /26 (255.255.255.192)
o	Sales: /25 (255.255.255.128)
o	Marketing: /26 (255.255.255.192)
o	IT: /24 (255.255.255.0)
o	Operations: /25 (255.255.255.128)
4. Documentation
•	IP Address Ranges:
o	Finance: 10.0.0.0 - 10.0.0.127
o	Human Resources: 10.0.0.128 - 10.0.0.191
o	Sales: 10.0.0.192 - 10.0.0.255
o	Marketing: 10.0.1.0 - 10.0.1.63
o	IT: 10.0.1.64 - 10.0.1.255
o	Operations: 10.0.2.0 - 10.0.2.127
•	Purpose:
o	Finance: Financial transactions and accounting systems.
o	Human Resources: Employee data and payroll systems.
o	Sales: Customer relationship management (CRM) and sales data.
o	Marketing: Marketing campaigns and analytics.
o	IT: Network infrastructure and servers.
o	Operations: Production and supply chain management.
5. Troubleshooting Scenarios
•	Connectivity Issues:
o	Check routing tables for correct subnet routes.
o	Verify firewall rules for inter-subnet communication.
•	IP Conflicts:
o	Use DHCP server logs to identify conflicting IP addresses.
o	Manually assign IP addresses to resolve conflicts.
•	Overlapping:
o	Ensure each subnet has a unique IP address range.
o	Adjust subnet masks to avoid overlapping ranges.
6. Future Growth
•	Expand Subnets:
o	Increase subnet sizes by adjusting subnet masks if needed.
o	Add new subnets for additional departments or teams.
•	Modify Documentation:
o	Update IP address ranges and subnet masks accordingly.
o	Keep track of changes for future reference.
7. Optimization
•	Efficient Routing:
o	Implement routing protocols to optimize traffic between subnets.
o	Use VLANs to segment traffic within departments.
•	IP Address Use:
o	Implement DHCP for dynamic IP address assignment.
o	Reserve static IP addresses for critical devices and servers.
This plan provides a scalable and efficient approach to subnetting for the organization, ensuring that it can adapt to future growth while maintaining network performance and security.


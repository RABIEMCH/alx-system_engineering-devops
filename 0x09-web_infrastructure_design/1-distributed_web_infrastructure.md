Distributed Web Infrastructure Overvier
![Image of a distributed web infrastructure](1-distributed_web_infrastructure.PNG)

Overview:
The distributed web infrastructure aims to enhance website performance and resilience by distributing traffic and responsibilities across multiple servers. This setup employs load balancers, primary-replica database configurations, and multiple servers to handle requests efficiently.

Key Elements:
Load Balancer:

Algorithm: Uses the Round Robin distribution, evenly distributing requests among servers based on their weights.
Mode: Operates in an Active-Passive mode. While one server handles requests, the other remains on standby, ready to take over if needed.
Database Configuration:

Primary-Replica (Master-Slave): One server acts as the Primary (or Master) for read/write operations, while the other serves as a Replica (or Slave) for read-only operations. Data synchronization ensures consistency between the two.
Server Roles:

Primary Node: Handles write operations, ensuring data integrity and consistency.
Replica Node: Manages read operations, reducing the read traffic on the primary node and enhancing performance.
Limitations:
Single Points of Failure (SPOF):

Several components, including the Primary MySQL database, the load balancer server, and the application server, pose SPOF risks. If any of these fail, the entire website's functionality could be compromised.
Security Concerns:

Lack of SSL encryption exposes transmitted data to potential eavesdropping.
Absence of firewalls leaves the infrastructure vulnerable to unauthorized access.
Monitoring Absence:

The infrastructure lacks monitoring tools or systems, making it challenging to identify and address issues promptly.
To ensure optimal performance and security, it's crucial to address these limitations, possibly by introducing redundancy, enhancing security measures, and implementing robust monitoring solutions.

Secured and Monitored Web Infrastructure Overview
![Image of a secured and monitored infrastructure](2-secured_and_monitored_web_infrastructure.PNG)

Overview:
This 3-server web infrastructure emphasizes security, encryption, and proactive monitoring to ensure robust performance and safeguarded data transmission.

Key Components and Their Roles:
Firewalls:

Purpose: These act as protective barriers, regulating and filtering incoming and outgoing traffic to prevent unauthorized access and potential threats. They stand between the internal web servers and the external network, only allowing legitimate traffic.
SSL Certificates:

Purpose: Essential for encrypting data traffic between the web servers and external users. They deter eavesdropping and man-in-the-middle attacks by ensuring that data remains confidential, maintains its integrity, and confirms the server's identity to users.
Monitoring Clients:

Purpose: Dedicated tools that continuously observe and assess the server performance. They offer insights into server health, alert administrators about potential issues, and provide vital metrics for informed decision-making. These tools also facilitate rapid response to anomalies, ensuring uninterrupted service.
Limitations:
SSL Termination at Load Balancer:

Encrypting traffic up to the load balancer level leaves intra-server communication unencrypted, potentially exposing data within the internal network.
Single MySQL Server:

This setup lacks scalability, posing a risk of becoming a bottleneck as traffic grows. Additionally, a failure in this server could disrupt the entire infrastructure, emphasizing the need for redundancy or clustering.
Homogeneous Server Configuration:

Uniform server components may lead to resource contention, where components compete for CPU, memory, and I/O resources. This can degrade performance and complicate troubleshooting. A more scalable and diversified infrastructure design would be beneficial for future growth and optimization.
To enhance this infrastructure further, consider diversifying server roles, introducing redundancy for critical components, and implementing advanced monitoring and alerting mechanisms for comprehensive oversight and rapid issue resolution.

Simplified Web Infrastructure Overview
![Image of a simple web stack](0-simple_web_stack.PNG)

Overview:
This basic web setup is responsible for hosting the www.foobar.com website. Here's a breakdown of its key components and functions.

Components Explained:
Server: A machine or software that provides services. In this context, it responds to requests from users.

Domain Name: A user-friendly name (like www.foobar.com) that maps to an IP address using the Domain Name System (DNS). It simplifies access for users over remembering numeric IP addresses.

DNS Record for www: The domain www.foobar.com is associated with an A record, indicating it points to a specific IPv4 address. This ensures users reach the right server when accessing the site.

Web Server: Acts as a mediator between users and the website. It processes HTTP/HTTPS requests and serves web pages or handles errors.

Application Server: Handles the website's applications and services, ensuring smooth interactions and data processing for end-users.

Database: Stores and manages organized data. It's crucial for web applications to retrieve, store, and update information efficiently.

Communication: The server communicates with users' computers (clients) using the TCP/IP protocol suite over the internet.

Limitations:
Single Points of Failure (SPOF): The infrastructure has vulnerabilities. For instance, if the database server (MySQL) fails, the entire website becomes inaccessible.

Maintenance Downtime: Any maintenance activity, such as updates or checks, requires taking components offline. Given the single-server setup, this leads to website downtime.

Scalability Concerns: With increasing traffic, the server's capacity might get overwhelmed. There's no provision for distributing the load or adding resources without redesigning the infrastructure.

**For every additional element, why are you adding it:**

**Firewalls and what they are for?**

Firewalls act as barriers or partitions, implemented through either hardware or software, between a private and an outer network, filtering traffic between the two networks. They enhance infrastructure security by inspecting traffic and can be configured to allow or block specific types of traffic based on factors such as IP addresses, ports, protocols, and application types.

**Why is the traffic served over HTTPS?**

HTTPS, which stands for HTTP Secure, is implemented by adding SSL certificates to encrypt data transmitted between the client's browser and the web server. It is installed on the web servers to establish a secure connection.

**What is monitoring used for?**

Monitoring server activity allows tracking of performance, availability, and security of infrastructure components. It involves collecting and analyzing data in the form of metrics and logs to ensure optimal system operation and detect anomalies.

**How is the monitoring tool collecting data?**

Monitoring agents or data collectors are installed on the monitored infrastructure components. The collected data is sent to a centralized monitoring server or service where it is processed, stored, and analyzed.

**Explain what to do if you want to monitor your web server QPS?**

To monitor web server QPS, you can install a monitoring agent to collect HTTP access logs or metrics directly from the web server software. Configure the agent to send the collected data to a centralized monitoring service for analysis and visualization.

**You must be able to explain what the issues are with this infrastructure:**

**Why is terminating SSL at the load balancer level an issue?**

Terminating SSL at the load balancer poses a security risk as not all traffic is encrypted. If traffic is intercepted while not encrypted, it represents a security vulnerability.

**Why is having only one MySQL server capable of accepting writes an issue?**

Having only one MySQL database server capable of handling writes creates a single point of failure. If it goes down, no other infrastructure component can take over, potentially leading to service disruption.

**Why might having servers with all the same components (database, web server, and application server) be a problem?**

This infrastructure setup may pose problems as it lacks redundancy and fault tolerance. If a failure occurs on one component, it could spread and affect all servers. Additionally, it may limit scaling and flexibility.
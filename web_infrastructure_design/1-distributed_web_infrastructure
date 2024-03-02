**For every additional element, why you are adding it:**

I am adding a second global server at IP 8.8.8.9 in order to resolve the single point of failure problem. Now, if a problem occurs on one server, the other one is able to take over.
Same thing for the traffic overload and maintenance, the other server can maintain the website functioning without interruption. 
It also enhances the infrastructure reliability, scalability and distributes the workload across multiple servers. 

I'm adding a HAProxy load balancer to improve incoming traffic distribution across multiple servers. 

I'm adding a set of application files to avoid SPOF as well as ensuring that the web application is deployed and accessible on each server. 

I'm adding a second MySql database to prevent SPOF.

**What distribution algorithm your load balancer is configured with and how it works ?**

I choose to opt for the least connection algorithm as it directs incoming traffic by selecting the server with the fewest active connections at the time of request. It prevents overloading from servers.

**Is your load-balancer enabling an Active-Active or Active-Passive setup, explain the difference between both:**

My load-balancer is enable as an Active-Active setup as I choose to use the above algorithm. The difference is that in an Active-Active setup, all resources are used at all time whereas in an Active-Passive setup, one of the server, in the present case, it wouldl be the Replica node (slave) as it serves as a sort of backup that can take over in case of problems occuring with the Primary node (master).

**How a database Primary-Replica (Master-Slave) cluster works:**

The Primary node, referring as the "master" or primary database server, handles write operations such as inserts, updates, deletes and maintains the copy or multiple copies, known as Replica nodes. The Replica nodes, or "slaves" maintain a copy of the primary node's data by continuously updating using a transaction log from the latter. They can be promoted as primary node if the current one fails. The Replica node operates in read-only mode. 

**What is the difference between the Primary node and the Replica node in regard to the application:**

In this application, the server IP 8.8.8.8 is the Primary Node, the "master" and the server at IP 8.8.8.9 is the Replica Node or "slave".
The Replica node serves as a backup for read operations and can take over write operations if the Primary node fails.

**You must be able to explain what the issues are with this infrastructure:**

**Where are SPOF**

Here the SPOF is the HAProxy as if it fails, all incoming traffic will be directed to a single server, and probably resulting in overloading and creating downtime for users.

**Security issues (no firewall, no HTTPS):**

In this configuration, there are no protection against unauthorized access, attacks. 
The absence of encryption leaves data transmission vulnerable to interception and compromise.

**No monitoring:**

Absence of monitoring is critical as systems weaknesses, potential failures, security threats are undetectable rendering the system unreliable, unstable and vulnerable to attacks. 

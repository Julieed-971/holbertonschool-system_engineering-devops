**You must be able to explain some specifics about this infrastructure:**

**What is a server?**

A server is a piece of computer, hardware or software which provides several services or functionnalities for other programs or devices, the "clients".
The server communicates over a TCP/IP network which stands for Transmission Control Protocol 
It is generally located in a data center, a building dedicated to host several servers. A server runs an OS, mainly Windows or Linux. 

**What is the role of the domain name?**

To reference and identifies a website or service provided through the internet.

**What type of DNS record www is in www.foobar.com?**

"www" stands for WorldWideWeb and is an A record because it points to an IP address.

**What is the role of the web server?**

The web server receives HTTP request and process them.It either serves directly static content or forward dynamic request to the application server.

**What is the role of the application server?**

The application server receives dynamic requests and process them. It is responsible for interacting with the application files and executing the code logic of the application.
It may of may not interact with the database depending on the request.

**What is the role of the database?**

The database server stores, organizes and manages data such as user's information, products data, financial records, content as tables.
The application server and web server may or may not interact with the database depending on the request.

**What is the server using to communicate with the computer of the user requesting the website ?**

Internet

**You must be able to explain what the issues are with this infrastructure:**

    - SPOF : 

Single Point Of Failure which is an identified item which, if it fails, makes the entire system inoperable.
It is critical to identify such SPOF as it compromises the entire system. Here the system is not redundant in the sense that there are no backups.

    - Downtime when maintenance needed (like deploying new code web server needs to be restarted): 

As there are only one of each items, none can take over in case of maintenance and the whole system is down.
During maintenance, the website is inaccessible when new code is implemented and the web server will need to restart.

    - Cannot scale if too much incoming traffic: 

Same as for the maintenance, if there is too much traffic, the actual system cannot handle and spread the load, it will crash.
The server can become overloaded with requests, leading to slow performance.
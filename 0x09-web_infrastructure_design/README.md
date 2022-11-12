This project is on web infrastructure design. 
Covers the following cocepts:
    DNS
    Monitoring
    Web Server
    Network basics
    Load balancer
    Server
A lot of websites are powered by simple web infrastructure, a lot of time it is composed of a single server with a LAMP stack.

0-simple_web_stack project
This is a design of a one server web infrastructure that hosts the website that is reachable via www.foobar.com. I have started by explaining how a user will access my website.

Requirements:

    I have used:
        1 server
        1 web server (Nginx)
        1 application server
        1 application files (your code base)
        1 database (MySQL)
        1 domain name foobar.com configured with a www record that points to your server IP 8.8.8.8


1-distributed_web_infrastructure
I have designed a three server web infrastructure that hosts the website www.foobar.com.

Requirements:

    I have used:
        2 servers
        1 web server (Nginx)
        1 application server
        1 load-balancer (HAproxy)
        1 set of application files (your code base)
        1 database (MySQL)

2-secured_and_monitored_web_infrastructure
This is a design of a three server web infrastructure that hosts the website www.foobar.com, it must be secured, serve encrypted traffic, and be monitored.

Requirements:

    I have used:
        3 firewalls
        1 SSL certificate to serve www.foobar.com over HTTPS
        3 monitoring clients (data collector for Sumologic or other monitoring services)

  contact me regarding the following issues:
   
        SPOF
        Downtime when maintenance needed (like deploying new code web server needs to be restarted)
        Cannot scale if too much incoming traffic
        on the second project:
        SPOF
        Security Issues (No firewall, no HTTPS)
        No monitoring


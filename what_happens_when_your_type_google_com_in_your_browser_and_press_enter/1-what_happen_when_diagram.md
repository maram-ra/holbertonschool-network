   +-------------------+
                  |   Client Browser  |
                  +---------+---------+
                            |
                            v
                  +-------------------+
                  |     Local DNS     |
                  +---------+---------+
                            |
                            v
                  +-------------------+
                  | Authoritative DNS |
                  +---------+---------+
                            |
                            v
                  [ Resolves www.google.com → IP address ]

                            |
                            v
                  +-------------------+
                  |     Firewall      |
                  | (allows HTTPS 443)|
                  +---------+---------+
                            |
                            v
                  +-------------------+
                  |   Load Balancer   |
                  | (distributes req) |
                  +---------+---------+
                            |
          +-----------------+-----------------+
          |                                   |
          v                                   v
+-------------------+               +-------------------+
|    Web Server     |               |    Web Server     |
|     (Nginx)       |               |     (Nginx)       |
+---------+---------+               +---------+---------+
          |                                   |
          v                                   v
+-------------------+               +-------------------+
| Application Server|               | Application Server|
| (business logic)  |               | (business logic)  |
+---------+---------+               +---------+---------+
          |                                   |
          v                                   v
                  +-------------------+
                  |     Database      |
                  |     (MySQL)       |
                  +-------------------+

Notes:
- DNS resolves domain name into server IP.
- Firewall filters traffic, only HTTPS (port 443) allowed.
- TLS/SSL ensures encrypted traffic.
- Load balancer distributes requests across multiple servers.
- Web servers serve static files and forward to app servers.
- Application servers generate dynamic pages.
- Database stores and provides data for the application.

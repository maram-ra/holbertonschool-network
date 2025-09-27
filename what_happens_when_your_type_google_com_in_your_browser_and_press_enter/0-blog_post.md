# What happens when you type `holbertonschool.com` in your browser and press Enter?

## Client and Server
The internet is based on the **client-server model**:  
- **Client:** your device or browser that requests information.  
- **Server:** the machine that stores the website and responds to requests.  

---

## DNS – The Directory
When you type `holbertonschool.com`, the browser queries the **DNS** to get the **IP Address** of the site.  
- Think of DNS like a phonebook: the name = holbertonschool.com, the number = 54.172.4.191 (example).  

---

## TCP/IP – Communication Rules
- **IP:** identifies the server’s address.  
- **TCP:** ensures that data is split into packets, delivered reliably, and reassembled correctly.  

---

## Firewall – The Gatekeeper
- Works like a guard.  
- Decides whether the request is safe or a potential threat.  
- Protects the server and network from attacks.  

---

## HTTPS/SSL – Security and Encryption
- The `https://` prefix means the connection is **encrypted**.  
- A TLS/SSL handshake happens between the browser and server.  
- Result: data is protected and cannot be intercepted by third parties.  

---

## Load Balancer
- Distributes incoming traffic across multiple servers.  
- Prevents overloading a single server.  
- Improves availability and reliability.  

---

## Web Server
- Serves **static files** like HTML, CSS, and images.  
- If the page requires dynamic content, it forwards the request to the **Application Server**.  

---

## Application Server
- Handles the website’s **business logic**.  
- Examples: validating a login, performing a search.  
- Communicates with the **database** to fetch or update data.  

---

## Database
- Stores persistent data: user accounts, articles, lessons, etc.  
- A DBMS like MySQL or PostgreSQL manages queries and transactions.  

---



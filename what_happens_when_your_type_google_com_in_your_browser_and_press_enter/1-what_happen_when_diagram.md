
```mermaid
flowchart LR
    A[Client (Browser)] -->|DNS query| B[DNS Server]
    B -->|Returns IP Address| C[Firewall / NAT]
    C --> D[Load Balancer]

    D --> E[Web Server<br/>(HTTPS - port 443)]
    E -->|TLS termination<br/>Processes request| F[Application Server<br/>(Business Logic)]
    F -->|Queries| G[(Database)]
    G -->|Returns data| F
    F -->|HTML page| E
    E --> D
    D --> A


flowchart LR
    A[User Browser] --> B[DNS Resolver]
    B --> C[IP Address of google.com]
    C --> D[Firewall]
    D --> E[Load Balancer]
    E --> F[Web Server]
    F --> G[Application Server]
    G --> H[Database]

    A -.->|HTTPS request| D
    D -.->|Traffic filtered| E
    E -.->|Distributes traffic| F
    G -.->|Queries| H

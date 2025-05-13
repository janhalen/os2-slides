

# Principle: Simple and fast to get started
_Make things simple for ME
Implementations: Monoliths for Mvps or Pocs with onle a few developers

```mermaid
flowchart TD
    subgraph Monolith["Monolithic Application (All-in-one)"]
        UI["User Interface"]
        Logic["Business Logic"]
        Data["Data Access"]
        DB["Central Database"]
    end

    UI --> Logic
    Logic --> Data
    Data --> DB

    Logic <--> UI & Data & DB
 

    Note1["All modules tightly connected<br>Changes in one part affect the whole"]
    Monolith -.-> Note1
```

```mermaid
flowchart TD
    subgraph Mono[Monolithic Application]
        UI[User Interface]
        Auth[Authentication Code]
        Sec[Security Code]
        Enc[Encryption]
        Order[Order Processing]
        Payment[Payment Handling]
        Notif[Notification Engine]
        SharedUtils(Shared Utility Functions)
        Networking["Networking Code<br/>(HTTP, Sockets, APIs)"]
        DataAccess[Data Access Code]
        DBCode["Database Code<br/>(SQL, ORM, Migrations)"]
        DB[(Columnar<br> Central Database<b)]
    end

    UI --> Networking
    Networking --> Auth
    Networking ---> Order
    Networking --> Payment
    Networking --> Notif

    Auth <--> SharedUtils
    Order <--> SharedUtils
    Payment <------> SharedUtils
    Notif <--> SharedUtils

    SharedUtils <--> Sec
    SharedUtils <--> Enc

    Auth <--> Order
    Order <--> Payment
    Payment <--> Notif
    Notif <--> Auth

    Auth --> DataAccess
    Order --> DataAccess
    Payment --> DataAccess
    Notif --> DataAccess
    DataAccess --> DBCode
    DBCode --> DB

    A((Developer A)) --> Mono


```

<br>

# ⏬

# Principle: Seperation of Concerns
_Let developers play to their strengths_

Implementation: Services

```mermaid
flowchart TD
subgraph application-services
    abstraction-layer<--> Client[Client Application] & Order[Order Service] & Payment[Payment Service] & Notif[Notification Service]
end
subgraph infrastructure-services
    APIGW[Gateway]
    Auth[Auth Service]
    DBAuth[(Auth DB)]
    DBOrder[(Order DB)]
    DBPayment[(Payment DB)]
    NotifExt[Notification Provider]
end

application-services<-->abstraction-layer<-->infrastructure-services
        Auth
        Order
        Payment
        Notif

```


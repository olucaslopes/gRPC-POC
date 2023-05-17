# gRPC-POC

```mermaid
graph LR
style A fill:#3498db,stroke:#ffffff,stroke-width:2px
style B fill:#e74c3c,stroke:#ffffff,stroke-width:2px
style F fill:#f1c40f,stroke:#ffffff,stroke-width:2px
style G fill:#2ecc71,stroke:#ffffff,stroke-width:2px

A[Servidor] -->|Implementa o serviço| B((SayHello))
F[Cliente] -->|Cria o stub| G((gRPC Stub))
G -->|Faz a chamada do método| B
B -->|Envia o HelloRequest| G
G -->|Recebe o HelloResponse| F

```

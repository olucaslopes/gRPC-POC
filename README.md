# gRPC-POC

```mermaid
graph LR
style A fill:#3498db,stroke:#ffffff,stroke-width:2px
style B fill:#e74c3c,stroke:#ffffff,stroke-width:2px
style F fill:#f1c40f,stroke:#ffffff,stroke-width:2px
style G fill:#2ecc71,stroke:#ffffff,stroke-width:2px

A[Servidor] -->|1. Implementa o serviço| B((SayHello))
F[Cliente] -->|6. Cria o stub| G((gRPC Stub))
G -->|7. Faz a chamada do método| B
B -->|8. Envia o HelloRequest| G
G -->|9. Recebe o HelloResponse| F

```

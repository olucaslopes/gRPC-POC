# gRPC-POC

Prova de conceito (PoC) do uso do gRPC (Google RPC) para a comunicação eficiente e escalável entre sistemas distribuídos. O gRPC é uma tecnologia de código aberto amplamente adotada que oferece alta performance, streaming bidirecional e suporte a várias linguagens de programação.

Principais recursos e destaques:

- Demonstração prática do uso do gRPC para comunicação cliente-servidor em sistemas distribuídos.
- Implementação de uma aplicação simples, com exemplos de chamadas de função e streaming bidirecional.
- Uso do Protocol Buffers (protobuf) para definir a estrutura dos dados e facilitar a interoperabilidade entre diferentes plataformas.
- Ênfase na performance e eficiência do gRPC, aproveitando as vantagens do protocolo HTTP/2.

## Diagrama da Prova de Conceito

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

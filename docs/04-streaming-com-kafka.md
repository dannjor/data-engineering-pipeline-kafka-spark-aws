# 4. Streaming de Dados com Apache Kafka

## Visão Geral
O Apache Kafka foi utilizado como plataforma central de streaming, permitindo a ingestão contínua de dados e o desacoplamento entre os sistemas produtores e consumidores.

Essa abordagem garante escalabilidade, resiliência e flexibilidade na arquitetura da pipeline.

---

## Papel do Kafka na Arquitetura
No projeto, o Kafka atua como:
- Camada intermediária entre a fonte de dados e o processamento
- Mecanismo de buffer para grandes volumes de eventos
- Plataforma de streaming distribuída

O uso do Kafka evita dependência direta entre os sistemas, permitindo evolução independente dos componentes.

---

## Kafka Connect
O Kafka Connect foi utilizado para integrar sistemas externos ao Kafka sem necessidade de desenvolvimento customizado.

Principais usos:
- **Source Connector:** ingestão de dados a partir do PostgreSQL
- **Sink Connector:** envio de dados para o Data Lake (Amazon S3)

Essa abordagem simplifica a ingestão e reduz complexidade operacional.

---

## Tópicos e Organização
Os dados são organizados em tópicos, permitindo:
- Paralelismo no consumo
- Escalabilidade horizontal
- Isolamento lógico dos fluxos de dados

Cada tópico representa um fluxo específico de informações.

---

## Benefícios do Streaming
- Ingestão contínua de dados
- Baixa latência
- Alta tolerância a falhas
- Escalabilidade
- Suporte a múltiplos consumidores

---

## Representação Visual

![Pipeline Kafka](../images/kafka_pipeline.png)

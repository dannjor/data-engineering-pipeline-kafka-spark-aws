# 2. Arquitetura da Solução

## Visão Geral
A arquitetura do projeto foi desenhada para suportar ingestão contínua de dados, processamento distribuído e armazenamento escalável, utilizando ferramentas consolidadas de Engenharia de Dados.

A solução adota uma abordagem desacoplada, onde cada componente possui uma responsabilidade bem definida, facilitando manutenção, escalabilidade e evolução da pipeline.

---

## Componentes da Arquitetura

### Banco de Dados Relacional (PostgreSQL)
Atua como fonte de dados transacionais, armazenando informações estruturadas que serão ingeridas pela pipeline.

### Apache Kafka
Responsável pela camada de streaming, permitindo ingestão contínua e desacoplamento entre produtores e consumidores de dados.

### Kafka Connect
Utilizado para:
- Extrair dados do PostgreSQL (Source Connector)
- Disponibilizar dados para consumo no Data Lake (Sink Connector)

### Apache Spark
Responsável pelo processamento e transformação dos dados:
- Leitura dos dados a partir do Kafka
- Aplicação de regras de limpeza e padronização
- Organização dos dados nas camadas Bronze, Silver e Gold

### Data Lake (Amazon S3)
Armazena os dados processados, garantindo escalabilidade, durabilidade e baixo custo de armazenamento.

### Docker
A infraestrutura foi executada em ambiente containerizado, permitindo padronização, reprodutibilidade e facilidade de execução.

---

## Fluxo de Dados
O fluxo de dados da arquitetura ocorre da seguinte forma:

1. Dados transacionais são gerados no PostgreSQL
2. Kafka Connect realiza a ingestão contínua desses dados
3. Apache Kafka atua como broker de mensagens
4. Apache Spark consome os dados do Kafka
5. Os dados são transformados e organizados nas camadas Bronze, Silver e Gold
6. Dados finais são armazenados no Amazon S3

---

## Diagrama da Arquitetura

![Arquitetura da Solução](../images/arquitetura_solucao.png)

---

## Benefícios da Arquitetura
- Arquitetura desacoplada e escalável
- Processamento distribuído
- Suporte a streaming e batch
- Organização clara dos dados
- Facilidade de manutenção e evolução

Essa arquitetura representa um cenário comum em ambientes modernos de Engenharia de Dados, aplicando boas práticas de mercado.

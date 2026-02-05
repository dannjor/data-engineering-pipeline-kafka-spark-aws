# 6. Implantação e Execução do Projeto

## Visão Geral
A solução foi implantada em ambiente containerizado utilizando **Docker** e **Docker Compose**, garantindo padronização, facilidade de execução e reprodutibilidade do ambiente.

Essa abordagem permite simular um cenário próximo ao ambiente produtivo, facilitando testes e validações da pipeline.

---

## Ambiente de Execução
O ambiente é composto por múltiplos containers, incluindo:
- Apache Kafka
- Zookeeper
- Kafka Connect
- Apache Spark
- PostgreSQL

Todos os serviços são orquestrados via Docker Compose.

---

## Estrutura de Containers
Cada componente da arquitetura possui seu próprio container, permitindo:
- Isolamento de responsabilidades
- Facilidade de manutenção
- Escalabilidade individual
- Inicialização controlada dos serviços

---

## Execução do Projeto
Para executar o projeto localmente, siga os passos:

1. Clone o repositório:

git clone https://github.com/dannjor/data-engineering-pipeline-kafka-spark-aws.git

2. Acesse o diretório do projeto:

cd data-engineering-pipeline-kafka-spark-aws

3. Suba os containers:

docker-compose up -d

## Observações Importantes

- O tempo de inicialização pode variar conforme o ambiente
- Certifique-se de que as portas necessárias estejam disponíveis
- O Docker e Docker Compose devem estar previamente instalados

## Benefícios da Containerização

- Padronização do ambiente
- Facilidade de reprodução
- Redução de dependências locais
- Melhor controle da infraestrutura


# 5. Processamento de Dados com Apache Spark

## Visão Geral
O Apache Spark foi utilizado como motor de processamento distribuído, sendo responsável pela transformação, enriquecimento e organização dos dados ingeridos a partir do Apache Kafka.

A escolha do Spark se deve à sua capacidade de processar grandes volumes de dados de forma eficiente e escalável.

---

## Leitura de Dados
O Spark consome os dados diretamente dos tópicos do Kafka, utilizando integração nativa para streaming.

Principais características:
- Processamento distribuído
- Suporte a dados em tempo quase real
- Escalabilidade horizontal

---

## Transformações Aplicadas
Durante o processamento, são aplicadas transformações para garantir qualidade e padronização dos dados, incluindo:
- Conversão de tipos de dados
- Tratamento de valores nulos
- Padronização de campos
- Aplicação de regras de negócio básicas

Essas transformações preparam os dados para uso analítico.

---

## Organização em Camadas
O processamento no Spark é responsável por distribuir os dados nas camadas:
- **Bronze:** persistência dos dados brutos
- **Silver:** dados tratados e padronizados
- **Gold:** dados consolidados e prontos para consumo

Essa separação facilita governança, auditoria e reprocessamento.

---

## Spark SQL e DataFrames
O projeto utiliza:
- **DataFrames** para manipulação eficiente dos dados
- **Spark SQL** para consultas e transformações declarativas

Essa abordagem combina performance e legibilidade do código.

---

## Benefícios do Uso do Spark
- Alto desempenho
- Processamento distribuído
- Integração nativa com Kafka e S3
- Facilidade para aplicar regras de negócio
- Escalabilidade para grandes volumes de dados

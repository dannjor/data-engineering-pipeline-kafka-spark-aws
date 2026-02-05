# 1. Contexto do Desafio

## Contexto
Este projeto foi desenvolvido como parte de um desafio prático de Engenharia de Dados, com o objetivo de simular um cenário real de ingestão, processamento e disponibilização de dados em larga escala.

O desafio propõe a construção de uma pipeline capaz de integrar dados transacionais armazenados em banco relacional, processá-los de forma distribuída e armazená-los em um Data Lake, utilizando ferramentas modernas amplamente adotadas pelo mercado.

O cenário considera:
- Crescimento contínuo do volume de dados
- Necessidade de processamento eficiente
- Separação clara entre dados brutos, tratados e analíticos
- Uso de tecnologias escaláveis e desacopladas

---

## Problema Proposto
Empresas que lidam com grandes volumes de dados enfrentam desafios relacionados a:
- Ingestão contínua de dados
- Processamento em tempo quase real
- Manutenção da qualidade dos dados
- Escalabilidade da infraestrutura
- Integração entre múltiplas tecnologias

O desafio consiste em projetar e implementar uma solução que atenda a esses requisitos, utilizando uma arquitetura moderna de Engenharia de Dados.

---

## Objetivo do Desafio
O objetivo principal é construir uma **pipeline de dados ponta a ponta**, contemplando ingestão, processamento e armazenamento, com foco nas ferramentas e na arquitetura adotada.

Objetivos específicos:
- Ingerir dados de um banco relacional utilizando Apache Kafka
- Processar dados com Apache Spark
- Organizar os dados em camadas Bronze, Silver e Gold
- Armazenar os dados em um Data Lake no Amazon S3
- Executar a solução em ambiente containerizado com Docker
- Demonstrar integração entre tecnologias de streaming e batch

Este projeto tem como foco evidenciar a aplicação prática de conceitos e ferramentas de Engenharia de Dados em um cenário próximo ao ambiente produtivo.

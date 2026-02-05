# 3. Pipeline de Dados – Bronze, Silver e Gold

## Visão Geral
A organização dos dados em camadas **Bronze, Silver e Gold** segue uma abordagem amplamente adotada em arquiteturas modernas de Data Lake, permitindo melhor governança, qualidade e reutilização dos dados.

Cada camada possui um propósito específico dentro da pipeline.

---

## Camada Bronze
A camada Bronze armazena os dados brutos, exatamente como são ingeridos das fontes de origem.

Características:
- Dados sem transformações
- Estrutura próxima à origem
- Possível presença de inconsistências e duplicidades
- Base para auditoria e reprocessamentos

No projeto, os dados ingeridos do Kafka são inicialmente persistidos nesta camada.

---

## Camada Silver
A camada Silver contém os dados tratados e padronizados.

Principais transformações aplicadas:
- Limpeza de dados inválidos
- Padronização de tipos e formatos
- Tratamento de valores nulos
- Remoção de duplicidades

Essa camada representa dados confiáveis para uso analítico intermediário.

---

## Camada Gold
A camada Gold disponibiliza os dados prontos para consumo analítico.

Características:
- Dados agregados e consolidados
- Estrutura orientada a análises e relatórios
- Preparada para consumo por ferramentas de BI ou análises avançadas

Essa camada entrega valor direto ao negócio.

---

## Benefícios da Arquitetura em Camadas
- Separação clara de responsabilidades
- Facilidade de manutenção
- Possibilidade de reprocessamento
- Governança e rastreabilidade
- Escalabilidade da solução

---

## Representação Visual

![Bronze Silver Gold](../images/bronze_silver_gold.png)

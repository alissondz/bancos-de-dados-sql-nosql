# Bancos de Dados Relacionais (SQL) e Não Relacionais (NoSQL)

Este repositório contém uma documentação detalhada sobre Bancos de Dados Relacionais e Não Relacionais, abrangendo conceitos, definições e insights úteis para engenheiros de dados.

## Índice

- [Bancos de Dados Relacionais (SQL) e Não Relacionais (NoSQL)](#bancos-de-dados-relacionais-sql-e-não-relacionais-nosql)
  - [Índice](#índice)
  - [Bancos de Dados Relacionais (SQL)](#bancos-de-dados-relacionais-sql)
    - [Conceitos](#conceitos)
    - [Características](#características)
    - [SQL Básico](#sql-básico)
  - [Bancos de Dados Não Relacionais (NoSQL)](#bancos-de-dados-não-relacionais-nosql)
    - [Conceitos](#conceitos-1)
    - [Características](#características-1)
    - [NoSQL Básico](#nosql-básico)
  - [Comparação Entre SQL e NoSQL](#comparação-entre-sql-e-nosql)
  - [Casos de Uso Comuns](#casos-de-uso-comuns)
  - [Referências](#referências)

## Bancos de Dados Relacionais (SQL)

### Conceitos

- **Definição**: Bancos de dados que utilizam um modelo relacional, baseado em tabelas com linhas e colunas. Utilizam SQL (Structured Query Language) para manipulação e consulta de dados.
- **Exemplos**: MySQL, PostgreSQL, Oracle, Microsoft SQL Server.

### Características

- **Estrutura**: Dados são armazenados em tabelas com um esquema fixo.
- **Integridade Referencial**: Suporte a chaves primárias e estrangeiras para garantir a integridade dos dados.
- **Transações**: Suporte a transações ACID (Atomicidade, Consistência, Isolamento, Durabilidade).

### SQL Básico

- **Seleção de Dados**: `SELECT * FROM tabela;`
- **Inserção de Dados**: `INSERT INTO tabela (coluna1, coluna2) VALUES (valor1, valor2);`
- **Atualização de Dados**: `UPDATE tabela SET coluna1 = valor1 WHERE condição;`
- **Exclusão de Dados**: `DELETE FROM tabela WHERE condição;`

## Bancos de Dados Não Relacionais (NoSQL)

### Conceitos

- **Definição**: Bancos de dados que não utilizam o modelo relacional tradicional. Podem utilizar modelos baseados em documentos, chave-valor, colunas ou grafos.
- **Exemplos**: MongoDB (documentos), Redis (chave-valor), Cassandra (colunas), Neo4j (grafos).

### Características

- **Estrutura**: Flexível, com esquemas dinâmicos. Os dados podem ser armazenados em formatos variados como JSON ou BSON.
- **Escalabilidade**: Facilita a escalabilidade horizontal, distribuindo dados em múltiplos servidores.
- **Consistência**: Pode adotar modelos de consistência eventual em vez de ACID.

### NoSQL Básico

- **Consulta de Dados**: `db.collection.find({});` (MongoDB)
- **Inserção de Dados**: `db.collection.insertOne({ campo1: valor1 });` (MongoDB)
- **Atualização de Dados**: `db.collection.updateOne({ campo: valor }, { $set: { campo: novo_valor } });` (MongoDB)
- **Exclusão de Dados**: `db.collection.deleteOne({ campo: valor });` (MongoDB)

## Comparação Entre SQL e NoSQL

| Característica        | SQL                             | NoSQL                        |
|-----------------------|---------------------------------|------------------------------|
| **Modelo de Dados**   | Relacional (tabelas)             | Variado (documentos, chave-valor, colunas, grafos) |
| **Esquema**           | Fixo                             | Flexível                     |
| **Escalabilidade**    | Vertical (aumentar hardware)     | Horizontal (aumentar servidores) |
| **Transações**        | ACID                             | Eventual ou ACID em alguns casos |

## Casos de Uso Comuns

- **SQL**: Sistemas de gestão de transações financeiras, ERP, sistemas de CRM.
- **NoSQL**: Aplicações web com grandes volumes de dados, redes sociais, sistemas de recomendação.

## Referências

- [Documentação do MySQL](https://dev.mysql.com/doc/)
- [Documentação do MongoDB](https://docs.mongodb.com/)
- [Comparação entre SQL e NoSQL](https://www.mongodb.com/nosql-explained)


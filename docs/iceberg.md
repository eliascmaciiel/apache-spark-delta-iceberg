# Apache Iceberg

Apache Iceberg é um formato de tabela aberto para Data Lakes, com foco em confiabilidade e performance.

## Conceitos principais
- tabela aberta independente de engine;
- catálogo para descoberta de tabelas;
- snapshots para histórico consistente;
- DML (`INSERT`, `UPDATE`, `DELETE`) com Spark SQL.

## Catálogo
No projeto usamos catálogo Hadoop local apontando para `warehouse/iceberg`.

## Exemplos no notebook
No notebook `02_apache_iceberg.ipynb`, são mostrados:
1. sessão Spark com pacote JVM do Iceberg;
2. criação de namespace e tabela;
3. `INSERT`, `UPDATE`, `DELETE`;
4. evidências via `SELECT`.

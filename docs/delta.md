# Delta Lake

Delta Lake é um formato de tabela que adiciona transações ACID sobre arquivos em Data Lake.

## Características
- ACID;
- schema enforcement;
- time travel;
- operações DML (`INSERT`, `UPDATE`, `DELETE`, `MERGE`).

## ACID e Versionamento
Cada operação gera uma nova versão no log `_delta_log`, permitindo auditoria e reprodutibilidade.

## Exemplos no notebook
No notebook `01_delta_lake.ipynb`, o projeto demonstra:
1. criação do banco e tabela Delta;
2. carga inicial dos dados;
3. `INSERT` de nova venda;
4. `UPDATE` de desconto;
5. `DELETE` de um item;
6. consultas de evidência após cada etapa.

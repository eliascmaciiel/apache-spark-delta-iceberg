# Apache Spark com Delta Lake e Apache Iceberg

Projeto acadêmico de Arquitetura de Dados com foco em um ambiente único **PySpark + JupyterLab**, gerenciado exclusivamente com **UV**.

## 1) Pré-requisitos (Windows)
- Git
- Python **3.11** (recomendado para compatibilidade com Spark/Delta/Iceberg)
- Java JDK **17** (compatível com Spark 3.5)
- UV
- VS Code (opcional) e/ou JupyterLab

## 2) Clonar o projeto
```bash
git clone https://github.com/eliascmaciiel/apache-spark-delta-iceberg.git
cd apache-spark-delta-iceberg
```

## 3) Criar ambiente virtual com UV
```bash
uv venv
```

## 4) Ativar ambiente no Windows
```powershell
.venv\Scripts\activate
```

## 5) Instalar dependências
```bash
uv sync
```

## 6) Executar JupyterLab
```bash
jupyter lab
```

## 7) Ordem sugerida dos notebooks
1. `notebooks/03_cenario_modelo_dados.ipynb`
2. `notebooks/01_delta_lake.ipynb`
3. `notebooks/02_apache_iceberg.ipynb`

## 8) Executar documentação com MkDocs
```bash
mkdocs serve
```

## 9) Build da documentação
```bash
mkdocs build
```

## 10) Publicar no GitHub Pages
```bash
mkdocs gh-deploy
```

Link esperado:
- https://eliascmaciiel.github.io/apache-spark-delta-iceberg/

## 11) Troubleshooting
### Erro de Java
- Verifique `java -version` (JDK 17).
- Configure `JAVA_HOME`.

### Erro de pacote Delta
- Confirme `delta-spark` instalado via `uv sync`.
- Reinicie o kernel do notebook.

### Erro de pacote Iceberg
- O notebook configura `spark.jars.packages` com runtime do Iceberg para Spark 3.5.
- Verifique acesso à internet para baixar jars no primeiro uso.

### Erro ao abrir Jupyter
- Rode `uv sync` novamente.
- Confira se o ambiente `.venv` está ativado.

### Erro no `mkdocs gh-deploy`
- Configure autenticação do GitHub no seu ambiente.
- Garanta permissão de escrita no repositório.


> Dica de compatibilidade: se houver qualquer instabilidade com Python 3.12 no seu ambiente, mantenha Python 3.11 como padrão.

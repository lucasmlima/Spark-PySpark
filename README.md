# 🚀 Apache Spark & PySpark — Fundamentals to Practical Pipelines

Repositório estruturado para demonstrar o domínio prático e conceitual do ecossistema **Apache Spark** utilizando **PySpark**. O projeto abrange desde a inicialização de sessões distribuídas e tipagem de esquemas até transformações complexas, agregações analíticas e resolução de desafios práticos aplicados à **Engenharia de Dados**.

---

## 📌 Visão Geral & Objetivos

- **Processamento Distribuído:** Compreensão do ciclo de vida de aplicações Spark, lazy evaluation, planos de execução e otimização de transformações.
- **Manipulação de Dados em Larga Escala:** Uso intensivo da API `pyspark.sql` (DataFrames, Funções Nativas, Schema Enforcement).
- **Boas Práticas de Engenharia:** Estruturação modular em Jupyter Notebooks, código limpo, controle de tipos e pipeline analítico final.

---

## 🛠️ Tecnologias & Ferramentas

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

- **Linguagem:** Python
- **Engine de Processamento:** Apache Spark / PySpark
- **Módulos Core:** `pyspark.sql.functions`, `pyspark.sql.types`

---

## 📂 Estrutura dos Módulos

O repositório está organizado em uma trilha progressiva de aprendizado e aplicação prática:

| # | Notebook | Conceitos & Operações Cobertas |
|---|:---|:---|
| **01** | `1.CriarSparkSession.ipynb` | Inicialização da `SparkSession`, configuração do app, gerenciamento de contexto (`SparkContext`) e alocação de recursos. |
| **02** | `2.CriarDataFrame.ipynb` | Criação de DataFrames a partir de coleções/listas, inferência vs. definição explícita de `StructType` e `StructField`. |
| **03** | `3.AlterarNomeColuna.ipynb` | Padronização e renomeação de colunas com `.withColumnRenamed()`, técnicas de saneamento de metadados. |
| **04** | `4.RetornarTipoDados.ipynb` | Inspeção de esquemas (`.printSchema()`, `.dtypes`), validação de integridade e tipos de dados em lote. |
| **05** | `5.AlterarTipoColuna.ipynb` | Type casting com `.cast()`, conversão segura de tipos numéricos, strings e datas com tratamento de nulos. |
| **06** | `6.SelecionarColunas.ipynb` | Projeções de colunas com `.select()`, `.col()`, expressões literais (`lit`) e otimização de largura de DataFrame. |
| **07** | `7.LeituraDeCsv.ipynb` | Ingestão de arquivos CSV (`spark.read.csv`), manipulação de delimitadores, `header`, inferência de schema e tratamento de corrupt records. |
| **08** | `8.FiltrarDataframe.ipynb` | Filtragem de dados com `.filter()` e `.where()`, operadores lógicos combinados (`&`, `|`, `~`) e expressões SQL-like. |
| **09** | `9.AgrupamentoAgragacao.ipynb` | Agregações com `.groupBy()`, `.agg()`, funções estatísticas (`count`, `sum`, `avg`, `min`, `max`) e cálculo de métricas de negócio. |
| **10** | `10.DesafioPratico.ipynb` | **Projeto Integrador / Desafio Prático:** Pipeline ponta a ponta envolvendo ingestão, limpeza, enriquecimento, agregações e geração de dataset analítico final. |

---

## 🧠 Principais Habilidades Demonstradas

- **Schema Enforcement:** Definição explícita de esquemas com tipos estritos (`IntegerType`, `StringType`, `DoubleType`, `TimestampType`) para garantir robustez e performance na ingestão.
- **Otimização de Consultas:** Escrita de transformações idiomáticas que aproveitam o Catalyst Optimizer e o Tungsten Execution Engine do Spark.
- **Limpeza & Normalização de Dados:** Tratamento de valores nulos, conversão de formatos inconsistentes e padronização de nomenclatura (*snake_case*).
- **Agregações Analíticas:** Construção de queries agregadas de alto desempenho para geração de relatórios e métricas de negócios.

---

## 💻 Como Executar Localmente

### Pré-requisitos
- Python 3.8+
- Java JDK 8 ou 11 (necessário para o core do Apache Spark)
- Jupyter Notebook / VS Code com extensão Python/Jupyter

### Passo a Passo

1. **Clone o repositório:**
```bash
git clone [https://github.com/lucasmlima/Spark-PySpark.git](https://github.com/lucasmlima/Spark-PySpark.git)
cd Spark-PySpark

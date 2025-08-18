# Pipeline no Databricks Comercio Exterior - Exportação e Importação (2024-2025)

## 📝 Descrição do Projeto

Este projeto consiste em um **pipeline ETL** desenvolvido no **Databricks**, com objetivo de processar e transformar dados de **exportação e importação** do Brasil referentes aos anos de 2024 e 2025, tornando-os prontos para análise no **Power BI**.

O fluxo segue a arquitetura de Medallion **Bronze → Silver → Gold**, garantindo organização, qualidade e performance.

---

## 🔹 Tecnologias Utilizadas

* **Databricks (PySpark)** – Processamento de dados em larga escala.
* **Delta Lake** – Armazenamento otimizado para ETL e análises.
* **Power BI** – Visualização e criação de dashboards interativos.
* **Git/GitHub** – Controle de versão do projeto.

---

## 🔹 Pipeline ETL

1. **Bronze (Raw)**

   * Importação dos dados originais de exportação e importação.
   * Armazenamento em Delta sem alterações.

2. **Silver (Transformada)**

   * Limpeza e padronização de dados (nulos, tipos, nomes).
   * Criação de dimensões:

     * `tb_Produto`
     * `tb_Pais`
     * `tb_Tempo`
     * `tb_Via`

3. **Gold (Agregada)**

   * Criação de tabelas fato prontas para análises:

     * `tb_Exportacao_final`
     * `tb_Importacao_final`
   * Métricas:

     * Valor FOB, Frete, Seguro, Peso líquido, Quantidade estatística.

---

## 📊 Dashboards e Análises 
(Será Implementado nos Próximos dias)

* Evolução de exportação e importação ao longo do tempo.
* Ranking de países parceiros e categorias de produtos.
* Visualizações interativas em mapas e gráficos comparativos.
* Análise de participação por via de transporte.
* Balança comercial (superávit/déficit).

---

## ⚡ Boas Práticas Implementadas

* Organização em **camadas Bronze → Silver → Gold**.
* **Z-Ordering e particionamento** para otimização no Power BI.
* Estrutura de **modelagem dimensional** (Fato + Dimensões) para performance.
* **Documentação e versionamento** de notebooks e transformações.

---


Quer que eu faça essa versão?


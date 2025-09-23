# Análise de Dados do E-commerce Olist

## 📄 Visão Geral do Projeto

Este projeto consiste em uma Análise Exploratória de Dados (EDA) completa sobre um conjunto de dados públicos de e-commerce da **Olist**, a maior loja de departamentos do Brasil. O objetivo é transformar dados brutos em insights acionáveis, explorando padrões de vendas, comportamento do cliente e desempenho logístico para identificar oportunidades de melhoria e estratégias de negócio.

Este repositório serve como um projeto de portfólio para demonstrar habilidades em limpeza, pré-processamento, engenharia de atributos e visualização de dados utilizando Python e suas principais bibliotecas.

## 🎯 Objetivos e Perguntas de Negócio

A análise foi guiada para responder às seguintes perguntas-chave:

1.  **Vendas:** Qual é a tendência de vendas ao longo do tempo? Existem picos de sazonalidade?
2.  **Produtos:** Quais são as categorias de produtos mais vendidas? E as menos relevantes?
3.  **Clientes:** Qual o nível de satisfação dos clientes? Quais fatores mais influenciam as avaliações?
4.  **Logística:** Como o tempo de entrega impacta a satisfação do cliente? Atrasos são um problema recorrente?
5.  **Geografia:** Qual a distribuição geográfica dos clientes e vendedores? Existem mercados regionais a serem explorados?

## 📊 Metodologia

O projeto foi estruturado em um fluxo de trabalho claro e sequencial, seguindo as melhores práticas de análise de dados:

1.  **Coleta e Carga dos Dados:** Carregamento dos 9 arquivos `.csv` que compõem o dataset.
2.  **Consolidação (Merge):** União das diferentes tabelas em um único DataFrame consolidado para facilitar a análise.
3.  **Limpeza e Pré-processamento:**
    -   Conversão de tipos de dados (especialmente para datas).
    -   Tratamento de valores ausentes (`NaN`) com estratégias adequadas para cada coluna.
    -   Remoção de dados duplicados.
4.  **Engenharia de Atributos:** Criação de novas variáveis para enriquecer a análise, como:
    -   `delivery_time_days`: Tempo total de entrega em dias.
    -   `delivery_delta_days`: Diferença entre a entrega estimada e a real.
    -   `is_late`: Indicador binário de atraso na entrega.
5.  **Análise Exploratória de Dados (EDA):** Geração de visualizações (gráficos e mapas de calor) para identificar tendências, correlações e outliers, respondendo às perguntas de negócio.

## ✨ Principais Insights Encontrados

-   **Tendência de Vendas:** O volume de vendas apresentou um crescimento significativo ao longo de 2017, atingindo um pico no final do ano, possivelmente impulsionado por datas comemorativas como a Black Friday.
-   **Satisfação do Cliente:** A maioria dos clientes avalia os pedidos com a nota máxima (5 estrelas). No entanto, há um volume considerável de avaliações de 1 estrela, indicando uma experiência polarizada.
-   **Impacto da Logística:** Existe uma forte correlação negativa entre o tempo de entrega e a nota de avaliação. Pedidos que chegam antes do prazo estimado recebem, em média, notas muito mais altas. Atrasos são o principal motor de insatisfação.
-   **Categorias Populares:** Categorias como `Cama, Mesa e Banho`, `Beleza e Saúde` e `Esporte e Lazer` dominam o volume de vendas da plataforma.

## 🛠️ Tecnologias Utilizadas

-   **Linguagem:** Python 3
-   **Bibliotecas:**
    -   **Pandas:** Para manipulação e análise dos dados.
    -   **NumPy:** Para operações numéricas.
    -   **Matplotlib & Seaborn:** Para visualização de dados e criação de gráficos.
    -   **Google Colab:** Como ambiente de desenvolvimento interativo.

## 🚀 Como Executar o Projeto

Para replicar esta análise, siga os passos abaixo:

1.  **Clone este repositório:**
    ```bash
    git clone https://github.com/Hoalys78/analise_olist.git
    cd analise_olist
    ```

2.  **Crie um ambiente virtual (recomendado):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows: venv\Scripts\activate
    ```

3.  **Instale as dependências:**
    ```bash
    pip install pandas numpy matplotlib seaborn jupyter
    ```

4.  **Estrutura de Diretórios:** Certifique-se de que os arquivos `.csv` da Olist estejam dentro de uma pasta chamada `data` na raiz do projeto:
    ```
    projeto-olist/
    ├── data/
    │   ├── olist_customers_dataset.csv
    │   └── ... (outros 8 arquivos .csv)
    ├── analise_olist.ipynb
    └── README.md
    ```

## 👨‍💻 Autor

-   **[Hoalys Anjos]**
-   **LinkedIn:** https://www.linkedin.com/in/hoalysanjos-analista/
-   **GitHub:** https://github.com/Hoalys78

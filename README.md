# Análise de Desempenho: Alura Store 🏪

Este projeto foi desenvolvido como parte do Desafio Alura (Python para Data Science). O foco é aplicar fundamentos da linguagem Python para realizar uma análise de desempenho em 4 lojas de e-commerce e fornecer uma recomendação estratégica baseada em dados.

## 🎯 O Contexto do Negócio

O Sr. João, proprietário da rede de e-commerce "Alura Store", enfrenta uma decisão estratégica: ele precisa levantar capital para um novo empreendimento e, para isso, decidiu vender uma de suas 4 lojas.

O objetivo desta análise é ir além dos números superficiais (como faturamento bruto) e identificar qual das lojas possui o **menor potencial estratégico** a longo prazo, fundamentando a recomendação de qual unidade deve ser vendida.

## 1. O Propósito da Análise

Este projeto foi desenvolvido para o **Challenge de Data Science da Alura**, com o objetivo de realizar uma análise de ponta a ponta sobre o desempenho de 4 lojas da rede "Alura Store".

O foco principal é utilizar **fundamentos nativos da linguagem Python** (`def`, `for`, `if`, `else`) para extrair métricas e embasar uma decisão estratégica: identificar a loja mais problemática (alto risco) e a mais saudável (potencial de crescimento), para recomendar qual unidade poderia ser vendida.

A análise revelou que a **Loja 1** é a de maior faturamento, mas também a mais problemática (pior avaliação, frete mais caro). A **Loja 4**, por outro lado, tem o menor faturamento, mas uma operação mais saudável (frete baixo, avaliações positivas).

## 2. Estrutura do Projeto e Organização

A análise completa está contida em um único Jupyter Notebook (`.ipynb`). A metodologia segue 6 passos principais:

1.  **Carregamento dos Dados:** Os 4 arquivos CSV (um para cada loja) são carregados do GitHub em DataFrames do Pandas.
2.  **Organização dos Dados:** Os DataFrames são agrupados em um dicionário (`dfs_lojas`) para facilitar a iteração.
3.  **Conversão para "Modo Raiz":** Cada DataFrame é convertido para uma lista de dicionários (`dados_por_loja`) usando `.to_dict('records')`.
4.  **Funções de Análise:** Funções reutilizáveis em Python puro são usadas para calcular Faturamento, Vendas por Categoria, Média de Avaliação, Ranking de Produtos e Média de Frete.
5.  **Armazenamento de Resultados:** Os resultados são salvos em dicionários (ex: `resultados_faturamento`) para fácil acesso.
6.  **Visualização:** Os resultados são plotados com `matplotlib` para gerar os gráficos da análise.

## 3. Exemplos de Gráficos e Insights Obtidos

A análise gerou diversas visualizações para identificar padrões. Os principais insights vêm do cruzamento de métricas:

* **Gráfico de Barras (Faturamento):** Demonstra visualmente a liderança de faturamento da **Loja 1 (R$ 1.53M)** e o menor volume da **Loja 4 (R$ 1.38M)**.
* **Gráfico de Dispersão (Faturamento vs. Avaliação):** Este é o *insight* principal. A **Loja 1** (que mais fatura) tem a **pior avaliação (3.98 estrelas)**. As lojas 2 e 3 estão melhores posicionadas (faturamento alto, avaliação boa).
* **Gráfico de Pizza (Categorias):** Mostra que "Móveis" e "Eletrônicos" dominam as vendas em todas as lojas, compondo a maior parte do faturamento.
* **Análise de Frete:** Um *insight* adicional confirma o problema da Loja 1: ela possui o **frete médio mais caro (R$ 34.69)**, enquanto a Loja 4 possui o **mais barato (R$ 31.28)**, reforçando a ideia de uma operação mais eficiente.

## 4. Instruções para Executar o Notebook

Os dados deste projeto são carregados diretamente de URLs públicas, não sendo necessário baixar arquivos CSV.

## 🚀 Recomendação Final

A recomendação estratégica, baseada nas evidências, foi **vender a Loja 1**.

Embora tenha o maior faturamento, ela representa um risco significativo devido à alta insatisfação dos clientes e à logística cara e limitada. A **Loja 4**, por outro lado, é o ativo mais estratégico da rede, com a melhor logística, maior alcance geográfico e maior potencial de crescimento futuro.

## 🖥️ Instruções para Execução

Para replicar esta análise, siga os passos abaixo:

1.  Clone este repositório para sua máquina local (ex: `git clone ...`).
2.  Abra o notebook `AluraStoreBrasil.ipynb` em um ambiente compatível com Jupyter (como Jupyter Lab, VS Code ou Google Colab).
3.  **Recomendação (Google Colab):**
      * Faça o upload do notebook para o Google Colab.
      * No menu, acesse "Ambiente de execução".
      * Clique em **"Executar tudo"**.
4.  O notebook processará os dados, executará todas as funções de análise nativas, gerará os 3 gráficos e exibirá o relatório final detalhado na última célula.

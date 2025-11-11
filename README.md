# Análise Estratégica: Decisão de Venda da Alura Store 🏪
Este projeto foi desenvolvido como parte do Desafio Alura (Python para Data Science). O foco é aplicar fundamentos da linguagem Python para realizar uma análise de desempenho em 4 lojas de e-commerce e fornecer uma recomendação estratégica baseada em dados.

🎯 O Contexto do Negócio
O Sr. João, proprietário da rede de e-commerce "Alura Store", enfrenta uma decisão estratégica: ele precisa levantar capital para um novo empreendimento e, para isso, decidiu vender uma de suas 4 lojas.

O objetivo desta análise é ir além dos números superficiais (como faturamento bruto) e identificar qual das lojas possui o menor potencial estratégico a longo prazo, fundamentando a recomendação de qual unidade deve ser vendida.

⚙️ Metodologia e Estrutura do Repositório
Toda a análise está consolidada em um único Jupyter Notebook, permitindo total reprodutibilidade. A ênfase foi usar o Python "raiz" (estruturas nativas) para construir a lógica de análise.

README.md: (Este arquivo) Uma visão geral do projeto, da metodologia e das conclusões.

AluraStoreBrasil.ipynb: O notebook Jupyter central que documenta todo o processo:

Extração de Dados: Carregamento e manipulação inicial dos dados utilizando a biblioteca Pandas.

Cálculo de Métricas: Desenvolvimento de 5 métricas de desempenho-chave usando funções Python puras (def), loops (for) e lógica condicional (if).

Visualização de Dados: Geração de 3 tipos de gráficos (Barras, Pizza e Dispersão) com a biblioteca matplotlib para ilustrar os achados.

Relatório Final: Conclusão da análise apresentada em Markdown ao final do notebook.

/graficos (Opcional): Diretório que pode ser usado para armazenar as visualizações de dados exportadas.

💡 Principais Descobertas e a Reviravolta
A análise revelou que a primeira impressão nem sempre é a correta.

A Análise Superficial
À primeira vista, a Loja 4 parecia a candidata ideal para a venda, pois apresentava o pior faturamento entre as quatro.

A Descoberta Geográfica: O Ponto de Virada
O insight decisivo surgiu da análise de geolocalização, cruzando os dados das colunas 'lat' (latitude) e 'lon' (longitude). O gráfico de dispersão (scatterplot) mostrou um padrão claro:

Operações Locais: As Lojas 1, 2 e 3 concentram suas operações em uma única região.

Operação Nacional: A Loja 4 (destacada em vermelho nos gráficos) era a única com uma rede de distribuição NACIONAL, atendendo clientes em todo o território.

Cruzando Métricas Adicionais
Essa descoberta mudou a perspectiva sobre a Loja 4, que passou de "pior loja" para "ativo oculto". Outras métricas reforçaram isso:

Loja 1 (Maior Faturamento): Apesar de liderar em receita, apresentava a pior avaliação média dos clientes (3.98 estrelas) e o frete mais caro, indicando sérios problemas logísticos e de satisfação.

Loja 4 (Pior Faturamento): Em contrapartida, possuía uma boa avaliação (4.00 estrelas) e o frete mais barato, demonstrando uma operação logística eficiente e com potencial de escala.

🚀 Recomendação Final
A recomendação estratégica, baseada nas evidências, foi vender a Loja 1.

Embora tenha o maior faturamento, ela representa um risco significativo devido à alta insatisfação dos clientes e à logística cara e limitada. A Loja 4, por outro lado, é o ativo mais estratégico da rede, com a melhor logística, maior alcance geográfico e maior potencial de crescimento futuro.

🖥️ Instruções para Execução
Para replicar esta análise, siga os passos abaixo:

Clone este repositório para sua máquina local (ex: git clone ...).

Abra o notebook AluraStoreBrasil.ipynb em um ambiente compatível com Jupyter (como Jupyter Lab, VS Code ou Google Colab).

Recomendação (Google Colab):

Faça o upload do notebook para o Google Colab.

No menu, acesse "Ambiente de execução".

Clique em "Executar tudo".

O notebook processará os dados, executará todas as funções de análise nativas, gerará os 3 gráficos e exibirá o relatório final detalhado na última célula.

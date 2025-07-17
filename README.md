# DataLAB para Amazon Sales

Este projeto tem como foco **investigar os fatores que influenciam as avaliações de produtos na Amazon**, a partir de um conjunto de dados com reviews e características dos itens disponíveis na plataforma. A análise visa identificar como variáveis como preço, descontos, quantidade de avaliações e categorias dos produtos estão relacionadas com as classificações fornecidas pelos consumidores, buscando compreender padrões de comportamento e preferências dos usuários.

## Objetivo

O objetivo foi **preparar e explorar os dados de forma estruturada para gerar insights relevantes**, com ênfase na relação entre as categorias dos produtos e as notas atribuídas pelos usuários, utilizando análises exploratórias e visualizações para apoiar a tomada de decisões estratégicas.

## Problema Central

Uma série de hipóteses foi formulada sobre os fatores que podem influenciar as avaliações de produtos na Amazon.

Para investigar esse problema, foram consideradas as seguintes hipóteses:

1 – Produtos com maiores descontos apresentam notas médias mais altas.
2 – Produtos avaliados por um maior número de pessoas recebem classificações mais altas.
3 – Produtos com preços originais mais elevados recebem avaliações melhores.
4 – Produtos com preços mais altos possuem valores absolutos de desconto maiores (em R$).

## Ferramentas e Tecnologias

- **Linguagem:** Python
- **Bibliotecas Python:** Pandas, NumPy, Matplotlib, Seaborn, SciPy, NLTK
- **Fonte dos Dados: arquivos CSV processados localmente
- **Visualização de Dados:** Matplotlib e Seaborn (gráficos estáticos para análise exploratória)
- **Ambiente de Desenvolvimento:** Google Colab - (`DataLab_Projeto4.ipynb`)

## Estrutura do Repositório

- `dados_brutos/`: Contém os arquivos CSV originais que foram fornecidos para a análise.
  - [`amazon_product.csv`](amazon_product.csv)
  - [`amazon_review.csv`](amazon_review.csv)
- `documentacao/`: Contém documentos explicativos sobre o projeto.
  - [`apresentacao_datalab.pdf`](apresentacao_datalab.pdf) — Apresentação do projeto com um resumo visual dos insights.
  - [`ficha_tecnica_codigos.ipynb`](ficha_tecnica_codigos.ipynb) — Ficha técnica com os códigos Python utilizados durante o projeto.
  - [`ficha_tecnica_datalab.pdf`](ficha_tecnica_datalab.pdf) — Ficha técnica do projeto detalhando o processo e resultados.
  - [`relatorio_datalab.pdf`](relatorio_datalab.pdf) — Relatório estratégico com os resultados do projeto.
- [`DataLab_Projeto4.ipynb`](DataLab_Projeto4.ipynb) — Notebook com análises exploratórias, testes de hipóteses e regressões.

## Metodologia

- **Coleta e Consolidação:** Dados carregados, processados e consolidados. Foram tratadas variáveis como preço real (actual_price), percentual de desconto, categorias e número de avaliações.
  
- **Tratamento:** Remoção de duplicatas, tratamento de valores nulos, padronização de formatos (datas) e seleção estratégica de colunas.

- **Análise Exploratória:** Gráficos de dispersão, boxplots e histogramas foram utilizados para explorar a relação entre variáveis-chave e o rating.

- **Testes Estatísticos:** Foram aplicados testes de:
  - Z-Score e IQR: Identificação e remoção de outliers.
  - Correlação de Pearson: Relação entre variáveis numéricas.
  - ANOVA: Comparação de médias entre categorias. 
  - Qui-quadrado: Associação entre variáveis categóricas.
  - Regressões Lineares: Análise de impacto de variáveis no rating.

- **Modelagem:** Regressões múltiplas foram utilizadas para avaliar o impacto conjunto de variáveis como preço, popularidade e categoria sobre o rating.

## Principais Resultados

- **Popularidade importa:** Produtos com maior número de avaliações tendem a exibir ratings médios ligeiramente superiores.

- **Descontos afetam percepção:** Percentuais de desconto mais elevados estão associados a ratings mais baixos, possivelmente por influência na percepção de valor ou qualidade.

- **Preço não influencia significativamente:** Não foi observada diferença significativa de rating entre produtos de preços altos e baixos.

- **Descontos maiores para produtos caros:** Produtos com preços reais mais altos recebem descontos mais elevados, evidenciando uma forte correlação entre preço e valor do desconto.

- **Categoria como fator-chave:** A categoria do produto impacta mais as avaliações do que preço ou desconto isoladamente, com Computers&Accessories e OfficeProducts apresentando melhor desempenho.


*Os resultados completos das análises e as recomendações estratégicas na [Ficha Técnica](/documentacao/ficha_tecnica_datalab.pdf).*


## Responsáveis pelo Projeto

| Nome           | Função           | Contato                                                                                                 |
|----------------|------------------|--------------------------------------------------------------------------------------------------------|
| Aline Dionizio | Analista de Dados| [LinkedIn](https://www.linkedin.com/in/aline-dionizio/) \| [Email](mailto:alinedioniziosilva@outlook.com) \| [GitHub](https://github.com/AlineDion)  |
| Taiza Ferreira | Analista de Dados| [LinkedIn](https://www.linkedin.com/in/taiza-ferreira-dados/) \| [Email](mailto:taiza.desouza@yahoo.com.br) \| [GitHub](https://github.com/TaizaFerreira) |
| Giullia Braga  | Analista de Dados| [LinkedIn](https://www.linkedin.com/in/bragagiu/) \| [Email](mailto:giubraga98@gmail.com) \| [GitHub](https://github.com/BragaGiu) |
















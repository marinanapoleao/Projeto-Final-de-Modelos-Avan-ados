# Projeto Final de Modelos Avançados
<img width="1280" height="853" alt="image" src="https://github.com/user-attachments/assets/b4e52bb0-f7fb-4164-8685-d21972141b91" />

## 📌 Sobre o Projeto

Desenvolvimento de um modelo de aprendizado não supervisionado utilizando o algoritmo K-Means para segmentar clientes de um shopping com base em características demográficas, renda anual e pontuação de gastos. O projeto explora técnicas de análise de dados, pré-processamento, clusterização e avaliação de modelos.

## 🎯 Objetivo

O objetivo deste projeto é aplicar os conceitos aprendidos nos módulos de conceitos avançados de modelagem para realizar uma segmentação de clientes utilizando o algoritmo de clustering K-Means.

### Problema de Negócio / Pergunta de Pesquisa

É possível segmentar os clientes de um shopping em grupos distintos a partir de sua idade, renda anual e pontuação de gastos? Como esses grupos podem ajudar o negócio a identificar clientes de alto valor e oportunidades para direcionar ações comerciais e de marketing?


## 📊 Fonte de Dados

Dataset Mall_Customers.csv, composto originalmente por 200 registros de clientes e cinco atributos:
- CustomerID: identificador do cliente.
- Gender: gênero.
- Age: idade.
- Annual Income (k$): renda anual em milhares de dólares.
- Spending Score (1-100): pontuação de gastos atribuída pelo shopping conforme o comportamento e o padrão de consumo.

Para a clusterização, foram utilizadas as variáveis idade, renda anual e pontuação de gastos, após a exclusão das colunas de identificação e gênero.

## 🛠️ LINGUAGENS E BIBLIOTECAS

- Python — desenvolvimento da análise e do modelo.
- Pandas e NumPy — manipulação e tratamento de dados.
- Matplotlib e Seaborn — visualizações estatísticas.
- Plotly Express e Plotly Graph Objects — gráficos interativos.
- Scikit-learn — padronização com StandardScaler, implementação do K-Means, redução de dimensionalidade com PCA e métricas de avaliação.
- Kneed — identificação automática do ponto de cotovelo para auxiliar na escolha do número de clusters.


## 🔍 Metodologia

1. Análise exploratória: inspeção dos tipos de dados, estatísticas descritivas e verificação de valores ausentes.
   
2. Tratamento dos dados: análise de valores extremos por meio de boxplots e do método do intervalo interquartil (IQR), com remoção de dois registros extremos de renda anual.
   
3. Análise de relações: avaliação das correlações entre as variáveis numéricas e construção de gráficos de dispersão e pairplots.

4. Preparação dos dados: seleção das variáveis relevantes e padronização de idade, renda anual e pontuação de gastos com StandardScaler.

5. Definição do número de grupos: análise da inércia pelo método do cotovelo, com auxílio do KneeLocator, e comparação de valores de \(k\).

6. Modelagem: aplicação do algoritmo K-Means com quatro clusters.

7. Avaliação: utilização das métricas Silhouette Score e Davies-Bouldin Index para avaliar a separação e a estrutura dos grupos.

8. Interpretação dos resultados: análise dos centroides e dos perfis encontrados, identificando grupos com diferentes combinações de idade, renda e gastos.

9. Aplicação ao negócio: identificação de possíveis oportunidades para segmentação de campanhas, personalização de ofertas e estratégias de relacionamento com clientes.


## 📈  Resultados e Métricas

Cluster --------   Perfil identificado

0 --------   Clientes mais velhos, com renda média e gastos médios a baixos.

1 --------   Clientes com renda alta e pontuação de gastos elevada.

2 --------   Clientes mais jovens, com renda menor e pontuação de gastos relativamente alta.

3 --------   Clientes com renda alta e pontuação de gastos baixa.


## 💡Principais Insights e Implicações

Esses resultados ajudam a avaliar a estrutura dos agrupamentos, mas não garantem, isoladamente, que os clusters sejam estáveis ou comercialmente eficazes. A interpretação dos perfis é o que permite relacionar os resultados às possíveis decisões de negócio.

## 👩‍💻 Sobre a Autora

Desenvolvido por Marina Napoleão — Cientista de Dados / Analista de Dados. 
### LinkedIn <https://www.linkedin.com/in/marina-napoleao/>
### GitHub <https://github.com/marinanapoleao> 

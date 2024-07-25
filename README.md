# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Neste projeto, utilizei uma IA (ChatGPT) e o SageMaker Canvas para criar um sistema de gerenciamento de estoque inteligente com o uso de Machine Learning. A finalidade era investigar as funcionalidades de ML com pouco código e compreender como a inteligência artificial pode ser uma ferramenta valiosa no ambiente corporativo, apoiando empresas na tomada de decisões e na previsão de tendências futuras

## 📋 Pré-requisitos

- Conta AWS
- Dataset
- Conhecimento no uso do SageMaker Canvas


## 🎯 Objetivos deste de Projeto 

- Desenvolver competências em Machine Learning low-code.
- Expandir o conhecimento sobre o Amazon SageMaker.
- Explorar como a inteligência artificial pode beneficiar o mercado profissional.
- Apoiar empresas na tomada de decisões e na realização de previsões futuras.
- Implementar soluções de ML com o SageMaker Canvas para otimizar a gestão de estoque.
- Aplicar técnicas de análise de dados para melhorar a eficiência operacional das empresas.


## 🚀 Passo a Passo

### 1. Dataset

Utilizei o ChatGPT para gerar um dataset com informações usando o seguinte prompt:

Crie um arquivo CSV contendo as colunas (Item, Comprador, Valor, Data_Compra, Quantidade_Estoque). Esses dados serão usados para treinar um modelo de gerenciamento de estoque inteligente.

{REGRAS}

- Sempre que um item atingir a quantidade de 20 unidades, reabasteça o material.
- Preencha o arquivo com no mínimo 10 compras de itens variados fictícios por dia.
- Preencha o arquivo com dados a partir de 01-01-2024 até 14-04-2024.
- Inclua a coluna "Categoria" para identificar o tipo de item (por exemplo, Eletrônicos, Roupas, Alimentos).
- Adicione uma coluna "Método de Pagamento" com opções como Cartão de Crédito, Dinheiro e Transferência Bancária.
- Insira uma coluna "Desconto Aplicado" com valores percentuais aleatórios (0%, 5%, 10%, 15%).
- Introduza uma coluna "Região" para indicar a localização de compra (por exemplo, Norte, Sul, Leste, Oeste).

### 2. Treinando o Modelo

- Carreguei o dataset gerad pelo ChatGPT no SageMaker Canvas
- Configurei as variáveis de entrada e saída.
- Iniciei o treinamento do modelo

### 3. Analisar

Após concluir o treinamento, avaliei detalhadamente as métricas de desempenho do modelo.
Analisei as principais variáveis que impactam as previsões, com ênfase na quantidade em estoque (Quantidade_Estoque) e no valor do item (Valor).

### 4. Prever

Utilizei o modelo treinado para realizar previsões de estoque. A análise revelou que o fator mais significativo nos resultados é a quantidade de material em estoque. Quando a quantidade em estoque aumenta de 20 para 60 unidades, observa-se uma redução substancial nas vendas de todos os itens.

Além disso, verificou-se que o item I020 não apresenta variações significativas nas vendas, independentemente da quantidade em estoque ou do valor, o que pode sugerir um alto volume de saída e a necessidade de aumento no estoque desse item.

O item I010 experimentou um aumento de 57% nas saídas quando o valor foi reduzido de 90 para 70. Por outro lado, o item I030 viu um incremento de 75% nas saídas quando a quantidade em estoque aumentou de 20 para 120, indicando uma tendência de maiores volumes de compras com maiores quantidades em estoque.

Os demais itens mostraram alterações relevantes apenas quando o período analisado foi reduzido, apresentando consequências negativas. Isso destaca a necessidade de um monitoramento mais rigoroso desses itens.

## 🔗Redes Sociais
https://www.linkedin.com/in/costairis/

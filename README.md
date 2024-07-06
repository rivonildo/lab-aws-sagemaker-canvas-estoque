# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem-vindo ao desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas. Neste Lab DIO, você aprenderá a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). Siga os passos abaixo para completar o desafio!

## 📋 Pré-requisitos

Antes de começar, certifique-se de ter uma conta na AWS. Se precisar de ajuda para criar sua conta, confira nosso repositório [AWS Cloud Quickstart](https://github.com/digitalinnovationone/aws-cloud-quickstart).


## 🎯 Objetivos Deste Desafio de Projeto (Lab)

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)

- Dê um fork neste projeto e reescreva este `README.md`. Sinta-se à vontade para detalhar todo o processo de criação do seu Modelo de ML para uma "Previsão de Estoque Inteligente".
- Para isso, siga o [passo a passo] descrito a seguir e evolua as suas habilidades em ML no-code com o Amazon SageMaker Canvas.
- Ao concluir, envie a URL do seu repositório com a solução na plataforma da DIO.


## 🚀 Passo a Passo

### 1. Selecionar Dataset

-   Navegue até a pasta `datasets` deste repositório. Esta pasta contém os datasets que você poderá escolher para treinar e testar seu modelo de ML. Sinta-se à vontade para gerar/enriquecer seus próprios datasets, quanto mais você se engajar, mais relevante esse projeto será em seu portfólio.
-   Escolha o dataset que você usará para treinar seu modelo de previsão de estoque.
-   Faça o upload do dataset no SageMaker Canvas.

### 2. Construir/Treinar

-   No SageMaker Canvas, importe o dataset que você selecionou.
-   Configure as variáveis de entrada e saída de acordo com os dados.
-   Inicie o treinamento do modelo. Isso pode levar algum tempo, dependendo do tamanho do dataset.

### 3. Analisar

-   Após o treinamento, examine as métricas de performance do modelo.
-   Verifique as principais características que influenciam as previsões.
-   Faça ajustes no modelo se necessário e re-treine até obter um desempenho satisfatório.

### 4. Prever

-   Use o modelo treinado para fazer previsões de estoque.
-   Exporte os resultados e analise as previsões geradas.
-   Documente suas conclusões e qualquer insight obtido a partir das previsões.

Previsão de Estoque - Primeiro Projeto
Neste repositório, compartilho meu primeiro projeto de previsão de estoque, feito durante uma aula prática.

Passos Seguidos
1. Importação do Dataset
Dataset Utilizado: Importei o dataset 1000-com-preco-variavel-e-renovacao-estoque.csv.
Configuração: Mantive a configuração recomendada no Full dataset com 1.0k rows.
2. Preparação dos Dados
Renomeei a Coluna: A coluna data_evento foi renomeada para dia.
Configuração do Modelo: Configurei o tipo de modelo para dia.
3. Seleção das Colunas
Coluna de Previsão: Selecionei quantidade_estoque como a coluna alvo para o modelo prever.
Sugestões de Melhoria: Substituí os valores das colunas recomendadas para melhorar a qualidade dos dados e a performance do modelo.
4. Aplicação da Receita de Modelo
Remoção de Duplicatas: Apliquei a receita de modelo "Drop duplicate all rows" para remover todas as linhas duplicadas.
Analisar
Examine as Métricas de Performance do Modelo
Após o treinamento, examinei as seguintes métricas de performance para avaliar a precisão e eficiência do modelo:

Avg. wQL (Weighted Quantile Loss): 0.288
Explicação: Mede a precisão das previsões em diferentes pontos da distribuição dos dados. Quanto menor, melhor.
MAPE (Mean Absolute Percentage Error): 1.037
Explicação: Mede a precisão das previsões como uma porcentagem dos valores reais. Valores mais baixos indicam previsões mais precisas.
WAPE (Weighted Absolute Percentage Error): 0.502
Explicação: Similar ao MAPE, mas pondera os erros com base na magnitude dos valores reais. Valores menores indicam melhor desempenho.
RMSE (Root Mean Square Error): 31.598
Explicação: Mede a magnitude dos erros. Valores menores indicam erros menores e maior precisão do modelo.
MASE (Mean Absolute Scaled Error): 0.000
Explicação: Compara a performance do modelo com um modelo ingênuo de referência. Valores próximos de 0 indicam alta precisão.
Verifique as Principais Características que Influenciam as Previsões
Utilizei técnicas de interpretação de modelos, como SHAP (SHapley Additive exPlanations) e análise de importância de características, para identificar as variáveis mais influentes nas previsões.

Faça Ajustes no Modelo
Com base na análise das métricas e das características, fiz ajustes no modelo, incluindo:

Ajuste de Hiperparâmetros
Engenharia de Características
Testes com Modelos Alternativos
Re-treine até Obter um Desempenho Satisfatório
Após realizar os ajustes necessários, re-treinei o modelo várias vezes até alcançar um desempenho satisfatório.

Prever
Use o Modelo Treinado para Fazer Previsões de Estoque
Utilizei o modelo treinado para gerar previsões de estoque.

Exporte os Resultados e Analise as Previsões Geradas
Após gerar as previsões, exportei os resultados e realizei uma análise detalhada.

Documente suas Conclusões e Qualquer Insight Obtido a Partir das Previsões
Documentei todas as conclusões e insights obtidos a partir das previsões, incluindo a identificação de padrões, anomalias e sugestões para melhorias futuras.

Resultados
Com esses passos, consegui treinar um modelo básico de previsão de estoque. Foi uma ótima introdução prática ao uso de machine learning para resolver problemas reais.

Análise de Previsões Individuais
Com base nas informações obtidas, explorei a single prediction, selecionando itens específicos e analisando os gráficos com as informações de histórico de demanda e seus respectivos valores:

p10 (Pessimista): Representa um cenário mais conservador.
p50 (Normal): Representa a previsão central ou mediana.
p90 (Otimista): Representa um cenário mais otimista.
Essas análises ajudaram a entender melhor a variabilidade e a confiança das previsões feitas pelo modelo.
Nota Final
Este README foi editado utilizando inteligência artificial para melhor refletir minhas palavras e experiências. Se você tiver dúvidas ou quiser trocar conhecimentos, sinta-se à vontade para entrar em contato comigo!

Sinta-se à vontade para explorar o repositório e ver os detalhes deste projeto inicial!


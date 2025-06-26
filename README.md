# Análise de Evasão de Clientes (Churn) - Telecom X


Este repositório contém um projeto de análise de dados focado na identificação dos fatores que contribuem para a evasão de clientes (churn) na Telecom X. O objetivo é fornecer insights valiosos para a equipe de Data Science, auxiliando no desenvolvimento de modelos preditivos e estratégias eficazes de retenção de clientes.

🎯 Objetivo do Projeto

O principal objetivo deste projeto é:

• Coletar e tratar dados de clientes da Telecom X.

• Realizar uma Análise Exploratória de Dados (EDA) para identificar padrões e tendências relacionadas ao churn.

• Gerar insights acionáveis para subsidiar a tomada de decisões e o desenvolvimento de estratégias de retenção.

🚀 Metodologia

A análise foi conduzida seguindo as etapas de um pipeline de dados, utilizando Python e suas principais bibliotecas (Pandas, Matplotlib, Seaborn):

1. Coleta e Importação de Dados:

• Os dados foram extraídos de uma API pública da Telecom X, disponível em formato JSON.

• O carregamento foi realizado diretamente via URL para um DataFrame do Pandas.



2. Limpeza e Tratamento de Dados (ETL):

• Valores Ausentes: Linhas com valores ausentes na coluna Charges_Total foram removidas.

• Inconsistências: Valores vazios na coluna Churn foram padronizados para 'No'.

• Tipos de Dados: A coluna Charges_Total foi convertida para tipo numérico e SeniorCitizen para booleano.

• Duplicatas: Verificação e remoção de linhas duplicadas (nenhuma encontrada).



3. Análise Exploratória de Dados (EDA) e Visualizações:

• Foram gerados diversos gráficos (distribuição de churn, churn por gênero, tipo de contrato, serviço de internet, cobranças mensais e totais, e tempo de permanência) para visualizar as relações entre as variáveis e o churn.



📊 Principais Insights e Conclusões

Com base na Análise Exploratória de Dados, os seguintes insights foram identificados:

• Tipo de Contrato: Clientes com contratos mensais (Month-to-month) apresentam uma taxa de churn significativamente maior em comparação com contratos de um ou dois anos. Isso sugere que a fidelização através de contratos de longo prazo é uma estratégia eficaz para reduzir a evasão.

• Serviço de Internet: Clientes que utilizam o serviço de internet Fibra Óptica (Fiber optic) tendem a ter uma taxa de churn mais alta do que aqueles com DSL ou sem serviço de internet. Isso pode indicar problemas de qualidade, estabilidade ou satisfação com o serviço de fibra óptica que precisam ser investigados.

• Cobranças Mensais e Totais: Observou-se uma tendência de clientes com cobranças mensais mais altas e cobranças totais mais baixas (o que geralmente indica um menor tempo de permanência) apresentarem maior probabilidade de churn. Isso reforça a ideia de que clientes novos ou com planos mais caros podem ser mais propensos a evadir se não perceberem valor adequado.

• Tempo de Permanência (Tenure): Como esperado, clientes com menor tempo de permanência são mais propensos a cancelar o serviço. Isso destaca a importância de estratégias de engajamento e retenção focadas nos primeiros meses de relacionamento com o cliente.

💡 Sugestões e Próximos Passos

Para a Telecom X, as seguintes ações são recomendadas com base nesta análise inicial:

1. Investigação Aprofundada: Realizar uma investigação mais detalhada sobre os motivos do alto churn entre clientes de fibra óptica e aqueles com contratos mensais. Pesquisas de satisfação e feedback direto podem ser valiosos.

2. Modelagem Preditiva: Utilizar as variáveis identificadas como relevantes para construir e treinar modelos de Machine Learning (e.g., Regressão Logística, Árvores de Decisão, Random Forest) capazes de prever quais clientes estão em alto risco de churn. Isso permitirá uma abordagem proativa na retenção.

3. Desenvolvimento de Estratégias de Retenção: Com base nos insights e nas previsões dos modelos, desenvolver e implementar estratégias de retenção direcionadas, tais como:

• Ofertas especiais ou incentivos para clientes de contratos mensais migrarem para planos de longo prazo.

• Melhorias na qualidade e suporte do serviço de fibra óptica.

• Programas de fidelidade ou comunicação personalizada para clientes nos primeiros meses de serviço.



💻 Como Reproduzir a Análise

Você pode reproduzir toda a análise e explorar o código Python através do notebook do Google Colab fornecido neste repositório. Siga os passos abaixo:

1.Acesse o Google Colab: Vá para colab.research.google.com.

2.Fazer Upload do Notebook: Clique em File (Arquivo) > Upload notebook (Fazer upload de notebook).

3.Selecione o Arquivo: Escolha o arquivo telecom_x_churn_analysis.md (ou telecom_x_churn_analysis.ipynb se já convertido) deste repositório.

4.Executar as Células: Uma vez carregado, você pode executar as células de código sequencialmente para ver a importação de dados, tratamento, análises e visualizações.

O notebook está estruturado para ser autoexplicativo, com comentários e saídas claras para cada etapa da análise.


# Previsao de churn - Empresa Telco
[![author](https://img.shields.io/badge/author-joaomr7-red.svg)](https://github.com/joaomr7) 

<p align="center">
  <img src="image/TelcoChurnImage.jpg">
</p>

Esse projeto faz parte de meu portifólio de data science. A idéia é estudar a exploração de dados e aplicação de modelos de machine learning para prever o churn de clientes da empresa Telco, uma empresa fictícia.

# Visão Geral do Projeto

Neste projeto, foi adotada a metodolgia CRISP-DM. A saber, as etapas abordadas foram:

  1. Entendimento do negócio
  2. Compreensão dos dados
  3. Preparação dos dados
  4. Modelagem
  5. Validação

Por tratar-se de um projeto de estudo e não possuir uma maneira no mundo real de entregar a solução para esse problema, visto que a empresa é fictícia, a etapa de implantação foi ignorada.
Abaixo segue as principais conclusões do projeto.

## Entendimento do negócio

A empresa fictícia em questão é a Telco, uma empresa de telecomunicação que, pelo que eu enferi do dataset, fornece serviços de:

 * Telefone
 * Internet
 * Segurança Online
 * Backup Online

O problema a ser resolvido é prever quais clientes irão abandonar a empresa ou não. Ou seja, claramente trata-se de um problema de classificação binária.

Para ser mais correto, queremos prever os clientes com maior probabilidade de abandonarem o serviço da empresa. Se fosse cobrir a etapa de implantação, esta ideia serial trivial, pois a solução final teria que ser capaz de retornar uma lista ordenada dos clientes da maior para a menor probabilidade de abandonarem o serviço. E apartir disso a empresa poderia tomar alguma ação para manter os clientes.

## Principais Insights do Projeto

Na etapa de compreensão dos dados, obtive os seguintes insights:

  * A maioria dos casos de churn ocorrem entre o 1º e o 20º mês

  * Os casos de churn são maiores entre US$ 120.00 de cobrança mensal

  * A grande maioria dos clientes que deixaram o serviço, assinavam o contrato mês-a-mês

  * Clientes com tenure baixo e alto montlhy_charge, tem mais chances de abandonar o serviço

## Solução do Problema

Após uma análise profunda dos dados e vários testes de diferentes modelos de classificação, o modelo que melhor solucionou o problema foi XGBoost Classifier, um modelo baseado em árvores que utiliza uma estrutura de gradient boosting.
De modo geral podemos destacar sobre o modelo:

  * não sofre com overfitting
  * consegure renconhecer entre 70% e 71% dos casos de churn
  * rechonhece entre 81% e 83% dos casos de não-churn

`Para acomponhar todo o processo, veja o arquivo Previsão_de_Churn.ipynb`

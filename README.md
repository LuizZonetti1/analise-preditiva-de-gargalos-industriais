# Análise Preditiva de Gargalos Industriais

Projeto de análise de dados aplicado ao contexto de produção industrial, com foco na identificação de gargalos operacionais, avaliação de desempenho produtivo e desenvolvimento de um modelo preditivo para estimar a produção real.

---

## Sobre o projeto

Este projeto foi desenvolvido com o objetivo de simular um cenário real de análise de dados na indústria, no qual a operação apresenta diferenças entre a produção planejada e a produção realizada, além de paradas de máquinas e variações na taxa de defeitos.

A proposta consiste em explorar os dados, identificar padrões operacionais, localizar possíveis gargalos e utilizar técnicas de machine learning para apoiar a previsão da produção real.

---

## Objetivos

- Analisar o comportamento geral dos dados de produção
- Avaliar o desempenho por máquina, produto e turno
- Identificar gargalos operacionais
- Investigar relações entre variáveis do processo
- Criar um indicador de eficiência produtiva
- Desenvolver um modelo preditivo para estimar a produção real
- Propor uma ideia inicial de automação para relatórios futuros

---

## Tecnologias utilizadas

- **Python**
- **Pandas**
- **Plotly Express**
- **Scikit-learn**
- **Jupyter Notebook**
- **Openpyxl**

---

## Estrutura do projeto

```bash
analise-preditiva-de-gargalos-industriais/
├── factory_production_dataset.xlsx
├── inicial.ipynb
└── README.md
```

---

## Base de dados

A base utilizada no projeto contém dados simulados de produção industrial, com informações relacionadas ao desempenho operacional.

### Principais colunas da base

| Coluna | Descrição |
|---|---|
| `date` | Data do registro |
| `product_id` | Identificador do produto |
| `machine_id` | Identificador da máquina |
| `shift` | Turno de produção |
| `planned_production` | Produção planejada |
| `actual_production` | Produção real |
| `machine_downtime_minutes` | Tempo de parada da máquina em minutos |
| `defect_rate` | Taxa de defeitos |
| `workers_on_shift` | Quantidade de trabalhadores no turno |

---

## Desafio proposto

O projeto foi desenvolvido a partir de um cenário simulado em que a empresa precisava entender melhor o desempenho da operação industrial e identificar os fatores que estavam impactando a produtividade.

A demanda consistia em:

- Analisar os dados de produção da fábrica
- Identificar gargalos operacionais
- Avaliar máquinas, produtos e turnos
- Investigar o impacto de variáveis operacionais na produção real
- Criar um indicador de eficiência
- Desenvolver um modelo preditivo para estimar a produção real
- Organizar os resultados de forma clara, com gráficos e interpretações objetivas
- Propor uma ideia inicial de automação para execução recorrente da análise

---

## Etapas desenvolvidas

### 1. Análise Exploratória dos Dados

Foi realizada uma exploração inicial da base para compreender sua estrutura, verificar estatísticas descritivas, avaliar a qualidade dos dados e analisar o desempenho por máquina, produto e turno.

Principais análises realizadas:

- Visualização inicial da base
- Verificação de dimensões e tipos de dados
- Análise de valores nulos e duplicados
- Estatísticas descritivas das variáveis numéricas
- Criação de gráficos para avaliação de desempenho por turno, produto e máquina
- Análise temporal da produção
- Visualização da distribuição da eficiência produtiva

### 2. Identificação de Gargalos Operacionais

Nesta etapa, foram identificados os principais pontos críticos da operação, com foco em:

- Máquinas com maior tempo de parada
- Produtos com menor eficiência produtiva
- Turnos com melhor e pior desempenho

A análise permitiu destacar os elementos com maior impacto negativo sobre a operação, facilitando a interpretação dos gargalos produtivos.

### 3. Análise de Relações entre Variáveis

Foi investigada a relação entre variáveis operacionais e a produção real, buscando entender como fatores do processo influenciam o desempenho produtivo.

Variáveis analisadas:

- Produção planejada
- Produção real
- Tempo de parada da máquina
- Taxa de defeitos
- Quantidade de trabalhadores
- Eficiência produtiva

Foram utilizadas análises de correlação e gráficos de dispersão para identificar padrões e relações entre os dados.

### 4. Criação de Indicador de Eficiência

Foi criado um indicador de eficiência produtiva com o objetivo de medir o quanto da produção planejada foi efetivamente atingido.

Fórmula utilizada:

```
Eficiência produtiva = produção real / produção planejada
```

Esse indicador foi utilizado ao longo do projeto para comparar o desempenho de máquinas, produtos e turnos.

### 5. Modelagem Preditiva

Foi desenvolvido um modelo de machine learning para prever a variável `actual_production`, ou seja, a produção real.

Variáveis utilizadas no modelo:

- `planned_production`
- `machine_downtime_minutes`
- `defect_rate`
- `workers_on_shift`

O modelo foi treinado com foco em verificar se variáveis operacionais são capazes de estimar o desempenho produtivo de forma satisfatória.

### 6. Apresentação dos Resultados

Ao final da análise, os principais achados foram organizados de forma objetiva, destacando:

- Gargalos operacionais identificados
- Diferenças de desempenho entre máquinas, produtos e turnos
- Impacto de variáveis operacionais sobre a produção real
- Desempenho do modelo preditivo
- Recomendações iniciais para melhoria da operação

## Principais análises realizadas

Ao longo do projeto, foram desenvolvidas análises como:

- Eficiência média por máquina
- Eficiência média por produto
- Eficiência média por turno
- Distribuição da eficiência produtiva
- Tempo total e médio de parada por máquina
- Taxa média de defeitos por produto
- Análise temporal da produção real
- Matriz de correlação entre variáveis numéricas
- Gráficos de dispersão entre variáveis operacionais e produção real
- Comparação entre valores reais e previstos no modelo preditivo

---

## Principais resultados

A análise permitiu identificar diferenças relevantes de desempenho entre máquinas, produtos e turnos, evidenciando a existência de gargalos operacionais na produção.

Também foi possível observar que o tempo de parada das máquinas se mostrou um fator importante para a redução da produção real, assim como a variação da taxa de defeitos e da eficiência produtiva.

Além disso, o modelo preditivo apresentou capacidade de estimar a produção real com base nas variáveis operacionais analisadas, demonstrando potencial de apoio à tomada de decisão.

---

## Recomendações iniciais

Com base nos resultados obtidos, algumas ações que poderiam ser consideradas são:

- Investigar as causas do alto tempo de parada da máquina com pior desempenho
- Avaliar o processo produtivo do produto com menor eficiência para identificar perdas
- Revisar práticas operacionais do turno com pior desempenho
- Monitorar continuamente os indicadores de eficiência, downtime e defeitos
- Evoluir a solução para relatórios automatizados e acompanhamento recorrente

---

## Competências desenvolvidas

Este projeto contribuiu para o fortalecimento das seguintes habilidades:

- Análise exploratória de dados
- Tratamento e manipulação de dados com Pandas
- Visualização de dados com Plotly Express
- Interpretação de indicadores operacionais
- Identificação de gargalos produtivos
- Aplicação de machine learning com Scikit-learn
- Raciocínio analítico voltado para problemas de negócio
- Estruturação de projeto em Python e Jupyter Notebook

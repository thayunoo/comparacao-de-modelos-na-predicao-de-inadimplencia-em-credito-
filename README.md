📊 #Comparação entre Regressão Logística e Random Forest para Predição de Inadimplência
📖 Sobre o Projeto

A avaliação do risco de crédito é essencial para a sustentabilidade de instituições financeiras e plataformas de concessão de empréstimos. A escolha entre modelos estatísticos tradicionais e técnicas de Machine Learning envolve não apenas desempenho preditivo, mas também interpretabilidade, estabilidade e aderência às exigências de governança regulatória.

Este trabalho realiza uma comparação entre os modelos Regressão Logística e Random Forest em condições operacionais equivalentes, utilizando:

mesmo conjunto de variáveis;
mesmo recorte temporal;
mesmas regras de preparação de dados.

O objetivo é prever a inadimplência em operações de crédito peer-to-peer.

🎯 #Objetivo

Comparar o desempenho preditivo, estabilidade e interpretabilidade de modelos de classificação aplicados à previsão de inadimplência de crédito.

🗂️ #Base de Dados

O estudo utiliza dados públicos da plataforma americana de empréstimos entre pessoas físicas LendingClub, contemplando operações realizadas entre 2007 e 2018.

⚙️ #Metodologia

Foi adotada uma abordagem:

quantitativa;
empírica;
comparativa;
observacional retrospectiva.

🧹 #Preparação dos Dados

O processo de tratamento incluiu:

imputação de valores ausentes;
codificação binária de variáveis categóricas;
padronização de variáveis numéricas;
remoção de variáveis com vazamento estrutural (data leakage);
tratamento do desbalanceamento de classes por ponderação.

🎯 #Variável-Alvo

A variável-alvo foi definida como:

inadimplência com atraso igual ou superior a 90 dias dentro de 12 meses após a concessão do crédito.

Classificação binária:

0 → Adimplente
1 → Inadimplente
🕒 Estratégia de Validação

O particionamento respeitou a ordem cronológica dos dados:

Conjunto	Período
Treinamento	Até 2016
Teste (Out-of-Time)	2017–2018

Essa abordagem reduz risco de vazamento temporal e aproxima o experimento de condições reais de operação.

🤖 #Modelos Avaliados

📌 Regressão Logística

Modelo estatístico tradicional amplamente utilizado em risco de crédito devido à sua:

interpretabilidade;
estabilidade;
facilidade de governança.
🌲 Random Forest

Modelo de Machine Learning baseado em ensemble de árvores de decisão, capaz de capturar relações não lineares e interações complexas.

📈 Resultados
Métrica	Regressão Logística	Random Forest
AUC-ROC	0,6911	0,6735
Brier Score	0,2213	0,2234
Captura dos 10% Maiores Riscos	35,7%	Inferior
PSI	0,0049	-

A diferença de desempenho foi estatisticamente significativa:

Teste de DeLong
Z = 20,68
p < 0,0001
✅ #Conclusão

Os resultados demonstraram que a Regressão Logística apresentou desempenho superior ao Random Forest em todas as métricas avaliadas.

O estudo evidencia que modelos mais simples, interpretáveis e amplamente aceitos em ambientes regulados podem permanecer altamente competitivos quando acompanhados de:

tratamento rigoroso dos dados;
validação temporal adequada;
controle de vazamento;
boas práticas de modelagem.
🛠️ Tecnologias Utilizadas
Python
Pandas
NumPy
Scikit-Learn
Matplotlib
Seaborn
Jupyter Notebook

📚 #Temas Relacionados
Credit Risk Modeling
Machine Learning
Explainable AI (XAI)
Model Risk Management
Basel III / IFRS 9
Validação de Modelos
Governança de Modelos

👩‍💻 #Autora

Thayna Gomes da Silva

Projeto desenvolvido como Trabalho de Conclusão de Curso (TCC).

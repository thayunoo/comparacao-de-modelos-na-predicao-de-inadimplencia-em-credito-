<h1> 📊  Comparação entre Regressão Logística e Random Forest para Predição de Inadimplência </h1>

<h2> 📖 Sobre o Projeto </h2>

A avaliação do risco de crédito é essencial para a sustentabilidade de instituições financeiras e plataformas de concessão de empréstimos. A escolha entre modelos estatísticos tradicionais e técnicas de Machine Learning envolve não apenas desempenho preditivo, mas também interpretabilidade, estabilidade e aderência às exigências de governança regulatória.

Este trabalho realiza uma comparação entre os modelos Regressão Logística e Random Forest em condições operacionais equivalentes, utilizando:

Mesmo conjunto de variáveis; <br>
Mesmo recorte temporal; <br>
Mesmas regras de preparação de dados. <br>

O objetivo é prever a inadimplência em operações de crédito peer-to-peer.

<h2> 🎯 Objetivo </h2>

Comparar o desempenho preditivo, estabilidade e interpretabilidade de modelos de classificação aplicados à previsão de inadimplência de crédito.

<h2> 🗂️ Base de Dados </h2>

O estudo utiliza dados públicos da plataforma americana de empréstimos entre pessoas físicas LendingClub, contemplando operações realizadas entre 2007 e 2018.

<h2> ⚙️ Metodologia </h2>

Foi adotada uma abordagem:

Quantitativa; <br>
Empírica; <br>
Comparativa; <br>
Observacional retrospectiva. <br>

<h2> 🧹 Preparação dos Dados </h2>

O processo de tratamento incluiu:

Imputação de valores ausentes; <br>
Codificação binária de variáveis categóricas; <br>
Padronização de variáveis numéricas; <br>
Remoção de variáveis com vazamento estrutural (data leakage); <br>
Tratamento do desbalanceamento de classes por ponderação.

<h2> 🎯 Variável-Alvo </h2>

A variável-alvo foi definida como:

Inadimplência com atraso igual ou superior a 90 dias dentro de 12 meses após a concessão do crédito.

Classificação binária:

0 → Adimplente <br>
1 → Inadimplente <br>
<h2> 🕒 Estratégia de Validação </h2>

O particionamento respeitou a ordem cronológica dos dados:

Conjunto	Período <br>
Treinamento	Até 2016 <br>
Teste (Out-of-Time)	2017–2018

Essa abordagem reduz risco de vazamento temporal e aproxima o experimento de condições reais de operação.

<h2> 🤖 Modelos Avaliados </h2>

📌 Regressão Logística

Modelo estatístico tradicional amplamente utilizado em risco de crédito devido à sua:

Interpretabilidade; <br>
Estabilidade; <br>
Facilidade de governança.


🌲 Random Forest

Modelo de Machine Learning baseado em ensemble de árvores de decisão, capaz de capturar relações não lineares e interações complexas.

<h2> 📈 Resultados </h2>
Métrica	Regressão Logística	Random Forest <br>
AUC-ROC	0,6911	0,6735 <br>
Brier Score	0,2213	0,2234 <br>
Captura dos 10% Maiores Riscos	35,7%	Inferior <br>
PSI	0,0049	

A diferença de desempenho foi estatisticamente significativa:

Teste de DeLong <br>
Z = 20,68
p < 0,0001
✅ #Conclusão

Os resultados demonstraram que a Regressão Logística apresentou desempenho superior ao Random Forest em todas as métricas avaliadas.

O estudo evidencia que modelos mais simples, interpretáveis e amplamente aceitos em ambientes regulados podem permanecer altamente competitivos quando acompanhados de:

Tratamento rigoroso dos dados;
Validação temporal adequada;
Controle de vazamento;
Boas práticas de modelagem.

<h2> 🛠️ Tecnologias Utilizadas </h2>
Python<br>
Pandas<br>
NumPy<br>
Scikit-Learn<br>
Matplotlib<br>
Seaborn<br>
Jupyter Notebook


<h2> 📚 Temas Relacionados </h2>
Credit Risk Modeling <br>
Machine Learning <br>
Explainable AI (XAI) <br>
Model Risk Management <br>
Basel III / IFRS 9 <br>
Validação de Modelos <br>
Governança de Modelos <br>

<h2> 👩‍💻 Autora </h2>

Thayna Gomes da Silva

Projeto desenvolvido como Trabalho de Conclusão de Curso (TCC).

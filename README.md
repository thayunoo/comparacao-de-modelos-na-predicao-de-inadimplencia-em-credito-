# comparacao-de-modelos-na-predicao-de-inadimplencia-em-credito

A avaliação do risco de crédito é determinante para a sustentabilidade de instituições que operam carteiras de empréstimos. A escolha entre modelos estatísticos tradicionais e “Machine Learning” envolve desempenho preditivo, interpretabilidade e adequação à governança.
Este trabalho comparou a Regressão Logística e o “Random Forest” em condições operacionais equivalentes (mesmo conjunto de variáveis, recorte temporal e regras de preparação) para prever inadimplência em empréstimos entrepares.Adotou-se abordagem quantitativa, empírica e comparativa, com desenho observacional retrospectivo, utilizando dados do “LendingClub”, plataforma americana de empréstimos entre pessoas físicas sem intermediação bancária, de 2007 a 2018. 

A variável-alvo foi atraso igual ou superior a 90 dias em 12 meses após a concessão, em escala binária: inadimplente ou adimplente. 
O particionamento respeitou a ordem cronológica: treino até 2016 e teste em período não visto (2017–2018). 
A preparação incluiu imputação de valores ausentes, codificação binária das variáveis categóricas, padronização das variáveis numéricas e exclusão de variáveis com vazamento estrutural, com desequilíbrio entre classes tratado por ponderação. 

A Regressão Logística obteve AUC-ROC de 0,6911, superando o “Random Forest” (0,6735), com diferença estatisticamente significativa (teste de DeLong: Z = 20,68; p < 0,0001). Os “Brier Scores” foram 0,2213 e 0,2234, respectivamente. 
A Regressão Logística capturou 35,7% dos inadimplentes nos 10% de maior risco, com Índice de Estabilidade Populacional de 0,0049. 

Concluiu-se que a Regressão Logística foi superior em todas as dimensões avaliadas, indicando que modelos mais simples e interpretáveis podem ser igualmente competitivos quando o tratamento dos dados é rigoroso. 

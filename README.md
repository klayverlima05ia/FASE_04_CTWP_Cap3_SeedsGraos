🌾 Classificação de Grãos de Trigo com Machine Learning

Este projeto aplica técnicas de aprendizado de máquina para classificar três tipos de grãos de trigo (Kama, Rosa e Canadian) com base em características físicas medidas em laboratório. A atividade segue a metodologia CRISP-DM, indo desde a compreensão do problema até a avaliação de diferentes algoritmos de classificação.

📌 1. Objetivo do Projeto

O objetivo é desenvolver um modelo capaz de identificar automaticamente a variedade de um grão de trigo, substituindo o processo manual utilizado em pequenas cooperativas agrícolas. A automação reduz erros humanos, aumenta a eficiência e traz maior precisão para a classificação.

📌 2. Conjunto de Dados

O projeto utiliza o Seeds Dataset, disponível no UCI Machine Learning Repository.

O conjunto possui:

210 amostras

3 classes de grãos:

Kama

Rosa

Canadian

7 atributos físicos:

Área

Perímetro

Compacidade

Comprimento do núcleo

Largura do núcleo

Coeficiente de assimetria

Comprimento do sulco

Todos os atributos são numéricos e não há valores ausentes.

📌 3. Metodologia (CRISP-DM)
1. Entendimento do Negócio

Automatizar a classificação dos grãos melhora a produtividade das cooperativas agrícolas e reduz falhas humanas.

2. Entendimento dos Dados

Foi realizada análise exploratória com:

head(), info(), describe()

histogramas

boxplots

heatmap de correlação

scatterplots

3. Preparação dos Dados

Separação de X (características) e y (classe)

Divisão em treino/teste (70% / 30%)

Padronização dos dados via StandardScaler

4. Modelagem

Foram treinados três modelos:

KNN

SVM

Random Forest

5. Avaliação

Cada modelo foi avaliado utilizando:

Acurácia

Precisão

Recall

F1-score

Matriz de confusão

6. Implantação (simulada)

O melhor modelo pode ser utilizado em sistemas de triagem automática de grãos.

📌 4. Resultados

Tabela comparativa dos modelos (baseline):

Modelo	Acurácia	Precisão	Recall	F1-score
KNN	~0.87	~0.87	~0.87	~0.87
SVM	~0.87	~0.87	~0.87	~0.87
Random Forest	~0.92	~0.92	~0.92	~0.92
📌 5. Conclusão

Os três modelos apresentaram bom desempenho na classificação dos grãos, mas o Random Forest se destacou com aproximadamente 92% de acurácia, além das melhores métricas de precisão, recall e F1-score.
Por sua robustez e boa capacidade de generalização, ele é o modelo mais indicado para uma aplicação real na classificação automática de grãos.

📌 6. Tecnologias Utilizadas

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Google Colab

📌 7. Como Executar o Projeto

Clone o repositório:

git clone <seu_repositorio_aqui>


Abra o notebook no Google Colab ou Jupyter Notebook.

Certifique-se de que o arquivo seeds_dataset.txt está na mesma pasta.

Execute as células em sequência.

<h1>Sistema de Recomendação de Livros</h1>
Este projeto tem como objetivo principal desenvolver um modelo de Machine Learning capaz de prever se um usuário gostará ou não de um livro, com base em seu perfil e em avaliações anteriores de outros leitores. 
<br> Utiliza-se uma adaptação do Book-Crossing Dataset, publicado pelo usuário ruchi798 na plataforma Kaggle, que reúne informações sobre livros, usuários e avaliações. O dataset original, com cerca de 1 milhão de avaliações, foi consolidado para este projeto. 

<h3>Pré-processamento e Modelo</h3>
Foram realizadas etapas de pré-processamento como o tratamento de dados nulos, tratamento de outliers e conversão de variáveis categóricas para numéricas usando LabelEncoder. Para evitar viés no modelo, foi aplicado o balanceamento de classes (Undersampling). 
O algoritmo escolhido foi a Árvore de Decisão, um modelo supervisionado adequado para dados variados. Os dados foram divididos em 70% para treinamento e 30% para teste. 

<h3>Resultados</h3>

<h4>Resultados Iniciais (sem balanceamento):</h4>

A acurácia foi de aproximadamente 67.84%. No entanto, o modelo apresentava um desempenho superior na previsão de que o usuário "gostaria" do livro, indicando um possível vício. 

<h4>Resultados Finais (com balanceamento):</h4>

Após o balanceamento das classes, a acurácia foi de aproximadamente 61.08%. O desempenho se tornou mais equilibrado entre as classes "gostou" e "não gostou", indicando um modelo mais consistente e imparcial, apesar da baixa na acurácia. 

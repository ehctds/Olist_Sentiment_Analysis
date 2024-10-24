# Projeto de Classificação de Sentimentos em Reviews - Olist
Este projeto utiliza técnicas de Processamento de Linguagem Natural (PLN) e aprendizado profundo para realizar a classificação de sentimentos em reviews de clientes da Olist. O objetivo é prever se um review tem uma avaliação positiva ou negativa com base em diferentes abordagens de modelagem. Foram implementados modelos clássicos e de deep learning, e também explorado o uso de embeddings pré-treinados e transferência de aprendizado.

Modelos Implementados

Multinomial Naive Bayes (TF-IDF): Abordagem clássica baseada em contagem de palavras.

LSTM (Long Short-Term Memory) com embeddings pré-treinados do NILC - Núcleo Interinstitucional de Linguística Computacional USP: Modelo de deep learning para capturar dependências de longo prazo nos textos.

GRU (Gated Recurrent Unit) com embeddings pré-treinados em português do NILC - Núcleo Interinstitucional de Linguística Computacional USP: Variante otimizada para tarefas de sequência com menor tempo de treinamento.

BERT (Transfer Learning): Utilização de um modelo de transferência de aprendizado para melhor desempenho em classificação de texto.

Desempenho dos Modelos

Abordagem,	Acurácia e	Tempo de Treinamento: 

Multinomial Naive Bayes (TF-IDF)	90%   > 1 min

LSTM (Embedding pré-treinado)	93%	  20 min

GRU (Embedding pré-treinado)	92%	  2 min

BERT (Transfer Learning)	95%	  45 min

Principais Desafios

Desbalanceamento de classes: O dataset apresentava um número desproporcional de reviews positivos em relação aos negativos, o que pode ter afetado a acurácia na detecção de sentimentos negativos. Esse desbalanceamento será tratado em trabalhos futuros, com técnicas como oversampling ou undersampling.
Tempo de treinamento: Apesar de modelos mais avançados como o BERT apresentarem melhores resultados de acurácia, o custo computacional é maior, o que foi um fator considerado na escolha do modelo ideal para diferentes cenários.
Tecnologias Utilizadas
Keras/TensorFlow: Para criação e treinamento dos modelos de deep learning.
Sklearn: Para abordagens clássicas de classificação.
Pré-processamento: Limpeza de textos com regex e tokenização utilizando Keras.
Transfer Learning: Utilização de BERT para classificação de sentimentos.

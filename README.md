## 🧠 Checkpoint 02 — Parte 01 
Redes Neurais com Keras (Classificação + Regressão)

Este projeto faz parte do Checkpoint 02 da disciplina Disruptive Architectures: IoT, IoB e Generative AI.
O objetivo desta etapa é treinar redes neurais com Keras, comparar com modelos clássicos do Scikit-learn e analisar os resultados obtidos.

## 📁 Estrutura da Pasta
parte01-redes-neurais/  
├── classificacao_wine.ipynb        # Exercício 1 - Classificação Multiclasse  
├── regressao_california.ipynb      # Exercício 2 - Regressão  
└── README.md                        

## 🧪 1. Exercício 1 – Classificação Multiclasse 🍷

# 📊 Dataset: Wine Dataset (UCI)

Objetivo: Classificar vinhos em 3 classes com base em características químicas.

Rede Neural:

2 camadas ocultas (32 neurônios, ReLU)

Camada de saída (3 neurônios, Softmax)

Otimizador: Adam

Perda: categorical_crossentropy

Modelo de comparação: RandomForestClassifier (Scikit-learn)

Métrica avaliada: Acurácia

# ✅ Resultados esperados:

Rede Neural e RandomForest atingem acurácias altas (acima de 0.95).

RandomForest costuma performar muito bem em dados tabulares pequenos.

## 🧮 2. Exercício 2 – Regressão 🏡

# 📊 Dataset: California Housing Dataset (Scikit-learn)

Objetivo: Prever o valor médio das casas na Califórnia com base em dados demográficos e geográficos.

Rede Neural:

3 camadas ocultas (64, 32 e 16 neurônios, ReLU)

Camada de saída (1 neurônio, Linear)

Otimizador: Adam

Perda: MSE

Modelos de comparação:

LinearRegression

RandomForestRegressor

Métrica avaliada: Erro Médio Absoluto (MAE)

# ✅ Resultados esperados:

Rede Neural apresenta erro competitivo em relação aos modelos clássicos.

RandomForest costuma ter melhor desempenho direto em dados tabulares.

## 🧰 3. Como Executar os Notebooks (Google Colab)

Acesse Google Colab

Faça upload dos notebooks:

classificacao_wine.ipynb

regressao_california.ipynb

Clique em “Copiar para o Drive” para salvar.

Execute todas as células (Ctrl + F9) — não é necessário instalar nada extra, o Colab já vem com TensorFlow e Scikit-learn.

## ⚙️ 4. Principais Hiperparâmetros
Parâmetro	Classificação	Regressão
Épocas	80	80
Batch size	8	32
Otimizador	Adam	Adam
Função de ativação saída	Softmax	Linear
Função de perda	Crossentropy	MSE  

## 📊 5. Comparação de Desempenho
Modelo	Tarefa	Métrica	Resultado aproximado
Rede Neural (Keras)	Classificação	Acurácia	> 0.95
RandomForestClassifier	Classificação	Acurácia	> 0.95
Rede Neural (Keras)	Regressão	MAE	~0.35–0.45
LinearRegression	Regressão	MAE	~0.45
RandomForestRegressor	Regressão	MAE	~0.30–0.35

(os valores podem variar um pouco conforme o treinamento)

## 📝 6. Observações Finais

Modelos clássicos como RandomForest costumam ter ótima performance em dados tabulares.

Redes neurais oferecem mais flexibilidade para ajustes e aprendizado profundo.

O uso do Colab simplifica a execução por já conter as dependências instaladas.

O histórico de treinamento (gráficos de acurácia e erro) facilita entender a evolução do modelo.

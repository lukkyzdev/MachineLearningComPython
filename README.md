# <img align="center" alt="Python" height="40" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg"> Machine Learning | Classificação Multiclasse com TensorFlow

Um projeto de **Machine Learning** focado na construção, treino e avaliação de uma Rede Neural Artificial (RNA) em Python. 

O sistema processa o clássico conjunto de dados *Iris*, aprendendo padrões morfológicos (medidas de sépalas e pétalas) para classificar de forma autónoma as diferentes espécies de flores.

## 🎯 Objetivo do Projeto
O objetivo deste projeto foi aplicar na prática os fundamentos de **Análise de Dados** e **Inteligência Artificial**, estruturando o ciclo de vida completo de um modelo preditivo:
- Pré-processamento e normalização de dados brutos.
- Divisão estratégica de conjuntos de treino e teste (*Train/Test Split*).
- Arquitetura, compilação e treino de uma rede neural profunda.
- Avaliação de acurácia e geração de inferências (previsões probabilísticas).

## 💻 Tecnologias e Ferramentas Aplicadas
- **Python:** Linguagem base utilizada no ambiente de desenvolvimento.
- **TensorFlow / Keras:** Construção da arquitetura da rede neural, definição do otimizador (`adam`) e função de perda (`sparse_categorical_crossentropy`).
- **Scikit-Learn:** Importação do dataset original, divisão dos dados para treino/teste e normalização das escalas.
- **Pandas:** Manipulação e estruturação inicial da base de dados.

## 🧠 Arquitetura do Modelo
O algoritmo foi estruturado num *pipeline* lógico de aprendizado:
1. **Preparação:** Os dados foram separados e normalizados para garantir que o modelo não sofresse distorções devido a diferentes escalas numéricas.
2. **Rede Neural:** 
   - **Camadas Ocultas:** Duas camadas densas (com 10 e 8 neurónios respetivamente), utilizando a função de ativação `ReLU`.
   - **Camada de Saída:** 3 neurónios com a função `Softmax`, ideal para tarefas de classificação multiclasse, pois converte as saídas em probabilidades.
3. **Treino e Avaliação:** O modelo foi treinado ao longo de 50 épocas (ajuste de pesos) e avaliado com dados nunca antes vistos (conjunto de teste) para medir a sua verdadeira capacidade de generalização.

## 📊 Execução e Demonstração
Abaixo é possível visualizar a rotina de execução, desde a compilação do modelo até à geração de previsões onde o algoritmo indica a classe com maior probabilidade de correspondência:

> **Testes e Execução do Modelo:**
> 
> ![Execução do Modelo](./images/exe.png)

> **Estrutura de Código (Importações e Arquitetura):**
> 
> ![Estrutura do Código 1](./images/code.png)
> ![Estrutura do Código 2](./images/code1.1.png)

## 📂 Acesso ao Código Fonte
Todo o *pipeline* de tratamento de dados, construção da rede e treino pode ser analisado no ficheiro abaixo:
- [📄 MachineLearningComPython.py](https://github.com/lukkyzdev/MachineLearningComPython/blob/main/MachineLearningComPython.py)

---
*Desenvolvido por Lucas Fontes com foco no aprimoramento de fundamentos em Inteligência Artificial e Análise de Dados.*

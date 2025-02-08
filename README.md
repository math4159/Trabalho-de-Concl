# 🔍 Aprendizado de Estruturas Bayesianas em Dados da ANEEL

## 📌 Visão Geral
Este projeto utiliza **Redes Bayesianas** para modelagem e inferência sobre dados da **ANEEL (Agência Nacional de Energia Elétrica)**. Ele inclui abordagens baseadas em **Aprendizado de Estruturas**, **Estimativa de Parâmetros** e **Inferência Probabilística**.

O código principal está implementado em **Python** utilizando **Jupyter Notebook**, e as bibliotecas principais incluem `pgmpy`, `pandas`, `networkx`, `matplotlib` e `numpy`.

## 🔧 Tecnologias Utilizadas
- **Python 3**
- **Pandas** – Manipulação e análise de dados da ANEEL.
- **NetworkX** – Construção e manipulação de grafos direcionados.
- **pgmpy** – Modelagem, aprendizado e inferência em Redes Bayesianas.
- **Matplotlib** – Visualização dos resultados.
- **NumPy** – Operações matemáticas e estatísticas.
- **Jupyter Notebook** – Ambiente interativo para execução dos experimentos.

## 📂 Estrutura do Projeto
```
📁 Projeto
│── notebook_estrutura.ipynb   # Notebook com aprendizado de estrutura
│── notebook_inferencia.ipynb  # Notebook com inferência na rede bayesiana
│── dados_aneel.csv            # Conjunto de dados da ANEEL
│── rede_ideal.bif             # Arquivo BIF com a estrutura ideal
│── README.md                  # Documentação do projeto
```

## 🎯 Funcionalidades Principais
### 1️⃣ **Aprendizado de Estrutura da Rede Bayesiana**
- Utiliza **Hill Climb Search** (`pgmpy.estimators.HillClimbSearch`) para encontrar a melhor estrutura.
- Avalia os modelos utilizando o **BIC (Bayesian Information Criterion)** (`pgmpy.estimators.BicScore`).
- Gera e plota o grafo da rede aprendida usando `networkx` e `matplotlib`.

### 2️⃣ **Estimativa de Parâmetros**
- Utiliza **Maximum Likelihood Estimation (MLE)** (`pgmpy.estimators.MaximumLikelihoodEstimator`).
- Possibilidade de usar **Bayesian Estimation** (`pgmpy.estimators.BayesianEstimator`).

### 3️⃣ **Inferência na Rede Bayesiana**
- Usa o **algoritmo de eliminação de variáveis** (`pgmpy.inference.VariableElimination`).
- Permite consultas probabilísticas condicionais sobre as variáveis da rede.

### 4️⃣ **Visualização da Estrutura da Rede**
- Utiliza `networkx.draw()` e `matplotlib.pyplot` para exibir a rede aprendida.

## 🚀 Como Executar
### 1️⃣ Instale as dependências:
```bash
pip install numpy pandas networkx pgmpy matplotlib jupyter
```

### 2️⃣ Execute os notebooks interativamente:
```bash
jupyter notebook
```

Abra os arquivos `.ipynb` e execute as células passo a passo.

## 📊 Resultados
- A estrutura aprendida da Rede Bayesiana é salva e pode ser comparada com uma rede ideal (`rede_ideal.bif`).
- As inferências probabilísticas permitem analisar dependências entre variáveis.
- Visualização da estrutura da rede para melhor compreensão das relações encontradas.

## 🛠 Possíveis Melhorias
- Implementar outros métodos de aprendizado de estrutura (ex: K2Score, Constraint-Based).
- Utilizar outros datasets para validação dos modelos.
- Criar uma interface gráfica para facilitar o uso.

---




# Classificador de Espécies de Íris com KNN

## Sobre o Projeto

Este projeto implementa um classificador de espécies de flores Íris utilizando o algoritmo **K-Nearest Neighbors (KNN)**. Desenvolvido como parte da AG2 (Atividade em Grupo) do Inatel para as engenharias de Computação e Software.

### Objetivo
Classificar espécies de flores Íris em três categorias:
- **Iris setosa** (1)
- **Iris versicolor** (2)  
- **Iris virginica** (3)

Com base em quatro medidas da flor:
- Comprimento da sépala (cm)
- Largura da sépala (cm)
- Comprimento da pétala (cm)
- Largura da pétala (cm)

## Dataset

**Fonte:** UCI Machine Learning Repository  
**Coletado por:** Ronald Fisher (1936)  
**Amostras:** 150  
**Atributos:** 4 numéricos  
**Classes:** 3 espécies (50 amostras cada)

## Tecnologias Utilizadas

- **Python 3.11+**
- **Pandas** - Manipulação de dados
- **Scikit-learn** - Machine Learning
- **NumPy** - Cálculos numéricos
- **Jupyter Notebook** - Desenvolvimento

## Instalação e Execução

### Pré-requisitos
```bash
pip install pandas scikit-learn numpy jupyter
```

## Execução

```bash
#clone o repositório
git clone https://github.com/guumarques/AG002.git
#execute o seguinte arquivo - iris_knn.ipynb
```

## Metodologia, Implementação e Resultados

### 1. Pré-processamento
- Carregamento do dataset Iris
- Mapeamento das espécies para números inteiros:
  - `Iris-setosa` → 1
  - `Iris-versicolor` → 2
  - `Iris-virginica` → 3

### 2. Divisão dos Dados
- **80%** para treinamento (120 amostras)
- **20%** para teste (30 amostras)
- Embaralhamento aleatório dos dados

### 3. Modelo KNN
- Algoritmo: K-Nearest Neighbors
- Parâmetro: k=3 vizinhos
- Métrica de distância: Euclidiana

### 4. Avaliação
- Acurácia no conjunto de teste
- Relatório de classificação detalhado

## Como Usar

### Classificação Interativa
Execute o código e insira as medidas quando solicitado:

Comprimento da sépala (cm): 5.1
Largura da sépala (cm): 3.5
Comprimento da pétala (cm): 1.4
Largura da pétala (cm): 0.2

RESULTADO: A amostra pertence à espécie: setosa


### Exemplo de Uso Programático
```python
# Classificar uma nova amostra
nova_flor = [[5.1, 3.5, 1.4, 0.2]]
especie = modelo.predict(nova_flor)[0]
print(f"Espécie: {especie}")  # Output: 1 (setosa)
```

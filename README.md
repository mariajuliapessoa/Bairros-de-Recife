# Bairros-de-Recife
Este projeto tem como objetivo construir e analisar um grafo rotulado representando a interconectividade entre os bairros do Recife, utilizando dados fornecidos em um arquivo .csv. Com base nesse grafo, exploramos características estruturais, métricas de conectividade e caminhos ótimos entre pontos da cidade.


# 📌 Análise de Grafos: Conectividade entre Bairros do Recife

## 📖 Descrição do Projeto
Este projeto tem como objetivo construir e analisar um grafo rotulado representando a interconectividade entre os bairros do Recife, utilizando dados fornecidos em um arquivo `.csv`. Com base nesse grafo, exploramos características estruturais, métricas de conectividade e caminhos ótimos entre pontos da cidade.

## 🔍 Funcionalidades Implementadas
- Construção de um **grafo rotulado** conectando bairros via logradouros.
- Determinação de **tamanho, ordem e densidade** do grafo global e por microrregião.
- Cálculo do **grau de cada vértice** (número de conexões por bairro).
- Algoritmo para determinar a **distância entre dois endereços**, considerando pesos personalizados nas arestas.
- Identificação do **bairro mais denso** e do **bairro com maior grau**.
- Cálculo do **menor caminho** entre dois bairros (exemplo: de Nova Descoberta até Setúbal).
- Conversão do percurso encontrado em uma **árvore de caminhos**.
- Visualizações interativas do grafo e insights exploratórios.

## 🛠 Tecnologias Utilizadas
- `Python`
- `NetworkX` (manipulação de grafos)
- `Matplotlib` e `Plotly` (visualização de dados)
- `Pandas` (leitura e manipulação do CSV)
- `Jupyter Notebook` (análise exploratória)

## 📁 Estrutura do Repositório
```
📂 NomeDoProjeto
│── 📂 data
│   ├── bairros_recife.csv  # Dados de entrada
│── 📂 src
│   ├── grafo.py            # Implementação da estrutura do grafo
│   ├── analise.py          # Cálculo de métricas do grafo
│   ├── caminhos.py         # Algoritmos de menor caminho
│   ├── visualizacao.py     # Visualização do grafo
│   ├── arvore.py           # Conversão de percurso em árvore
│   ├── utils.py            # Funções auxiliares
│── 📂 notebooks
│   ├── Exploracao_Dados.ipynb  # Análise interativa dos dados
│── 📂 docs
│   ├── Relatorio.md        # Relatório detalhado do projeto
│── 📂 tests
│   ├── test_grafo.py       # Testes unitários
│   ├── test_caminhos.py    # Testes dos algoritmos de menor caminho
│── requirements.txt        # Dependências do projeto
│── README.md               # Documentação principal
│── .gitignore              # Arquivos a serem ignorados pelo Git
```

## 🚀 Como Executar o Projeto
### 1️⃣ Clonar o Repositório
```sh
git clone https://github.com/seu-usuario/seu-repositorio.git
cd NomeDoProjeto
```

### 2️⃣ Criar um Ambiente Virtual e Instalar Dependências
```sh
python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 3️⃣ Rodar a Construção do Grafo e as Análises
```sh
python src/grafo.py
python src/analise.py
python src/caminhos.py
```

### 4️⃣ Executar a Visualização Interativa
```sh
python src/visualizacao.py
```

## 📊 Exemplos de Saída
**Menor caminho entre dois bairros:**
```
Menor caminho entre Nova Descoberta e Setúbal:
Nova Descoberta → Bairro X → Bairro Y → Setúbal
Distância total: 15 km
```

**Bairro com maior grau:**
```
O bairro com maior grau é Boa Viagem, com 12 conexões.
```

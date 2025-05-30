# Projeto de Machine Learning - Predição de Sucesso em Tarefas de IA

Este projeto apresenta uma esteira completa de aprendizado de máquina para prever o sucesso em tarefas de desenvolvedores de IA, utilizando o dataset "AI Developer Productivity".

---

## Requisitos do Sistema

- Python 3.8 ou superior
- Git (opcional, para clonar o repositório)
- Jupyter Notebook ou VS Code com extensão Python

---

## Instalação e Configuração

### 1. Obtendo o Projeto

**Opção A: Download direto**
- Baixe os arquivos do projeto e extraia em uma pasta de sua escolha.

**Opção B: Clone via Git**
```bash
git clone <url-do-repositorio>
cd ia-produtividade
```

### 2. Configuração do Ambiente Virtual

O uso de ambiente virtual é altamente recomendado para evitar conflitos entre dependências.

#### Windows

**PowerShell:**
```powershell
cd ia-produtividade
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

**CMD:**
```cmd
cd ia-produtividade
python -m venv .venv
.\.venv\Scripts\activate.bat
python -m pip install --upgrade pip
pip install -r requirements.txt
```

#### Linux / macOS

```bash
cd ia-produtividade
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

---

### 3. Dependências Instaladas

O arquivo `requirements.txt` inclui:

- pandas (manipulação de dados)
- numpy (computação numérica)
- matplotlib (visualizações)
- scikit-learn (machine learning)

**Obs:** Se não houver um `requirements.txt`, instale manualmente:
```bash
pip install pandas numpy matplotlib scikit-learn
```

---

## Executando o Projeto

### Opção 1: Jupyter Notebook

- Abra o terminal com o ambiente virtual ativado e execute:
  ```bash
  jupyter notebook
  ```
- Abra o arquivo `esteira_aprendizado_aidev_productivity.ipynb`
- Execute as células sequencialmente (Shift + Enter)

### Opção 2: VS Code

- Abra o VS Code na pasta do projeto:
  ```bash
  code .
  ```
- Instale a extensão Python do VS Code (se necessário)
- Abra o arquivo `esteira_aprendizado_aidev_productivity.ipynb`
- Selecione o interpretador Python do ambiente virtual:
  - Pressione Ctrl + Shift + P
  - Digite "Python: Select Interpreter"
  - Escolha o Python da pasta `.venv`
- Execute as células clicando em "Run" ou usando Shift + Enter

---

## Estrutura do Projeto

```
ia-produtividade/
├── esteira_aprendizado_aidev_productivity.ipynb  # Notebook principal
├── ai_dev_productivity.csv                       # Dataset utilizado
├── README.md                                     # Este arquivo
└── .venv/                                        # Ambiente virtual (criado após setup)
```

---

## O que o Projeto Faz

### Objetivo

Prever o sucesso em tarefas de desenvolvedores de IA com base em dados comportamentais e de produtividade.

---

### Metodologia (9 Etapas)

1. **Dataset**: AI Developer Productivity
2. **Estatísticas Descritivas**: Análise exploratória dos dados
3. **Transformação em Colunas**: Codificação de variáveis categóricas
4. **Transformação em Linhas**: Remoção de outliers
5. **Divisão em 3 Conjuntos**: Treino, Validação, Teste
6. **Treinamento**: Modelo Random Forest
7. **Avaliação**: Matriz de confusão e acurácia
8. **Predição**: Exemplo prático com amostra do conjunto de teste
9. **Documentação**: Comentários e explicações no notebook

---

## Resultados Esperados

- Acurácia: ~80-90% (pode variar conforme o split)
- Modelo: Random Forest
- Visualizações: Matriz de confusão

---

## Resolução de Problemas

**Erro: "Module not found"**
- Certifique-se de que o ambiente virtual está ativado
- Reinstale as dependências: `pip install -r requirements.txt`

**Jupyter não abre**
- Instale o Jupyter: `pip install jupyter`
- Ou use o notebook do VS Code

---

## Desativando o Ambiente Virtual

Quando terminar de usar o projeto:
```bash
deactivate
```

---

## Licença

Este projeto é para fins educacionais e de aprendizado em Machine Learning.

---

**Objetivo Educacional:** Este projeto demonstra uma esteira completa de Machine Learning, desde a análise exploratória até a predição final, seguindo as melhores práticas da área.
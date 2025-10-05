# 🎯 Projeto Disciplina Tópicos em Computação em Nuvem


Este projeto foca no desenvolvimento e treinamento de um modelo de deep learning para classificar doenças de plantas a partir de imagens de folhas. O modelo é otimizado para implantação em dispositivos embarcados como o Raspberry Pi.

**Status do Projeto:** Em Desenvolvimento

---

### 📌 Tabela de Conteúdos

- [🚀 Visão Geral](#🚀-visão-geral)
- [✨ Funcionalidades](#✨-funcionalidades)
- [🛠️ Tecnologias Utilizadas](#🛠️-tecnologias-utilizadas)
- [📋 Pré-requisitos](#📋-pré-requisitos)
- [🚀 Como Usar o UV e Executar o Projeto](#🚀-como-usar-o-uv-e-executar-o-projeto)
- [📁 Estrutura do Projeto](#📁-estrutura-do-projeto)
- [🤝 Como Contribuir](#🤝-como-contribuir)
- [👨‍💻 Autor](#👨‍💻-autor)
- [🌿 Plant Disease Detection with TensorFlow and Keras](#🌿-plant-disease-detection-with-tensorflow-and-keras)
- [1. Project Overview](#1-project-overview)
- [2. Setup and Installation](#2-setup-and-installation)
- [3. Running the Project](#3-running-the-project)
- [4. Project Structure (DD)](#4-project-structure-dd)

---

### 🚀 Visão Geral

Este projeto tem como objetivo explorar e aplicar conceitos avançados de computação através de experimentos práticos e análises de dados. Através de **notebooks Jupyter**, são realizadas análises exploratórias, desenvolvimento de modelos e visualizações interativas, permitindo um aprendizado *hands-on* sobre as tecnologias estudadas na disciplina.

---

### ✨ Funcionalidades

- **Análise de Dados:** Processamento e visualização de dados utilizando `pandas` e `matplotlib`.
- **Experimentação Interativa:** Desenvolvimento e teste de hipóteses em notebooks Jupyter.
- **Reprodutibilidade:** Configuração de ambiente isolado e controlado com `uv`.
- **Desenvolvimento Colaborativo:** Estrutura organizada para trabalho em equipe.

---

### 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python
- **Gerenciamento de Projetos:** [uv](https://astral.sh/uv)
- **Ambiente Interativo:** [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/)
- **Principais Bibliotecas:**
    - [pandas](https://pandas.pydata.org/) - Para manipulação e análise de dados
    - [matplotlib](https://matplotlib.org/) - Para criação de visualizações e gráficos
    - [numpy](https://numpy.org/) - Para computação numérica
    - [jupyter](https://jupyter.org/) - Para notebooks interativos
    - [TensorFlow/Keras](https://www.tensorflow.org/) - Para Deep Learning e modelos de classificação de imagens**
    - [scikit-learn](https://scikit-learn.org/stable/) - Para ferramentas de machine learning e avaliação de modelos**

---

### 📋 Pré-requisitos

Antes de começar, você precisa ter o **uv** instalado em sua máquina. É uma ferramenta extremamente rápida para gerenciar projetos Python, escrita em Rust.

**Instalação no macOS e Linux:**
```bash
curl -LsSf [https://astral.sh/uv/install.sh](https://astral.sh/uv/install.sh) | sh
```

# 🚀 Como Usar o UV e Executar o Projeto

Siga estes passos para configurar o ambiente e executar os notebooks.

---

## 1. Clonar e Acessar o Repositório

```bash
git clone https://github.com/ericmochiutti/projeto_topicos.git
cd projeto_topicos
uv sync
```

## 2. Configuração do Dataset

A seção de **Detecção de Doenças de Plantas** requer o **PlantVillage dataset**.

1. Baixe o dataset completo no formato **ZIP/RAR** a partir do [PlantVillage dataset no Kaggle](https://www.kaggle.com/).
2. Descompacte todo o conteúdo.
3. Mova a pasta descompactada (`PlantVillage` ou similar) para o diretório `data/` na raiz deste projeto.

A estrutura de diretórios esperada deve ser:

projeto_topicos/
├── data/
│ └── PlantVillage/
│ ├── ... (todas as subpastas de classes de doenças)
└── ...

### Estrutura do Projeto

- `data/` – Contém o dataset **PlantVillage**.  
- `model/` – Armazena os modelos treinados nos formatos `.h5`, `.keras` e `.tflite`.  
- `notebook/` – Contém o notebook principal em Jupyter com o código completo do projeto.  
- `pyproject.toml` – Define as dependências do projeto para o `uv`.
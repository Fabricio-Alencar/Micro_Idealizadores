# 💡 Projack Impulse — Microsserviço de Gestão de Idealizadores

> Microsserviço responsável pelo gerenciamento de idealizadores (criadores de projetos) na plataforma **Projack Impulse**.

## 📌 Sobre o Microsserviço

O **Micro_Idealizadores** é um serviço independente desenvolvido em Python responsável pela gestão e manutenção dos dados relativos aos idealizadores de projetos no sistema.

Ele faz parte do ecossistema de microsserviços do **Projack Impulse** e provê endpoints para criação, edição e consulta dos perfis dos criadores de projetos.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.12 (`runtime.txt`)
* **API / Servidor:** Python (`main.py`)
* **Banco de Dados:** SQLite (`banco.db`) com gerenciamento em `database.py`
* **Modelagem de Dados:** `models.py`
* **Servidor de Produção:** Gunicorn (`startup.sh`)

## 🏗️ Estrutura do Projeto

```text
Micro_Idealizadores-main/
│
├── banco.db           # Banco de dados SQLite
├── database.py        # Módulo de conexão e configuração do banco
├── main.py            # Ponto de entrada da API e definição das rotas
├── models.py          # Modelos e esquemas de dados
├── requirements.txt   # Dependências do projeto
├── runtime.txt        # Versão do Python (3.12)
├── startup.sh         # Script de inicialização
└── README.md          # Documentação do microsserviço

```

## 🚀 Como Executar Localmente

### Pré-requisitos

* Python 3.12
* Git e pip

### 1. Clone o repositório e entre na pasta

```bash
git clone https://github.com/Fabricio-Alencar/Micro_Idealizadores.git
cd Micro_Idealizadores-main

```

### 2. Crie e ative um ambiente virtual

* **Linux/macOS:**
```bash
python3 -m venv venv
source venv/bin/activate

```


* **Windows:**
```bash
python -m venv venv
venv\Scripts\activate

```



### 3. Instale as dependências

```bash
pip install -r requirements.txt

```

### 4. Execute a aplicação

```bash
python main.py

```

Ou via script de inicialização:

```bash
bash startup.sh

```

## 🔗 Integração com o Ecossistema

Este microsserviço fornece a API para criação e gestão dos idealizadores, conectando os perfis dos criadores aos projetos no **Projack Impulse**.

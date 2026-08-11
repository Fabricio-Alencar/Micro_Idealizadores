# 💡 Projack Impulse — Microsserviço de Gestão de Idealizadores

> Microsserviço responsável pelo gerenciamento de idealizadores (criadores de projetos) na plataforma **Projack Impulse**[cite: 7].

## 📌 Sobre o Microsserviço

O **Micro_Idealizadores** é um serviço independente desenvolvido em Python responsável pela gestão e manutenção dos dados relativos aos idealizadores de projetos no sistema[cite: 7].

Ele faz parte do ecossistema de microsserviços do **Projack Impulse** e provê endpoints para criação, edição e consulta dos perfis dos criadores de projetos[cite: 7].

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.12 (`runtime.txt`)[cite: 7]
* **API / Servidor:** Python (`main.py`)[cite: 7]
* **Banco de Dados:** SQLite (`banco.db`) com gerenciamento em `database.py`[cite: 7]
* **Modelagem de Dados:** `models.py`[cite: 7]
* **Servidor de Produção:** Gunicorn (`startup.sh`)[cite: 7]

## 🏗️ Estrutura do Projeto

```text
Micro_Idealizadores-main/
│
├── banco.db           # Banco de dados SQLite[cite: 7]
├── database.py        # Módulo de conexão e configuração do banco[cite: 7]
├── main.py            # Ponto de entrada da API e definição das rotas[cite: 7]
├── models.py          # Modelos e esquemas de dados[cite: 7]
├── requirements.txt   # Dependências do projeto[cite: 7]
├── runtime.txt        # Versão do Python (3.12)[cite: 7]
├── startup.sh         # Script de inicialização[cite: 7]
└── README.md          # Documentação do microsserviço[cite: 7]

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


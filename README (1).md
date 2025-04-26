# 📦 E-Shop Brasil NoSQL - CRUD com MongoDB e Streamlit

Este projeto é uma aplicação de exemplo para a empresa fictícia **E-Shop Brasil**, utilizando tecnologias modernas como **MongoDB**, **Streamlit**, **Docker** e **Python**.

A aplicação permite realizar operações **CRUD** (Criar, Ler, Atualizar e Deletar) em uma base de dados **NoSQL**.

## ✨ Tecnologias Usadas

- **MongoDB** (banco de dados NoSQL)
- **Streamlit** (interface web simples)
- **Docker** (containerizar MongoDB)
- **Python** (linguagem principal)
- **Faker** (geração de dados falsos)

## 🛠️ Como Rodar o Projeto

### 1. Clone o Repositório
Primeiro, clone este projeto em sua máquina:

```bash
git clone https://github.com/seu-usuario/e-shop-brasil-nosql.git
cd e-shop-brasil-nosql
```

> Se preferir, apenas crie a pasta manualmente e copie os arquivos.

### 2. Suba o MongoDB com Docker
Dentro da pasta principal (`e-shop-brasil-nosql/`), execute:

```bash
docker-compose up -d
```

### 3. Instale as Dependências Python
Entre na pasta `app/`:

```bash
cd app
```

Instale as bibliotecas necessárias:

```bash
pip install -r requirements.txt
```

### 4. Gere os Dados de Exemplo
Execute o gerador de dados para criar **1 milhão** de produtos falsos:

```bash
python data_generator.py
```

### 5. Rode a Aplicação Streamlit
Agora, rode a aplicação com:

```bash
streamlit run app.py
```

O navegador abrirá automaticamente com a interface do sistema.

## 📋 Funcionalidades Disponíveis

- **Adicionar Produto**: cadastrar novos produtos.
- **Listar Produtos**: ver todos os produtos cadastrados.
- **Atualizar Produto**: alterar informações de um produto existente.
- **Deletar Produto**: excluir um produto do banco de dados.

## 🗂️ Estrutura de Pastas

```
e-shop-brasil-nosql/
│
├── docker-compose.yml
├── README.md
└── app/
    ├── app.py
    ├── crud.py
    ├── db_connection.py
    ├── data_generator.py
    └── requirements.txt
```

## ⚙️ Configurações Importantes

- O MongoDB roda localmente em `localhost:27017`.
- O banco de dados se chama `eshop_db`.
- A coleção usada é `products`.

## 👨‍💻 Autor

Desenvolvido como parte do projeto de modernização de infraestrutura da **E-Shop Brasil**.

## 📽️ Entrega Final

- ✅ Código fonte no GitHub
- ✅ Docker funcionando para MongoDB
- ✅ Geração automática de 1 milhão de registros
- ✅ Aplicação CRUD completa via Streamlit
- ✅ Vídeo explicativo (caso necessário)

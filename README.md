# API_RECEITAS
API que permite CRUD de ingredientes e receitas


Este projeto utilizou Django Framework e Django REST Framework para criar e executar a API localmente. O banco de dados utilizado foi SQLite, um BD simples que vem embutida com a instalação do Python 3.

# Como instalar e executar o Projeto

1. Clonando o Repositório
   Primeiro, faça o **clone** deste repositório para a máquina local:
    ```bash
         git clone https://github.com/usuario/recipes_project.git
         cd recipes_project

3. Instalar as dependências
   No diretório do projeto, instale as dependências usando o pip:
   ```bash
              pip install -r requirements.txt

4. Acessar o diretório do projeto:
   ```bash
            cd recipes_project/

5. Executar a API localmente
  Com tudo configurado, você pode agora rodar a API localmente. No terminal, execute o comando:
   ```bash
         .../recipes_project/py manage.py runserver
   
A API oferece os seguintes endpoints para CRUD (Criar, Ler, Atualizar e Deletar) de ingredientes e Receitas:

**INGREDIENTES**
- **GET** `/ingredientes`: Retorna todos os ingredientes.
- **GET** `/ingredientes/<id>`: Retorna um ingrediente específico pelo nome.
- **POST** `/ingredientes`: Adiciona um novo ingrediente.
- **PUT** `/ingredientes/<id>`: Atualiza as informações de um ingrediente existente.
- **DELETE** `/ingredientes/<id>`: Exclui um ingrediente.

**RECEITAS**
- **GET** `/receitas`: Retorna todos as receitas.
- **GET** `/receitas/<nome%20...>`: Retorna uma receita específica pelo nome.
- **POST** `/receitas`: Adiciona uma nova receita.
- **PUT** `/receitas/<nome%20...>`: Atualiza as informações de uma receita existente.
- **DELETE** `/receitas/<nome%20...>`: Exclui uma receita.

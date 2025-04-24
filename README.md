# RECIPES_PROJECT
API que permite CRUD de ingredientes e receitas


Este projeto utilizou Django Framework e Django REST Framework para criar e executar a API localmente. O banco de dados utilizado foi SQLite, um BD simples que vem embutida com a instalação do Python 3.

# Como instalar e executar o Projeto
1. Instalando o git
   Caso não possua o git em seu computador, execute o comando abaixo (Windows):
    ```bash
          winget install --id Git.Git -e --source winget
    
2. Clonando o Repositório
   Faça o **clone** deste repositório para a máquina local:
    ```bash
         git clone https://github.com/Johnnywbs/recipes_project.git
         cd recipes_project

3. Instalar as dependências
   No diretório do projeto, instale as dependências usando o pip:
   ```bash
              pip install -r requirements.txt

4. Executar a API localmente
  Com tudo configurado, você pode agora rodar a API localmente. No terminal, execute o comando:
   ```bash
         .../recipes_project/py manage.py runserver
   
A API oferece os seguintes endpoints para CRUD (Criar, Ler, Atualizar e Deletar) de ingredientes e Receitas:

**INGREDIENTES**
- **GET** `http://127.0.0.1:8000/ingredientes/`: Retorna todos os ingredientes.
- **GET** `http://127.0.0.1:8000/ingredientes/<id>`: Retorna um ingrediente específico pelo id.
- **POST** `http://127.0.0.1:8000/ingredientes/`: Adiciona um novo ingrediente.
- **PUT** `http://127.0.0.1:8000/ingredientes/<id>`: Atualiza as informações de um ingrediente existente.
- **DELETE** `http://127.0.0.1:8000/ingredientes/<id>`: Exclui um ingrediente.

**RECEITAS**
- **GET** `http://127.0.0.1:8000/receitas/`: Retorna todas as receitas.
- **GET** `http://127.0.0.1:8000/receitas/<id>`: Retorna uma receita específica pelo id.
- **POST** `http://127.0.0.1:8000/receitas/`: Adiciona uma nova receita.
- **PUT** `http://127.0.0.1:8000/receitas/<id>`: Atualiza as informações de uma receita existente.
- **DELETE** `http://127.0.0.1:8000/recipes/<id>`: Exclui uma receita.

Os ingredientes são adicionados às receitas por meio de objetos JSON, como no exemplo abaixo:
```code
    {
        "nome": "XXXXXXX",
        "modo_preparo": "XXXXX XXXXX XXXX XXXXX XXXX",
        "ingredientes": [
            {
                "ingrediente": {
                    "nome": "ABCD",
                    "unidade_medida": "g"
                },
                "quantidade": X.XX
            }
        ]
    }

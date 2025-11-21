# Projeto 1 – IEI

# Instalação do WordPress com Docker Compose (WordPress + MariaDB)

Este projeto configura um ambiente WordPress ao usar Docker Compose para criar um site de anúncios da turma de forma simples e reprodutível.



# Requisitos:

- WSL2 (Ubuntu)

- Docker Desktop com integração WSL

- Git

# Como levantar o projeto:

# Passo 1:

git clone https://github.com/Git-MiguelSilva/site-anuncios-turma
cd site-anuncios-turma

# Passo 2:

cp .env.example .env

# Passo 2.1(opcional):

nano .env #para modificar as credenciais se for desejado

# Passo 3:

docker compose up -d

Agora se for ao site http://localhost:8080/ deve aparecer lá para fazer a instalação do WordPress!

# Quando quiser desligar o site tem duas escolhas:

No WSL:

docker compose down #Se quiser ficar com os volumes do site

docker compose down -v #Se quiser que o site volte ao 0, pedindo a instalação outra vez

# Importar o site já configurado (anúncios + tema)

Depois de concluir a instalação do WordPress:

Entrar no painel de administração:
http://localhost:8080/wp-admin

No menu do WordPress, ir a:
Ferramentas → Importar → WordPress

Se necessário, instalar o importador de WordPress.

Importar o ficheiro:

export/anunciosturma.xml


Atribuir o conteúdo a um utilizador e confirmar a importação dos ficheiros.


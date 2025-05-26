[README.md](https://github.com/user-attachments/files/20433369/README.md)
[Uploading READ
#  Projeto: Gerenciador de Tarefas e Disciplinas

##  Tema do Projeto

O tema escolhido pelo grupo é um **Sistema Web para Gerenciamento de Tarefas e Disciplinas**. O objetivo é permitir que estudantes possam cadastrar, visualizar e organizar suas tarefas escolares e disciplinas em um único lugar.

O sistema oferece uma interface simples para cadastrar tarefas com prazos, bem como disciplinas com informações como matéria, professor e curso.

---

##  Funcionalidades Implementadas

###  Tarefas
- Cadastrar nova tarefa com:
  - Descrição
  - Data de início
  - Data final
- Listar todas as tarefas registradas

###  Disciplinas
- Cadastrar nova disciplina com:
  - Nome da matéria
  - Nome do professor
  - Curso relacionado
- Listar todas as disciplinas cadastradas

---

##  Como rodar o projeto localmente

### 1. Clone o repositório:

faca download deste repositório: https://github.com/mmarianaPinho/1023A-backend-main-main/tree/main/1023A-backend-main-main
### 2. no terminal digite:
npm install
### 3.  no myslq coloque
```
CREATE DATABASE ListarTarefas;

USE ListarTarefas;

CREATE TABLE tarefas (

    id INT PRIMARY KEY AUTO_INCREMENT,
    descricao VARCHAR(300),
    prazoInicial text,
    prazoFinal text
);

CREATE TABLE disciplinas (

    id INT PRIMARY KEY AUTO_INCREMENT,
    materia VARCHAR(100),
    professor VARCHAR(100),
    curso VARCHAR(100)
);
```
### 4. no terminal digite:

npm run dev

## Exemplo de fluxograma:
Usuário preenche o formulário de tarefas e clica em "Cadastrar".

O JS envia uma POST /tarefas para o servidor.

O Fastify processa os dados e insere no MySQL.

O frontend recarrega a lista com GET /tarefas.

## diagrama
```barry
Usuário - Navegador
      |     
      | (HTML + JS + CSS)
      |
Frontend (index.html, cadastro.html, disciplina.html)
      |
      | → Requisições HTTP (GET: Buscar dados / POST: Criar dados)
      |
Backend Fastify (index.ts)
      |
      | → Validação dos dados
      | → Execução de querys SQL (SELECT, INSERT)
      |
Banco de Dados MySQL
      | → Armazena e retorna informações


ME.md…]()

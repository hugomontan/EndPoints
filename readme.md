# Módulo 2 Aula 04 

Explicação de alguns conceitos utilizados durante o exercício e desenvolvimento do projeto

## Models

Models é o elemento da arquitetura MVC responsável por realizar as ações no banco de dados de acordo com as requisições passadas pelo Controller

- models/aluno.js

Responsável por fazer o CRUD na tabela aluno de acordo com o que é passado pelo controllers/alunoController.js

- models/curso.js

Responsável por fazer o CRUD na tabela curso de acordo com o que é passado pelo controllers/cursoController.js

- models/professor.js

Responsável por fazer o CRUDO na tabela professor de acordo com o que é passado pelo controllers/professorController.js 

## Controller

- controllers/alunoController.js

Responsável por mandar as ações que o models/aluno.js deve fazer de acordo com o que o usuário selecionar no views/alunos/index.ejs.

- controllers/cursoController.js

Responsável por mandar as ações que o models/curso.js deve fazer de acordo com o que o usuário selecionar no views/alunos/index.ejs.

- controllers/professorController.js

Responsável por mandar as ações que o models/professor.js deve fazer de acordo com o que o usuário selecionar no view/professores/index.ejs

## Endpoint

São os caminhos da URL para mostrar a view da aplicação de acordo com a construção da plataforma.

- /alunos

Mostra a views/alunos/index.ejs para mostrar as ações possíveis em relação ao aluno e curso
  
- /professores

Mostra a views/professores/index.ejs para mostrar as ações possíveis em relação aos professores.
  

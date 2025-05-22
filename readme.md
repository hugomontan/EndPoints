# Módulo 2 - Aula 04

Explicação de alguns conceitos utilizados durante o exercício e o desenvolvimento do projeto.

---

## 📦 Models

Os **Models** são responsáveis por realizar as operações no banco de dados, seguindo as instruções recebidas dos Controllers. São a camada da arquitetura **MVC** que interage diretamente com as tabelas.

- **models/aluno.js**  
  Responsável por realizar as operações de **CRUD** (Create, Read, Update, Delete) na tabela `aluno`, conforme as instruções enviadas pelo `controllers/alunoController.js`.

- **models/curso.js**  
  Responsável por realizar as operações de **CRUD** na tabela `curso`, conforme as instruções enviadas pelo `controllers/cursoController.js`.

- **models/professor.js**  
  Responsável por realizar as operações de **CRUD** na tabela `professor`, conforme as instruções enviadas pelo `controllers/professorController.js`.

---

## 🕹️ Controllers

Os **Controllers** são responsáveis por processar as requisições do usuário, definir as regras de negócio e repassar as instruções para os Models executarem.

- **controllers/alunoController.js**  
  Processa as ações relacionadas aos alunos e define as operações que o `models/aluno.js` deve executar, de acordo com as escolhas feitas pelo usuário na interface `views/alunos/index.ejs`.

- **controllers/cursoController.js**  
  Processa as ações relacionadas aos cursos e define as operações que o `models/curso.js` deve executar, com base nas interações do usuário na interface `views/alunos/index.ejs`.

- **controllers/professorController.js**  
  Processa as ações relacionadas aos professores e define as operações que o `models/professor.js` deve executar, conforme as escolhas feitas pelo usuário na interface `views/professores/index.ejs`.

---

## 🌐 Endpoints

Os **Endpoints** são os caminhos definidos na URL que direcionam para as views da aplicação, permitindo que o usuário acesse e interaja com diferentes funcionalidades da plataforma.

- **/alunos**  
  Exibe a view `views/alunos/index.ejs`, mostrando as ações possíveis em relação aos alunos e cursos.

- **/professores**  
  Exibe a view `views/professores/index.ejs`, mostrando as ações possíveis em relação aos professores.


---

**1) Explique com suas palavras o papel de cada camada da arquitetura MVC usada neste projeto.  
Como o Model, o Controller e a View interagem entre si?**

O **Model** cuida dos dados, ele pega e guarda as informações no banco de dados.  
O **Controller** recebe o que o usuário quer fazer, manda o Model fazer e depois escolhe o que mostrar.  
A **View** é a tela, ela mostra as informações para o usuário.

Eles funcionam assim: o usuário faz algo → o Controller recebe → o Model mexe no banco → a View mostra o resultado.

---

**2) Como ocorre o envio e o recebimento de dados no formato JSON neste projeto?  
Cite uma rota que responde em JSON e explique seu funcionamento.**

Acontece quando o sistema troca dados com o usuário ou outro sistema, usando JSON.  
Por exemplo, a rota `/alunos` pode responder em JSON com a lista de alunos. Quando alguém faz uma requisição, o Controller pega os dados no Model e responde com um JSON.

---

**3) Qual a importância de usar HTML básico com formulários e tabelas para organizar e manipular dados no navegador?  
Por que esse tipo de estrutura ainda é útil em projetos back-end com Node.js?**

É importante porque o HTML básico é simples e funciona em qualquer navegador.  
Formulários e tabelas ajudam a organizar e enviar informações de forma fácil.  
Mesmo com Node.js, usar isso é útil porque permite que o usuário interaja com o sistema sem precisar de coisas complicadas, só com o navegador mesmo.

# Sistema de Cadastro de Professores, Alunos e Turmas
Este é um projeto desenvolvido com Flask para gerenciar o cadastro
de professores, alunos e turmas. Através de uma API RESTful, é
possível realizar operações como listar, cadastrar, atualizar e
deletar professores, alunos e turmas.
## Requisitos
- Python 3.x
- Flask
## Instalação
1. Clone o repositório ou baixe os arquivos.
```bash
git clone <URL_DO_REPOSITORIO>
cd <DIRETORIO_DO_PROJETO>
Crie e ative um ambiente virtual (opcional, mas recomendado).
python -m venv venv
source venv/bin/activate # Para sistemas Unix
venv\Scripts\activate # Para Windows
Instale as dependências.
pip install -r requirements.txt
Caso não tenha o arquivo requirements.txt, instale o Flask diretamente.
pip install Flask
Como Rodar o Projeto
Para rodar a aplicação, execute o seguinte comando:
python app.py
A aplicação será iniciada no endereço http://127.0.0.1:5000/.
Endpoints
A aplicação possui os seguintes endpoints:
Professores
GET /professores: Lista todos os professores.
POST /professores: Cadastra um novo professor.
PUT /professores/int:index: Atualiza os dados de um professor.
DELETE /professores/int:index: Deleta um professor.
Alunos
GET /alunos: Lista todos os alunos.
POST /alunos: Cadastra um novo aluno.
PUT /alunos/int:index: Atualiza os dados de um aluno.
DELETE /alunos/int:index: Deleta um aluno.
Turmas
GET /turma: Lista todas as turmas.
POST /turma: Cadastra uma nova turma.
PUT /turma/int:index: Atualiza os dados de uma turma.
DELETE /turma/int:index: Deleta uma turma.
Exemplos de Requisições
Cadastrar Professor
POST /professores
{
 "nome": "Professor Pedro",
 "disciplina": "Geografia"
}
Cadastrar Aluno
POST /alunos
{
 "nome": "Aluno João",
 "idade": 20,
 "matricula": "12345"
}
Cadastrar Turma
POST /turma
{
 "nome": "Turma A",
 "professor_id": 1,
 "alunos": [1, 2]
}
Contribuindo
Sinta-se à vontade para contribuir com melhorias, correções de bugs ou novas
funcionalidades. Para isso, basta seguir os passos abaixo:
Faça um fork do projeto.
Crie uma branch para a sua feature (git checkout -b nova-feature).
Faça as modificações necessárias.
Comite suas mudanças (git commit -am 'Adicionando nova feature').
Faça o push para a branch (git push origin nova-feature).
Crie um pull request.

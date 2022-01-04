<h1 align="center"> API Financeira</h1>

<h3 align="center">
    Criação de uma API para controle bancário.
</h3>

<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/MiguelMarcola/finance-api?color=%2304D361">

  <img alt="Repository size" src="https://img.shields.io/github/repo-size/MiguelMarcola/finance-api">
  
  <a href="https://github.com/MiguelMarcola/finance-api/commits/main">
    <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/MiguelMarcola/finance-api">
  </a>
    
   <img alt="License" src="https://img.shields.io/badge/license-MIT-brightgreen">
  
  <img alt="Feito pela Rocketseat" src="https://img.shields.io/badge/feito%20por-Miguel-%237519C1">
  
 
</p>

<h4 align="center">
	🚧   Concluído 🚀 🚧
</h4>

### Requisitos

- [X] Deve ser possível criar uma conta
- [X] Deve ser possível buscar o extrato
- [X] Deve ser possível realizar um depósito
- [X] Deve ser possível realizar um saque
- [X] Deve ser possível buscar o extrato bancário do cliente por data
- [X] Deve ser possível atualizar dados da conta do cliente
- [X] Deve ser possível obter dados da conta do cliente
- [X] Deve ser possível deletar uma conta
- [X] Deve ser possível retornar o balance

### Regras de negócio

- [X] Não deve ser possível cadastrar uma conta com o CPF já existente 
- [X] Não deve ser possível buscar extrato em uma conta não existente
- [X] Não deve ser possível fazer depósito em uma conta não existente
- [X] Não deve ser possível fazer saque em uma conta não existente 
- [X] Não deve ser possível fazer saque quando o saldo for insuficiente
- [X] Não deve ser possível excluir uma conta não existente

## 🛠 Tecnologias

#### [NodeJS](https://nodejs.org/)  +  [Express](https://expressjs.com/pt-br/))

## 🚀 Como executar o projeto

- Clonando a aplicação:

<pre>
<code>
  git clone https://github.com/MiguelMarcola/finance-api.git
</code>
</pre>

- Executando 

<pre>
<code>
  yarn
  yarn dev
</code>
</pre>

<pre>
<code>
  // Rotas da Aplicação

  // O cpf deve ser passado no Header das requisições para validação dos dados
  
  // GET

  //Retorna a conta do cpf do Header
  http://localhost:3333/account

  //Retorna as transações do cpf do Header
  http://localhost:3333/statement

  //Retorna o saldo do cpf do Header
  http://localhost:3333/balance

  //Retorna as transações feitas no dia enviado na Query referentes ao cpf no Header
  http://localhost:3333/statement/date?date={data}

  // Post

  //Para criar uma conta
  http://localhost:3333/account

    {
        "cpf": "11111111",
        "name": "Teste 1"
    }

  //Para realizar um depósito na conta referente ao cpf no Header 
  http://localhost:3333/deposit

    {
        "description": "transfer test",
        "amount": 500.00
    }


  //Para realizar uma retirada na conta referente ao cpf no Header 
  http://localhost:3333/withdraw

    {
        "amount": 100
    }

  // PUT

  //Para alterar o nome na conta referente ao cpf no Header 
  http://localhost:3333/account

    {
        "name": "New name"
    }

  // DELETE
  //Para excluir a conta referente ao cpf no Header
  http://localhost:3333/account

</code>
</pre>

## 🦸 Autor

<img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/95949825?s=400&u=71abea02fa5086704e648496f0de845501599ca0&v=4" width="100px;" alt=""/>
 <br />
 <sub><b>Miguel Marçola</b></sub></a> 🚀
 <br />

[![Linkedin Badge](https://img.shields.io/badge/-Miguel-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/miguel-mar%C3%A7ola-28535a151/)](https://www.linkedin.com/in/miguel-mar%C3%A7ola-28535a151/) 
[![Gmail Badge](https://img.shields.io/badge/Miguel%20Mar%C3%A7ola-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:miguelmarcola@gmail.com)](miguelmarcola@gmail.com)

---

## 📝 Licença

Este projeto esta sobe a licença [MIT](./LICENSE).

Feito com muita dedicação por Miguel Marçola 👋🏽 [Entre em contato!](https://www.linkedin.com/in/miguel-mar%C3%A7ola-28535a151/)

---

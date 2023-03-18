# MongoDB
Atividade MongoDB

Repositório para Anexo referente a Banco de Dados não relacional 

Comando: show dbs
Função: Mostra todos os Bancos de Dados criados no MongoDB 

Comando: use aula
Função: Seleciona o banco citado para criação/pesquisa 

Comando: show collection
Função: Mostra as coleções criadas no banco de dados atual 

Comando: db.livros.count()
Função: Conta todos os itens da coleção 

Comando: db.livros.count({pageCount:{$lte: 100}})
Função: Faz uma contagem dos os livros que tenha a quantidade de páginas menor ou igual a 100

Comando: db.livros.count({isbn:{$gt: "1933988746"}})
Função: Retornará os livros que tenham o campo "isbn" maiores que 1933988746 

Comando: db.livros.find({title: /G/, isbn: {$tle:1617200000}})
Função: Consulta os livros com o campo "isbn" menor ou igual a "1617200000" que tenha o titulo com a letra "G" no início

Comando: db.livros.find({isbn: "10"}}).limit(2)
Função: Consulta os livros com o campo "isbn" igual a 10, mas só irá aparecer 2 livros(.limit) 

Comando: db.livros.find({title: /Windows/}).count()
Função: Conta os livros que tenha o titulo "Windows"

Comando: db.livros.find({}).sort({"pageCount": -1}).limit(2)
Função: Consulta os livros pela quantidade de folhas na ordem decrescente(.sort) com o limite de visualização de 2 itens(.limit)

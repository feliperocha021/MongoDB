# Databases

Mostra todos os banco de dados:
``show dbs``

Usar/Criar um tipo de banco de dados:
``use db_name``

Criar uma coleção em um banco de dados:
``db.createCollection("collection_name")``

Excluir o banco de dados atual:
``db.dropDatabase()``

Inserir um documento em um banco de dados atual:
``db.collection_name.insertOne({name: "Spongebob",age: 30})``

Retornar todos os documentos de uma coleção
``db.collection_name.find()``

Inserir vários documentos em um banco de dados atual:
``db.collection_name.insertMany([{name: "Spongebob",age: 30}, {name: "Patrick",age: 38}])``

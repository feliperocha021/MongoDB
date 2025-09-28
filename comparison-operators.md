# Comparison Operators

``$eq`` → Igual a.. Exemplo: { idade: { $eq: 25 } } → retorna documentos onde idade = 25.

``$ne`` → Diferente de. Exemplo: { status: { $ne: "ativo" } }.

``$gt`` → Maior que. Exemplo: { preco: { $gt: 100 } }.

``$gte`` → Maior ou igual a. Exemplo: { idade: { $gte: 18 } }.

``$lt`` → Menor que. Exemplo: { estoque: { $lt: 50 } }.

``$lte`` → Menor ou igual a. Exemplo: { desconto: { $lte: 0.2 } }.

``$in`` → Valor dentro de uma lista. Exemplo: { cor: { $in: ["azul", "verde"] } }.

``$nin`` → Valor não está na lista. Exemplo: { categoria: { $nin: ["eletronico", "roupa"] } }.


## Exemplos

``db.collection_name.find({name: {$ne: "Spongebob"}})``

``db.collection_name.find({age: {$lt: 27}})``

``db.collection_name.find({age: {$gte: 18, lte: 30}})``
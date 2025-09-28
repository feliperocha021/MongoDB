# Sorting and Limiting

Retornar todos os documentos com base em alguma classificação. Neste exemplo em ordem crescente:
``db.collection_name.find().sort({name:1})``

Limitar a quantidade de documentos:
``db.collection_name.find().sort({name:-1}).limit(5)``


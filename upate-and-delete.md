# Update

``db.collection_name.updateOne(filter, update)``
- ``filter``: critério de seleção
- ``update``: parâmetro de atualização

Criar/Atualizar propriedade(s) de um documento:
``db.collection_name.updateOne({_id: ObjectId("507f1f77bcf86cd799439011")}, {$set: {fullTime: true}})``

Destruir propriedade(s) de um documento:
``db.collection_name.updateOne({_id: ObjectId("507f1f77bcf86cd799439011")}, {$unset: {fullTime: ""}})``

Atualizar muitos documeentos:
``db.collection_name.updateMany({fullTime: {$exists: false}}, {$set: {fullTime: true}})``

# Delete

Excluir um documento:
``db.collection_name.deleteOne({_id: ObjectId("507f1f77bcf86cd799439011")})``

Excluir vários documentos:
``db.collection_name.deleteMany({registerDate: {$exists: false}})``

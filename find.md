# Find

Buscando documentos especificos .find({query}, {projection}). Neste exemplo estamos passandos as queries e o retorno terá apenas a propriedade name:
``db.collection_name.find({age: 30, fullTime: false}, {_id: false, name: true})``

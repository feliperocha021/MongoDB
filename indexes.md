# Indexes

Permite pesquisa rápida de um campo, no entando, ele ocupa mais memória e retarda as operações de iserção, atualização e remoção.

Campos que à alta pesquisa e pouca atualização, um índice é uma boa sugestão.

``db.students.createIndex({name: 1})``

Ao realizar uma busca por nome é bem mais rápido
``db.students.find({name: "Larry"})``

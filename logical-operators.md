# Logical Operators

Os operadores lógicos permitem combinar múltiplas condições em uma consulta.

## $and
Retorna documentos que atendem **todas** as condições especificadas.

```js
db.usuarios.find({
  $and: [
    { idade: { $gte: 18 } },
    { ativo: true }
  ]
})
```

## $or
Retorna documentos que atendem pelo menos uma das condições.
```js
db.produtos.find({
  $or: [
    { categoria: "eletronico" },
    { preco: { $lt: 100 } }
  ]
})
```

## $nor
Retorna documentos que não atendem nenhuma das condições listadas.
```js
db.pedidos.find({
  $nor: [
    { status: "entregue" },
    { status: "cancelado" }
  ]
})
```
## $not
Inverte o resultado de uma expressão, retornando documentos que não correspondem à condição.
```js
db.usuarios.find({
  idade: { $not: { $gte: 18 } }
})
```

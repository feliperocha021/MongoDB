# Data Types

O MongoDB utiliza **BSON** (Binary JSON), que amplia os tipos de dados do JSON tradicional.  
Aqui estão os principais tipos suportados:

``String`` → Texto em UTF-8 (ex.: "nome": "Felipe")

``Integer`` (Int32, Int64/Long) → Números inteiros de 32 ou 64 bits (ex.: "idade": 30)

``Double`` → Números de ponto flutuante (ex.: "preco": 29.99)

``Decimal128`` → Número decimal de 128 bits, usado em cálculos financeiros/científicos (ex.: "saldo": NumberDecimal("1234.56"))

``Boolean`` → Valores lógicos true ou false

``Date`` → Datas e horas com precisão de milissegundos desde 01/01/1970 (ex.: "criadoEm": ISODate("2023-05-24T14:00:00Z"))

``Timestamp`` → Usado internamente para replicação e controle de alterações

``ObjectId`` → Identificador único gerado automaticamente para cada documento (ex.: "_id": ObjectId("507f1f77bcf86cd799439011"))

``Array`` → Lista de valores (ex.: "tags": ["nodejs", "mongodb", "api"])

``Object (Embedded Document)`` → Documento aninhado (ex.: "endereco": { "rua": "A", "cidade": "SP" })

``Null`` → Representa valor nulo ou ausente (ex.: "telefone": null)

``Regular Expression`` → Expressões regulares para buscas de texto (ex.: "nome": /felipe/i)

``Binary Data`` → Dados binários (ex.: imagens, arquivos, etc.)

``Code`` → Código JavaScript armazenado dentro do documento

``Symbol`` → Similar a String, mas pouco usado (mais histórico/legado)

``MinKey / MaxKey`` → Valores especiais usados em comparações, representando o menor e o maior valor possível no BSON

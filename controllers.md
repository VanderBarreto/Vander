# Descrição de campos dos endpoint da API BARTANA

###SubCategory(Subcategorias)
- Listar as subcategorias

>$ GET http://localhost:5000/subcategory

- Listar as subcategorias específicas
Para listar as subcategorias de uma única categoria, é necessário fornecer o ID da categoria na URL, como mostrado abaixo.

>$ GET http://localhost:5000/subcategory/{inteiro:ID_CATEGORIA}

- Adicionar subcategoria
Para adicionar uma nova subcategoria, é necessário fornecer o ID da categoria na qual a subcategoria será vinculada e o nome da nova subcategoria.

>$ GET http://localhost:5000/subcategory/add/{inteiro:ID_CATEGORIA}/{string:NOME_SUBCATEGORIA}&{string:TAG_SUBCATEGORIA}

- Remover subcategorias
Para remover uma subcategoria, é necessário fornecer o ID da categoria na qual a subcategoria está vinculada e o nome da subcategoria. Ao deletar a subcategoria, as palavras-chave associadas também serão apagadas.

>$ DELETE http://localhost:5000/subcategory/delete/{inteiro:ID_CATEGORIA}/{string:NOME_SUBCATEGORIA}

###Keyword(Palavras-chave)
- Listar as palavras-chave

>$ GET http://localhost:5000/subcategory

- Listar as palavras-chave específicas
Para listar as palavras-chave de uma única categoria, é necessário fornecer o ID da categoria na URL, como mostrado abaixo.

>$ GET http://localhost:5000/keyword/category/{inteiro:ID_CATEGORIA}	

Para listar as palavras-chave de uma única subcategoria, é necessário fornecer o ID da subcategoria na URL, como mostrado abaixo.

>$ GET http://localhost:5000/keyword/subcategory/{inteiro:ID_SUBCATEGORIA}

- Adicionar palavra-chave
Para adicionar uma nova palavra-chave, é necessário fornecer o ID da categoria e o ID da subcategoria no qual a palavra-chave será vinculada e o nome da palavra-chave

>$ GET http://localhost:5000/keyword/add/{inteiro:ID_CATEGORIA}/{inteiro:ID_SUBCATEGORIA /{string:NOME_PALAVRA-CHAVE}

- Remover palavra-chave

Para remover uma palavra-chave, é necessário fornecer o ID da subcategoria na qual a subcategoria está vinculada e o nome da palavra-chave.

>$ DELETE http://localhost:5000/keyword/delete/{inteiro:ID_SUBCATEGORIA}/{string:NOME_PALAVRA-CHAVE}




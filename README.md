# MongoDB CRUD

Projeto realizado para consolidar todos os conhecimentos adquiridos de MongoDB até o momento.

A idéia é trabalhar com o banco de dados "commerce" que contém dados do cardápio do McDonalds, como: ingredientes, valores nutricionais e dados fictícios de vendas utilizando vários operadores para ler, criar, filtrar, atualizar e deletar dados.

### Para restaurar o banco "commerce"

Na raiz do diretório do projeto, execute o seguinte comando que fará a restauração da base de dados `commerce`:
   ```sh
   DBNAME=commerce ./scripts/resetdb.sh assets/produtos
   ```

A execução desse script criará um banco de dados chamado `commerce` e importará os dados para a coleção `produtos`.

### Listagem de Requisitos

Os requisitos do projeto estão armazenados na pasta `challenges`. Segue abaixo a listagem do que foi proposto para cada um:

1 - Inclua o campo `criadoPor` em todos os documentos, colocando `"Ronald McDonald"` no valor desse campo.

2 - Inclua o campo `valorUnitario` em todos os documentos em que esse campo não existe e atribua a ele o valor `"0.00"`, com o tipo `NumberDecimal`.

3 - Adicione o campo `avaliacao` em todos os documentos da coleção e efetue alterações nesse campo.

4 - Atribua a data corrente ao campo `ultimaModificacao` no sanduíche `Big Mac`.

5 - Adicione `ketchup` aos `ingredientes` para todos os sanduíches menos o `McChicken`, garantindo que não haja duplicidade nos `ingredientes`.

6 - Inclua `bacon` no final da lista de `ingredientes` dos sanduíches `Big Mac` e `Quarteirão com Queijo`.

7 - Remova o item `cebola` de todos os sanduíches.

8 - Remova o **primeiro** `ingrediente` do sanduíche `Quarteirão com Queijo`.

9 - Remova o **último** `ingrediente` do sanduíche `Cheddar McMelt`.

10 - Adicione a quantidade de vendas dos sanduíches por dia da semana.

11 - Insira os elementos `combo` e `tasty` no _array_ `tags` de todos os sanduíches e aproveite para deixar os elementos em ordem alfabética ascendente.

12 - Ordene em todos os documentos os elementos do _array_ `valoresNutricionais` pelo campo `percentual` de forma descendente.

13 - Adicione o elemento `muito sódio` ao final do _array_ `tags` nos produtos em que o `percentual` de `sódio` seja maior ou igual a `40`.

14 - Adicione o elemento `contém sódio` ao final do _array_ `tags` nos produtos em que o `percentual` de `sódio` seja maior do que `20` e menor do que `40`.

15 - Conte quantos produtos contêm `Mc` no nome, sem considerar letras maiúsculas ou minúsculas.

16 - Conte quantos produtos têm `4` ingredientes.

17 - Conte quantos documentos contêm as palavras `frango` ou `hamburguer` utilizando o operador `$text`.

18 - Conte quantos documentos contêm a **expressão** `feito com` utilizando o operador `$text`.

19 - Renomeie o campo `descricao` para `descricaoSite` em todos os documentos.

20 - Remova o campo `curtidas` do item `Big Mac`.

21 - Retorne o `nome` dos sanduíches em que o número de `curtidas` é maior que o número de sanduíches `vendidos`.

22 - Retorne o `nome` e a quantidade de vendas (`vendidos`) dos sanduíches em que o número de vendas é múltiplo de `5`.

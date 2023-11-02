# O que é uma estrutura de dados?


 Uma estrutura de dados é um formato de armazenamento em computação usado para organizar, processar e recuperar dados.
 As estruturas de dados são frequentemente aplicadas na engenharia de software para simplificar e otimizar algoritmos, bem como direcionar a forma como os programas de software são executados.

## JAVASCRIPT

*Estruturas de dados comuns*

- Stack
- Queue
- Linked List
- Set
- Hash Table
- Tree
- Trie
- Graph


*Métodos comuns de pilha*

- push: Insira um novo elemento.
- pop: Remova o elemento superior, retorne o elemento removido.
- peek: Retorna o elemento superior.
- length: retorna o número de elementos na pilha.

*Métodos de Fila*

- enqueue: Entre na fila, adicione um elemento no final.
- dequeue: Sai da fila, remove o elemento frontal e devolve-o.
- front: Obtenha o primeiro elemento.
- isEmpty: determine se a fila está vazia.
- size: Obtenha o número de elementos na fila.

*Métodos de lista vinculada unilateral*

- size: retorna o número de nós.
- head: Retorna o elemento da cabeça.
- add: Adicione outro nó na cauda.
- remover: Remove um determinado nó.
- indexOf: Retorna o índice de um nó.
- elementAt: Retorna o nó de um índice.
- addAt: Insere um nó em um índice específico.
- removeAt: exclui um nó em um índice específico.

*Métodos de conjunto típicos*

- values: retorna todos os elementos de um conjunto.
- size: retorna o número de elementos.
- has: Determine se um elemento existe.
- add: Insere elementos em um conjunto.
- remover: exclui elementos de um conjunto.
- união: Retorna a interseção de dois conjuntos.
- difference: Retorna a diferença de dois conjuntos.
- subset: determine se um determinado conjunto é um subconjunto de outro conjunto.

*Métodos de tabela hash*

- add: Adicione um par de valores-chave.
- remover: exclui um par de valores-chave.
- lookup: Encontre um valor correspondente usando uma chave.

*Conceitos de estrutura de dados em árvore*

- Root: Nó raiz de uma árvore; nenhum nó pai para root
- Parent node: Nó direto da camada superior; só tem um
- Child node: Nó(s) direto(s) da camada inferior; pode ter vários
- Siblings: compartilham o mesmo nó pai
- Leaf: Nó sem filho
- Edge: Ramificação ou ligação entre nós
- Path: as arestas de um nó inicial até o nó de destino
- Height of Node:: Número de arestas do caminho mais longo de um nó específico até o nó folha
- Height of Tree: Número de arestas do caminho mais longo do nó raiz até o nó folha
- Depth of Node: número de arestas do nó raiz ao nó específico
- Degree of Node: número de nós filhos

*Métodos comuns de árvore de pesquisa binária*

- add: Insere um nó na árvore.
- findMin: Obtenha o nó mínimo.
- findMax: Obtenha o nó máximo.
- find: Pesquise um nó específico.
- isPresent: Determina a existência de um determinado nó.
- remover: Exclui um nó da árvore.

*Métodos de tentativa*

- add: Insere uma palavra na árvore do dicionário.
- isWord: Determine se a árvore consiste em uma determinada palavra.
- print: Retorna todas as palavras da árvore.

### Exemplo

```javascript
function Stack() {
this.count = 0;
  this.storage = {};

  this.push = function (value) {
    this.storage[this.count] = value;
    this.count++;
  }

  this.pop = function () {
    if (this.count === 0) {
      return undefined;
    }
    this.count--;
    var result = this.storage[this.count];
    delete this.storage[this.count];
    return result;
  }

  this.peek = function () {
    return this.storage[this.count - 1];
  }

  this.size = function () {
    return this.count;
  }
}
```

## JAVA

*Estruturas de dados lineares*

- Arrays: Um array é uma estrutura de dados linear que representa um grupo de elementos semelhantes, acessados ​​por índice. O tamanho de uma matriz deve ser fornecido antes de armazenar os dados.
- Linked List: Uma lista vinculada é uma estrutura de dados linear com a coleção de vários nós, onde cada elemento armazena seus próprios dados e um ponteiro para a localização do próximo elemento.
- Stacks: Stack, uma estrutura de dados abstrata, é uma coleção de objetos que são inseridos e removidos de acordo com o princípio LIFO (último a entrar, primeiro a sair).
- Queues: As filas também são outro tipo de estrutura de dados abstrata. Ao contrário de uma pilha, a fila é uma coleção de objetos que são inseridos e removidos de acordo com o princípio FIFO (primeiro a entrar, primeiro a sair).

*Estruturas de dados hierárquicas*

- Binary Trees
- Heaps
- Hash Tables

### Exemplo

```java
package com.dataflair.arrayclass;
class ExceptionArrayIndex {
  public static void main(String[] args) {
    int arr[] = new int[] {1,2,3,4,5};
    int j;
    for (j = 0; j <= arr.length; j++) {
      System.out.println(arr[j]);
    }
  }
}
```

## Csharp (.net)

**Fonte:**
*https://learn.microsoft.com/en-us/dotnet/standard/collections/*

*Em coleções baseadas em IList ou diretamente em ICollection, cada elemento contém apenas um valor. Esses tipos incluem:*

- Array
- ArrayList
- List<T>
- Queue
- ConcurrentQueue<T>
- Stack
- ConcurrentStack<T>
- LinkedList<T>

*Em coleções baseadas na interface IDictionary, cada elemento contém uma chave e um valor. Esses tipos incluem:*


- Hashtable
- SortedList
- SortedList<TKey,TValue>
- Dictionary<TKey,TValue>
- ConcurrentDictionary<TKey,TValue>

### Exemplo

```csharp
using System;
using System.Collections;
public class SamplesStack  {

   public static void Main()  {

      // Creates and initializes a new Stack.
      Stack myStack = new Stack();
      myStack.Push("Hello");
      myStack.Push("World");
      myStack.Push("!");

      // Displays the properties and values of the Stack.
      Console.WriteLine( "myStack" );
      Console.WriteLine( "\tCount:    {0}", myStack.Count );
      Console.Write( "\tValues:" );
      PrintValues( myStack );
   }

   public static void PrintValues( IEnumerable myCollection )  {
      foreach ( Object obj in myCollection )
         Console.Write( "    {0}", obj );
      Console.WriteLine();
   }
}

/*
Este código produz a seguinte saída.
minha pilha
Contagem: 3
Valores: ! Olá mundo
*/
```

## Python

**Fonte:**
*https://docs.python.org/3/tutorial/datastructures.html*

*Estruturas de dados comuns*

- Stack
- Queue
- Linked List
- Hash Table
- Tree
- Tries
- Graphs
- Heaps


### Exemplo

```python
my_tuple = ('sara', 6, 5, 0.97)
my_list = ['sara', 6, 5, 0.97]
print(my_tuple[0])     #saída => 'sara'
print(my_list[0])      #saída => 'sara'

my_tuple[0] = 'ansh'   # modificando tupla => gera um erro
my_list[0] = 'ansh'    # modificando lista => lista modificada
print(my_tuple[0])     #saída => 'sara'
print(my_list[0])      #saída => 'ansh'
```


## Golang

*As estruturas de dados básicas do Golang incluem:*

- Array
- Slice
- Map
- Struct

### Exemplo

```golang
package main

import "fmt"

func main() {

	s := []int{10, 20, 30, 40}

	// We can loop through this slice in two ways:

	// 1. using "range"
	for key, value := range s {
		fmt.Println(key, ":", value)
	}
	//If we dont want the key, we do, replace "key" with "_":
	for _, value := range s {
		fmt.Println(value)
	}

	// 2. Using traditional forloop:
	for i := 0; i < len(s); i++ {
		fmt.Println(s[i]) //get the value at index "i"
	}
}

/*
Primeira Saída:
0 : 10
1 : 20
2 : 30
3 : 40

Segunda Saída:
10
20
30
40
10
20
30
40
*/
```
**IDE Go:**
*https://go.dev/play/*
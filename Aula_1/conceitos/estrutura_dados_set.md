
#  Estrutura de Dados em Python: Sets e Frozen Sets

Neste artigo, exploraremos a estrutura de dados conhecida como \"set\" (conjunto) e \"frozenset\" (conjunto imutável) em Python. Os sets são coleções não ordenadas de elementos únicos, enquanto os frozensets são versões imutáveis dessas coleções. Vamos examinar como criar, manipular e utilizar essas estruturas de dados em Python.

# O que é um Set em Python?

Um set em Python é uma coleção não ordenada de elementos, onde cada elemento só pode aparecer uma vez. Existem duas formas de representar um set em Python:

-  Set mutável: Permite adicionar e remover elementos.
-  Frozenset imutável: Uma vez criado, não pode ser modificado.

# Criando Sets em Python

Para criar um set em Python, você pode simplesmente usar chaves `{}` ou a função `set()`. Aqui estão alguns exemplos:

```python
 Criando um conjunto vazio
conjunto_vazio = set()
conjunto_vazio2 = {}

 Criando um conjunto com elementos
frutas = {"maçã", "banana", "laranja"}

 Criando um conjunto a partir de uma lista
numeros = set(1, 2, 3, 4, 5)
```

Lembre-se de que para criar um conjunto vazio, não use chaves vazias `{}` porque isso criará um dicionário vazio, não um conjunto.

# Operações com Sets

Os sets em Python suportam várias operações úteis, incluindo:

-  Verificar se um elemento está no conjunto.
-  Calcular o tamanho (cardinalidade) do conjunto.
-  Operações de conjunto, como união, interseção e diferença.

 Verificando a Presença de Elementos

Para verificar se um elemento está presente em um conjunto, você pode usar a palavra-chave `in`. Por exemplo:

```python
frutas = {"maçã", "banana", "laranja"}
print("banana" in frutas)   True
print("uva" in frutas)      False
```

# Cardinalidade de um Conjunto

Para calcular o tamanho de um conjunto (ou seja, o número de elementos), você pode usar a função `len()`. Por exemplo:

```python
frutas = {"maçã", "banana", "laranja"}
tamanho = len(frutas)
print(tamanho)   3
```

# Operações de Conjunto

As operações de conjunto, como união, interseção e diferença, são realizadas usando operadores ou métodos específicos.

-  União: O operador `|` ou o método `.union()` cria um novo conjunto contendo todos os elementos de dois conjuntos.
-  Interseção: O operador `&` ou o método `.intersection()` cria um novo conjunto contendo apenas os elementos que estão em ambos os conjuntos.
-  Diferença: O operador `-` ou o método `.difference()` cria um novo conjunto contendo os elementos que estão em um conjunto, mas não no outro.

```python
A = {1, 2, 3}
B = {3, 4, 5}

uniao = A | B             União
intersecao = A & B        Interseção
diferenca = A -  B         Diferença

print(uniao)         {1, 2, 3, 4, 5}
print(intersecao)    {3}
print(diferenca)     {1, 2}
```

Lembre-se de que essas operações não modificam os conjuntos originais, criam novos conjuntos com os resultados.

# Sets Imutáveis (Frozen Sets)

Além dos sets mutáveis, Python também oferece os frozensets, que são conjuntos imutáveis. Uma vez criados, eles não podem ser modificados. Você pode criar um frozenset usando a função `frozenset()`.

```python
conjunto_imutavel = frozenset(1, 2, 3)
```

Os frozensets são úteis quando você precisa de um conjunto de elementos que não deve ser alterado após a criação.

# Conclusão

Neste artigo, exploramos a estrutura de dados de sets e frozensets em Python. Aprendemos como criar, manipular e realizar operações com sets, bem como a utilidade dos frozensets em situações em que a imutabilidade é desejada. Essas estruturas de dados são valiosas para lidar com coleções de elementos únicos em Python, oferecendo flexibilidade e desempenho.

Esperamos que este artigo tenha esclarecido o funcionamento de sets e frozensets em Python, e que você possa utilizá-los de forma eficaz em seus projetos futuros. Até a próxima oportunidade!

# Expressões Regulares em Python: Quantificadores e Conjuntos

As expressões regulares desempenham um papel fundamental na manipulação de texto em Python. Elas são poderosas ferramentas para buscar e manipular padrões em strings. Neste artigo, exploraremos os quantificadores e conjuntos em expressões regulares.

# Quantificadores

## Asterisco (\*)

O asterisco (\*) é um dos quantificadores mais comuns em expressões regulares. Ele significa \"zero ou mais ocorrências\" do caractere ou grupo que o antecede. Por exemplo, se tivermos a expressão regular `a*`, ela corresponderá a qualquer número de caracteres \"a\" consecutivos, incluindo nenhum \"a\".

**Exemplo:**
-  `a*` corresponde a: \"\", \"a\", \"aa\", \"aaa\", ...

## Mais (+)

O quantificador de mais (+) significa \"uma ou mais ocorrências\" do caractere ou grupo que o antecede. Ou seja, ele exige pelo menos uma ocorrência do caractere.

**Exemplo:**
-  `a+` corresponde a: \"a\", \"aa\", \"aaa\", ...

## Interrogação (?)

A interrogação (?) torna o caractere ou grupo que o antecede opcional, ou seja, ele pode ocorrer uma vez ou nenhuma vez na string de entrada.

**Exemplo:**
-  `a?` corresponde a: \"\", \"a\"

## Chaves ({n})

As chaves ({n}) permitem especificar um número exato de ocorrências do caractere ou grupo que as precede. Por exemplo, `{3}` significa exatamente três ocorrências.

**Exemplo:**
-  `a{3}` corresponde a: \"aaa\"

## Chaves ({n,})

As chaves ({n,}) especificam um mínimo de \"n\" ocorrências do caractere ou grupo que as precede, mas não há limite superior. Ou seja, corresponde a \"n\" ou mais ocorrências.

**Exemplo:**
-  `a{2,}` corresponde a: \"aa\", \"aaa\", \"aaaa\", ...

## Chaves ({n,m})

As chaves ({n,m}) definem um intervalo de ocorrências permitidas. Corresponde a qualquer número de ocorrências entre \"n\" e \"m\", inclusive.

**Exemplo:**
-  `a{2,4}` corresponde a: \"aa\", \"aaa\", \"aaaa\"

## Conjuntos

Em expressões regulares, os conjuntos são definidos entre colchetes `[ ]` e correspondem a qualquer caractere dentro do conjunto. Os conjuntos podem ser compostos de diferentes maneiras:

-  `[abc]`: Corresponde a \"a\", \"b\" ou \"c\".
-  `[a-z]`: Corresponde a qualquer letra minúscula de \"a\" a \"z\".
-  `[0-9]`: Corresponde a qualquer dígito de \"0\" a \"9\".

Você também pode usar conjuntos negados, indicados pelo caractere `^` logo após o colchete de abertura. Por exemplo, `[^0-9]` corresponde a qualquer caractere que não seja um dígito.

# Exemplos Práticos

## Validando Números de Telefone

Suponha que você deseje validar números de telefone que consistem apenas em dígitos numéricos. Você pode usar a seguinte expressão regular:

```python
^[0-9]+$
```

-  `^` e `$` são âncoras que garantem que a expressão corresponda a toda a string.
-  `[0-9]+` corresponde a um ou mais dígitos numéricos.

# Encontrando Palavras com Três ou Mais Vogais

Se você deseja encontrar palavras em um texto que contenham três ou mais vogais consecutivas, pode usar a seguinte expressão regular:

```python
w*[aeiou]{3,}w*
```

-  `\w*` corresponde a zero ou mais caracteres alfanuméricos.
-  `[aeiou]{3,}` corresponde a três ou mais vogais consecutivas.
-  `\w*` corresponde novamente a zero ou mais caracteres alfanuméricos.

# Conclusão

Os quantificadores e conjuntos são componentes essenciais para criar expressões regulares poderosas em Python. Eles permitem que você especifique padrões de texto de maneira flexível e precisa. Ao dominar esses conceitos, você estará preparado para lidar com tarefas complexas de manipulação de texto em suas aplicações Python. Lembre-se de praticar e experimentar diferentes expressões regulares para aprimorar suas habilidades.
 

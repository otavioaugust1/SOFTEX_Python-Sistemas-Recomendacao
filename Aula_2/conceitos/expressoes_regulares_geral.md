
# Expressões Regulares em Python: Um Guia Completo

As expressões regulares, também conhecidas como regex ou regexp, são uma poderosa ferramenta utilizada para manipular e processar strings em Python e em muitas outras linguagens de programação. Neste artigo, vamos explorar o mundo das expressões regulares em Python, desde conceitos básicos até exemplos práticos de uso.

# Introdução às Expressões Regulares

As expressões regulares são sequências de caracteres que definem um padrão de busca em uma string. Elas são amplamente utilizadas para realizar tarefas como validação de entradas de usuários, busca e substituição de texto, extração de informações de strings complexas, entre outras.

No Python, as expressões regulares são suportadas pelo módulo `re`. Antes de começarmos a trabalhar com expressões regulares, é importante importar esse módulo:

```python
import re
```

# Sintaxe Básica

Vamos começar com alguns conceitos fundamentais:

-  **Metacaracteres:** São caracteres especiais com significados especiais em expressões regulares. Alguns exemplos comuns são `.`, `*`, `+`, `?`, `()`, ``, `{}`, entre outros.

-  **Âncoras:** São metacaracteres utilizados para especificar a posição de um padrão na string. Exemplos incluem `^` (início da linha) e `$` (fim da linha).

-  **Conjuntos e intervalos:** Permitem definir um conjunto de caracteres válidos em uma determinada posição da string. Por exemplo, `aeiou` corresponde a qualquer vogal.

-  **Quantificadores:** Permitem especificar quantas vezes um padrão deve ser repetido. Alguns quantificadores comuns são `*` (zero ou mais), `+` (uma ou mais), `?` (zero ou uma) e `{}` (um número específico de vezes).

Vamos ver alguns exemplos de uso desses conceitos.

# Exemplos Práticos

## Validando Números

Vamos começar com um exemplo simples. Suponha que você queira validar se uma string contém um número inteiro de um ou mais dígitos. Você pode usar o seguinte padrão de expressão regular:

```python
pattern = r'\d+'
```

-  `\d` corresponde a qualquer dígito numérico.
-  `+` significa que o dígito deve aparecer uma ou mais vezes.

Aqui está como você pode usar isso em Python:

```python
import re

pattern = r'd+'
texto = "12345"

if re.fullmatch(pattern, texto):
    print("É um número válido.")
else:
    print("Não é um número válido.")
```

Essa expressão regular irá corresponder a qualquer sequência de dígitos, como \"123\", \"4567\" e assim por diante.

## Validando Endereços de Email

Outro exemplo comum é validar endereços de email. Embora a validação completa de endereços de email seja bastante complexa, podemos criar uma expressão regular simples para verificar se uma string parece ser um endereço de email válido:

```python
pattern = r'\bA-Za-z0-9._%+-+@A-Za-z0-9.- +\.A-Z|a-z{2,7}\b'
```

-  `A-Za-z0-9._%+-+` corresponde ao nome de usuário.
-  `@A-Za-z0-9.- +` corresponde ao domínio.
-  `\.A-Z|a-z{2,7}` corresponde à extensão do domínio (por exemplo, .com, .org).

Aqui está um exemplo de uso:

```python
import re

pattern = r'\bA-Za-z0-9._%+-+@A-Za-z0-9.- +\.A-Z|a-z{2,7}\b'
email = "exemplo@email.com"

if re.fullmatch(pattern, email):
    print("É um endereço de email válido.")
else:
    print("Não é um endereço de email válido.")
```

## Extração de Dados

Expressões regulares também são úteis para extrair informações de uma string. Suponha que você tenha uma string que contenha datas no formato \"DD/MM/AAAA\". Você pode usar uma expressão regular para extrair essas datas:

```python
import re

texto = "Nasceu em 25/12/1990 e casou em 05/09/2015."
pattern = r'\d{2}/\d{2}/\d{4}'

datas = re.findall(pattern, texto)

print("Datas encontradas:")
for data in datas:
    print(data)
```

Neste exemplo, usamos a função `re.findall` para encontrar todas as ocorrências de datas na string. O padrão `\d{2}/\d{2}/\d{4}` corresponde a datas no formato especificado.

# Conclusão

As expressões regulares são uma ferramenta poderosa para lidar com strings em Python. Este artigo forneceu uma introdução básica ao uso de expressões regulares, cobrindo os conceitos fundamentais e fornecendo exemplos práticos de uso.

À medida que você se aprofunda no mundo das expressões regulares, você descobrirá que elas podem ser extremamente úteis em uma variedade de situações, desde validação de entradas de usuário até processamento de dados complexos. Continue explorando e praticando, e você se tornará um mestre em expressões regulares em pouco tempo!

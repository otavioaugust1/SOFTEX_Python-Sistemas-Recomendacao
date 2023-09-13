
#  Estruturas de Repetição em Python

Neste artigo, vamos explorar as estruturas de repetição em Python. Python é uma linguagem de programação poderosa que oferece diversas maneiras de repetir ações em seu código. Vamos examinar as principais estruturas de repetição, como o `while` e o `for`, e entender como usá-las de forma eficaz.

# O Loop `while`

O loop `while` é uma das estruturas de repetição mais simples em Python. Ele funciona da seguinte maneira:

```python
while condição:
     Código a ser repetido enquanto a condição for verdadeira
```

-  A condição é uma expressão booleana que determina se o loop deve continuar executando.
-  Enquanto a condição for verdadeira, o bloco de código dentro do loop será executado repetidamente.

Vamos ver um exemplo simples:

```python
i = 0
while i < 10:
    print(i)
    i += 1
```

Neste exemplo, o loop `while` imprimirá os números de 0 a 9, incrementando a variável `i` a cada iteração. Quando `i` se tornar igual a 10, a condição se tornará falsa, e o loop terminará.

É importante notar que, se não houver um mecanismo para alterar a variável de controle dentro do loop, ele pode se tornar um loop infinito.

# Jogo de Adivinhação

Vamos aplicar o conceito de loops em um jogo de adivinhação. Neste jogo, o programa escolhe um número secreto, e o jogador deve adivinhar o número. O jogo continua até que o jogador adivinhe corretamente.

```python
import random

numero_secreto = random.randint(1, 100)   Número secreto entre 1 e 100

while True:
    palpite = int(input("Digite seu palpite (ou 0 para sair):"))
    
    if palpite == 0:
        print("Encerrando o jogo.")
        break   Sai do loop
        
    if palpite == numero_secreto:
        print("Você acertou! O número era", numero_secreto)
        break   Sai do loop
```

Neste exemplo, utilizamos um loop `while` infinito (`while True`) e o comando `break` para sair do loop quando o jogador acertar o número ou escolher sair do jogo.

# O comando `continue`

O comando `continue` é usado para encerrar a iteração atual de um loop e retornar ao início. Isso pode ser útil quando você deseja ignorar uma parte do código em uma iteração específica.

Vamos ver um exemplo usando o comando `continue`:

```python
for i in range(10):
    if i % 2 == 0:
        continue   Pula os números pares
    print(i)
```

Neste exemplo, o loop `for` percorre os números de 0 a 9. Quando encontra um número par, ele utiliza o `continue` para pular para a próxima iteração, evitando a impressão de números pares.

# O Loop `for`

O loop `for` é outra estrutura de repetição essencial em Python. Ele é frequentemente usado para percorrer sequências, como listas, strings e objetos iteráveis. Aqui está a sintaxe básica:

```python
for elemento in sequência:
     Código a ser executado para cada elemento na sequência
```

Vamos explorar alguns exemplos de uso do `for`:

## Percorrendo uma Lista

```python
frutas = "maçã", "banana", "laranja"

for fruta in frutas:
    print(fruta)
```

Neste exemplo, o loop `for` percorre a lista de frutas e imprime cada uma delas.

## Percorrendo uma String

```python
palavra = "Python"

for letra in palavra:
    print(letra)
```

Aqui, o loop `for` percorre os caracteres da string \"Python\" e os imprime individualmente.

## Usando `range()`

A função `range()` é frequentemente usada com o loop `for` para gerar uma sequência de números:

```python
for i in range(5):
    print(i)
```

Este código imprimirá os números de 0 a 4, pois `range(5)` cria uma sequência que vai de 0 a 4.

# Conclusão

Neste artigo, exploramos as estruturas de repetição em Python, incluindo o loop `while` e o loop `for`. Aprendemos como usar o comando `break` para sair de um loop e o comando `continue` para pular iterações. Além disso, vimos exemplos práticos de como aplicar esses conceitos em situações reais de programação.

Lembre-se de que a prática é fundamental para o aprendizado da programação. Continue explorando e experimentando com as estruturas de repetição em Python para aprimorar suas habilidades de programação. Boa sorte em seus estudos!

- --

**Observação:** O código Python apresentado neste artigo pode ser executado em um ambiente de desenvolvimento Python para testar e compreender melhor os conceitos apresentados.
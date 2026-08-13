---
title: "Variáveis"
nav_order: 5
parent: "Python"
---

No Python, não é necessário declarar explicitamente o tipo de variável antes de atribuir um valor a ela. O Python é uma linguagem de tipagem dinâmica, o que significa que as variáveis podem assumir diferentes tipos de dados ao longo do tempo.

Ao atribuir um valor a uma variável, o Python inferirá automaticamente o tipo de dados com base no valor atribuído.

# Exemplo 1

```
## Entrada de dados
Num1 = int(input("Digite o primeiro número: "))
Num2 = int(input("Digite o segundo número: "))

## Operações matemáticas
soma = Num1 + Num2
subtracao = Num1 - Num2
multiplicacao = Num1 * Num2
divisao = Num1 / Num2

## Saída de resultados
print("A soma é", soma)
print("A subtração é", subtracao)
print("O valor multiplicado é", multiplicacao)
print("A divisão é", divisao)
```

# Exemplo 2

```
numero = 10  # 'numero' é do tipo int
texto = "Olá, mundo!"  # 'texto' é do tipo str
pi = 3.14159  # 'pi' é do tipo float
```

Nesse exemplo, o Python deduz que numero é um número inteiro (int), texto é uma sequência de caracteres (str) e pi é um número de ponto flutuante (float), com base nos valores atribuídos.

# Exemplo 3

Essa inferência automática de tipos de dados é uma das características do Python e permite que você escreva código mais conciso e flexível. No entanto, se você precisar converter uma variável para um tipo específico, você pode usar as funções de conversão de tipo, como int(), float(), str(), entre outras.


```
numero = "10"  # 'numero' é uma string
numero_inteiro = int(numero)  # Converte 'numero' para um número inteiro
```
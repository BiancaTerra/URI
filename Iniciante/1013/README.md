# 1013
Faça um programa que leia três valores e apresente o maior dos três valores lidos seguido da mensagem “eh o maior”. Utilize a fórmula:

Maior AB = |(a+b+abs(a-b))
|2

Obs.: a fórmula apenas calcula o maior entre os dois primeiros (a e b). Um segundo passo, portanto é necessário para chegar no resultado esperado.

## Entrada
O arquivo de entrada contém três valores inteiros.

## Saída
Imprima o maior dos três valores seguido por um espaço e a mensagem "eh o maior".

**Entrada:** |**Saída:**
-------------|----------
7 14 106|106 eh o maior
-------------|----------
217 14 6|217 eh o maior


## Resposta
linha = input().split(" ")

A,B,C = linha

maior = (float(A) + float(B) + abs(float(A) - float(B))) /2
result = (float(maior) + float(C) + abs(float(maior) - float(C))) /2

print("%d eh o maior" %result)
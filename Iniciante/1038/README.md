# 1038
Com base na tabela abaixo, escreva um programa que leia o código de um item e a quantidade deste item. A seguir, calcule e mostre o valor da conta a pagar.
**CODIGO**|**ESPECIFICAÇÃO**|**PREÇO**
----------|-----------------|----------
1|Cachorro-quente|R$ 4.00
2|X-Salada|R$ 4.50
3|X-Bacon|R$ 5.00
4|Torrada Simples|R$ 2.00
5|Refrigerante|R$ 1.50

**Entrada:**|**Saída:**
------------|-----------
3 2|Total: R$ 10.00
------------|-----------
4 3|Total: R$ 6.00
------------|-----------
2 3|Total: R$ 13.50

## Resposta
X = input().split()
A,B = X

if(A == '1'):
  print('Total: R$ {:.2f}'.format(4.00 * float(B)))
if(A == '2'):
  print('Total: R$ {:.2f}'.format(4.50 * float(B)))
if(A == '3'):
  print('Total: R$ {:.2f}'.format(5.00 * float(B)))
if(A == '4'):
  print('Total: R$ {:.2f}'.format(2.00 * float(B)))
if(A == '5'):
  print('Total: R$ {:.2f}'.format(1.00 * float(B)))
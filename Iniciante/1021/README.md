# 1021
Leia um valor de ponto flutuante com duas casas decimais. Este valor representa um valor monetário. A seguir, calcule o menor número de notas e moedas possíveis no qual o valor pode ser decomposto. As notas consideradas são de 100, 50, 20, 10, 5, 2. As moedas possíveis são de 1, 0.50, 0.25, 0.10, 0.05 e 0.01. A seguir mostre a relação de notas necessárias.

## Entrada
O arquivo de entrada contém um valor de ponto flutuante **N** (0 ≤ **N** ≤ 1000000.00).

## Saída
Imprima a quantidade mínima de notas e moedas necessárias para trocar o valor inicial, conforme exemplo fornecido.

Obs: Utilize ponto (.) para separar a parte decimal.

**Entrada:**|**Saída:**
------------|----------
576.73|NOTAS:
|5 nota(s) de R$ 100.00
|1 nota(s) de R$ 50.00
|1 nota(s) de R$ 20.00
|0 nota(s) de R$ 10.00
|1 nota(s) de R$ 5.00
|0 nota(s) de R$ 2.00
|MOEDAS:
|1 moeda(s) de R$ 1.00
|1 moeda(s) de R$ 0.50
|0 moeda(s) de R$ 0.25
|2 moeda(s) de R$ 0.10
|0 moeda(s) de R$ 0.05
|3 moeda(s) de R$ 0.01
-----------|-----------
4.00|NOTAS:
|0 nota(s) de R$ 100.00
|0 nota(s) de R$ 50.00
|0 nota(s) de R$ 20.00
|0 nota(s) de R$ 10.00
|0 nota(s) de R$ 5.00
|2 nota(s) de R$ 2.00
|MOEDAS:
|0 moeda(s) de R$ 1.00
|0 moeda(s) de R$ 0.50
|0 moeda(s) de R$ 0.25
|0 moeda(s) de R$ 0.10
|0 moeda(s) de R$ 0.05
|0 moeda(s) de R$ 0.01

## Resposta
n = float(input())

n100 = n//100
n = n - n100*100

n50 = n//50
n = n - n50*50

n20 = n//20
n = n - n20*20

n10 = n//10
n = n - n10*10

n5 = n//5
n = n - n5*5

n2 = n//2
n = n - n2*2

n1 = n//1
n = n - n1*1
n1=float("%.2f"%n1)
n=float("%.2f"%n)

m50 = n//0.5
n = n - m50*0.5
m50=float("%.2f"%m50)
n=float("%.2f"%n)

m25 = n//0.25
n = n - m25*0.25
m25=float("%.2f"%m25)
n=float("%.2f"%n)

m10 = n//0.1
n = n - m10*0.1
m10=float("%.2f"%m10)
n=float("%.2f"%n)

m5 = n//0.05
n = n - m5*0.05
m5=float("%.2f"%m5)
n=float("%.2f"%n)

m1 = n * 100
m1=float("%.2f"%m1)
n=float("%.2f"%n)

print("NOTAS:")
print("%0.0f nota(s) de R$ 100.00" %n100)
print("%0.0f nota(s) de R$ 50.00" %n50)
print("%0.0f nota(s) de R$ 20.00" %n20)
print("%0.0f nota(s) de R$ 10.00" %n10)
print("%0.0f nota(s) de R$ 5.00" %n5)
print("%0.0f nota(s) de R$ 2.00" %n2)

print("MOEDAS:")
print("%0.0f moeda(s) de R$ 1.00" %n1)
print("%0.0f moeda(s) de R$ 0.50" %m50)
print("%0.0f moeda(s) de R$ 0.25" %m25)
print("%0.0f moeda(s) de R$ 0.10" %m10)
print("%0.0f moeda(s) de R$ 0.05" %m5)
print("%0.0f moeda(s) de R$ 0.01" %m1)
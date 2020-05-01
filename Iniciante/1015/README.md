# 1015
Leia os quatro valores correspondentes aos eixos x e y de dois pontos quaisquer no plano, p1(x1,y1) e p2(x2,y2) e calcule a distância entre eles, mostrando 4 casas decimais após a vírgula, segundo a fórmula:

Distancia = raiz quadrada de [(x2 - x1)² + (y2 - y1)²]

## Entrada
O arquivo de entrada contém duas linhas de dados. A primeira linha contém dois valores de ponto flutuante: ***x1 y1*** e a segunda linha contém dois valores de ponto flutuante ***x2 y2***.

## Saída
Calcule e imprima o valor da distância segundo a fórmula fornecida, com 4 casas após o ponto decimal.

**Entrada:**|**Saída:**
------------|----------
1.0 7.0|4.4721
5.0 9.0|
------------|----------
-2.5 0.4|16.1484
12.1 7.3|
------------|----------
2.5 -0.4|16.4575
-12.2 7.0|

## Resposta
A = input().split(" ")
B = input().split(" ")

x1,y1 = A
x2,y2 = B

DISTANCIA = (((float(x2) - float(x1)) * (float(x2) - float(x1))) + ((float(y2) - float(y1)) * (float(y2) - float(y1)))) ** (1/2)

print("%0.4f" %DISTANCIA)
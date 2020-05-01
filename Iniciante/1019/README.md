# 1019
Leia um valor inteiro, que é o tempo de duração em segundos de um determinado evento em uma fábrica, e informe-o expresso no formato horas:minutos:segundos.

## Entrada
O arquivo de entrada contém um valor inteiro **N**.

## Saída
Imprima o tempo lido no arquivo de entrada (segundos), convertido para horas:minutos:segundos, conforme exemplo fornecido.

**Entrada:**|**Saída:**
------------|----------
556|0:9:16
------------|----------
1|0:0:1
------------|----------
140153|38:55:53

## Resposta
seg = int(input())
h = seg//60**2
r = seg - h*60**2
m = r//60
s = r - m*60
print("{}:{}:{}".format(h, m, s))
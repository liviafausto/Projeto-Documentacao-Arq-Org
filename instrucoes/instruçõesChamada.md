## Instruções de Chamada

<br>

### **`1. CALL`**

&nbsp; &nbsp; &nbsp; **1.1 Descrição:**

A função call irá chamar um procedimento a ser executado, existindo dois conceitos para esse chamado, o primeiro é o **"far"** e  o **"near"** e o segundo o **“relative”** e **“absolut”**.
 

&nbsp; &nbsp; &nbsp; **1.2 Parâmetros:**

&nbsp; &nbsp; &nbsp; &nbsp; **a. Near relative call**
Recebe um número negativo ou positivo indicando o número de bytes  que devem ser desviados da seguinte forma.

```asm
call rel8/rel16
```

&nbsp; &nbsp; &nbsp; &nbsp; **b. Near absolut call**
Na chamada absoluta você irá chamar o endereço exato que deseja chamar, utilizando os parâmetros da seguinte maneira.
call funçãochamada
 
&nbsp; &nbsp; &nbsp; **1.3 Usando a instrução:**

```asm
LimpaTela:
	push fr
	push r0
	push r1
	push r3

 
loadn r0, #1200
loadn r1, #’ ‘
loadn r3, #0
 
Call LimpaTela;
```

> Dessa forma independente de onde estejam as funções no código, ao executar o call ele irá chamar a função LimpaTela para ser executada.


<br>

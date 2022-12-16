## Instruções de Salto

<br>

### **`1. JMP`**
&nbsp; &nbsp; &nbsp; 	**1.1 Descrição:**

 O JUMP é uma instrução que desvia o fluxo do código, alterando a ordem em que as instruções são executadas, podendo ser condicional ou incondicional. Um Jump incondicional é usado na forma JMP ,já o jump incodicional assume a forma J??, em que no local da interrogação se colocar outras letras a fim de determinar uma execução específica 
 
&nbsp; &nbsp; &nbsp; **1.2 Parâmetros:**

O salto condicional irá utilizar o comparador que está dentro da ULA para verificar a condição e realizar o salto. Os parâmetros desta instrução são o label que indica o ponto do desvio da seguinte forma.

```asm
jmp PontodoDesvio
```
 
&nbsp; &nbsp; &nbsp;  **1.3 Usando a instrução:**

```asm
jmp PontodoDesvio; o fluxo do codigo ira pular para o label PontodoDesvio.
```
 
<br>


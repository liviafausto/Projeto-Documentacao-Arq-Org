## Instruções Aritméticas

<br>

### **`1. INC`**

&nbsp; &nbsp; &nbsp; **1.1 Descrição:**

A instrução inc é usada para incrementar um operando (registo ou um endereço de memória) em 1 (um). Ela funciona com somente um operando.


&nbsp; &nbsp; &nbsp;**1.2 Parâmetros:**

Os parâmetros desse operador são a instrução (inc) e o operando.

```asm
inc destino
```
> Importante ressaltar que o operando pode ser de **8-bit, 16-bit ou 32-bit.**

&nbsp; &nbsp; &nbsp; **1.3 Usando a instrução:**

 ```asm
inc r0 ; incrementa um registo
```

<br> 

### **`2. DEC`**

&nbsp; &nbsp; &nbsp; **2.1 Descrição:**

A instrução dec é usada para decrementar um operando (registo ou um endereço de memória) em 1 (um). Ela funciona com somente um operando.

&nbsp; &nbsp; &nbsp;**2.2 Parâmetros:**

Os parâmetros desse operador são a instrução (dec) e o operando.

```asm
dec destino
```
> Importante ressaltar que o operando pode ser de **8-bit, 16-bit ou 32-bit.**

&nbsp; &nbsp; &nbsp; **2.3 Usando a instrução:**

 ```asm
dec r0 ; decrementa um registo
```

<br>

<br> 

### **`3. ADD`**

&nbsp; &nbsp; &nbsp; **3.1 Descrição:**

A instrução add é usada para realizar adição binária de dados em byte (8-bit), word (16-bit) ou doubleword (32-bit). Ela funciona para operações do tipo: registo para registo, memória para registo, registo para memória, registos para dados constantes, e memória para dados constantes.

&nbsp; &nbsp; &nbsp;**3.2 Parâmetros:**

Os parâmetros desse operador são a instrução (add), registrador destino e os dois registradores de origem.

```asm
add destino, origemA, origemB
```
> Em memória-para-memória, a operação add pode alterar as **flags de overflow ou de carry.**

&nbsp; &nbsp; &nbsp; **3.3 Usando a instrução:**

 ```asm
add r0, r0, r1 ; atribui o valor da soma r0 + r1 ao registrador r0
```

<br>

<br> 

### **`4. SUB`**

&nbsp; &nbsp; &nbsp; **4.1 Descrição:**

A instrução sub é usada para realizar subtração binária de dados em byte (8-bit), word (16-bit) ou doubleword (32-bit). Ela funciona para operações do tipo: registo para registo, memória para registo, registo para memória, registos para dados constantes, e memória para dados constantes.

&nbsp; &nbsp; &nbsp;**4.2 Parâmetros:**

Os parâmetros desse operador são a instrução (sub), registrador destino, minuendo e subtraendo.

```asm
sub destino, minuendo, subtraendo
```
> Em memória-para-memória, a operação sub pode alterar as **flags de overflow ou de carry.**

&nbsp; &nbsp; &nbsp; **4.3 Usando a instrução:**

 ```asm
sub r0, r0, r1 ; atribui o valor da subtração r0 - r1 ao registrador r0
```

<br>

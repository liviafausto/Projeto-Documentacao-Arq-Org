## **`Instruções de Manipulação de Dados`**

### Padrão geral das instruções de manipulação de dados:

Apesar de parecer complicado, especialmente para aqueles que estão ambientados com linguagens de programação de alto nível, existe um padrão lógico nas instruções que consideramos importante que o usuário entenda. A seguir, apresentamos esse padrão.

`<nome da instrução> <destino da instrução>, <origem da instrução>`

Ressaltamos que as "<>" são ilustrativas e não fazem parte da estrutura das instruções.

<br>


### **`1. Load`**

#### &nbsp; &nbsp; &nbsp; **1.1 - Descrição**
A instrução load é do tipo direto e tem como objetivo carregar um valor para um registrador. A instrução load é composta por um registrador destino e um endereço de memória.



#### &nbsp; &nbsp; &nbsp; **1.2 - Parâmetros**
Os parâmetros são o registrador destino e o endereço de memória que você deseja carregar no registrador, no formato:

```asm
load identificadorDoRegistrador, endereçoNaMemória
```


#### &nbsp; &nbsp; &nbsp; **1.3 - Usando a instrução**
```asm
static meuDado, #10
load R0, meuDado ;O registrador R0 recebe o endereço de meuDado
```
<br>

### **`2. Loadn`**

#### &nbsp; &nbsp; &nbsp; **1.1 - Descrição**
A instrução loadn é do tipo imediato e tem como objetivo carregar um valor numérico para um registrador. A instrução loadn é composta por um registrador destino e um valor numérico.



#### &nbsp; &nbsp; &nbsp; **1.2 - Parâmetros**
Os parâmetros são o endereço de memória destino e o registrador de origem que você deseja passar o dado para a memória, no formato:

```asm
loadn identificadorDoRegistrador, #valorNumerico
```



#### &nbsp; &nbsp; &nbsp; **1.3 - Usando a instrução**
```asm
loadn R1, #10 ;O registrador R1 recebe o valor 10.
```

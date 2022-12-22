## Informações preliminares

<br>

1. ### **`Tipos de dados:`**  
    &nbsp; &nbsp; &nbsp; **1.1 Numérico sem sinal** 

    &nbsp; &nbsp; &nbsp; **1.2 Char**

    &nbsp; &nbsp; &nbsp; **1.3 String**

<br>

2. ### **`Tamanho dos dados:`** 
    
    &nbsp; &nbsp; &nbsp; **2.1 Inteiro sem sinal:** 16 bits.

    
    > Importante ressaltar que **NÃO há float ou double nativamente.**
    
   
    &nbsp; &nbsp; &nbsp; **2.2 Caractere:** 16 bits.
    

    &nbsp; &nbsp; &nbsp; **2.3 String:** 16 bits por posição + 16 bits para o '\0'.


<br>

## Instruções usadas pelo montador

<br>

### **`1. Label:`** 

 &nbsp; &nbsp; &nbsp; **1.1 Descrição:** 
    
 Rótulo/Nome que indica um endereço na memória - sendo que esse endereço pode pertencer a uma instrução ou a um dado.
    
 &nbsp; &nbsp; &nbsp;  **1.2. Utilização:** 

```asm
label: 
```

<br>

### **`2. Var`**

&nbsp; &nbsp; &nbsp; **2.1 Descrição:**

Operador para reservar uma quantidade de posições na memória - sendo que cada posição corresponde a 16 bits, determinada pelo número digitado. Está normalmente associada a um rótulo - ou *label*. 

&nbsp; &nbsp; &nbsp;**2.2 Parâmetros:**

Os parâmetros desse operador são o label  que aponta para o endereço inicial da memória reservada, o operador var e o número de posições a serem reservadas.
    
```asm
label: var #<num>
```

&nbsp; &nbsp; &nbsp; **2.3 Usando a instrução:**

 ```asm
 minhaVar: var #20 ; reserva 20 posições de 16 bits na memória, sendo que o rótulo "minhaVar" aponta para a primeira posição
 ```

<br> 

### **`3. Static`**

&nbsp; &nbsp; &nbsp; **3.1 Descrição:**
Operador para preencher a memória na posição apontada por *label*, mas em uma posição específica do espaço alocado na memória - aqui chamado de  *"pos"* - com um número *num* - o qual deve ser inteiro e sem sinal.

Isso significa que o *"pos"* permite acessar qualquer posição apontada pelo rótulo, e não somente a primeira

&nbsp; &nbsp; &nbsp;**3.2 Parâmetros:**

Os parâmetros desse operador são o static, o label  que aponta para o endereço inicial da memória reservada, a posição (pos) que você deseja alterar e o número(num) que você deseja inserir na posição.

```asm
<label> + #<pos>, #<num>
```

&nbsp; &nbsp; &nbsp; **3.3 Usando a instrução:**

 ```asm
 static minhaVar #0, #5  ;preenche a primeira posição apontada pelo rótulo "minhaVar" com o número 5
 static minhaVar #1, #8  ;preenche a segunda posição apontada pelo rótulo "minhaVar" com o número 8
 static minhaVar #2, #'a'  ;preenche a terceira posição apontada pelo rótulo "minhaVar" com o char "a"
 ```
<br> 

### **`4. String`**

&nbsp; &nbsp; &nbsp; **4.1 Descrição:**

Operador para alocar a quantidade necessária de posições de memória para armazenar a string em *"caracteres"* e mais uma posição para o '\0'. 

Preenche as posições de memória alocadas com os códigos ASCII da string, sendo que cada posição de memória tem 16 bits.

&nbsp; &nbsp; &nbsp;**4.2 Parâmetros:**

Os parâmetros desse operador são o label, que aponta para o endereço inicial da memória reservada, operador string , a string - sequência de caractéres - que você deseja alocar na memória.

```asm
<label>: string "<caracteres>"
```


&nbsp; &nbsp; &nbsp; **4.3 Usando a instrução:**

 ```asm
 mensagem: string "Exemplo" ;aloca 8 posições de memória ao todo: 7 para todas as letras e mais 1 para '\0' no final. 
                            ;O rótulo "mensagem" aponta para o primeiro caracter da string.
 ```
<br> 


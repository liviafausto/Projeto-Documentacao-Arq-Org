# Documentação das Instruções do Processador do ICMC

<br>

## Como ler essse Guia

Nesse guia, você encontrará as instruções do processador do ICMC. Cada instrução é detalhada em uma seção separada, contendo uma descrição da instrução, os parâmetros da instrução, os códigos de operação e um exemplo de uso com código comentado.

É importante ressaltar que a leitura desse guia não é obrigatória para o desenvolvimento de programas para o processador do ICMC. O guia foi criado para auxiliar os alunos que desejam entender o funcionamento do processador do ICMC.

Apesar disso, é recomendado que os alunos leiam esse guia para entender como as instruções do processador funcionam.

A recomendação é que a leitura das instruções seja feita de forma sequencial. Porém, caso você queira saber mais sobre uma instrução específica, você pode pular para a seção da instrução desejada.

<br>

## Suposições de nível de conhecimento

Para entender esse guia, você deve ter conhecimento básico de programação, preferencialmente em C ou em outra linguagem que permite manipulação da memória em nível mais baixo. Além disso, você deve ter conhecimento básico de arquitetura de computadores.

A recomendação do professor responsável pelo projeto é que o usuário desse guia tenha conhecimento igual ou superior ao equivalente da UNIDADE X DO `livro`.

<br>

## Instalação do Processador

Para instalar o simulador, você deve seguir os seguintes passos:

Caso seja usuário de Windows, você deve baixar o arquivo nesse link e seguir as instruções:

INSTRUÇÕES AQUI



Caso seja usuário de Linux, você deve baixar o arquivo nesse link e seguir as instruções:

INSTRUÇÕES AQUI




<br>

## Teste de Sumário

### Instruções de Manipulação de Dados

<br>

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

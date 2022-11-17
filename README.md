# Documentação das Instruções do Processador do ICMC

<br>

## Descrição

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec at porttitor odio. Maecenas orci massa, viverra vel elit eget, feugiat mollis quam.

<br>

## Como ler essse Guia

Nesse guia, você encontrará as instruções do processador do ICMC. Cada instrução é descrita em uma seção separada, contendo uma descrição da instrução, os parâmetros da instrução, os códigos de operação e um exemplo de uso com código comentado.

É importante ressaltar que a leitura desse guia não é obrigatória para o desenvolvimento de programas para o processador do ICMC. O guia foi criado para auxiliar os alunos que desejam entender o funcionamento do processador do ICMC.

Apesar disso, é recomendado que os alunos leiam esse guia para entender como o processador funciona e como os programas são executados.

A recomendação é que a leitura das instruções seja feita de forma sequencial. Porém, caso você queira saber mais sobre uma instrução específica, você pode pular para a seção da instrução desejada.

<br>

## Suposições de nível de conhecimento

Para entender esse guia, você deve ter conhecimento básico de programação, preferencialmente em C. Além disso, você deve ter conhecimento básico de arquitetura de computadores.

A recomendação do professor responsável pelo projeto é que o usuário desse guia tenha conhecimento igual ou superior ao equivalente da UNIDADE X DO `livro`.

<br>

## Instalação do Processador

Para instalar o simulador, você deve seguir os seguintes passos:


<br>

## **`Instruções de Manipulação de Dados`**


### **`1. Load`**

#### &nbsp; &nbsp; &nbsp; **1.1 - Descrição**
A instrução load é do tipo direto e tem como objetivo carregar um valor para um registrador. A instrução load é composta por um registrador destino e um endereço de memória.

<br>

#### &nbsp; &nbsp; &nbsp; **1.2 - Parâmetros**
Os parâmetros são o registrador destino e o endereço de memória que você deseja carregar no registrador, no formato:

```asm
load identificadorDoRegistrador, endereçoNaMemória
```

<br>

#### &nbsp; &nbsp; &nbsp; **1.3 - Usando a instrução**
```asm
loadR0, posAntNave
```

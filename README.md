# Documentação das Instruções do Processador do ICMC
Participantes:

Amanda Valukas Breviglieri Joioso;

Fernando Mezher Silva Lopes;

Guilherme Henrique Galdini Tosi;

João Pedro Dias Melo; 

Laura Fernandes Camargos; 

Livia Fausto Carnio;

Lucas Loureiro Rodrigues; 

Paulo Henrique Vedovatto Turquetti; 

Pedro Augusto Martins Gagini;

Pedro Guilherme Tolvo;

Pedro Henrique Salmaze;

Pedro Santos Souza;

Rafael Garcia Fortunato;

Rafaela Ferreira Lovatti.
<br>

## Como ler essse Guia

Nesse guia, você encontrará as instruções do processador do ICMC. Cada instrução é detalhada em uma seção separada, contendo uma descrição da instrução, os parâmetros da instrução, os códigos de operação e um exemplo de uso com código comentado.

É importante ressaltar que a leitura desse guia não é obrigatória para o desenvolvimento de programas para o processador do ICMC. O guia foi criado para auxiliar os alunos que desejam entender o funcionamento do processador do ICMC.

Apesar disso, é recomendado que os alunos leiam esse guia para entender como as instruções do processador funcionam.

A recomendação é que a leitura das instruções seja feita de forma sequencial. Porém, caso você queira saber mais sobre uma instrução específica, você pode pular para a seção da instrução desejada.

<br>

## Suposições de nível de conhecimento

Para entender esse guia, você deve ter conhecimento básico de programação, preferencialmente em C ou em outra linguagem que permite manipulação da memória em nível mais baixo. Além disso, você deve ter conhecimento básico de arquitetura de computadores.

A recomendação do professor responsável pelo projeto é que o usuário desse guia tenha conhecimento igual ou superior ao livro:

> PATTERSON, D. A., HENNESSY, J.L. Computer Organization and Design, Fifth Edition: The Hardware/Software Interface. Morgan Kaufmann Publishers, 2013

<br>

## Instalação do Simulador do Processador

Para instalar o simulador e obter orientações, você deve seguir os seguintes passos no GitLab do professor [aqui](https://gitlab.com/simoesusp/disciplinas/-/tree/master/SSC0513-BSI_Organizacao-e-Arquitetura-de-Computadores#simulador-para-programa%C3%A7%C3%A3o-em-assembly).

O tópico com as instruções já é aberto automaticamente no link, mas caso aconteça algum problema, o nome do tópico é: Simulador para programação em Assembly.




<br>

## Sumário

### [**`Declaração de Dados na Memória`**](/instrucoes/declaracao_de_dados.md)
1. Inteiro sem sinal
2. Char
2. String

### [**`Instruções de Manipulação de Dados`**](/instrucoes/manipulacao_de_dados.md)
1. Load
2. Loadn
3. Loadi
4. Store
5. Storei
6. MOV

### [**`Instruções Aritméticas`**](/instrucoes/aritmeticas.md)
1. Inc
2. Dec
3. Add
4. Sub
5. Div
6. Mul

### [**`Insctuções de Salto`**](/instrucoes/intruçõesSalto.md)
1. JMP

### [**`Insctuções de Chamada`**](/instrucoes/instruçõesChamada.md)
1. CALL

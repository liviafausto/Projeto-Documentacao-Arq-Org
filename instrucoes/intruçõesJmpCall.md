1. JMP
      1.1 Descrição:
 O JUMP é uma instrução que desvia o fluxo do código, alterando a ordem em que as instruções são executadas, podendo ser condicional ou incondicional. Um Jump incondicional é usado na forma JMP ,já o jump incodicional assume a forma J??, em que no local da interrogação se colocar outras letras a fim de determinar uma execução específica 
 
   1.2 Parâmetros:
O salto condicional irá utilizar o comparador que está dentro da ULA para verificar a condição e realizar o salto. Os parâmetros desta instrução são o label que indica o ponto do desvio da seguinte forma.
jmp PontodoDesvio
 
  1.3 Usando a instrução:
jmp PontodoDesvio; o fluxo do codigo ira pular para o label PontodoDesvio.
 
 
2. CALL
	2.1 Descrição
	A função call irá chamar um procedimento a ser executado, existindo 	dois conceitos para esse chamado, o primeiro é o “far” e  o “near” e o 	segundo o “relative” e “absolut”.
 
	2. 2 Parâmetros
1.Near relative call
Recebe um número negativo ou positivo indicando o número de bytes  que devem ser desviados da seguinte forma.
call rel8/rel16
2. Near absolut call
Na chamada absoluta você irá chamar o endereço exato que deseja chamar, utilizando os parâmetros da seguinte maneira.
call funçãochamada
 
2.3 Usando a instrução
LimpaTela:
	push fr
	push r0
	push r1
	push r3
 
loadn r0, #1200
loadn r1, #’ ‘
loadn r3, #0
 
Call LimpaTela;
Dessa forma independente de onde estejam as funções no código, ao executar o call ele irá chamar a função LimpaTela para ser executada.

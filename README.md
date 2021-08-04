# Eletromagnetismo
Trabalho computacional da disciplina de eletromagnetismo

Trabalho computacional feito para a disciplina de eletromagnetismo.

Entregue no dia 28/07/21

Foi feito em conjunto com José Agusto dos Santos. (Não sei seu github)

Eu trabalhei na parte computacional e o José no relatório. Nós dois fizemos a parte teórica das rotinas. Foi uma ótima experiência para aprender uma linguagem de programação nova.

Esse trabalho computacional consiste em 4 rotinas. 

As rotinas a e b era pra procurar o campo elétrico em um ponto do espaço gerado por um anel muito fino de cargas centralizado no sistema de coordenadas. 
Posicionamos o anel com a seguinte equação paramétrica:

( r*cos(phi), r*sin(phi), 0) , com r (raio do anel) definido pelo usuário e 0 <= phi <= 2*pi

A diferença entre as rotinas é que a rotina a pedia para acharmos o campo para um ponto no eixo do anel. Isso facilita muito a execução pois as componentes horizontais opostas 
do campo se cancelam, facilitando as contas pois podemos portanto calcular o campo sem a necessidade de uma integral. Já na rotina b era preciso achar o capo em qualquer ponto do 
espaço, assim tinhamos que considerar todas as 3 contribuições do campo nos eixos x, y e z. Para resolver isso poderíamos usar uma forma numérica para solucionarmos a integral.
Eu fiz o estudo teórico da rotina b e trabalhei na procura de um método numérico para solucionar a integração. Trabalhei com o método de 1/3 de Simpson.

As rotinas c e d queriam agora o campo magnético em um ponto gerado por uma linha percorrida por uma corrente I

Na rotina c, a fonte do campo era uma linha infinita paralela ao eixo z. Devido a natureza infinita do campo, o cálculo deste campo era bem mais simples que a rotina d. Analíticamente
foi possível descrever o módulo do campo eletromagnético com apenas uma equação simples. Já o exercício d era para definirmos o campo magnético em qualquer ponto do espaço gerado por
uma linha qualquer escolhida pelo usuário. Para solucionar o d foi necessário um método numérico para solucionar a integral necessária para este campo
Eu fiz o estudo teórico da rotina d. Escolhi novamente o método 1/3 de Simpson.

De maneira geral este trabalho foi uma ótima oportunidade para conhecer a linguagem Julia

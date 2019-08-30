# Prova-01---DCA1202

Questao 01 -
1. (2,0 pontos) Um desenvolvedor precisa enviar as informacoes de uma matriz de 8x8 inteiros (64
ao todo) para um dispositivo usando um enlace de r ́adio de baixa velocidade. Na aplica ̧c ̃ao que
desenvolveu, os inteiros assumem valores iguais APENAS a “0” e “1”, nunca outros valores. Em
testes realizados, verificou-se que a taxa de transferˆencia dos bits n ̃ao era r ́apida o suficiente para
que enviasse os 64 inteiros na velocidade necess ́aria para fazer o sistema operar corretamente.
Uma ideia surgiu: codificar grupos de 32 elementos da matriz em um ́unico inteiro (unsigned int),
transmiti-lo via r ́adio e decodific ́a-lo no receptor. As quatro primeiras linhas da matriz foram co-
dificadas mapeando os valores “0” ou “1” nos bits de um inteiro, repetindo a mesma ideia para
os bits de outro inteiro. E a ideia funcionou muito bem! O desenvolvedor criou duas funcoes codificar() 
que prepara os bytes da matriz “ matrizEnviada” para serem codicados nas variaveis inteiro1 e inteiro2, e
decodificar() que realiza o processo inverso, escrevendo a decodificacao na matriz “ matrizRecebida ”.

#include <stdio.h>
int matrizEnviada[8][8];
int matrizRecebida[8][8];
unsigned int inteiro1, inteiro2;
void codificar(){
}
void decodificar(){
}
int main(void){
int i, j;
for(i=0; i<8; i++){
for(j=0; j<8; j++){
matrizEnviada[i][j] = rand()%2;
}
}
// mostra matrizEnviada
codificar();
// mostra inteiro1 e inteiro2
decodificar();
// mostra matrizRecebida
}
Neste contexto, apresente sua solu ̧c ̃ao para a codifica ̧c ̃ao pedida. Se necess ́ario, modifique o c ́odigo
de referˆencia fornecido, mas garantindo que a codifica ̧c ̃ao ser ́a conforme solicitado

Questao 02 (2,0 pontos)- Um desenvolvedor precisa bolar um esquema para copiar matrizes tridimensionais com porcoes de memoria, mas pelo menos uma condicao ser levada em conta: TODOS OS VALORES DA MATRIZ devem ser armazenados em apenas UM UNICO BLOCO DE MEMORIA alocado dinamicamente, de sorte que a copia destes blocos entre as porcoes de memoria possa ser feita com UMA UNICA chamada da funcao memcpy(). Implemente esse esquema.

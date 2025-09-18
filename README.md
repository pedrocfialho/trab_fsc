# trab_fsc
Trabalho 1 de FUNDAMENTOS DE SISTEMAS COMPUTACIONAIS
Grupo: Pedro Constante Fialho, Francisco Reis, Bernardo Lacerda e Leonardo Azambuja

Questão 1 – N primeiros números ímpares

Escreve os N primeiros números inteiros positivos maiores que zero, armazenando-os de forma sequencial a partir do endereço 0x20.
O programa lê N da memória, inicializa os registradores: v1 recebe 1 (primeiro ímpar), v2 é o ponteiro de endereço e v3 o contador de números gerados.
Dentro do loop, o valor de v1 é gravado na memória e atualizado somando 2, v2 é incrementado e v3 aumenta até alcançar N.
O programa termina com hlt.

<img width="1255" height="948" alt="rd1" src="https://github.com/user-attachments/assets/7f78cb0e-4831-4d9b-8333-f2c39926674f" />

Questão 2 – Sequência de Fibonacci

Gera os N primeiros números da sequência de Fibonacci e armazena na memória a partir de 0x30.
Registradores usados: v0 = 0, v1 = 1 (início da sequência), v3 contador de termos, v4 guarda N, v7 ponteiro da memória.
A cada loop, o próximo termo é calculado somando os dois anteriores, armazenado na memória, e os registradores são atualizados. Loop termina quando todos os N termos foram calculados.

<img width="1258" height="933" alt="rd2" src="https://github.com/user-attachments/assets/8be1393d-1979-48b4-8a13-9548fd3ed70f" />

Questão 3 – Maior número na memória

Procura o maior número entre os endereços 0x40 e 0x80 e grava em 0x90.
Registradores: v0 guarda maior valor encontrado, v2 percorre a memória, v3 é o limite (0x80).
No loop, cada valor é comparado e atualizado se maior que v0. Após percorrer todo intervalo, grava v0 em 0x90.

<img width="1244" height="951" alt="rd3" src="https://github.com/user-attachments/assets/441516d3-ae74-4b2c-9518-23663e130066" />

Questão 4 – Tornar valores ímpares

Lê os valores entre 0x40 e 0x90 e escreve a partir de 0x90, somando 1 aos pares.
Loop percorre cada valor, verifica se é ímpar; se não, soma 1 e armazena. Processo se repete até percorrer os 64 valores.

<img width="1258" height="940" alt="rd4" src="https://github.com/user-attachments/assets/589b0598-4289-451c-8c0a-4a738d9174c3" />

Questão 5 – Soma igual a 10

Procura entre 0x60 e 0x70 dois números cuja soma seja 10 e, se encontrados, salva suas posições em 0x80 e 0x90.
Usa dois loops aninhados: o primeiro percorre o intervalo, o segundo compara cada número com os subsequentes. Se a soma for 10, grava endereços e encerra com hlt.

<img width="1263" height="944" alt="rd5" src="https://github.com/user-attachments/assets/10b63f58-da7a-4c8e-8362-e4a6852fef2b" />

Questão 6 – Inverter valores na memória

Inverte os valores entre 0x40 e 0x60.
Inicializa ponteiros para os blocos de memória e percorre os valores em loops, gravando na ordem inversa. Condições de parada evitam ler ou escrever fora do intervalo.

<img width="1263" height="938" alt="rd6" src="https://github.com/user-attachments/assets/7bbf0c45-2bf4-4e24-8ac7-e19f6bd662b0" />

Questão 7 – Diagonal principal da matriz

Lê M e N (0x40 e 0x42) e elementos da matriz a partir de 0x44.
Calcula k = min(M, N) para percorrer a diagonal principal e escreve os elementos a partir de 0x100. Ponteiros avançam adequadamente para ler cada elemento da diagonal.

<img width="1256" height="928" alt="rd7" src="https://github.com/user-attachments/assets/fdb34c88-1711-4529-bb4d-8dd206a121ec" />


Questão 8 – Escrever nomes completos

Cria variáveis com os nomes dos integrantes e escreve cada letra na saída do simulador (0xf006).
Loop percorre cada letra, imprime, e repete para cada nome. Ao final, pula linha entre os nomes.

<img width="1260" height="945" alt="rd8" src="https://github.com/user-attachments/assets/539751ac-aa51-4775-a511-3fbe6997d030" />

Questão 9 – Verificar palíndromo

Lê a palavra a partir de 0x70 e o tamanho em 0x60.
Compara os caracteres do início e do fim, avançando os ponteiros até o meio. Se todos coincidirem, é palíndromo. Depois, escreve a palavra na saída do simulador.

<img width="1256" height="944" alt="rd9" src="https://github.com/user-attachments/assets/b58ce6be-c45e-4c44-8075-c8eb996dcc88" />

Questão 10 – Contador de vogais

Conta quantas vezes aparecem as vogais A, E, I, O e U em uma palavra.

Palavra inicia em 0x60, tamanho em 0x58

Contadores armazenados em: A → 0x40, E → 0x44, I → 0x48, O → 0x50, U → 0x52
Loop percorre cada caractere, compara com valores ASCII das vogais, incrementa contadores e grava resultados na memória.


<img width="1257" height="937" alt="rd10" src="https://github.com/user-attachments/assets/4e6d7e1c-9979-4f75-9df0-46ef9b087f9f" />

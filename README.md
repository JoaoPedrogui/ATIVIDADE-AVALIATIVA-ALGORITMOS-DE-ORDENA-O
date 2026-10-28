Organização de Notas de Alunos com Bubble Sort e Quick Sort
1. Objetivo da Aplicação

O objetivo desta aplicação é desenvolver um programa na linguagem C capaz de organizar as notas de alunos em ordem crescente, utilizando dois algoritmos de ordenação: Bubble Sort e Quick Sort.

A aplicação permite visualizar as notas originais e comparar os resultados obtidos pelos dois métodos.

2. Situação-Problema

Em uma escola, um professor precisa organizar as notas dos alunos para facilitar a análise do desempenho da turma. Quando há várias notas, organizá-las manualmente pode ser demorado e sujeito a erros.

Para resolver esse problema, foi desenvolvido um programa que recebe um conjunto de 10 notas e as organiza automaticamente em ordem crescente.

A aplicação utiliza os algoritmos Bubble Sort e Quick Sort para realizar a mesma tarefa, permitindo observar como diferentes métodos podem resolver um mesmo problema do cotidiano.

3. Tecnologias Utilizadas
Linguagem de programação: C.
Biblioteca utilizada: stdio.h.
Algoritmos de ordenação: Bubble Sort e Quick Sort.
Compilador: GCC, Code::Blocks ou outro compilador compatível com C.
4. Instruções de Execução
Passo 1 — Salvar o código

Salve o código-fonte do programa em um arquivo chamado main.c.

Passo 2 — Compilar o programa

Se estiver utilizando o GCC, abra o terminal na pasta do projeto e execute:

bash
gcc main.c -o notas

Passo 3 — Executar o programa

No Linux ou macOS, execute:

bash
./notas


No Windows, execute:

bash
notas.exe


Caso esteja utilizando o Code::Blocks ou outro ambiente de desenvolvimento, basta abrir o projeto, compilar e executar o programa.

5. Explicação dos Algoritmos
5.1 Bubble Sort

O Bubble Sort é um algoritmo de ordenação que compara elementos vizinhos de um vetor. Quando dois elementos estão fora da ordem desejada, suas posições são trocadas.

Esse processo é repetido até que todos os elementos estejam organizados.

Neste projeto, o Bubble Sort compara as notas dos alunos e as organiza da menor para a maior.

Complexidade de tempo:

Melhor caso: O(n), com uma implementação que detecta quando não há mais trocas.
Caso médio: O(n²).
Pior caso: O(n²).

A implementação deste projeto não utiliza a detecção antecipada de ausência de trocas; portanto, sua complexidade de tempo permanece O(n²), mesmo quando as notas já estão ordenadas.

5.2 Quick Sort

O Quick Sort é um algoritmo de ordenação que utiliza a estratégia de divisão e conquista.

Ele escolhe um elemento como pivô e reorganiza o vetor, colocando os elementos menores ou iguais ao pivô de um lado e os maiores do outro. Em seguida, aplica o mesmo procedimento recursivamente às partes restantes.

Neste projeto, o último elemento de cada trecho do vetor é escolhido como pivô.

Complexidade de tempo:

Caso médio: O(n log n).
Melhor caso: O(n log n).
Pior caso: O(n²).

O Quick Sort costuma apresentar bom desempenho em conjuntos maiores de dados, embora seu desempenho dependa da escolha do pivô.

6. Exemplo de Execução

O programa utiliza as seguintes notas iniciais:

text
78 45 92 60 85 30 70 55 98 66


Após a execução dos dois algoritmos, o resultado esperado é:

text
=== ORGANIZACAO DAS NOTAS ===
Notas originais: 78 45 92 60 85 30 70 55 98 66
Bubble Sort:     30 45 55 60 66 70 78 85 92 98
Quick Sort:      30 45 55 60 66 70 78 85 92 98


Os dois algoritmos produzem a mesma sequência ordenada, pois utilizam os mesmos dados de entrada e organizam as notas em ordem crescente.

7. Conclusão

O desenvolvimento desta aplicação permitiu compreender e implementar dois algoritmos importantes de ordenação na linguagem C.

O Bubble Sort realiza comparações e trocas entre elementos vizinhos, enquanto o Quick Sort divide o vetor em partes menores para realizar a ordenação.

Conclui-se que ambos resolvem o problema proposto corretamente, mas apresentam diferenças de funcionamento e desempenho. O Quick Sort geralmente é mais eficiente para conjuntos maiores de dados, enquanto o Bubble Sort é útil para compreender os conceitos básicos de ordenação.

A aplicação demonstra como os algoritmos de ordenação podem ser utilizados para resolver situações práticas, como a organização das notas de alunos em uma escola.

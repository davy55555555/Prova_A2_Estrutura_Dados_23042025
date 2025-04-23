# Prova A2 de Estrutura de Dados - 23/04/2025
**Nome:** Deivid Cerqueira 
**RGM:** 39670953

## Índice
- [Questões Objetivas](#parte-1-questões-objetivas) (neste arquivo)
- [Análise de Código](analise_codigo.md)
- [Questões Subjetivas](questoes_subjetivas.md)

## Parte 1: Questões Objetivas

### Questão 1
**Qual das seguintes alternativas define corretamente uma estrutura de dados?**
- a) É uma forma de organizar os dados de forma aleatória.
- b) É uma forma de armazenar e organizar os dados para uso posterior.
- c) É um conjunto de algoritmos para processar os dados.
- d) É um tipo de dado primitivo.

**Resposta:** A alternativa correta é a **b**, pois uma estrutura de dados é fundamentalmente um método para organizar, gerenciar e armazenar dados de forma que permitam acesso e modificações eficientes para uso futuro.

### Questão 2
**Qual a principal diferença entre um vetor e uma matriz?**
- a) Vetores armazenam dados de tipos diferentes, enquanto matrizes armazenam dados de um mesmo tipo.
- b) Vetores têm tamanho dinâmico, enquanto matrizes têm tamanho fixo.
- c) Vetores são unidimensionais, enquanto matrizes podem ser multidimensionais.
- d) Não há diferença, ambos são a mesma estrutura de dados.

**Resposta:** A alternativa correta é a **c**. Vetores representam coleções de dados em uma única dimensão (linha ou coluna), enquanto matrizes são estruturas bidimensionais ou multidimensionais que organizam elementos em linhas e colunas.

### Questão 3
**Qual das seguintes alternativas descreve corretamente a estrutura de dados Pilha?**
- a) Os elementos são acessados de forma aleatória.
- b) O primeiro elemento a entrar é o primeiro a sair (FIFO).
- c) O último elemento a entrar é o primeiro a sair (LIFO).
- d) Os elementos são dispostos em uma estrutura linear.

**Resposta:** A alternativa correta é a **c**. Uma pilha segue o princípio LIFO (Last In, First Out), onde apenas o elemento mais recentemente adicionado (topo) pode ser acessado ou removido.

### Questão 4
**Em uma fila, qual a ordem de entrada e saída dos elementos?**
- a) O primeiro elemento a entrar é o último a sair (LIFO).
- b) O último elemento a entrar é o primeiro a sair (LIFO).
- c) O primeiro elemento a entrar é o primeiro a sair (FIFO).
- d) A ordem de entrada e saída é aleatória.

**Resposta:** A alternativa correta é a **c**. Uma fila implementa o princípio FIFO (First In, First Out), onde os elementos são processados na mesma ordem em que foram inseridos.

### Questão 5
**Qual das seguintes alternativas descreve corretamente uma lista?**
- a) É uma estrutura de dados onde os elementos são organizados de forma hierárquica.
- b) É uma estrutura de dados com tamanho fixo.
- c) É uma estrutura de dados onde os elementos são organizados linearmente.
- d) É uma estrutura de dados que só permite acesso sequencial.

**Resposta:** A alternativa correta é a **c**. Uma lista é uma estrutura de dados que organiza elementos em uma sequência linear, podendo ser implementada de diversas formas (encadeada, duplamente encadeada, etc.).

### Questão 6
**Qual a principal característica de uma árvore?**
- a) Os elementos são organizados em uma sequência linear.
- b) Os elementos têm uma relação do tipo pai e filho.
- c) Os elementos são todos do mesmo tipo de dado.
- d) A árvore não possui um nó raiz.

**Resposta:** A alternativa correta é a **b**. A característica fundamental de uma árvore é a organização hierárquica dos seus elementos, estabelecendo relações pai-filho entre os nós.

### Questão 7
**Qual a principal diferença entre um grafo e uma árvore?**
- a) Grafos são direcionados, enquanto árvores não são.
- b) Em grafos, os elementos podem ter relações mais complexas do que em árvores.
- c) Árvores são mais eficientes para representar mapas.
- d) Grafos não possuem nós raiz.

**Resposta:** A alternativa correta é a **b**. Em um grafo, os elementos (ou vértices) podem ter relações (arestas) arbitrárias, formando ciclos, enquanto uma árvore é um tipo especial de grafo acíclico, com exatamente um caminho entre quaisquer dois nós.

### Questão 8
**Qual das seguintes alternativas NÃO é uma operação básica em uma Pilha?**
- a) PUSH
- b) POP
- c) ENQUEUE
- d) TOP

**Resposta:** A alternativa correta é a **c**. ENQUEUE é uma operação específica de filas (adiciona um elemento ao final da fila), enquanto as operações típicas de pilha são PUSH (adiciona ao topo), POP (remove do topo) e TOP/PEEK (consulta o topo).

### Questão 9
**Qual das seguintes alternativas é uma operação básica em uma Fila?**
- a) PUSH
- b) POP
- c) ENQUEUE
- d) TOP

**Resposta:** A alternativa correta é a **c**. ENQUEUE é a operação que adiciona um elemento ao final da fila, sendo uma das operações fundamentais dessa estrutura junto com DEQUEUE (remove do início).

### Questão 10
**Qual a função da operação SIZE?**
- a) Adicionar um elemento.
- b) Remover um elemento.
- c) Retornar o número de elementos.
- d) Retornar o elemento do topo/cabeça.

**Resposta:** A alternativa correta é a **c**. A operação SIZE retorna a quantidade de elementos presentes na estrutura de dados, sem modificá-la.

### Questão 11
**Qual a função da operação EMPTY?**
- a) Verificar se a estrutura está vazia.
- b) Retornar o elemento do topo/cabeça.
- c) Inverter a ordem dos elementos.
- d) Ordenar os elementos.

**Resposta:** A alternativa correta é a **a**. A operação EMPTY verifica se a estrutura está vazia, geralmente retornando um valor booleano (true se vazia, false se contiver elementos).

### Questão 12
**Qual a estrutura de dados que utiliza o conceito de LIFO?**
- a) Fila
- b) Lista
- c) Pilha
- d) Vetor

**Resposta:** A alternativa correta é a **c**. A Pilha (Stack) é baseada no princípio LIFO (Last In, First Out), onde apenas o elemento mais recentemente adicionado pode ser acessado ou removido.

### Questão 13
**Qual a estrutura de dados que utiliza o conceito de FIFO?**
- a) Fila
- b) Lista
- c) Pilha
- d) Vetor

**Resposta:** A alternativa correta é a **a**. A Fila (Queue) implementa o princípio FIFO (First In, First Out), garantindo que os elementos sejam processados na mesma ordem em que foram adicionados.

### Questão 14
**Em que situação usaríamos a estrutura de dados Pilha?**
- a) Para simular uma fila de atendimento.
- b) Para organizar os arquivos em um diretório.
- c) Para implementar a função "desfazer" de um editor de texto.
- d) Para armazenar os contatos de um celular.

**Resposta:** A alternativa correta é a **c**. A função "desfazer" (undo) em editores de texto é uma aplicação típica de pilha, pois as ações são desfeitas na ordem inversa em que foram realizadas (LIFO).

### Questão 15
**Em que situação usaríamos a estrutura de dados Fila?**
- a) Para controlar a ordem de impressão de documentos.
- b) Para armazenar as páginas visitadas em um navegador.
- c) Para implementar um jogo de cartas.
- d) Para organizar os livros em uma biblioteca.

**Resposta:** A alternativa correta é a **a**. Filas de impressão são um exemplo clássico da aplicação de filas em sistemas reais, garantindo que os documentos sejam impressos na ordem em que foram enviados.

### Questão 16
**Qual a forma de acesso aos elementos em um vetor?**
- a) Através de chaves.
- b) Através de índices.
- c) Através de ponteiros.
- d) De forma aleatória.

**Resposta:** A alternativa correta é a **b**. Em um vetor, os elementos são acessados diretamente através de índices numéricos, permitindo o acesso aleatório em tempo constante O(1).

### Questão 17
**Qual a vantagem de usar uma matriz em relação a um vetor?**
- a) Matrizes podem armazenar mais dados.
- b) Matrizes têm um acesso mais rápido aos elementos.
- c) Matrizes podem representar dados com mais de uma dimensão.
- d) Não há vantagem, vetores são sempre mais eficientes.

**Resposta:** A alternativa correta é a **c**. A principal vantagem das matrizes é permitir a representação de dados bidimensionais ou multidimensionais, como tabelas, grades e relações espaciais.

### Questão 18
**Qual a operação utilizada para adicionar um elemento em uma lista?**
- a) PUSH
- b) POP
- c) ENQUEUE
- d) ADD

**Resposta:** A alternativa correta é a **d**. A operação ADD (ou INSERT) é utilizada para adicionar elementos em uma lista, podendo especificar a posição da inserção.

### Questão 19
**Qual a operação utilizada para remover um elemento de uma lista?**
- a) REMOVE
- b) POP
- c) DEQUEUE
- d) ADD

**Resposta:** A alternativa correta é a **a**. REMOVE é a operação padrão para eliminar elementos de uma lista, podendo especificar o elemento ou a posição a ser removida.

### Questão 20
**Qual a estrutura de dados mais adequada para representar uma árvore genealógica?**
- a) Fila
- b) Lista
- c) Pilha
- d) Árvore

**Resposta:** A alternativa correta é a **d**. A estrutura de dados Árvore é naturalmente adequada para representar relações hierárquicas como árvores genealógicas, onde cada nó pode ter ancestrais e descendentes.

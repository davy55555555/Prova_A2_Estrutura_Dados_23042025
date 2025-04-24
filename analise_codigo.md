# Parte 2: Análise de Código

## 1. Análise de Código em C
```c
#include <stdio.h>
int main() {
    int vetor[5] = {10, 20, 30, 40, 50};
    int *ptr = vetor;
    printf("%d", *(ptr + 2));
    return 0;
}
```

**Código explicado e comentado:**
```c
#include <stdio.h>  // Inclui biblioteca para funções de entrada/saída

int main() {
    /* Declara e inicializa um vetor de 5 elementos inteiros */
    int vetor[5] = {10, 20, 30, 40, 50};
    
    /* Cria um ponteiro que aponta para o primeiro elemento do vetor
       Em C, o nome do vetor é um ponteiro para seu primeiro elemento */
    int *ptr = vetor;
    
    /* Acessa o elemento na posição ptr + 2 (terceiro elemento)
       A operação ponteiro + 2 desloca 2 posições, considerando o tamanho do tipo */
    printf("%d", *(ptr + 2));  /* Equivalente a vetor[2] ou *(vetor + 2) */
    
    return 0;  // Retorna 0 para indicar que o programa foi executado com sucesso
}
```

**Resultado:** O programa imprime `30`, pois `*(ptr + 2)` acessa o terceiro elemento do vetor (índice 2).

## 2. Análise de Código em Java
```java
public class Main {
    public static void main(String[] args) {
        Stack<String> stack = new Stack<>();
        stack.push("A");
        stack.push("B");
        stack.push("C");
        System.out.println(stack.pop());
        System.out.println(stack.peek());
    }
}
```

**Código explicado e comentado:**
```java
import java.util.Stack;  // Importação necessária para utilizar a classe Stack

public class Main {
    public static void main(String[] args) {
        // Instancia uma nova pilha para armazenar strings
        Stack<String> stack = new Stack<>();
        
        // Adiciona três elementos na pilha em sequência (de baixo para cima)
        stack.push("A");  // Base da pilha
        stack.push("B");  // Meio da pilha
        stack.push("C");  // Topo da pilha
        
        // Remove e retorna o elemento do topo (C) 
        // A pilha agora contém apenas [A, B]
        System.out.println(stack.pop());
        
        // Retorna o novo elemento do topo (B) sem removê-lo
        System.out.println(stack.peek());
    }
}
```

**Resultado:**
```
C
B
```

## 3. Análise de Código em Python
```python
fila = ["A", "B", "C"]
fila.append("D")
print(fila.pop(0))
print(fila[0])
```

**Código explicado e comentado:**
```python
# Cria uma lista que será usada para simular o comportamento de uma fila
fila = ["A", "B", "C"]  # Inicializa com três elementos

# Adiciona o elemento "D" ao final da fila
fila.append("D")  # Fila: ["A", "B", "C", "D"]

# Remove e retorna o primeiro elemento (índice 0) da fila
# Implementa o comportamento de dequeue da estrutura de dados fila
print(fila.pop(0))  # Remove e imprime "A", fila agora é ["B", "C", "D"]

# Imprime o elemento que agora está no início da fila, sem removê-lo
print(fila[0])  # Imprime "B"
```

**Resultado:**
```
A
B
```

## 4. Análise de Código em C#
```csharp
public class Program {
    public static void Main(string[] args) {
        LinkedList<int> lista = new LinkedList<int>();
        lista.AddLast(1);
        lista.AddLast(2);
        lista.AddFirst(0);
        Console.WriteLine(lista.First.Value);
        Console.WriteLine(lista.Last.Value);
    }
}
```

**Código explicado e comentado:**
```csharp
using System;  // Namespace para recursos básicos
using System.Collections.Generic;  // Namespace para coleções genéricas, incluindo LinkedList

public class Program {
    public static void Main(string[] args) {
        // Cria uma nova lista duplamente encadeada para armazenar inteiros
        LinkedList<int> lista = new LinkedList<int>();
        
        // Adiciona o valor 1 ao final da lista vazia
        lista.AddLast(1);  // Lista: [1]
        
        // Adiciona o valor 2 ao final da lista
        lista.AddLast(2);  // Lista: [1, 2]
        
        // Adiciona o valor 0 ao início da lista
        lista.AddFirst(0);  // Lista: [0, 1, 2]
        
        // Imprime o valor do primeiro nó da lista (First é uma propriedade que retorna o primeiro nó)
        Console.WriteLine(lista.First.Value);  // Imprime: 0
        
        // Imprime o valor do último nó da lista (Last é uma propriedade que retorna o último nó)
        Console.WriteLine(lista.Last.Value);  // Imprime: 2
    }
}
```

**Resultado:**
```
0
2
```

## 5. Análise de Código em JavaScript
```javascript
let vetor = [1, 2, 3, 4, 5];
vetor.splice(2, 1);
console.log(vetor.length);
console.log(vetor[2]);
```

**Código explicado e comentado:**
```javascript
// Cria um array com 5 elementos inteiros
let vetor = [1, 2, 3, 4, 5];

// O método splice() modifica o array original:
// - Primeiro parâmetro (2): índice a partir do qual modificar o array
// - Segundo parâmetro (1): quantidade de elementos a remover
vetor.splice(2, 1);  // Remove 1 elemento a partir do índice 2 (valor 3)
                     // Resulta em: [1, 2, 4, 5]

// Imprime o comprimento (tamanho) do array após a remoção do elemento
console.log(vetor.length);  // Resultado: 4

// Imprime o elemento que agora está na posição de índice 2
// Após a remoção, o elemento nesta posição mudou de 3 para 4
console.log(vetor[2]);  // Resultado: 4
```

**Resultado:**
```
4
4
```

## 6. Análise de Código em Python
```python
def funcao_misteriosa(lista):
    resultado = []
    for elemento in lista:
        if elemento % 2 == 0:
            resultado.append(elemento * 2)
        else:
            resultado.append(elemento + 1)
    return resultado
lista_exemplo = [1, 2, 3, 4, 5]
print(funcao_misteriosa(lista_exemplo))
```

**Código explicado e comentado:**
```python
def funcao_misteriosa(lista):
    """
    Esta função processa cada elemento de uma lista de números inteiros:
    - Se o elemento for par (divisível por 2), multiplica o elemento por 2
    - Se o elemento for ímpar, adiciona 1 ao elemento
    Retorna uma nova lista com os resultados das operações
    """
    resultado = []  # Inicializa uma lista vazia para armazenar os resultados
    
    # Itera por cada elemento da lista recebida como parâmetro
    for elemento in lista:
        # Verifica se o elemento é par usando o operador de módulo (%)
        # Se o resto da divisão por 2 for 0, o número é par
        if elemento % 2 == 0:
            resultado.append(elemento * 2)  # Multiplica o elemento por 2
        else:
            resultado.append(elemento + 1)  # Adiciona 1 ao elemento
    
    return resultado  # Retorna a lista de resultados

# Lista de teste para a função
lista_exemplo = [1, 2, 3, 4, 5]

# Chama a função e imprime o resultado
# Processamento esperado:
# 1 (ímpar) -> 1+1 = 2
# 2 (par) -> 2*2 = 4
# 3 (ímpar) -> 3+1 = 4
# 4 (par) -> 4*2 = 8
# 5 (ímpar) -> 5+1 = 6
print(funcao_misteriosa(lista_exemplo))
```

**Resultado:** `[2, 4, 4, 8, 6]`

## 7. Análise de Código em C
```c
#include <stdio.h>
#include <stdlib.h>
struct No {
    int valor;
    struct No *proximo;
};
int main() {
    struct No *inicio = malloc(sizeof(struct No));
    inicio->valor = 10;
    inicio->proximo = NULL;
    struct No *segundo = malloc(sizeof(struct No));
    segundo->valor = 20;
    segundo->proximo = inicio;
    printf("%d", segundo->proximo->valor);
    free(inicio);
    free(segundo);
    return 0;
}
```

**Código explicado e comentado:**
```c
#include <stdio.h>    // Biblioteca para operações de entrada/saída
#include <stdlib.h>   // Biblioteca para alocação dinâmica de memória (malloc, free)

// Define uma estrutura para representar um nó em uma lista encadeada
struct No {
    int valor;         // Campo para armazenar um valor inteiro
    struct No *proximo; // Ponteiro para o próximo nó na lista
};

int main() {
    // Aloca dinamicamente memória para o primeiro nó
    struct No *inicio = malloc(sizeof(struct No));
    inicio->valor = 10;        // Atribui o valor 10 ao primeiro nó
    inicio->proximo = NULL;    // Inicialmente, não há próximo nó
    
    // Aloca dinamicamente memória para o segundo nó
    struct No *segundo = malloc(sizeof(struct No));
    segundo->valor = 20;          // Atribui o valor 20 ao segundo nó
    segundo->proximo = inicio;    // O segundo nó aponta para o primeiro nó
    
    // Imprime o valor armazenado no nó apontado pelo campo 'proximo' do segundo nó
    // Ou seja, imprime o valor do primeiro nó (10)
    printf("%d", segundo->proximo->valor);
    
    // Libera a memória alocada para os nós, evitando vazamento de memória
    free(inicio);
    free(segundo);
    
    return 0;  // Termina o programa com código de saída 0 (sucesso)
}
```

**Resultado:** `10`

## 8. Análise de Código em Java
```java
import java.util.LinkedList;
public class Main {
    public static void main(String[] args) {
        LinkedList<Integer> fila = new LinkedList<>();
        fila.add(10);
        fila.add(20);
        fila.add(30);
        System.out.println(fila.poll());
        System.out.println(fila.peek());
    }
}
```

**Código explicado e comentado:**
```java
import java.util.LinkedList;  // Importa a classe LinkedList do pacote java.util

public class Main {
    public static void main(String[] args) {
        // Cria uma LinkedList para armazenar Integers
        // LinkedList pode ser usada como fila em Java
        LinkedList<Integer> fila = new LinkedList<>();
        
        // Adiciona três elementos à fila (na ordem FIFO)
        fila.add(10);  // Primeiro elemento: 10
        fila.add(20);  // Segundo elemento: 20
        fila.add(30);  // Terceiro elemento: 30
        // Estado atual da fila: [10, 20, 30]
        
        // poll() remove e retorna o primeiro elemento da fila
        System.out.println(fila.poll());  // Imprime 10 e remove da fila
        // Estado atual da fila: [20, 30]
        
        // peek() retorna, mas não remove, o primeiro elemento da fila
        System.out.println(fila.peek());  // Imprime 20 sem removê-lo
        // Estado final da fila: [20, 30]
    }
}
```

**Resultado:**
```
10
20
```

## 9. Análise de Código em Python
```python
def recursiva(n):
    if n == 0:
        return 0
    else:
        return n + recursiva(n-1)
print(recursiva(5))
```

**Código explicado e comentado:**
```python
def recursiva(n):
    """
    Função recursiva que calcula a soma de todos os números inteiros de 0 até n.
    Cada chamada recursiva adiciona n ao resultado da chamada para n-1.
    
    Exemplos:
    recursiva(0) = 0
    recursiva(1) = 1 + 0 = 1
    recursiva(2) = 2 + 1 + 0 = 3
    recursiva(3) = 3 + 2 + 1 + 0 = 6
    recursiva(4) = 4 + 3 + 2 + 1 + 0 = 10
    recursiva(5) = 5 + 4 + 3 + 2 + 1 + 0 = 15
    
    Params:
        n: número inteiro não negativo
    
    Return:
        Soma de todos os inteiros de 0 até n
    """
    # Caso base: quando n é 0, retorna 0
    if n == 0:
        return 0
    
    # Caso recursivo: retorna n + resultado da soma de 0 até (n-1)
    else:
        return n + recursiva(n-1)

# Testa a função com n = 5
print(recursiva(5))  # Resultado esperado: 15
```

**Resultado:** `15`

## 10. Análise de Código em JavaScript
```javascript
function arvore(n) {
    if (n <= 1) {
        return 1;
    } else {
        return arvore(n - 1) + arvore(n - 2);
    }
}
console.log(arvore(4));
```

**Código explicado e comentado:**
```javascript
/**
 * Calcula o n-ésimo número da sequência de Fibonacci
 * A sequência é definida como:
 * F(0) = 1, F(1) = 1, F(n) = F(n-1) + F(n-2) para n > 1
 * 
 * A sequência começa: 1, 1, 2, 3, 5, 8, 13, 21, ...
 * 
 * Esta é uma implementação recursiva, que para cada valor n > 1, 
 * faz duas chamadas recursivas, resultando em uma complexidade exponencial O(2^n).
 * 
 * @param {number} n - Posição na sequência de Fibonacci (começando do 0)
 * @return {number} O n-ésimo número de Fibonacci
 */
function arvore(n) {
    // Casos base: F(0) = 1 e F(1) = 1
    if (n <= 1) {
        return 1;
    } 
    // Caso recursivo: F(n) = F(n-1) + F(n-2)
    else {
        return arvore(n - 1) + arvore(n - 2);
    }
}

// Calcula o valor de F(4) na sequência de Fibonacci
// F(4) = F(3) + F(2) = (F(2) + F(1)) + (F(1) + F(0)) = (2 + 1) + (1 + 1) = 5
console.log(arvore(4));
```

**Resultado:** `5`

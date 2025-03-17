# Árvore Rubro-Negra

Este projeto implementa uma árvore rubro-negra (Red-Black Tree) em C, incluindo operações como inserção, rotações e ajustes para manter as propriedades da estrutura.

## Estrutura do Projeto

- **rb.h**: Arquivo de cabeçalho contendo definições e protótipos das funções.
- **rb.c**: Implementação das funções para manipulação da árvore.
- **main.c**: Arquivo principal para testes e execução do programa.

## Funcionalidades

### 1. Inicialização da árvore
```c
void inicializar(arvore *raiz);
```
Inicializa a árvore com a raiz nula e define um nó especial para remoção.

### 2. Inserção de elementos
```c
void adicionar(int valor, arvore *raiz);
```
Adiciona um novo elemento na árvore, garantindo o balanceamento por meio de rotações e ajustes de cor.

### 3. Ajuste da estrutura após inserção
```c
void ajustar(arvore *raiz, arvore elemento);
```
Verifica e corrige violações das regras da árvore rubro-negra após uma inserção.

### 4. Rotações para balanceamento
```c
void rotacao_simples_direita(arvore *raiz, arvore pivo);
void rotacao_simples_esquerda(arvore *raiz, arvore pivo);
```
Realiza rotações simples para restaurar o balanceamento da árvore.

### 5. Funções auxiliares
- **cor**: Retorna a cor de um nó.
- **eh_raiz**: Verifica se um nó é raiz.
- **eh_filho_esquerdo**: Verifica se um nó é filho esquerdo.
- **irmao** e **tio**: Retornam o irmão e o tio de um nó, respectivamente.
- **imprimir**: Exibe a árvore no formato aninhado.
- **altura**: Calcula a altura da árvore.

## Como Compilar e Executar

Para compilar o código, use um compilador como `gcc`:
```sh
gcc -o rb main.c rb.c
```
Para executar:
```sh
./rb
```

## Autor
Desenvolvido por Analice da Silva Nascimento.


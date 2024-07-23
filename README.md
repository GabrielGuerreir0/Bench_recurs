# Projeto de Geração e Busca de Números

## Descrição do Projeto

Este projeto em C gera um arquivo de números aleatórios e implementa três algoritmos de busca (linear, sentinela e binária) e três algoritmos de ordenação (insertion sort, bubble sort e quick sort). O objetivo é permitir a análise do desempenho de cada um desses algoritmos.

## Estrutura do Projeto

O código principal do projeto está contido em um arquivo `.c` e é composto pelas seguintes funções:

### Funções de Geração de Arquivo

- `void gerar_arquivo_numeros(char *nome_arquivo, int quantidade)`: Gera um arquivo com uma quantidade especificada de números aleatórios.

### Funções de Busca

- `double busca_linear(int numero, char *nome_arquivo)`: Implementa a busca linear.
- `double busca_sentinela(int numero, char *nome_arquivo)`: Implementa a busca linear com sentinela.
- `double busca_binaria(int numero, char *nome_arquivo)`: Implementa a busca binária.

### Funções de Ordenação

- `void insertion_sort(int *numeros, int tamanho)`: Implementa o insertion sort.
- `void bubble_sort(int *numeros, int tamanho)`: Implementa o bubble sort.
- `void quick_sort(int *numeros, int baixo, int alto)`: Implementa o quick sort.

### Função Principal

- `int main()`: Função principal que interage com o usuário, permitindo a geração de números, busca e ordenação.

## Requisitos

- Compilador C (GCC, Clang, etc.)
- Sistema operacional compatível (Windows, macOS, Linux)

## Como Compilar e Executar

1. Clone este repositório para sua máquina local:
    ```bash
    git clone https://github.com/GabrielGuerreir0/Bench_recurs.git
    ```

2. Navegue até o diretório do projeto:
    ```bash
    cd projeto-busca-ordenacao
    ```

3. Compile o programa:
    ```bash
    gcc -o programa principal.c -lm
    ```

4. Execute o programa:
    ```bash
    ./programa
    ```

## Exemplo de Uso

Ao executar o programa, você será solicitado a informar a quantidade de números a serem gerados. Após a geração do arquivo, o menu de operações permitirá realizar buscas e ordenações nos números gerados.

```bash
Quantidade de números a gerar: 1000

Menu de Operações:
1. Busca de elemento
2. Sair
Escolha a operação (1/2): 1
Digite o número a ser buscado: 500

Tempo da busca linear: 0.002000 segundos
Tempo da busca sentinela: 0.001500 segundos
Tempo da busca binária: 0.000050 segundos

Tempo do Insertion Sort: 0.001200 segundos
Tempo do Bubble Sort: 0.001800 segundos
Tempo do Quick Sort: 0.000600 segundos

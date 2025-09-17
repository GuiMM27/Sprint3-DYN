# Sprint3-DYN

# Controle de Insumos - Unidade de Diagnóstico

### Visão Geral

Este projeto simula o gerenciamento de consumo de insumos (reagentes, descartáveis, etc.) em uma unidade de diagnóstico, utilizando estruturas de dados e algoritmos clássicos para organizar e analisar os registros de forma eficiente. O objetivo é demonstrar como o uso de **filas**, **pilhas**, **busca** e **ordenação** pode otimizar o controle de estoque e a tomada de decisões.

### Estruturas de Dados e Algoritmos Utilizados

O código implementa diversas soluções para lidar com os dados de consumo diário:

#### Fila e Pilha
* **Fila (`collections.deque`)**: Utilizada para registrar o consumo de insumos em ordem cronológica (FIFO - First-In, First-Out). Cada novo consumo é adicionado ao final da fila, mantendo um histórico preciso e na ordem em que os eventos ocorreram.
* **Pilha (`list`)**: É usada para simular consultas em ordem inversa (LIFO - Last-In, First-Out). Isso é útil para verificar rapidamente os últimos insumos consumidos, permitindo uma análise imediata dos itens mais recentes do estoque.

#### Estruturas de Busca
* **Busca Sequencial**: Um algoritmo de busca linear que percorre a lista de insumos item por item. Embora menos eficiente para grandes volumes de dados, é útil para listas pequenas ou não ordenadas, como a busca por um item específico.
* **Busca Binária**: Um algoritmo de busca muito mais rápido, mas que exige que a lista esteja **ordenada**. Ele divide o conjunto de dados repetidamente ao meio até encontrar o insumo desejado. É ideal para localizar rapidamente um item em um registro extenso de insumos.

#### Algoritmos de Ordenação
* **Merge Sort**: Este algoritmo de ordenação divide a lista em sub-listas, as ordena individualmente e depois as mescla. É um método estável e eficiente, utilizado aqui para **ordenar os insumos pela quantidade consumida**.
* **Quick Sort**: Geralmente mais rápido na prática, ele seleciona um "pivô" e particiona a lista, ordenando-a recursivamente. É aplicado para **ordenar os insumos pela data de validade**, permitindo identificar rapidamente quais itens estão próximos de vencer.

### Como Rodar o Código

1.  Clone este repositório para sua máquina local:
    `git clone <URL do seu repositório>`
2.  Navegue até o diretório do projeto.
3.  Execute o script Python:
    `python seu_arquivo.py`

O console exibirá os resultados de cada simulação (fila, pilha, busca e ordenação), demonstrando a aplicação prática de cada estrutura e algoritmo.

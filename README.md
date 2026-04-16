# RecipeList Manager-C

Este projeto é uma aplicação de linha de comando desenvolvida em **C** para gerenciar um livro de receitas digital. A aplicação utiliza estruturas de dados dinâmicas para permitir o armazenamento eficiente de receitas e seus respectivos ingredientes.

Funcionalidades

O sistema oferece um menu interativo com as seguintes operações:
- Gerenciamento de Receitas: Inserir, remover e visualizar receitas.
- Gerenciamento de Ingredientes: Adicionar ingredientes a receitas específicas, remover ou substituir itens.
- Busca Avançada: Localizar quais receitas utilizam um determinado ingrediente.
- Personalização: Marcar ingredientes como "Essenciais" e receitas como "Favoritas".
- Relatórios: Exibição filtrada de itens favoritos e essenciais.

Estrutura de Dados

O projeto demonstra o uso de listas encadeadas dinâmicas:
1.  Lista de Receitas: Uma lista encadeada simples onde cada nó representa uma receita.
2.  Lista de Ingredientes: Cada nó de receita contém uma **Lista Duplamente Encadeada** de ingredientes, permitindo navegação bidirecional e manipulação flexível.


Organização do Projeto

* `main.c`: Ponto de entrada do programa e interface de menu.
* `receitas.h / receitas.c`: Lógica de manipulação das receitas.
* `ingredientes.h / ingredientes.c`: Lógica de manipulação dos ingredientes.
* `dados.h`: Definições globais e forward declarations para evitar dependências circulares.

🛠️ Como Executar

Para compilar e rodar o projeto, você precisará de um compilador C (como o GCC).

1. Clone o repositório:
   git clone https://github.com/Coelho09/RecipeList-Manager-C.git

2. Compile os arquivos:
gcc -o programa main.c receitas.c ingredientes.c

3.Execute:
./programa

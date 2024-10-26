# Projeto Calculadora

Este projeto é uma calculadora simples construída com Vue.js. Ela permite que os usuários realizem operações aritméticas básicas, como adição, subtração, multiplicação e divisão. A interface consiste em campos de entrada onde os usuários podem inserir dois números, escolher um operador e ver o resultado do cálculo.

## Índice

- [Recursos](#recursos)
- [Tecnologias](#tecnologias)
- [Configuração do Projeto](#configuração-do-projeto)
- [Uso](#uso)
- [Licença](#licença)

## Recursos

- Adição, subtração, multiplicação e divisão.
- Exibição do resultado em tempo real com base na operação selecionada.
- Design responsivo.
- Interface amigável.

## Tecnologias

- **Vue.js 3** - Framework JavaScript para construção do front-end.
- **Vite** - Uma ferramenta de construção rápida para Vue.js.
- **HTML5 & CSS3** - Estrutura e estilos.
- **JavaScript** - Lógica principal da calculadora.
- **PostCSS** - Processamento de CSS (opcional, se você tiver base.css ou outras necessidades de pré-processamento de CSS).

## Configuração do Projeto

Para configurar o projeto localmente, siga estes passos:

1. Clone o repositório:

    ```bash
    git clone https://github.com/seu-usuario/calc-project.git
    ```

2. Navegue até o diretório do projeto:

    ```bash
    cd calc-project
    ```

3. Instale as dependências:

    ```bash
    npm install
    ```

4. Execute o projeto:

    ```bash
    npm run dev
    ```

A aplicação será servida em `http://localhost:3000` (ou na porta que o Vite atribuir).

## Uso

1. Insira valores nos dois campos de entrada para os números A e B.
2. Selecione um operador aritmético no dropdown.
3. O resultado será calculado e exibido automaticamente.
4. Se a divisão for selecionada, ela lidará com a divisão por zero retornando uma mensagem de erro (Erro).

**Exemplo:**

- **Entrada:**
  - `numbA = 10`, `numbB = 5`, `Operador = "+"`
  
- **Saída:**
  - O resultado mostrará 15.

## Licença

Este projeto está licenciado sob a Licença MIT. Você está livre para usar, modificar e distribuir o código.

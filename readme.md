# Black Hole Criativo

Um projeto web inovador que exibe uma animação interativa e visualmente impressionante de um “buraco negro” utilizando Web Components, canvas 2D e técnicas avançadas de animação com easing.

---

## Sumário

- [Descrição](#descrição)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Como Usar](#como-usar)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Como Funciona](#como-funciona)
- [Como Ativar e Rodar o Projeto](#como-ativar-e-rodar-o-projeto)
- [Contribuições](#contribuições)
- [Licença](#licença)

---

## Descrição

Este projeto cria um componente customizado `<a-hole>` que representa um buraco negro animado, combinando vários elementos gráficos:

- Discos elípticos que se contraem;
- Linhas radiais animadas;
- Partículas com movimento fluido;
- Sobreposição de efeitos visuais com gradientes e blur.

A animação é gerada dinamicamente usando a API Canvas 2D, combinada com easing para suavizar os movimentos.

---

## Tecnologias Utilizadas

- HTML5 com Web Components (Custom Elements)
- JavaScript moderno (ES6 modules)
- Canvas API 2D para desenho gráfico
- CSS3 avançado com gradientes, animações e mix-blend-mode
- Biblioteca externa para easing: [easing-utils](https://esm.sh/easing-utils)
- Servidor HTTP local para evitar problemas CORS

---

## Como Usar

### Pré-requisitos

- Ter [Node.js](https://nodejs.org/) instalado (para rodar servidor local)
- Navegador moderno com suporte a ES Modules e Canvas 2D (Chrome, Firefox, Edge atualizados)

### Passo a passo

1. Clone ou baixe o projeto na sua máquina:

    ```bash
    git clone https://github.com/seuusuario/black-hole-criativo.git
    cd black-hole-criativo
    ```

2. Instale o http-server globalmente (caso ainda não tenha):

    ```bash
    npm install -g http-server
    ```

3. Inicie o servidor local na pasta do projeto:

    ```bash
    http-server
    ```

4. Acesse o endereço no navegador (exemplo padrão):

    ```
    http://localhost:8080
    ```

5. Veja a animação do buraco negro preenchendo a tela.

---

## Estrutura do Projeto


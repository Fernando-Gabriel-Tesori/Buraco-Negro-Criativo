# Black Hole Criativo

Um projeto web inovador que exibe uma animação interativa e visualmente impressionante de um “buraco negro” utilizando Web Components, canvas 2D e técnicas avançadas de animação com easing.

---

## Sumário

- [Descrição](#descrição)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Como Usar](#como-usar)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Como Funciona](#como-funciona)
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
Instale o http-server globalmente (caso ainda não tenha):

bash
Copiar código
npm install -g http-server
Inicie o servidor local na pasta do projeto:

bash
Copiar código
http-server
Acesse o endereço no navegador (exemplo):

arduino
Copiar código
http://localhost:8080
Veja a animação do buraco negro preenchendo a tela.

Estrutura do Projeto
graphql
Copiar código
/black-hole-criativo
│
├── index.html          # Arquivo principal HTML que usa o componente <a-hole>
├── main.js             # Código JavaScript do Web Component, animador do canvas
├── style.css           # Estilos CSS para o componente e body
└── README.md           # Este arquivo de documentação
Como Funciona
Web Component <a-hole>
O componente define o canvas e elementos visuais.

Usa o método connectedCallback para inicializar a cena, capturando o contexto 2D do canvas.

Cria discos, linhas e partículas, posicionados e animados com base no tamanho da viewport.

Usa requestAnimationFrame para atualização contínua do quadro.

Aplica easing via easing-utils para transições suaves, principalmente no movimento dos discos.

Canvas e Animação
Discos: elipses com tamanho e posição animados para simular a curvatura do buraco negro.

Linhas: segmentos radiais que se animam e são recortados para criar profundidade.

Partículas: pequenos quadrados com movimento ascendente e dispersão, criando o efeito de “energia” fluindo.

Estilo CSS: efeitos visuais com gradientes, blur e blend modes, para dar sensação de aura e brilho.

Importante
O projeto precisa rodar em ambiente HTTP para que a importação via módulo (import easingUtils from "https://esm.sh/easing-utils") funcione sem bloqueios CORS.

O uso de OffscreenCanvas otimiza o desenho das linhas para performance em navegadores compatíveis.

Contribuições
Contribuições são bem-vindas! Para melhorar este projeto:

Abra uma issue para reportar bugs ou sugerir melhorias.

Faça um fork e envie pull requests com novas funcionalidades ou correções.

Sugestões para suporte a navegadores ou novas animações serão valorizadas.

Licença
Este projeto é licenciado sob a MIT License.

Como Ativar e Rodar o Projeto Black Hole Criativo
Passo 1 — Preparação do ambiente
Requisitos mínimos
Node.js instalado (versão recomendada 14+)

Navegador moderno com suporte a ES Modules e Canvas 2D (Chrome, Firefox, Edge atualizados)

Se ainda não tem o Node.js, instale-o em:
https://nodejs.org/

Passo 2 — Obter o código
Clone o repositório do projeto para sua máquina local ou baixe o ZIP:

bash
Copiar código
git clone https://github.com/seuusuario/black-hole-criativo.git
cd black-hole-criativo
Se você baixou o ZIP, extraia e abra o terminal na pasta extraída.

Passo 3 — Instalar um servidor HTTP local
Por motivos técnicos, o projeto precisa ser servido via HTTP para que o navegador permita a execução do código de módulos JS e evite erros CORS.

Se você já tem um servidor HTTP, pode usar ele. Caso contrário, recomendo usar o http-server, que é simples, leve e rápido.

Instalando http-server globalmente:
bash
Copiar código
npm install -g http-server
Passo 4 — Rodar o servidor local
Na pasta raiz do projeto, execute:

bash
Copiar código
http-server
Por padrão, o servidor rodará no endereço:

arduino
Copiar código
http://localhost:8080
Caso esse endereço ou porta estejam ocupados, o http-server avisará e você poderá usar a porta alternativa que ele sugerir.

Passo 5 — Acessar o projeto no navegador
Abra o navegador e digite:

arduino
Copiar código
http://localhost:8080
Se tudo estiver correto, a página abrirá e a animação do buraco negro começará automaticamente na tela.

Passo 6 — Explorar e testar
Verifique o console do navegador (F12 > Console) para garantir que não há erros de carregamento.

Se a animação não aparecer, recarregue a página e certifique-se que o servidor está ativo.

Ajuste o tamanho da janela para ver a responsividade do componente <a-hole>.

Resumo rápido do comando para rodar
bash
Copiar código
git clone https://github.com/seuusuario/black-hole-criativo.git
cd black-hole-criativo
npm install -g http-server  # se ainda não instalou
http-server
Dicas avançadas
Se quiser mudar a porta do http-server, use:

bash
Copiar código
http-server -p 3000
para rodar em http://localhost:3000.

Você pode usar outros servidores locais, como Live Server do VSCode, ou serve (npm package), contanto que sirvam os arquivos via HTTP.

Evite abrir diretamente o arquivo index.html no navegador via file://, pois módulos JS podem não funcionar corretamente devido a restrições CORS.

Desenvolvido por Fernando
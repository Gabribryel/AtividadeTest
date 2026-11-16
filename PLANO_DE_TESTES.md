Plano de Testes da Loja Super Tech

1. Equipe e Responsabilidades

Líder de Qualidade (QA Lead): Roger Matos Do Nascimento
Testador UI/UX & Usabilidade: Gabriel Yury Bezerra Monteiro
Testador de Performance & Técnico: Gabriel Yury Bezerra Monteiro



2. Escopo dos Testes

O que será testado:

Páginas: Página inicial (`index.html`) e Visual CSS (`style.css`).
Recursos e Componentes: Navegação (menus e links internos/externos), formulários de entrada, botões de ação (CTAs), responsividade de imagens e textos, semântica HTML e contrastes de cores.

O que NÃO será testado:

Integrações com back-end real ou bancos de dados (escopo puramente front-end/estático via GitHub Pages).
Testes de carga/estresse em servidor ou testes de segurança/penetração.



3. Critérios de Aceitação (Passou / Falhou)

Para que a aplicação seja considerada aprovada, deve atender aos seguintes requisitos mínimos:

Funcionalidade: 100% dos links e botões devem funcionar sem erros `404` ou travamentos no console.
Design / Responsividade: Nenhum elemento deve quebrar, sobrepor outro ou gerar barra de rolagem horizontal indesejada em resoluções mobile (`360x800` e `390x844`) e desktop (`1366x768` e `1920x1080`).
Acessibilidade: Ausência de erros críticos apontados pela extensão WAVE (ex: imagens sem atributo `alt`, contraste insuficiente abaixo de 4.5:1).
Performance Pontuação igual ou superior a 80 nas métricas de Performance, Acessibilidade, Boas Práticas e SEO no Google Lighthouse.



4. Ambiente de Testes

URL de Homologação: `https://gabribryel.github.io/AtividadeTest/`

Navegadores: Google Chrome (v. [159.0]) e Mozilla Firefox (v. [160.0]).

Resoluções / Dispositivos (via DevTools Device Mode):

Desktop: `1920x1080` (Full HD) e `1366x768` (Notebook).
Mobile: `390x844` (iPhone 12/13/14) e `360x800` (Android padrão).



5. Tipos de Testes e Ferramentas

1: Testes de Usabilidade e Acessibilidade: Inspeção manual de navegação por teclado (`Tab`), verificação de hierarquia de títulos (`<h1>` a `<h6>`), contraste de cores e análise automatizada via WAVE Evaluation Tool.
2: Testes de Design (UI): Validação visual de alinhamento, fontes, espaçamentos e quebra de layout utilizando o **Chrome DevTools (Device Mode).
3: Testes de Performance e Técnicos: Auditoria de tempo de carregamento (FCP, LCP, CLS), peso de imagens e validação de erros no Console/DOM utilizando o Google Lighthouse.

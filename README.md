# 🎲 Projeto WebDesign — Plataforma de RPG

O **Projeto WebDesign — Plataforma de RPG** é um assistente digital completo para modernizar e agilizar partidas de RPG de mesa, substituindo componentes analógicos por um ecossistema digital automatizado e de uso intuitivo.

---

## 🔗 Link do Projeto no Ar (Deploy)

O site está publicado e pode ser acessado em tempo real pelo link abaixo:
🚀 **Acesse a aplicação:** [https://javascriptwebdesign.vercel.app/](https://javascriptwebdesign.vercel.app/)

---

> ⚠️ **AVISO DE DESENVOLVIMENTO:** Este projeto encontra-se em fase de desenvolvimento ativo e validação acadêmica, estando sujeito a melhorias contínuas. **Esta ainda não é a versão final da aplicação.**

---

## 📂 Organização das Pastas do Repositório

O projeto adota uma arquitetura modular para separar as responsabilidades e manter o código limpo:

```text
├── Img_folder/          # Ativos visuais, ilustrações medievais e imagens de suporte
├── documentos/          # Documentos e relatórios de suporte acadêmico do projeto
├── pages/               # Telas e módulos secundários estruturados em HTML5
├── scripts/             # Camada de lógica computacional desenvolvida em JavaScript
├── stylesheets/         # Folhas de estilo responsáveis pelo design em CSS3
├── index.html           # Portal de entrada e página inicial do sistema
└── README.md            # Documentação técnica e guia do repositório
```

---

## 🏗️ Estrutura de Telas e Marcação (HTML5)

O esqueleto estrutural do site foi planejado de forma semântica utilizando tags da especificação HTML5. As páginas que compõem o sistema são:

*   **`index.html`:** O portal de entrada do sistema. Apresenta o projeto, os desenvolvedores e serve como o hub inicial de navegação.
*   **`pages/dados.html`:** Interface que abriga o simulador de dados virtuais, contendo menus de seleção e campos numéricos para as jogadas.
*   **`pages/criarFichas.html`:** Módulo complexo de formulário com campos de texto e numéricos estruturados para a criação completa de novos heróis.
*   **`pages/minhasFichas.html`:** Painel privado (*dashboard*) preparado com contêineres para listar os personagens que o usuário salvou na memória.
*   **`pages/bibliotecaFichas.html`:** Aba pública que organiza e exibe modelos prontos de personagens criados pela comunidade para servir de inspiração.
*   **`pages/components.html`:** Arquivo de suporte global utilizado para isolar e padronizar elementos que se repetem no site, como menus e rodapés.

---

## 🎨 Identidade Visual e Temas (CSS3)

A estilização foi isolada de forma modular para dar personalidade ao sistema e garantir que o visual se adaptasse a qualquer tela através de regras de responsividade (*Media Queries*). Os arquivos utilizados são:

*   **`stylesheets/dados.css`:** Desenha o painel em modo escuro (*dashboard*), usando tons escuros para dar foco nas rolagens e destacar o somatório dos dados.
*   **`stylesheets/criarFichas.css`:** Aplica um tema claro e limpo que imita esteticamente a textura e a organização de uma ficha clássica de papel.
*   **`stylesheets/minhasFichas.css`:** Organiza a exibição dos personagens salvos em uma grade automática e fluida usando propriedades de CSS Grid.
*   **`stylesheets/bibliotecaFichas.css`:** Gerencia o alinhamento visual e os espaçamentos dos blocos de exibição da galeria comunitária.
*   **`stylesheets/components.css`:** A espinha dorsal da consistência visual, padronizando os estilos da barra de navegação (`<nav>`) e do rodapé (`<footer>`).

---

## 🧠 Lógica e Comportamento Dinâmico (JavaScript)

A camada de inteligência da aplicação manipula o Modelo de Objeto do Documento (DOM) de forma não obstrutiva através de scripts externos. O sistema conta com as seguintes funções lógicas distribuídas nos arquivos:

*   **`scripts/dados.js`**
    1. *Funcionalidade 1 — Captura e Validação:* Monitora o clique de rolagem, extrai as faces do dado e valida se a quantidade de dados é positiva.
    2. *Funcionalidade 2 — Algoritmo Rolador:* Sorteia valores pseudo-aleatórios utilizando a lógica matemática do método `Math.random()`.
    3. *Funcionalidade 3 — Exibição de Resultados:* Soma todas as rolagens individuais e injeta o resultado final formatado na tela via `.innerHTML`.
*   **`scripts/criarFichas.js`**
    4. *Funcionalidade 4 — Manipulação de Formulários:* Intercepta o envio do cadastro através de `preventDefault()`, salvando os atributos informados.
*   **`scripts/minhasFichas.js`**
    5. *Funcionalidade 5 — Renderização Dinâmica (CRUD):* Varre a lista de memória para desenhar os cartões na tela e permite apagar fichas do painel.
*   **`scripts/loader.js`**
    6. *Funcionalidade 6 — Sincronização Inicial:* Roda de forma automática com o evento `DOMContentLoaded`, limpando o ambiente e validando os scripts.

---

## 🚀 Como Executar o Projeto Localmente

1. Clone o repositório em sua máquina:
   ```bash
   git clone https://github.com
   ```
2. Abra a pasta do projeto no VS Code.
3. Certifique-se de executar o arquivo raiz `index.html` utilizando a extensão **Live Server** para habilitar a navegação correta entre as pastas.

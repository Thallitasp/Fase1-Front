# </> TSP DevWeb Studio — Arquitetura Front-End Acessível & Responsiva

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Acessibilidade WCAG](https://img.shields.io/badge/Acessibilidade-WCAG%20AA-0284c7?style=for-the-badge)

Página web estática desenvolvida como projeto de conclusão da **Fase 1 – Desenvolvimento Front-End** (Centro Universitário Celso Lisboa). O projeto consolida práticas modernas de marcação semântica em **HTML5**, estilização responsiva com **CSS3 (Flexbox & Grid)**, validação nativa de formulários e diretrizes de acessibilidade digital (**WCAG / ARIA**).

---

## 📋 Visão Geral do Projeto

O **TSP DevWeb Studio** simula o portal institucional e portfólio de um estúdio de desenvolvimento front-end, apresentando:

- 🎨 **Identidade Visual:** Cabeçalho institucional com logotipo vetorial em **SVG** (`TSP DevWeb Studio`) e barra de navegação interna;
- 🖼️ **Seção Hero:** Apresentação principal com ilustração responsiva em SVG e lista de diferenciais técnicos;
- 🧩 **Vitrine de Projetos:** Grade bidimensional responsiva acompanhada de barra lateral informativa (`<aside>`);
- 📬 **Formulário Interativo:** Seção de contato e inscrição com validação nativa em HTML5 e feedback acessível em tempo real;
- 📌 **Rodapé Institucional:** Informações de direitos autorais e vínculo acadêmico.

---

## 🚀 Tecnologias e Conceitos Aplicados

- **🧱 HTML5 Semântico:** Uso estruturado das tags `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<figure>`, `<figcaption>` e `<footer>`.
- **🎨 CSS3 Moderno:**
  - Variáveis customizadas (`:root`) para padronização de paleta de cores, sombras e bordas;
  - **CSS Flexbox** para alinhamento de cabeçalho, navegação, botões e rodapé;
  - **CSS Grid** para a composição em duas colunas (`<section>` + `<aside>`), grade de projetos e layout do formulário;
  - **Media Queries** adaptadas para Desktop (`> 1024px`), Tablet (`601px – 1024px`) e Smartphone (`≤ 600px`), além de suporte a `prefers-reduced-motion`.
- **♿ Acessibilidade Web (WCAG / ARIA):**
  - Link de salto rápido para o conteúdo principal (*Skip Link* visível ao foco);
  - Atributos `alt` descritivos nas ilustrações vetoriais;
  - Associação explícita de `<label for="...">` em todos os campos do formulário;
  - Indicadores nítidos de foco (`:focus-visible`), alto contraste cromático e regiões dinâmicas com `role="status"` e `aria-live="polite"`.
- **⚡ JavaScript (Vanilla):** Interceptação da submissão do formulário via `checkValidity()` para exibir mensagem de confirmação acessível sem recarregar a página.

---

## 📁 Estrutura de Arquivos

- 📄 `index.html` — Estrutura semântica HTML5, SVGs inline, formulário e script de validação.
- 🎨 `styles.css` — Folha de estilos CSS3 (variáveis, Flexbox, Grid, acessibilidade e media queries).
- 📘 `README.md` — Documentação completa do projeto.

---

## 📱 Breakpoints de Responsividade

| Dispositivo | Largura de Tela | Comportamento do Layout |
| :--- | :--- | :--- |
| 🖥️ **Desktop** | `> 1024px` | Seção *hero* em 2 colunas, área principal dividida entre vitrine e `<aside>`, grade de projetos em 3 colunas e formulário em 2 colunas. |
| 📱 **Tablet** | `601px – 1024px` | Seção *hero* e área principal em coluna única; grade de projetos reorganizada para 2 colunas (`repeat(2, 1fr)`). |
| 📲 **Smartphone** | `≤ 600px` | Todas as grades convertidas para 1 coluna (`1fr`), menu de navegação empilhado e botões expandidos para `width: 100%` (ergonomia de toque). |

---

## 💻 Como Executar Localmente

1. **Clone o repositório:**
   `git clone https://github.com/Thallitasp/Fase1-Front.git`
2. **Acesse a pasta do projeto:**
   `cd Fase1-Front`
3. **Execute no navegador:**
   Abra o arquivo `index.html` diretamente em qualquer navegador web atualizado (ou utilize a extensão *Live Server* no VS Code).

---

## 👩‍💻 Autoria

**Thallita da Silva Pedreira**  
🔗 Repositório: github.com/Thallitasp/Fase1-Front
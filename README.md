# Procurepédia — Wikipédia de Procurement & Supply Chain

Projeto do **Módulo 3 — Trilha HTML**: "Recriando a Wikipedia, com um layout melhor :)".

A Procurepédia é uma enciclopédia temática sobre Compras Corporativas, Gestão de Fornecedores, Supply Chain, ESG e Transformação Digital, construída com HTML semântico e CSS, com foco em estrutura, acessibilidade e responsividade.

## Estrutura do projeto

```
├── index.html               Página principal (portal estilo Wikipédia)
├── procurement.html         Fundamentos: definição, etimologia, história, objetivos, KPIs
├── strategic-sourcing.html  Kraljic, categorias, negociação, TCO, Should Cost, BATNA, leilão reverso
├── fornecedores.html        Homologação, due diligence, IDF, SRM, desenvolvimento local, diversidade
├── e-procurement.html       P2P, S2P, eSourcing, catálogos, automação, Coupa/Ariba/Oracle/Jaggaer/Ivalua
├── tecnologia-e-ia.html     IA, automação, spend analytics, dashboards, Power BI, Databricks, Copilot, agentes
├── esg.html                 Compras sustentáveis, ISO 20400, Escopo 3, diversidade, governança
├── carreira.html            Trilha, competências técnicas, soft skills, certificações
├── eventos.html             INBRASC, Live University, ABRALOG
├── referencias.html         Bibliografia em formato ABNT
├── css
│   └── style.css            Folha de estilo única
```

## Layout

- **Cabeçalho**: logotipo próprio (globo com rede de fornecedores e a letra "P"), nome, descrição e busca.
- **Três colunas**, inspiradas na Wikipédia:
  - esquerda: menu "Conteúdo" com todas as páginas, agrupadas por tema;
  - centro: o artigo, com infobox, tabelas, quadros de destaque e notas de rodapé;
  - direita: "Neste artigo", com links para cada seção da página.
- **Rodapé**: data da última edição e links de apoio.

## Técnicas utilizadas

- **HTML5 semântico**: `header`, `nav`, `main`, `article`, `section`, `aside`, `footer`, `figure`/`figcaption`, `details`/`summary`, `dl`/`dt`/`dd`, `abbr`, `dfn`, `cite`, `kbd`, `code`.
- **CSS3**: pilhas de fontes com alternativas para Windows, macOS, Android e Linux, terminando em família genérica (`sans-serif`, `monospace`); CSS Grid (layout de três colunas e cartões), Flexbox (cabeçalho e fluxos de processo), variáveis CSS, contadores CSS (etapas numeradas), `position: sticky` (menus fixos na rolagem), `aspect-ratio` (vídeo e mapa).
- **Iframes**: vídeo do YouTube (página inicial e Strategic Sourcing), painel ilustrativo com `srcdoc` (IA e Analytics) e mapa do OpenStreetMap (Eventos).
- **JavaScript mínimo**: um único trecho recolhe o menu em celulares; o site funciona normalmente sem ele.

<img width="1285" height="671" alt="image" src="https://github.com/user-attachments/assets/42a06e4b-2c93-4b3c-8bdf-69d9c00b159c" />
<img width="1280" height="669" alt="image" src="https://github.com/user-attachments/assets/758d09ee-d509-40ca-9015-5cbe8ab26cdd" />



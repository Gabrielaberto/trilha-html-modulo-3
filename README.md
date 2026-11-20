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
└── README.md
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

## Acessibilidade

- `lang="pt-BR"` em todas as páginas e `lang="en"` / `lang="la"` em termos estrangeiros, para o leitor de tela pronunciar corretamente.
- Link **"Pular para o conteúdo"** (aparece ao pressionar `Tab`) e foco visível em todos os elementos.
- Hierarquia de títulos `h1 → h2 → h3` sem saltos; cada `section` é rotulada com `aria-labelledby`.
- Página atual marcada no menu com `aria-current="page"`.
- Tabelas com `caption` e `th scope="col|row"`, dentro de contêineres roláveis acessíveis por teclado (`tabindex="0"`, `role="region"`).
- Links externos com `target="_blank"`, `rel="noopener noreferrer"` e texto oculto "(abre em nova janela)" para leitores de tela.
- SVGs com `title` e `desc`; iframes com `title` descritivo e `loading="lazy"`.
- Respeito à preferência de redução de movimento (`prefers-reduced-motion`).

### Atalhos para navegar com teclado e NVDA

| Ação | Teclado | Com o NVDA ativo |
|---|---|---|
| Pular direto para o artigo | `Tab` e `Enter` no link "Pular para o conteúdo" | `D` salta entre regiões (landmarks) |
| Ir para o próximo título | Usar o "Neste artigo" | `H` (ou `1` a `6` por nível) |
| Listar todos os links | — | `Insert` + `F7` |
| Navegar por tabelas | Rolar horizontalmente no celular | `T` e `Ctrl` + `Alt` + setas |
| Abrir em nova janela | Link "Abrir em nova janela" ou `Shift` + clique | Links externos são anunciados como "abre em nova janela" |

## Responsividade

| Largura da tela | Comportamento |
|---|---|
| Acima de 1100 px | Três colunas: menu, artigo e "Neste artigo" |
| De 761 a 1100 px | Duas colunas: menu à esquerda; "Neste artigo" acima do texto |
| Até 760 px (celular) | Uma coluna; menu recolhível; infobox ocupa a largura toda |

## Navegação

- Navegação entre páginas pelo menu lateral e por links internos nos textos.
- Navegação **dentro da página** pelo "Neste artigo", links "Voltar ao topo" e notas de rodapé `[1]` ligadas às referências.
- Navegação **em novas janelas**: link "Abrir em nova janela" em cada artigo, links "Saiba mais" externos e busca do cabeçalho, que pesquisa o termo na Wikipédia em uma nova aba.

## Como montar o repositório

1. Crie a pasta do projeto e, dentro dela, a subpasta `css`.
2. Crie cada arquivo com o nome exato da estrutura acima e cole o código correspondente.
3. Salve tudo com codificação **UTF-8** (para os acentos aparecerem corretamente).
4. No GitHub: `git add .`, `git commit -m "Procurepédia: desafio Módulo 3"` e `git push`.
5. Opcional: ative o **GitHub Pages** (Settings → Pages → branch `main`) para publicar o site.

## Como testar

- Abra `index.html` no navegador.
- Navegue apenas com `Tab`, `Shift + Tab` e `Enter`.
- Instale o [NVDA](https://www.nvaccess.org/download/) e use os atalhos da tabela acima.
- Reduza a largura da janela (ou use `F12` → modo dispositivo) para ver as versões tablet e celular.

## Referências técnicas

- W3C — [WCAG 2.1](https://www.w3.org/WAI/standards-guidelines/wcag/pt-BR/)
- MDN — [Semântica em HTML](https://developer.mozilla.org/pt-BR/docs/Glossary/Semantics)
- NV Access — [NVDA](https://www.nvaccess.org/download/)
- Governo Digital — [eMAG](https://emag.governoeletronico.gov.br/)

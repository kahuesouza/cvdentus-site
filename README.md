# CVDentus — site

Site institucional da CVDentus, hospedado via GitHub Pages.

## Páginas

| Página | Arquivo |
| --- | --- |
| Home | `index.html` → `CVDentus.dc.html` |
| Optymus | `Optymus-Landing.dc.html` |
| Clinical Plus | `Clinical-Plus-Landing.dc.html` |
| DentSurg Pro | `DentSurg-Pro-Landing.dc.html` |
| Elo | `Elo-Landing.dc.html` |
| Lupas | `Lupas-Landing.dc.html` |

## Como funciona

As páginas `.dc.html` são componentes Claude Design (template + lógica React/DCLogic)
interpretados no navegador por `support.js`. React, ReactDOM e Babel são carregados
via CDN (unpkg). `image-slot.js` cuida dos slots de imagem. Mídia em `uploads/`,
ícones e imagens compartilhadas em `assets/`.

O header (logo, navegação, dropdown Produtos, seletor PT/ES/EN, tema claro/escuro,
ícones de login e carrinho) é idêntico em todas as páginas. Tema e idioma persistem
em `localStorage` (`cvd_theme`, `cvd_lang`) e são compartilhados entre as páginas.

## Rodar localmente

```bash
python -m http.server 8000
# abrir http://localhost:8000/
```

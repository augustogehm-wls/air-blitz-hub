# Air Blitz Hub

Landing page do playable **Air Blitz** — side-scrolling air-shooter cartoon
estilo Cuphead, side-project derivado do Playable Blitz workshop.

Produzido a partir de `playables-blitz/playables/air-blitz/dist/playable.html`.

## Como atualizar o playable

1. No repo `playables-blitz`, rebuilda o air-blitz:
   ```
   cd playables/air-blitz
   npx build-playable .
   ```
2. Copia o output pra cá:
   ```
   cp <playables-blitz>/playables/air-blitz/dist/playable.html ./playable.html
   ```
3. Commit + push. GitHub Pages atualiza em ~30 segundos.

## Como adicionar mais playables nesse mesmo repo

A versão atual é single-playable. Pra virar um hub com múltiplos jogos,
copia o template do site pai
[`new-games-playable/index.html`](https://github.com/augustogehm-wls/new-games-playable/blob/main/index.html)
— ele tem o sistema de categorias + modal pronto.

## Estrutura

```
air-blitz-hub/
├── index.html      # Landing page (header + iframe do playable + meta + footer)
├── playable.html   # Build inlined do air-blitz (PixiJS v8, ~530 KB)
└── README.md
```

## Hosting

GitHub Pages servindo `main` / root. URL ao vivo:
`https://augustogehm-wls.github.io/air-blitz-hub/`

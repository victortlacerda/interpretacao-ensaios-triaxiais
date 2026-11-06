# Changelog

Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/).

## [Não lançado]

### Adicionado
- Ícone próprio da aba e do histórico do navegador (SVG embutido no `index.html`).
- Capturas de tela do app em `docs/img/` e README com apresentação visual.

## [1.0.0] - 2026-11-03

### Adicionado
- Trajetória de tensões (p, q) de Lambe para CIU, CID e UU, com TTT e TTE.
- Entrada por σ₁/σ₃ ou por p/q, com colagem do Excel e vários corpos de prova.
- Linha K<sub>f</sub> por regressão, círculos de Mohr e envoltória de Mohr-Coulomb.
- Linha de estado crítico.
- Análise de Olson & Mattson (2008).
- Exemplos prontos de compressão e extensão, axial e lateral, e CIU.
- Zoom com roda do mouse, arrastar para mover, e exportação em PNG e SVG.
- Aba com a curva ε × q (e ε × u no CIU).
- Botão para plotar todos os exemplos juntos.

### Alterado
- Paleta de cores revisada para distinguir compressão axial e extensão lateral.
- Rótulos das linhas K<sub>f</sub> e LEC posicionados junto aos dados, visíveis sem zoom.

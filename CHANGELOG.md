# Changelog

Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/).

## [Não lançado]

### Adicionado
- Convenção de Cambridge (Roscoe) para a trajetória de tensões: p = (σ₁ + 2σ₃)/3, q = σ₁ − σ₃.
- Envoltória q = q₀ + M·p′ com φ′ e c′ calculados de M, e M de compressão e de extensão nos cartões.
- Linha de estado crítico com ramos de compressão (M<sub>c</sub>) e extensão (M<sub>e</sub>).
- Conversão automática da tabela ao trocar a convenção ou a forma de entrada (σ₁/σ₃ ↔ p/q).
- Capturas de tela da convenção de Cambridge no README.
- Ícone próprio da aba e do histórico do navegador (SVG embutido no `index.html`).
- Capturas de tela do app em `docs/img/` e README com apresentação visual.

### Corrigido
- Linha K<sub>f</sub> desenhada do lado errado (q positivo) nos ensaios de extensão.
- φ<sub>cs</sub> automático passa a vir do φ′ ajustado, sem depender da convenção.
- Rótulos das linhas mudam de lado quando ficariam cortados na borda do gráfico.

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

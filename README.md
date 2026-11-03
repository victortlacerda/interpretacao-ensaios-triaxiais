# Interpretação de ensaios triaxiais

Aplicativo web (um único `index.html`, sem instalação nem dependências) para plotar **trajetórias de tensões** e interpretar resultados de ensaios triaxiais.

## Funcionalidades

- **Tipos de ensaio:** CIU, CID e UU. No CIU há coluna de poropressão (u) e é possível ver tensões totais (TTT), efetivas (TTE) ou ambas.
- **Entrada de dados:** informe σ₁ e σ₃ (o programa calcula p e q) ou informe p e q diretamente. Aceita vírgula decimal e colagem direta do Excel.
- **Vários corpos de prova**, cada um com uma cor.
- **Trajetória (p, q) de Lambe**, com a ruptura marcada no ponto de q máximo.
- **Linha K<sub>f</sub>**, ajustada por regressão linear entre os pontos de ruptura, com α, a, φ e c.
- **Círculos de Mohr** na ruptura e **envoltória de Mohr-Coulomb**.
- **Linha de estado crítico** (φ<sub>cs</sub> informado ou estimado do φ′ ajustado).
- **Curva ε × q** (e ε × u nos ensaios CIU).
- **Análise de Olson & Mattson (2008)** da resistência não drenada normalizada.
- **Exemplos prontos:** CIU, compressão axial, extensão axial, compressão lateral e extensão lateral, além do botão que plota todos juntos para comparação.
- **Zoom** com a roda do mouse, arrastar para mover e **exportação** em PNG e SVG.

## Fórmulas

Para σ₂ = σ₃ (coordenadas de Lambe):

```
p  = (σ₁ + σ₃) / 2        p′ = p − u
q  = (σ₁ − σ₃) / 2        q′ = q
```

Linha K<sub>f</sub> no plano p–q: `q = a + p·tan α`, com

```
sen φ = tan α        c = a / cos φ
```

Resistência não drenada normalizada (Olson & Mattson, 2008):

```
Su / σ′₃c = (σ₁ − σ₃) / (2σ₃)
```

onde S<sub>u</sub> = q (valor máximo ou final) e σ′<sub>3c</sub> é a tensão confinante efetiva de adensamento, tomada na primeira linha de cada ensaio.

## Como usar

Abra o `index.html` em qualquer navegador moderno. Para publicar online, ative o GitHub Pages em **Settings → Pages → Deploy from a branch → `main` / root**.

## Observações

- Unidades em kPa.
- Os exemplos prontos são dados sintéticos (φ′ = 32°), apenas para demonstração.
- A ruptura é tomada como o ponto de q máximo de cada ensaio.
- Ferramenta de apoio ao estudo; não substitui a análise de um engenheiro geotécnico.

## Licença

[MIT](LICENSE)

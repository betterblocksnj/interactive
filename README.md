# Better Blocks NJ — Interactive Widgets

Interactive data visualizations and calculators for embedding in [betterblocksnj.org](https://betterblocksnj.org) articles via iframe.

## Widgets

| File | Description | Article |
|------|-------------|---------|
| `five-year-exemption.html` | Stacked bar chart showing how five-year tax exemptions phase in property taxes | Three Myths about PILOTs |
| `pilot-vs-conventional-flow.html` | SVG diagram comparing where tax dollars flow under conventional tax vs. PILOT | Three Myths about PILOTs |
| `pilot-three-scenario.html` | Interactive calculator: empty lot vs. PILOT vs. full conventional tax | Three Myths about PILOTs |
| `permits-vs-pilots.html` | Bar chart of residential permits vs. PILOT agreements (2013–2025) | Three Myths about PILOTs |
| `affordable-setaside-calculator.html` | Calculator: school children and PILOT costs at different affordable set-asides | Three Myths about PILOTs |

## Embedding in WordPress

Since WordPress.com Business blocks inline JavaScript, embed these via iframe using a Custom HTML block:

```html
<iframe src="https://betterblocksnj.github.io/interactive/pilot-three-scenario.html"
        width="100%"
        height="900"
        style="border: none;"
        loading="lazy">
</iframe>
```

### Recommended iframe heights

| Widget | Recommended height |
|--------|-------------------|
| `five-year-exemption.html` | 550px |
| `pilot-vs-conventional-flow.html` | 560px |
| `pilot-three-scenario.html` | 1100px |
| `permits-vs-pilots.html` | 650px |
| `affordable-setaside-calculator.html` | 1200px |

## Setup

1. Enable GitHub Pages on this repo (Settings → Pages → Source: main branch)
2. Widgets will be available at `https://betterblocksnj.github.io/interactive/{filename}`
3. No build step required — all files are standalone HTML with Chart.js loaded from CDN

## Dependencies

- [Chart.js 4.4.1](https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.js) (loaded from CDN, no local install needed)

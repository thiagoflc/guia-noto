# Noto · Guia Interativo

Guia turístico interativo *single-page* (SPA) para uma manhã pela cidade barroca de **Noto** (Val di Noto, Sicília), com estética *quiet luxury*.

**6 paragens** em 3 atos (08h30 → 13h30), subindo o Corso Vittorio Emanuele — de Porta Reale a Santa Chiara.

## Funcionalidades

- **Mapa interativo** claro em tom amarelo-cobre (Leaflet + CartoDB Positron com filtro sépia/âmbar), sempre visível, com `flyTo` dinâmico.
- **Timeline rolável** sincronizada com o mapa (scroll-spy bidirecional).
- Pontos de **foco** com cards expansíveis e **modal glassmorphism** acessível (descrição, história, horário ideal, custo, insights), com **link de rota para o Google Maps** em cada ponto.
- **Mobile-first**, otimizado para iPhone Pro Max: app-shell, `dvh`, *safe areas*, *swipe-para-fechar*, alvos de toque ≥44px, web-app instalável.
- **Acessibilidade**: cards operáveis por teclado, modal `role="dialog"` com *focus trap*, contraste WCAG AA, `prefers-reduced-motion`.
- **Imagens reais** de licença livre (Wikimedia Commons), com atribuição no rodapé.

## Stack

HTML5 · Tailwind CSS (pré-compilado e embutido) · Alpine.js (+ plugin focus) · Leaflet — tudo em um único arquivo (`index.html`), sem build em runtime.

## Rodar localmente

Basta abrir `index.html` no navegador, ou servir a pasta:

```bash
npx serve .
```

## Créditos das imagens

Todas as fotografias são reais e de licença livre via **Wikimedia Commons** — autoria e licença listadas na seção "Créditos das imagens" do próprio guia.

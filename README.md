# Maya Protege — Design System

Sistema de design da marca **Maya Protege**, um plano funerário criado para oferecer tranquilidade, cuidado e proteção às famílias.

---

## Estrutura

```
maya-protege-design-system/
├── index.css                  ← Entrada principal (importa tudo)
├── assets/
│   └── logos/                 ← Logos da marca (SVG) + guia de uso
├── tokens/
│   ├── colors.css             ← Paleta de cores e roles semânticos
│   ├── typography.css         ← Famílias, escala tipográfica, utilitários
│   └── spacing.css            ← Espaçamento, raios, sombras, transições
├── components/
│   ├── buttons.css            ← Botões (primary, secondary, accent, ghost)
│   ├── cards.css              ← Cards (default, dark, tinted)
│   ├── badges.css             ← Badges / tags
│   ├── forms.css              ← Inputs, selects, textareas
│   └── layout.css             ← Container, grid, utilitários
└── docs/
    └── index.html             ← Documentação visual interativa
```

---

## Como usar

### 1. Importar o CSS completo
```html
<link rel="stylesheet" href="path/to/maya-protege-design-system/index.css">
```

### 2. Fontes (Google Fonts)
```html
<link href="https://fonts.googleapis.com/css2?family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
```

### 3. Usar tokens via CSS variables
```css
.meu-componente {
  background: var(--color-timber-green-950);
  color: var(--color-text-on-dark);
  font-family: var(--font-display);
  padding: var(--space-6) var(--space-8);
  border-radius: var(--radius-lg);
}
```

---

## Paleta de Cores

| Token | Hex | Uso |
|-------|-----|-----|
| `--color-timber-green-950` | `#0C332A` | Background escuro, cor principal |
| `--color-sea-green-700` | `#0D9448` | Brand primary, CTAs |
| `--color-sea-green-500` | `#14D366` | Acentos vibrantes, highlights |
| `--color-dull-lavender` | `#A29DFF` | Acento complementar, links |
| `--color-timber-green-50` | `#EFFAF5` | Background claro, tints |

---

## Tipografia

| Fonte | Uso |
|-------|-----|
| **Libre Baskerville** | Títulos, headings — presença institucional |
| **Inter** | Corpo de texto, labels, UI — clareza e funcionalidade |

### Escala
- `--text-xs` → 12px
- `--text-sm` → 14px
- `--text-base` → 16px
- `--text-md` → 18px
- `--text-xl` → 24px
- `--text-2xl` → 32px
- `--text-4xl` → 56px

---

## Componentes

### Botões
```html
<button class="btn btn--primary btn--md">Contratar Plano</button>
<button class="btn btn--secondary btn--md">Saiba Mais</button>
<button class="btn btn--accent btn--md">Solicitar Contato</button>
<button class="btn btn--ghost btn--md">Cancelar</button>
```

**Modificadores de tamanho:** `btn--sm`, `btn--md`, `btn--lg`

---

### Cards
```html
<div class="card">
  <div class="card__header">
    <h3 class="card__title">Título</h3>
  </div>
  <div class="card__body">Descrição...</div>
  <div class="card__footer">
    <button class="btn btn--primary btn--sm">Ação</button>
  </div>
</div>
```

**Variantes:** `card--dark`, `card--tinted`, `card--flat`

---

### Badges
```html
<span class="badge badge--primary">Proteção</span>
<span class="badge badge--green">Disponível</span>
<span class="badge badge--accent">Destaque</span>
<span class="badge badge--dark">Premium</span>
```

---

### Formulários
```html
<div class="form-group">
  <label class="form-label form-label--required">Nome</label>
  <input type="text" class="form-input" placeholder="Seu nome">
  <span class="form-hint">Dica opcional</span>
</div>
```

---

## Valores da Marca

> **Planejamento · Proteção · Respeito**

O sistema de design reflete esses pilares em cada decisão: tons de verde profundos transmitem estabilidade e cuidado; tipografia institucional equilibrada com corpo acessível; espaços generosos que respiram tranquilidade.

---

## Logos

As logos da marca estão em [`assets/logos/`](assets/logos/) em formato SVG, com variantes
horizontal, empilhada e símbolo isolado — em versões clara e escura. Veja o
[guia de uso](assets/logos/README.md) para escolher a variante correta.

```html
<img src="assets/logos/maya-protege-horizontal-dark.svg" alt="Maya Protege" height="40">
```

---

## Documentação Visual

Abra `docs/index.html` no navegador para visualizar todos os tokens e componentes interativos.

---

*Design by [YagoBispo](https://yagobispo.com) · Brand Identity for Maya Protege*

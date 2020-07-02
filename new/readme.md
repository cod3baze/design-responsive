# Responsividade

## CSS Units

Unidade de medidas do CSS

Layout

- [x] Fixo
      `px` - Pixels
- [x] Fluido
      `%` - Porcentagem
      `auto` - Automática
      `vh` - Viewport Height
      `vw` - Viewport width

Textos

- [x] Fixos
      `1px` = 0.75pt
      `16px` = 12pt
- [x] Fluidos
      `em` - Multiplicado pelo pai
      `rem` - Multiplicado pelo root

---

## CSS Media Queries

```css
  @media (max-width: 630px) {
  .hero .container {
    flex-direction: column;
    text-align: center;
  }
```

## HTML Media Atrib

```html
<link
  rel="stylesheet"
  href="./css/responsive.css"
  media="screen and (max-width: 768px)"
/>
<link rel="stylesheet" href="./css/print.css" media="print" />
```

## Images

`<picture>`

JPG, PNG vs SVG

---

- GRID Strategy

  - [x] auto-fit: vai prencher o números de colunas automaticamente
  - [x] minmax(x, y): `x`: o mínimo da coluna, `y`: o maximo da coluna

```css
grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
```

# 🎨 Portfolio Personal

Aquest portfolio està dissenyat amb aproximació **mobile-first**, seguint les millors pràctiques del desenvolupament web modern.
El disseny garanteix una experiència òptima en **mòbils, tauletes i escriptoris**.

🎓 **Projecte desenvolupat com a pràctica del curs de Desenvolupament Front-End a CIFO La Violeta**

---

## 📱 Dispositius i Breakpoints

| Dispositiu | Width          | Descripció         |
| ---------- | -------------- | ------------------- |
| Mòbil     | 320px - 767px  | Prioritat principal |
| Tauleta    | 768px - 1023px | Vista intermèdia   |
| Escriptori | 1024px+        | Vista completa      |

---

## 🏠 Estructura de Pàgines del Portfolio

El portfolio és una **Single Page Application (SPA)** amb navegació **smooth scroll**.

### Hero / Benvinguda

- 🌅 Presentació amb **gradient tomato** de fons
- 🖋 Tipografia: **Poppins Bold**
- 🎯 Elements: Nom, rol (Estudiant Front-End), descripció breu, **botons CTA**

### Sobre Mi

- 📸 Foto personal i informació de formació
- 💻 Tecnologies: HTML, CSS, JavaScript
- 🎫 Elements: Foto, text, badges de tecnologies

### Els Meus Projectes

- 🖼 Galeria responsive amb **targetes interactives**
- 📝 Elements: Imatge, descripció, **etiquetes tomato**, enllaços a GitHub
- 📊 Grid: 1 col mòbil, 2 cols tablet, 3 cols desktop

### Habilitats

- ⚡ Visualització de tecnologies i eines per categories
- 🏷 Elements: Badges, nivell d'aprenentatge, icones

### Contacte

- ✉️ Formulari de contacte i xarxes socials
- 🔗 Elements: Formulari responsive, GitHub, LinkedIn, email

---

## 📐 Principis de Disseny Mobile-First

1. Començar pel **mòbil**
2. Contingut prioritzat
3. **Touch-friendly** (àrea mínima 44px)
4. **Imatges responsive** (`max-width: 100%`)
5. Navegació simple (hamburguesa mòbil / horitzontal desktop)
6. Performance i càrrega ràpida

---

## 🖋 Tipografia - Poppins

- **Font principal:** `'Poppins', sans-serif`
- **Pesos utilitzats:** 300, 400, 500, 600, 700, 800

### Jerarquia Tipogràfica

| Element    | Pes          | Ús                             |
| ---------- | ------------ | ------------------------------- |
| H1         | Bold 700     | Hero / Títol principal         |
| H2         | Bold 700     | Títols de secció              |
| H3         | SemiBold 600 | Subtítols / títols targetes   |
| H4         | SemiBold 600 | Títols projectes / tecnologies |
| Body Large | Regular 400  | Paràgrafs introductoris        |
| Body       | Regular 400  | Text general                    |
| Small Text | Regular 400  | Notes, metadata                 |

**✅ Per què Poppins?**

- Llegibilitat excel·lent
- Geomètrica i moderna
- Versàtil amb 6 pesos
- Perfecta amb color tomato
- Optimitzada per web i multiidioma

---

## 🎨 Gama Cromàtica - Color Tomato

- **Color protagonista:** `#FF6347`
- Paleta:

| Nom              | Hex     | Ús                         |
| ---------------- | ------- | --------------------------- |
| Tomato 50        | #fff5f3 | Fons clars, accents subtils |
| Tomato 100       | #ffebe6 | Hover targetes              |
| Tomato (Primary) | #ff6347 | Botons, enllaços           |
| Tomato 700       | #d84a2e | Hover elements actius       |
| Tomato 900       | #a33822 | Text sobre fons clar        |

**Per què Tomato?**

- 🔥 Energia i passió
- 👀 Visibilitat i contrast
- 🌟 Modern i fresc
- 📝 Memorable i destacable

---

## 📐 Layout i Componentes

### Header Fix amb Navegació

- Mòbil: Logo esquerra, menú hamburguesa dreta
- Desktop: Logo esquerra, navegació horitzontal, hover tomato

### Hero Section

- Flexbox centrat, altura 100vh
- Tipografia: Poppins Bold 48px mobile, 72px desktop
- Colors: Gradient tomato de fons, text blanc

### Seccions

- Sobre Mi: 1 col mòbil, 2 cols desktop
- Projectes: Grid responsive (1-3 cols)
- Habilitats: Flexbox wrap, badges interactius

### Breakpoints

- **sm:** 640px - 1 col projectes
- **md:** 768px - 2 col projectes
- **lg:** 1024px - 3 col projectes, max-width 1280px

### Exemple CSS Mobile-First

```css
.projects-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.5rem;
}
@media (min-width: 768px) {
  .projects-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
  }
}
@media (min-width: 1024px) {
  .projects-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}
```

<div align="center">

# 👟 Shoe Nova

### A Modern, Interactive Sneaker Shopping Experience

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Responsive](https://img.shields.io/badge/Responsive-Design-green?style=for-the-badge)](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)

<br/>

![Shoe Nova Banner](https://images.unsplash.com/photo-1604147495798-57beb5d6af73?ixlib=rb-1.2.1&auto=format&fit=crop&w=1200&q=80)

<br/>

> **Shoe Nova** is a fully responsive, front-end sneaker e-commerce website built with pure HTML, CSS, and Vanilla JavaScript — no frameworks, no libraries, just clean and powerful web fundamentals.

<br/>

[🚀 Live Demo](#) &nbsp;|&nbsp; [📸 Screenshots](#-screenshots) &nbsp;|&nbsp; [✨ Features](#-features) &nbsp;|&nbsp; [🛠️ Tech Stack](#️-tech-stack) &nbsp;|&nbsp; [📁 Project Structure](#-project-structure) &nbsp;|&nbsp; [🚀 Getting Started](#-getting-started)

</div>

---

## 📌 Overview

**Shoe Nova** is a pixel-perfect, fully functional sneaker store landing page that simulates a real shopping experience. Users can browse through multiple Nike shoe collections, switch between color variants, select sizes, and proceed through a checkout flow — all without a single page reload.

This project showcases modern front-end development skills including CSS animations, dynamic DOM manipulation, interactive UI components, and a mobile-first responsive design.

---

## ✨ Features

### 🛒 Shopping Experience
- **Interactive Product Slider** — Smooth animated slider to browse 5 shoe collections (Air Force, Air Jordan, Blazer, Crater, Hippie)
- **Dynamic Product Panel** — Selecting a shoe from the navbar instantly updates the product image, title, price, and color swatches
- **Color Variants** — Each product has 2 color options; clicking a swatch live-updates the displayed product image
- **Size Selector** — Clickable shoe sizes (42, 43, 44) with active state highlighting
- **Checkout Modal** — A sleek payment popup with personal info and card details form

### 🎨 UI & Design
- Diagonal clip-path sections for a modern, editorial aesthetic
- Full-screen hero slider with background circles per product theme
- Features strip — Free Shipping, 30 Days Return, Gift Cards, Contact Us
- Lifestyle photo gallery section
- New Season collection banner
- Fully structured footer with navigation menus, newsletter signup, and social media links

### 📱 Responsive Design
- Mobile-first media queries (`max-width: 480px`)
- Collapsible navigation, hidden search bar on mobile
- Stacked layouts for product section, new season, footer
- Adaptive payment modal width

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Semantic page structure |
| **CSS3** | Styling, animations, clip-paths, flexbox, media queries |
| **Vanilla JavaScript** | DOM manipulation, event handling, dynamic rendering |
| **Google Fonts** | Lato font family |
| **Pexels** | Lifestyle imagery (CDN) |
| **Unsplash** | Hero background imagery (CDN) |

> ⚡ Zero dependencies. No npm, no build tools, no frameworks. Just open and run.

---

## 📁 Project Structure

```
shoe-nova/
│
├── index.html          # Main HTML structure & layout
├── style.css           # All styles, animations & responsive rules
├── app.js              # JavaScript for interactivity & DOM logic
│
└── img/
    ├── air.png          # Air Force - Color 1
    ├── air2.png         # Air Force - Color 2
    ├── jordan.png       # Air Jordan - Color 1
    ├── jordan2.png      # Air Jordan - Color 2
    ├── blazer.png       # Blazer - Color 1
    ├── blazer2.png      # Blazer - Color 2
    ├── crater.png       # Crater - Color 1
    ├── crater2.png      # Crater - Color 2
    ├── hippie.png       # Hippie - Color 1
    ├── hippie2.png      # Hippie - Color 2
    ├── sneakers.png     # Logo
    ├── search.png       # Search icon
    ├── shipping.png     # Feature icon
    ├── return.png       # Feature icon
    ├── gift.png         # Feature icon
    ├── contact.png      # Feature icon
    ├── visa.png         # Payment icon
    ├── master.png       # Payment icon
    ├── facebook.png     # Social icon
    ├── twitter.png      # Social icon
    ├── instagram.png    # Social icon
    └── whatsapp.png     # Social icon
```

---

## 🚀 Getting Started

### Prerequisites
No installs needed. Just a modern web browser.

### Run Locally

```bash
# 1. Clone the repository
git clone https://github.com/your-username/shoe-nova.git

# 2. Navigate into the project
cd shoe-nova

# 3. Open in your browser
open index.html
```

Or simply **double-click** `index.html` to launch it in your default browser.

> 💡 For the best experience, use **VS Code** with the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension.

---

## 🧠 JavaScript Logic Breakdown

### Slider Navigation
```js
menuItems.forEach((item, index) => {
  item.addEventListener("click", () => {
    wrapper.style.transform = `translateX(${-100 * index}vw)`;
    // Updates product info dynamically
  });
});
```
Clicking a nav item translates the slider wrapper by `-100vw` per step, creating a smooth CSS transition effect.

### Dynamic Color Swatches
```js
currentProductColors.forEach((color, index) => {
  color.addEventListener("click", () => {
    currentProductImg.src = choosenProduct.colors[index].img;
  });
});
```
Swapping a color swatch directly maps to a different image path stored in the product data array.

### Checkout Modal Toggle
```js
productButton.addEventListener("click", () => {
  payment.style.display = "flex";
});
close.addEventListener("click", () => {
  payment.style.display = "none";
});
```

---

## 📸 Screenshots

| Hero Slider | Product Detail | Checkout Modal |
|---|---|---|
| ![Slider](https://images.unsplash.com/photo-1604147495798-57beb5d6af73?auto=format&fit=crop&w=400&q=60) | ![Product](https://images.pexels.com/photos/9295809/pexels-photo-9295809.jpeg?auto=compress&w=400) | ![Checkout](https://images.pexels.com/photos/1040427/pexels-photo-1040427.jpeg?auto=compress&w=400) |

---

## 📋 Product Catalog

| # | Name | Price | Colors |
|---|---|---|---|
| 1 | Air Force | $119 | Black, Dark Blue |
| 2 | Air Jordan | $149 | Light Gray, Green |
| 3 | Blazer | $109 | Light Gray, Green |
| 4 | Crater | $129 | Black, Light Gray |
| 5 | Hippie | $99 | Gray, Black |

---

## 🔮 Future Improvements

- [ ] 🛍️ Add a working shopping cart with item count badge
- [ ] 🔍 Implement search functionality
- [ ] 💾 Persist cart to `localStorage`
- [ ] 🌐 Connect to a backend API (Node.js / Firebase)
- [ ] 💳 Integrate Stripe for real payment processing
- [ ] 🌙 Add dark mode toggle
- [ ] ♿ Improve accessibility (ARIA labels, keyboard navigation)
- [ ] 🧪 Add unit tests with Jest

---

## 🤝 Contributing

Contributions are always welcome! Here's how:

```bash
# 1. Fork the project
# 2. Create your feature branch
git checkout -b feature/AmazingFeature

# 3. Commit your changes
git commit -m 'Add some AmazingFeature'

# 4. Push to the branch
git push origin feature/AmazingFeature

# 5. Open a Pull Request
```

---

## 📄 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for more information.

---

## 👨‍💻 Author

**Your Name**

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/your-username)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/your-username)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=todoist&logoColor=white)](https://your-portfolio.com)

---

<div align="center">

### ⭐ If you found this project helpful, please give it a star!

*Made with ❤️ and lots of ☕*

</div>

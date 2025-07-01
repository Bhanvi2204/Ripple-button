# 🌊 Ripple Button

An interactive **ripple effect button** built with **HTML**, **CSS**, and **JavaScript**, inspired by Material Design. A circular ripple animates outward from the cursor's position when hovering or clicking, providing tactile visual feedback.

---

## 🚀 Demo

Live demo showcasing dynamic ripple interaction:

*(Include your demo URL if hosted, e.g. GitHub Pages)*

---

## 🧱 Technologies

- **HTML5** – semantic markup and structure  
- **CSS3** – styling, pseudo-elements, custom properties, animations  
- **JavaScript** – event handling, position calculation, dynamic CSS variables

---

## ⚙️ How It Works

1. **HTML structure:**
    ```html
    <a href="#" class="btn">
      <span>Button</span>
    </a>
    ```

2. **CSS**:
   - `.btn { position: relative; overflow: hidden; }`
   - A `::before` pseudo-element forms the ripple bubble, styled via CSS and animated using `transition`.
   - Uses CSS variables `--posX` and `--posY` for ripple's origin.

3. **JavaScript**:
   - Listens for `mouseover` or `click` events on the button.
   - Calculates local cursor position inside the button using `e.pageX`, `e.pageY`, and `offsetLeft`, `offsetTop`.
   - Dynamically updates CSS variables to center ripple properly:
     ```js
     btnEl.style.setProperty("--posX", x + "px");
     btnEl.style.setProperty("--posY", y + "px");
     ```

---

## 🎯 Features

- **Dynamic initiation** – ripple originates from actual cursor position  
- **Smooth animation** – expands and fades seamlessly  
- **Minimal DOM** – uses pseudo-element, no extra markup  
- **Customizable** – easily tweak color, size, duration via CSS  

---


## 👨‍💻 Further Enhancements

- Trigger ripple on **click** or **touch** events  
- Add **fade-out effect** or **multiple ripple stacks**  
- Create a **reusable component** (e.g. React, Vue, Web Component)  
- Ensure **accessibility**: support keyboard navigation and focus states  

---

## 📄 License

This project is licensed under the MIT License – feel free to use and modify it!

---

**Enjoy creating ripples! 💧**

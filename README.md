# 🌟 Shopify Landing Page Development Guide 🌟

## 🎯 Overview
This project is a **custom Shopify landing page** built using **Shopify Liquid**, **HTML**, **CSS**, and **JavaScript**. It is designed to **enhance user experience**, **boost conversions**, and provide a **fully responsive layout**.

## 🚀 Features
- 🎨 **Custom Shopify Liquid Sections** for flexibility.
- 🔥 **Dynamic Content** powered by Shopify’s data objects.
- 📱 **Fully Responsive Design** for mobile and desktop.
- 🔍 **SEO Optimized Structure** to improve search visibility.
- 🎭 **Interactive UI** using JavaScript for enhanced user engagement.

## ⚙️ Installation & Setup
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/selimurraji/shopifylp.git
   ```
2. **Navigate to the Project Folder:**
   ```bash
   cd shopifylp
   ```
3. 📂 **Upload the Liquid files** to your Shopify theme under `Sections` or `Templates`.
4. 🏗 **Add the new block section** inside `sections/custom-block.liquid`.
5. 🎨 **Customize CSS & JS** inside Shopify’s `Assets` folder.
6. ✅ **Preview & Publish** on your Shopify store.

## 🎨 Styling with CSS
Modify the styles in `assets/theme.css`:
```css
body {
    background-color: #f4f4f4;
    font-family: Arial, sans-serif;
}
.button {
    background-color: #ff5733;
    color: white;
    padding: 10px 20px;
    border-radius: 5px;
    text-decoration: none;
}
```

## 🛠️ Interactive Elements with JavaScript
Enhance user experience with JavaScript in `assets/theme.js`:
```js
document.addEventListener("DOMContentLoaded", function() {
    const button = document.querySelector(".button");
    button.addEventListener("click", function() {
        alert("Button Clicked!");
    });
});
```

## 🏗 Adding a New Block Section
Create a new section file at `sections/custom-block.liquid`:
```liquid
{% schema %}
{
  "name": "Custom Block Section",
  "settings": [],
  "blocks": [
    {
      "type": "text",
      "name": "Text Block",
      "settings": [
        {
          "type": "text",
          "id": "text",
          "label": "Text Content"
        }
      ]
    }
  ],
  "presets": [
    {
      "name": "Custom Block"
    }
  ]
}
{% endschema %}
```
Include the section in `templates/index.json` or `templates/page.liquid`:
```liquid
{% section 'custom-block' %}
```

## 📁 File Structure
```
/shopify-landing-page
│── 🎨 assets/                # CSS & JS files
│── 🛠️ sections/              # Custom Liquid sections
│   │── 🏗 custom-block.liquid  # New Shopify block section
│── 🔄 snippets/              # Reusable Liquid components
│── 📄 templates/             # Page templates
│── ⚙️ config/                # Theme settings
│── 📜 README.md              # Project documentation
```

## 🔧 Usage
- 🖋 Modify `sections/custom-landing.liquid` to update the page layout.
- 🏗 Use `sections/custom-block.liquid` for new block-based content.
- 🛠 Use Shopify's `{% for %}`, `{% if %}`, and `{% assign %}` Liquid tags for dynamic content.
- 🎨 Add styles in `assets/theme.css`.
- ✨ Include interactive elements in `assets/theme.js`.

## 🎨 Customization
- ⚙️ Adjust settings in `config/settings_schema.json` for theme customizations.
- 🏗 Add Shopify metafields for dynamic content integration.
- 🔀 Modify JSON templates for different landing page variations.

## 🤝 Contributing
Pull requests are welcome! Please ensure your code follows Shopify's best practices. 🚀

## 📜 License
This project is **open-source** and available under the **MIT License**.

## 📬 Contact
For support or customization inquiries, reach out at **[selimurraji@gmail.com]**. ✉️

# محمد - Personal Arabic Blog

A clean, minimalist Hugo blog designed for Arabic content with a focus on simplicity and readability.

## ✨ Features

- **🌍 Arabic RTL Support**: Full right-to-left layout for Arabic content
- **🎨 Clean Design**: Minimalist aesthetic inspired by modern design principles
- **🌓 Dark/Light Mode**: Beautiful dark mode with custom color scheme
- **📧 Email Integration**: Kit (ConvertKit) email signup form
- **📱 Responsive**: Works perfectly on all device sizes
- **⚡ Fast Performance**: Optimized loading with Tailwind CSS
- **📝 Markdown Support**: Rich content authoring with emojis

## 🎨 Design

### Color Palette
- **Light Background**: `#FFFCF0` (Warm cream)
- **Dark Background**: `#100F0F` (Rich black)
- **Dark Mode Text**: `#CECDC3` (Soft gray)
- **Accent Color**: `#3AA89E` (Elegant teal)

### Typography
- Clean, readable fonts optimized for Arabic text
- Proper spacing and hierarchy
- Code syntax highlighting support

## 🚀 Quick Start

### Prerequisites
- [Hugo Extended](https://gohugo.io/installation/) (v0.135.0+)
- [Node.js](https://nodejs.org/) (for Tailwind CSS)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Haqbani/mohammad-blog.git
cd mohammad-blog
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
# Terminal 1: Hugo server
cd exampleSite
hugo server --themesDir ../.. --theme zahi --buildDrafts --buildFuture

# Terminal 2: Tailwind CSS watcher
cd ..
npx tailwindcss -i ./static/css/style.css -o ./static/css/output.css --watch
```

4. Open your browser to `http://localhost:1313`

## 📁 Project Structure

```
mohammad-blog/
├── archetypes/          # Content templates
├── exampleSite/         # Example site with content
│   ├── content/         # Blog posts and pages
│   │   └── posts/       # Blog articles
│   └── hugo.toml        # Site configuration
├── layouts/             # Hugo templates
│   ├── _default/        # Default page templates
│   ├── partials/        # Reusable template parts
│   └── index.html       # Homepage template
├── static/              # Static assets
│   ├── css/            # Stylesheets
│   └── js/             # JavaScript files
├── package.json         # Node.js dependencies
├── tailwind.config.js   # Tailwind CSS configuration
└── theme.toml          # Theme metadata
```

## ✍️ Creating Content

### New Blog Post

Create a new post in `exampleSite/content/posts/`:

```markdown
---
title: "عنوان المقال"
date: 2024-06-08
tags: ["علامة1", "علامة2"]
description: "وصف المقال"
---

محتوى المقال هنا...
```

### Supported Front Matter
- `title`: Post title
- `date`: Publication date
- `tags`: Array of tags
- `description`: Meta description
- `direction`: Text direction (`rtl` or `ltr`)

## 🎛️ Configuration

### Site Settings
Edit `exampleSite/hugo.toml`:

```toml
title = "اسم الموقع"
languageCode = "ar"
defaultContentLanguage = "ar"

[params]
github = "https://github.com/username"
mail = "mailto:email@example.com"
```

### Email Form
Replace the Kit form script in `layouts/index.html`:
```html
<script async data-uid="your-kit-id" src="https://your-domain.kit.com/your-kit-id/index.js"></script>
```

## 🔧 Customization

### Colors
Update color variables in `layouts/partials/header.html`:
```css
:root {
    --bg-light: #FFFCF0;
    --bg-dark: #100F0F;
    --text-dark: #CECDC3;
    --hover-color: #3AA89E;
}
```

### Typography
Modify Tailwind classes in templates or extend `tailwind.config.js`.

## 📦 Deployment

### Netlify
1. Connect your GitHub repository to Netlify
2. Set build command: `cd exampleSite && hugo --themesDir ../.. --theme zahi --minify`
3. Set publish directory: `exampleSite/public`

### Vercel
1. Import GitHub repository
2. Set framework preset to "Hugo"
3. Set build command: `cd exampleSite && hugo --themesDir ../.. --theme zahi --minify`
4. Set output directory: `exampleSite/public`

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues and pull requests.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [Hugo](https://gohugo.io/)
- Styled with [Tailwind CSS](https://tailwindcss.com/)
- Email integration by [Kit (ConvertKit)](https://kit.com/)
- Icons from the original Zahi theme

---

**Live Demo**: [Your site URL here]
**Author**: محمد
**GitHub**: [@Haqbani](https://github.com/Haqbani)

## Zahi Hugo Theme
![Zahi Hugo Theme](https://raw.githubusercontent.com/mohamedelhefni/zahi/main/images/screenshot.png)

Zahi is a Hugo theme designed to primarily support Arabic content with a simple and clean user interface.

### Features
- 🚀 **Outstanding Performance:** Zahi excels in high performance and fast loading speed.
- 💡 **Table of Contents:** Provides an organized table of contents for easy content navigation.
- 📌 **Featured Articles:** Allows pinning important articles for prominent visibility.
- 🔖 **Tags:** Enables easy content categorization using tags.
- 💬 **Disqus Support:** Facilitates interaction with readers through Disqus comments section.
- 📄 **Pagination Feature:** Allows dividing content into separate pages for smoother navigation.
- 🎨 **Syntax Highlighting:** Highlights and makes code more readable and clear.
- 📱 **Responsive Design:** Displays well on all screen sizes for a consistent user experience.
- 🌓 **Dark and Light Modes:** Offers users the choice between dark and light mode for a comfortable reading experience.

### Demo
You can view a live demo of the Zahi Hugo Theme [here](https://zahi.netlify.app/).

### Development
To start the development environment:

1. Start Hugo Server:
```bash
hugo server
```

Start Tailwind CSS Watcher:
```
npx tailwindcss -i ./static/css/style.css -o ./static/css/output.css --watch
```




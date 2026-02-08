# Homework-1: Simple Signup Form 📝

![Signup Form Preview](https://github.com/user-attachments/assets/b253ef16-c389-459f-bccd-e9eea6b145cd) 
*(Note: Replace this placeholder with an actual screenshot of the form for better visualization.)*

## 📖 Overview
Welcome to **Homework-1**, a beginner-friendly project demonstrating a basic user signup form built with pure HTML and CSS. This project serves as a practice exercise for creating responsive web forms with a clean, RTL (Right-to-Left) layout suitable for Persian/Farsi users. It includes no JavaScript, backend, or database integration—it's purely frontend and static.  

The form collects user details like name, lastname, phone number, email, and password, with a submit button. It's styled for a simple, aesthetically pleasing look and deployed via GitHub Pages for easy hosting.  

This documentation provides a complete guide to the project, including structure, features, usage, and more. Feel free to fork, modify, or use it as a starting point for your own projects! 🚀

## ✨ Features
- **RTL Support** 🇮🇷: Designed for right-to-left languages like Farsi, ensuring proper text alignment and input direction.
- **Responsive Design** 📱: Adjusts for smaller screens (e.g., mobile) using media queries.
- **Simple Styling** 🎨: Uses CSS for borders, shadows, hover effects, and a warm color scheme (bisque background with aliceblue inputs).
- **Form Validation (Basic)**: Relies on HTML5 input types (e.g., `type="email"`, `type="tel"`) for client-side validation—no custom JS yet.
- **Deployment Ready** ☁️: Includes a GitHub Actions workflow for automatic deployment to GitHub Pages.
- **MIT Licensed** 📜: Free to use, modify, and distribute.
- **No Backend/Database** ⚠️: This is a static page; form submission doesn't send data anywhere (use it as a template for full apps).

## 🛠️ Project Structure
The project follows a minimal structure for a static web page. Here's the file tree:

```
Homework-1/
├── index.html          # Main HTML file with the signup form structure
├── style.css           # CSS stylesheet for layout, colors, and responsiveness
├── LICENSE             # MIT License file
├── README.md           # Project documentation (this file or the original social links version)
└── .github/
    └── workflows/
        └── static.yml  # GitHub Actions workflow for deploying to GitHub Pages
```

- **Total Files**: 5 (including workflow).
- **No Folders for Assets**: No images or additional resources are used beyond a favicon (linked but not included in source).
- **Build Tools**: None required—pure HTML/CSS, no bundlers or preprocessors.

## 📋 Detailed File Explanations
Here's a breakdown of every file and its contents:

### 1. `index.html` 🏠
- **Purpose**: The core HTML file rendering the signup form.
- **Key Elements**:
  - `<head>`: Meta tags for charset (UTF-8), viewport (mobile-friendly), description, keywords, title, stylesheet link, and favicon.
  - `<body>`: 
    - `.title`: Header with `<h1>` and `<p>` for instructions.
    - `.forum-singup`: Container for the form inputs.
    - Inputs: Text fields for name, lastname, phone, email, password; submit button.
    - Link: "Already have an account? Click to login." (non-functional placeholder).
- **Classes/IDs**: Uses classes like `.input-row`, `.first`, `.middle`, `.last` for styling; IDs like `#first-label`, `#first-input`, `#last-input` for specific overrides.
- **No Scripts**: Pure markup—no JavaScript functions or event handlers.
- **Language/Dir**: `lang="fa-IR"` and `dir="rtl"` for Farsi support.

### 2. `style.css` 🎨
- **Purpose**: Styles the HTML elements for visual appeal and layout.
- **Key Sections**:
  - Global Reset: `* { margin: 0; padding: 0; box-sizing: border-box; }` to normalize.
  - Body: Sets background (bisque), text color, and font family.
  - `.title`: Centers text with large headings.
  - `.forum-singup`: Main form container with border, background, padding, and RTL direction.
  - `.input-row`: Flexbox for label-input pairs.
  - Inputs/Labels: Custom borders, radii, shadows, hover/active states.
  - Media Query: `@media (max-width: 800px)` adjusts margins for responsiveness.
- **No Advanced Features**: No variables, grids, or animations—basic CSS2/3.

### 3. `LICENSE` 📜
- **Purpose**: Defines the MIT License for open-source usage.
- **Details**: Grants permission to use, copy, modify, etc., without warranty. Copyright 2025 Sobhan.

### 4. `README.md` (Original) 📄
- **Purpose**: Provides contact info and social links.
- **Content**: HTML embeds for Telegram, Instagram, Twitch, YouTube, GitHub, Discord servers, and user widgets.
- **Note**: This documentation replaces or expands it for GitHub.

### 5. `.github/workflows/static.yml` ⚙️
- **Purpose**: Automates deployment to GitHub Pages.
- **Triggers**: On push to `main` branch or manual workflow dispatch.
- **Permissions**: Reads contents, writes to Pages.
- **Jobs**: 
  - Checkout code.
  - Setup Pages.
  - Upload artifact (entire repo).
  - Deploy to Pages.
- **Concurrency**: Allows only one deployment at a time, no cancellations.

## 🔧 Usage and Commands
Since this is a static HTML project, there are no runtime commands or servers needed. Here's how to use it:

### Setup and Run Locally 🖥️
1. Clone the repo: `git clone https://github.com/your-username/Homework-1.git`
2. Open `index.html` in any browser (e.g., Chrome, Firefox).
3. That's it! No installation required.

### Deployment to GitHub Pages ☁️
- Push to `main`: The workflow auto-deploys.
- Manual: Go to GitHub Actions tab > Run workflow.
- Access: Visit `https://your-username.github.io/Homework-1/`.

### Common Commands (CLI) 📟
- **View in Browser**: No command—double-click `index.html`.
- **Lint/Check**: Use tools like `htmlhint index.html` or `stylelint style.css` (install via npm if needed).
- **No Build Step**: No `npm install`, `yarn build`, etc.—static only.

## ⚙️ Frequently Used Functions/Elements
This project has **no JavaScript**, so no functions. Instead, here's a list of commonly used HTML elements and CSS selectors:

- **HTML Elements**:
  - `<input type="text">`: For name and lastname.
  - `<input type="tel">`: For phone number.
  - `<input type="email">`: For email validation.
  - `<input type="password">`: Hides password input.
  - `<input type="submit">`: Form submission button.
- **CSS Selectors**:
  - `.input-row input`: Styles all inputs with borders and RTL direction.
  - `#last-input:hover`: Hover effect for submit button.
  - `.forum-singup a`: Styles the login link.

If you add JS later, common functions might include form validation (e.g., `checkEmail()` or `submitForm()`).

## 🗄️ Databases and Data Storage
This project has **no databases** or storage mechanisms—it's frontend-only. Form data isn't saved or sent anywhere.  

- **Potential Future Additions**:
  - Use LocalStorage (JS) for temporary data: e.g., `{ "name": "string", "email": "string" }`.
  - Backend Integration: Connect to a database like MongoDB or SQLite via API.
  - Sample Data Structure (Hypothetical):
    - **User Table**:
      - `id`: Integer (auto-increment).
      - `name`: String (e.g., "Sobhan").
      - `lastname`: String (e.g., "SRZA").
      - `phone`: String (e.g., "+989123456789").
      - `email`: String (e.g., "example@email.com").
      - `password`: String (hashed, e.g., "hashedpass123").
    - No real implementation here.

## 🤝 Contributing
Fork the repo, make changes, and submit a PR! Suggestions for adding JS validation or backend are welcome. 😊

## 📞 Contact
See the original README.md for social links, or reach out via GitHub issues.

## 🔒 License
MIT License—see [LICENSE](LICENSE) for details.

Thanks for checking out Homework-1! If you have questions, open an issue. ⭐

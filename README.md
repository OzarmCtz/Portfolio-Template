Voici un `README.md` plus court et simple sans mention de la licence :

```markdown
# Personal Portfolio - Vue.js

This is a personal portfolio built with Vue.js. It displays sections like About Me, Tech Stack, Experience, Projects, and Certifications. You can easily enable or disable sections by modifying a simple configuration.

## Features

- **Dynamic Sections**: Enable or disable sections with a simple `true/false` configuration.
- **Customizable**: Modify content and style to match your needs.

## Configuration

In the `src/App.vue` file, modify the `config` object to control which sections are shown:

```javascript
const config = {
    aboutMe: true,        // Enable/Disable "About Me" section
    techno: true,         // Enable/Disable "Tech Stack" section
    xp: true,             // Enable/Disable "Experience" section
    projects: true,       // Enable/Disable "Projects" section
    certification: true   // Enable/Disable "Certifications" section
};
```

- **true**: Section is enabled.
- **false**: Section is disabled.

## Project Setup

1. **Clone the repository**:

    ```bash
    git clone https://github.com/your-username/portfolio.git
    ```

2. **Install dependencies**:

    ```bash
    cd portfolio
    npm install
    ```

3. **Run the project**:

    ```bash
    npm run dev
    ```

4. Open [http://http://localhost:5173/](http://http://localhost:5173/) in your browser.

## Customization

- Modify the components in `src/components/` to change content.
- Customize styles in `src/assets/` or component-level styles.

---

That's it! Enjoy customizing your portfolio.
```

### Key Changes:
- **Concise Description**: Shortened the explanation of features and configuration.
- **No License**: Removed the license section as requested.
- **Clear Setup Instructions**: Simplified the setup instructions for getting the project running quickly.
  
Let me know if this fits your needs!
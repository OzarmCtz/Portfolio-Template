```markdown
# Personal Portfolio - Vue.js

This is a personal portfolio built with Vue.js. It displays sections like About Me, Tech Stack, Experience, Projects, and Certifications. You can easily enable or disable sections by modifying a simple configuration.

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

4. Open [http://http://localhost:8080/](http://http://localhost:8080/) in your browser.

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

## Customization

- Modify the components in `src/components/` to change content.
- Customize styles in `src/assets/` or component-level styles.

---

That's it! Enjoy customizing your portfolio.

Crédit : Udemy Course (https://www.udemy.com/course/formation-vue-js-par-la-pratique-le-cours-ultime-tout-en-1-vuejs/?couponCode=KEEPLEARNING)
By Anthony Cardinale
```


  

# 🌟 Personal Portfolio - Vue.js

![image](https://github.com/user-attachments/assets/b8f1d352-ced5-42af-9bbd-6119ab5c75ba)


Welcome to my **Personal Portfolio** built with Vue.js! 🎨 This project showcases dynamic sections such as About Me, Tech Stack, Experience, Projects, and Certifications. It's fully customizable and easy to manage. 

## 🚀 Getting Started

Follow these steps to set up and run the portfolio locally:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/OzarmCtz/Portfolio-Template.git
    ```

2. **Navigate to the project folder**:
    ```bash
    cd MyPortfolio
    ```

3. **Install dependencies**:
    ```bash
    npm install
    ```

4. **Run the development server**:
    ```bash
    npm run dev
    ```

5. Open your browser and go to [http://localhost:8080](http://localhost:8080).

---

## ✨ Features

- **Dynamic Sections**: Control visibility of sections using a simple configuration.
- **Modular Design**: Each section is a separate component for easy customization.
- **Tech Stack**: Built with modern technologies including Vue.js and Vite.

---

## ⚙️ Configuration

Easily enable or disable sections by editing the `config` object in the `src/App.vue` file:

```javascript
const config = {
    aboutMe: true,        // Enable/Disable "About Me" section
    techno: true,         // Enable/Disable "Tech Stack" section
    xp: true,             // Enable/Disable "Experience" section
    projects: true,       // Enable/Disable "Projects" section
    certification: true   // Enable/Disable "Certifications" section
};
```

---

## 🚧 TODO

- ✨ **Add a contact form to the "Contact" page** (`src/pages/contactPage`)
  - 📝 Include fields for the user's **name**, **email**, and **message**.
  - ✅ Add **form validation** (ensure required fields are filled out).
  - ✉️ Implement functionality for **form submission** (e.g., sending an email or storing data).
  - 🎨 **Style the form** to match the overall design of the portfolio.

---


## 👨‍🏫 Credit

Anthony Cardinale (Teacher) 
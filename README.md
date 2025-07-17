# 🏡 ALX Listing App

## 📘 Project Overview

**ALX Listing App** is a modern, production-ready scaffold for an **Airbnb-style property listing application**, built with:

- **Next.js**
- **TypeScript**
- **TailwindCSS**
- **ESLint**

This milestone sets the foundation for creating a responsive, reusable, and scalable front-end structure. It includes initial configurations, folder structure setup, asset management, and base components.

## 🎯 Goals

- Set up a clean and scalable Next.js project
- Use **TypeScript** for strong typing and maintainability
- Configure **TailwindCSS** for efficient styling
- Establish a clear project structure with reusable components
- Organize assets for easy access and maintenance

## 🧱 Project Structure

```
alx-listing-app/
│
├── components/
│   └── common/
│       ├── Card.tsx       # Reusable Card component
│       └── Button.tsx     # Reusable Button component
│
├── constants/
│   └── index.ts           # Reusable strings, API URLs, configs
│
├── interfaces/
│   └── index.ts           # TypeScript interfaces (e.g., CardProps, ButtonProps)
│
├── pages/
│   ├── index.tsx          # Home page
│
├── public/
│   └── assets/            # Images, SVGs, placeholders
│
├── styles/
│   └── globals.css        # Tailwind CSS base styles
│
├── tailwind.config.js     # Tailwind configuration
├── postcss.config.js      # PostCSS configuration
├── tsconfig.json          # TypeScript configuration
├── next.config.js         # Next.js configuration
├── package.json           # Project dependencies and scripts
└── README.md              # Project documentation
```

## ⚙️ Tech Stack

- [Next.js 13+](https://nextjs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [TailwindCSS](https://tailwindcss.com/)
- [ESLint](https://eslint.org/)
- [Node.js 16+](https://nodejs.org/)

## 🛠 TailwindCSS Setup

### `tailwind.config.js`

```js
module.exports = {
  content: ["./pages/**/*.{ts,tsx}", "./components/**/*.{js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

### `styles/globals.css`

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## 🖼 Asset Management

All static files like images and icons should go in the `public/assets/` directory.

**Example:**

```
public/assets/
├── logo.svg
├── placeholder.jpg
└── house-icon.svg
```

These assets can be referenced in components using:

```tsx
<img src="/assets/placeholder.jpg" alt="Placeholder" />
```

## 🧪 How to Run the Project Locally

### 1. Create the App

```bash
npx create-next-app@latest alx-listing-app \
  --typescript \
  --tailwind \
  --eslint \
  --no-app-router \
  --no-src-dir
```

### 2. Navigate into the Project

```bash
cd alx-listing-app
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Start the Development Server

```bash
npm run dev
```

Visit [http://localhost:3000](http://localhost:3000) in your browser.

## 📁 Key Directories Explained

| Directory           | Purpose                                                     |
| ------------------- | ----------------------------------------------------------- |
| `components/common` | Reusable UI components like `Card` and `Button`             |
| `interfaces`        | TypeScript interfaces for props and data types              |
| `constants`         | Centralized values like API URLs, labels, and configuration |
| `public/assets`     | All images and icons used in the app                        |
| `styles`            | Global Tailwind CSS styles                                  |

## 📄 License

This project is part of the ALX Software Engineering Program and follows its guidelines.

## 🤝 Contributing

Feel free to fork this project and experiment. Contributions are welcome once the base milestone is complete.

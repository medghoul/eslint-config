# ESLint Configurations

Complete collection of ESLint configurations for modern JavaScript/TypeScript projects.

## 🛠 Available Configurations

- Node.js
- React
- Angular
- Next.js
- Vue.js

## 📦 Installation

Choose the configuration based on your framework:

### Angular
```bash
npm i -D @angular-eslint/eslint-plugin @angular-eslint/eslint-plugin-template @angular-eslint/template-parser @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-config-prettier eslint-plugin-prettier prettier
```

### Next.js
```bash
npm i -D eslint eslint-config-next @typescript-eslint/parser @typescript-eslint/eslint-plugin eslint-config-prettier eslint-plugin-prettier prettier
```

### Vue.js
```bash
npm i -D eslint eslint-plugin-vue @vue/eslint-config-typescript @typescript-eslint/parser @typescript-eslint/eslint-plugin eslint-config-prettier eslint-plugin-prettier prettier
```

### Node.js
```bash
npm i -D eslint eslint-config-airbnb-base eslint-config-prettier eslint-plugin-import eslint-plugin-node eslint-plugin-prettier prettier
```

### React
```bash
npm i -D eslint eslint-config-airbnb eslint-config-prettier eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react eslint-plugin-react-hooks eslint-plugin-prettier prettier
```

## 🚀 Usage

1. Choose the configuration you need from the corresponding folder
2. Copy the `.eslintrc.json` file to your project
3. Install the necessary dependencies using the provided npm command
4. (Optional) Copy the `.prettierrc` file if you want to use the same Prettier configuration

## ✨ Features

- Optimized configurations for each framework
- Integrated TypeScript support
- Prettier integration
- Best practices for each ecosystem
- Customizable rules

## 📝 Notes

- Angular configurations require a valid `tsconfig.json` file
- For Next.js, make sure you have Next.js installed in your project
- For Vue.js, the configuration is optimized for Vue 3

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## 📄 License

MIT License - See LICENSE file for details

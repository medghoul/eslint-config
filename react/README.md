# React (.eslintrc.json)

# 1- Install these packages in your dev dependencies using this command:
# npm i -D eslint eslint-config-airbnb eslint-config-prettier eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react eslint-plugin-react-hooks eslint-plugin-prettier prettier

# 2- Create ".eslintrc.json" file in the root directory with these configration:

# File: .eslintrc.json per React

{
    "extends": [
      "airbnb",
      "prettier",
      "plugin:react/recommended",
      "plugin:react-hooks/recommended"
    ],
    "plugins": [
      "prettier",
      "react",
      "react-hooks"
    ],
    "env": {
      "browser": true,
      "es6": true,
      "node": true
    },
    "parserOptions": {
      "ecmaVersion": 2022,
      "sourceType": "module",
      "ecmaFeatures": {
        "jsx": true
      }
    },
    "settings": {
      "react": {
        "version": "detect"
      }
    },
    "rules": {
      "prettier/prettier": ["error", {
        "singleQuote": true,
        "printWidth": 80,
        "tabWidth": 2,
        "semi": true,
        "jsxSingleQuote": false
      }],
      "react/react-in-jsx-scope": "off",
      "react/prop-types": "warn",
      "react/jsx-filename-extension": [1, { "extensions": [".jsx", ".tsx"] }],
      "react/jsx-props-no-spreading": "off",
      "react-hooks/rules-of-hooks": "error",
      "react-hooks/exhaustive-deps": "warn",
      "import/prefer-default-export": "off",
      "no-console": "warn",
      "no-unused-vars": ["warn", { "argsIgnorePattern": "^_" }],
      "import/no-extraneous-dependencies": ["error", {
        "devDependencies": [
          "**/*.test.js",
          "**/*.spec.js",
          "**/*.test.jsx",
          "**/*.spec.jsx"
        ]
      }]
    }
  }
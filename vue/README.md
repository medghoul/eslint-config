## Vue.js (.eslintrc.json)

# 1- Install these packages in your dev dependencies using this command:
# npm i -D eslint eslint-plugin-vue @vue/eslint-config-typescript @typescript-eslint/parser @typescript-eslint/eslint-plugin eslint-config-prettier eslint-plugin-prettier prettier

# 2- Create ".eslintrc.json" file in the root directory with these configration:

{
  "env": {
    "browser": true,
    "es2022": true,
    "node": true
  },
  "extends": [
    "plugin:vue/vue3-recommended",
    "plugin:@typescript-eslint/recommended",
    "prettier"
  ],
  "parser": "vue-eslint-parser",
  "parserOptions": {
    "parser": "@typescript-eslint/parser",
    "ecmaVersion": 2022,
    "sourceType": "module"
  },
  "plugins": ["vue", "@typescript-eslint", "prettier"],
  "rules": {
    "prettier/prettier": ["error", {
      "singleQuote": true,
      "printWidth": 80,
      "tabWidth": 2,
      "semi": true
    }],
    "vue/multi-word-component-names": "warn",
    "vue/require-default-prop": "error",
    "vue/require-explicit-emits": "error",
    "vue/component-name-in-template-casing": ["error", "PascalCase"],
    "vue/script-setup-uses-vars": "error",
    "@typescript-eslint/no-unused-vars": ["warn", { "argsIgnorePattern": "^_" }],
    "@typescript-eslint/explicit-function-return-type": "warn",
    "@typescript-eslint/no-explicit-any": "warn",
    "no-console": ["warn", { "allow": ["warn", "error"] }]
  }
}
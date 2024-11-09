## Node.js (.eslintrc.json)
# 1- Install these packages in your dev dependencies using this command:

# npm i -D eslint eslint-config-airbnb-base eslint-config-prettier eslint-plugin-import eslint-plugin-node eslint-plugin-prettier prettier

# 2- Create ".eslintrc.json" file in the root directory with these configration:

# File: .eslintrc.json per Node.js

{
  "extends": [
    "airbnb-base",
    "prettier",
    "plugin:node/recommended"
  ],
  "plugins": ["prettier"],
  "env": {
    "node": true,
    "es6": true
  },
  "parserOptions": {
    "ecmaVersion": 2022
  },
  "rules": {
    "prettier/prettier": ["error", {
      "singleQuote": true,
      "printWidth": 80,
      "tabWidth": 2,
      "semi": true
    }],
    "spaced-comment": "off",
    "no-console": "warn",
    "consistent-return": "off",
    "func-names": "off",
    "object-shorthand": "off",
    "no-process-exit": "off",
    "no-param-reassign": "off",
    "no-return-await": "off",
    "no-underscore-dangle": "off",
    "class-methods-use-this": "off",
    "no-undef": "error",
    "prefer-destructuring": ["error", { "object": true, "array": false }],
    "no-unused-vars": ["warn", { "argsIgnorePattern": "req|res|next|val" }],
    "import/no-extraneous-dependencies": ["error", {
      "devDependencies": ["**/*.test.js", "**/*.spec.js"]
    }]
  }
}

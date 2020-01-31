# Testes automatizados com Node.js

Nesse projeto foi construída uma simples API utilizando o desenvolvimento guiado
por testes TDD através da biblioteca Jest no Node.js

## Para iniciar os testes, alterar os scripts no package.json conforme seu OS:

OS X & Linux:

```sh
"pretest": "NODE_ENV=test sequelize db:migrate",
"test": "NODE_ENV=test jest",
"posttest": "NODE_ENV=test sequelize db:migrate:undo:all"
```

Windows:

```sh
"pretest": "cross-env NODE_ENV=test sequelize db:migrate",
"test": "jest",
"posttest": "cross-env NODE_ENV=test sequelize db:migrate:undo:all"
```

## Inicialização

```sh
yarn
yarn test
```

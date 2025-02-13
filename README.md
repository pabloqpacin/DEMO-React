# DEMO-React

Hello World


## Crear proyecto

<!-- 
- ~~`pnpm`~~
```sh
npm install pnpm -g
pnpm install
```
 -->


-  `npm`

```sh
NVM_VERSION=0.40.1
NODE_VERSION=23

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v${NVM_VERSION}/install.sh | bash

nvm install node ${NODE_VERSION}
echo ${NODE_VERSION} > .nvmrc

nvm use
```

<!-- ```bash
npx create-react-app hello-world --template typescript | yes

mv hello-world/* .
rmdir hello-world

# Si aparece el error: Could not resolve dependency: peer react@"^18.0.0" from @testing-library/react@13.4.0
npm install react@18 react-dom@18

# npm start
# NO ME ESTÁ GUSTANDO EL TEMA
``` -->

```sh
# Creates package.json
npm init
  # ...

# Creates package-log.json
npm install --save-dev typescript
  # With --save-dev it's saved as a development dependency, thus not required for the production build of the app

echo "node_modules" >> .gitignore
```

```sh
npm install --save-dev @tsconfig/recommended

# Creates tsconfig.json
echo "..." > tsconfig.json

npm install react react-dom

npm install --save-dev @types/react @types/react-dom
```

```sh
npm install --save-dev webpack webpack-cli webpack-dev-server html-webpack-plugin ts-loader

echo "..." > webpack.config.js

npm install --save-dev ts-node
```




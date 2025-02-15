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

## Construir proyecto

```sh
echo "..." > src/index.tsx
``` 

```sh
node_modules/.bin/webpack serve --mode development --open
  # [webpack-cli] Failed to load '/home/pabloqpacin/repos/DEMO-React_HelloWorld/webpack.config.ts' config
  # [webpack-cli] ReferenceError: module is not defined
  #     at /home/pabloqpacin/repos/DEMO-React_HelloWorld/webpack.config.ts:3:1
  #     at ModuleJobSync.runSync (node:internal/modules/esm/module_job:396:35)
  #     at ModuleLoader.importSyncForRequire (node:internal/modules/esm/loader:366:47)
  #     at loadESMFromCJS (node:internal/modules/cjs/loader:1554:24)
  #     at Module._compile (node:internal/modules/cjs/loader:1705:5)
  #     at Object.loadTS [as .ts] (node:internal/modules/cjs/loader:1815:10)
  #     at Module.load (node:internal/modules/cjs/loader:1458:32)
  #     at Function._load (node:internal/modules/cjs/loader:1275:12)
  #     at TracingChannel.traceSync (node:diagnostics_channel:322:14)
  #     at wrapModuleLoad (node:internal/modules/cjs/loader:234:24)
```




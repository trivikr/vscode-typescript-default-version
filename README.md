# vscode-typescript-default-version
Repo for testing default version of typescript used by VSCode

Steps to reproduce:
* `yarn` or `npm install` to install dependencies
* `./node_modules/.bin/tsc --version` to confirm installed version is `2.4.2`
* Open the project in VSCode (tested with Version 1.22.2)
* Confirm that `.vscode/settings.json` has following setting to use typescript version fron `node_modules` as defined in [documentation](https://code.visualstudio.com/docs/languages/typescript#_using-newer-typescript-versions):
```json
{
  "typescript.tsdk": "./node_modules/typescript/lib"
}
```
* Open `index.ts` and notice that VSCode's version of TypeScript is used by default

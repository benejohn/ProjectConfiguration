# ProjectConfiguration
Project Configuration

I have my main configuration from my typescript projects

## I use Eslint and Prettier to do my script nice
 
 We need to create <b>editorconfig</b> directly in visual studio code to make the code standardized
 
 Use <b>"yarn add eslint -D"</b> to add eslint as dev
<ol> 
  later i use <b>"yarn eslint --init"</b> to init the project
  <li>"To check syntax, find problems, and enforce code style"</li>
  <li>JavaScript modules (import/export)</li>
  <li>None (because it is nodejs project)</li>
  <li>Yes (i'm using typescript)</li>
  <li>Node</li>
  <li>Use a popular style guide</li>
  <li>Airbnb (because it is using semicolon at end of sentence)</li>
  <li>JSON (format of file)</li>
  <li>No. If i want install with NPM, i'm using Yarn so NO</li>
</ol>

after i use <b>"yarn add eslint-import-resolver-typescript -D"</b> because eslint not check about typescript files

added it in .eslintrc.json to work this one

> "import/extensions" and "import/resolver" 

and add Prettier

> "yarn add -D prettier eslint-config-prettier eslint-plugin-prettier"

## Configuration of Debugger in VSCODE

changed "name" to "Debug" but it is random

changed "request" to "attach" because attach will work at project running

and added ' "restart": true ' to reload project

### line of package.json to work everything

install "yarn add -D ts-node-dev" to reload project, --inspect to Debbuger in VsCode, --transpile-only to do fast script and --ignore-watch to ignore node_modules 

> ts-node-dev --inspect --transpile-only --ignore-watch node_modules src/server.ts

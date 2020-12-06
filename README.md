# ProjectConfiguration
Project Configuration

I have my main configuration from my typescript projects

## I use Eslint and Prettier to do my script nice
 
 first i use <b>"yarn add eslint -D"</b> to add eslint as dev
<ol> 
  later i use <b>"yarn eslint --init" to init the project
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

after i use <b>"yarn add eslint-import-resolver-typescript -D"</b> because eslint not check about typescript files]

added it in .eslintrc.json

> "import/resolver": {
>      "typescript": {
>
>      }


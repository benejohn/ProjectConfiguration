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

>  "dev:server": "ts-node-dev --inspect --transpile-only --ignore-watch node_modules src/server.ts"


# DockerConfiguration

<ol>
  <li>You need to go from docker website and download and install</li>
  <li>Search in google "docker postgres"</li>
  <li>"docker run --name gostack_postgres -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres" to install a container of postgres in docker</li>
  <li>"docker ps" to check if container is working(active). About check all container in machine "docker ps -a"</li>
  <li>"docker logs IDFromMachine" to check logs and problems</li>
  <li>"docker stop IDFromMachine" to stop container</li>
  <li>"docker start (IDFromMachine || Name)" example "docker start postgres"</li>
  <li>Install Dbeaver or Postbird to check about Database projects</li>
</ol>

# TypeORM

1. "https://typeorm.io/" getting started and "Using ormconfig.json"
2. install typeorm and database drive(postgres, mysql). Example: "yarn add typeorm pg"
3. Create folder database in src and do index.ts with imports from typeorm { createConnection }

> "typeorm": "ts-node-dev ./node_modules/typeorm/cli.js"

added this in package.json at scripts to do migrations with js because we are in project with ts

We use "yarn typeorm migration:create -n (name of table)" to do the file to do modifications in database. Up is the updagred and down to downgrade 
Example 
"yarn typeorm migration:create -n CreateAppointments"

We use "yarn typeorm migration:run" to execute the migrations in database.


# Customized Bootstrap.v4 SASS environment
Basic init front-end development environment using bootstrap 4, sass and node modules to build css
<br><small></small>

### Pre-setup <small>pré-requisitos</small>

You need [**_Node.js_**](https://nodejs.org/en/) and [**_Sass_**](http://sass-lang.com/install) installed _(ignore this step if you already have)_:<br>
<sup>Você precisa do [**_Node.js_**](https://nodejs.org/en/) e do [**_Sass_**](http://sass-lang.com/install) instalado _(ignore este passo se você já os tem)_</sup>

1. To install node go to [nodejs.org](https://nodejs.org/) download and install the lastest version to your OS.
<br><small>Para instalar o node vá até o site [nodejs.org](https://nodejs.org/) e baixe a versão mais recente para o seu Sistema Operacional.</small>

2. To install sass run this line in terminal.
<br><small>Para instalar o sass execute a linha abaixo no terminal</small>
```sh
$ sudo gem install sass
```
------
### Setup <small>instalação</small>
1. Clone this repo whatever you want...
<br><small>Clone este repositório onde quiser...</small>
```sh
$ git clone https://github.com/MaickellVilela/Customized-Bootstrap.v4-sass-environment.git
```
2. Then instal node modules
<br><small>Então instale os módulos do node</small>
  * **botstrap** _v4.0.0.alpha.2_ // The most popular front-end framework
  * **autoprefixer**                // write vendor prefixes (no longer inside bootstrap)
  * **node-sass**                   // compile sass
  * **node-sass-asset-functions**   // provide image-size functions
  * **postcss-cli**                 // command line interface for css
  * **onchange**                    // watch file changes

  ```sh
  $ npm install
  ```

3. :tada: That's it! :beer:
<br><small>É isso aí!</small>

---

### Usage <small>uso</small>
  #### File structure <small>estrutura de arquivos</small>
  ```
  project
  │   README.md
  │   package.json
  │
  └─  style/
      |
      └─  scss/
      |   |
      |   └─  _local-variables.scss
      |   └─  custom-bootstrap.scss
      |   └─  main.scss
      |
      └─  css/   << scss will be compiled to this folder

  ```
##### scripts
  To compile scss files to css folder with vendor prefixes
  <br><small>para compilar os arquivos .scss para a pasta "css" com os prefixos dos navegadores</small>
  ```sh
  $ npm run build:css
  ```

  Run build after every scss file change in scss folder
  <br><small>O seguinte comando compila o css sempre que houver uma mudança na pasta "scss"</small>
  ```sh
  $ npm run watch:css
  ```

### Todo:

We will keep it _simple_ for now, but we have a lot to do in other repos.
- :white_check_mark: Custom bootstrap file structure
- :white_check_mark: Compile SASS
- :white_check_mark: Watch file changes and compile
- :white_check_mark: Vendor prefixes
- [ ] bootstrap 4 customization tutorial
- [ ] Interface test with [**BackstopJS**](https://garris.github.io/BackstopJS/)
- [ ] Performance improvements like mify
- [ ] Automate tasks

# Customized Bootstrap.v4 SASS environment
Basic init front-end development environment using bootstrap 4, sass and node modules to build css
<br><sup>Estrutura básica de desenvolvimento front-end para customizar o bootstrap utilizando modulos node para compilar o sass.</sup>

### Pre-setup <sub>pré-requisitos</sub>

You need [**_Node.js_**](https://nodejs.org/en/) and [**_Sass_**](http://sass-lang.com/install) installed _(ignore this step if you already have)_:<br>
<sup>Você precisa do [**_Node.js_**](https://nodejs.org/en/) e do [**_Sass_**](http://sass-lang.com/install) instalado _(ignore este passo se você já os tem)_</sup>

1. To install node go to [nodejs.org](https://nodejs.org/) download and install the lastest version to your OS.
<br><sup>Para instalar o node vá até o site [nodejs.org](https://nodejs.org/) e baixe a versão mais recente para o seu Sistema Operacional.</sup>

2. To install sass run this line in terminal.
<br><sup>Para instalar o sass execute a linha abaixo no terminal</sup>
```sh
$ sudo gem install sass
```
------
### Setup <sub>instalação</sub>
1. Clone this repo whatever you want...
<br><sup>Clone este repositório onde quiser...</sup>
```sh
$ git clone https://github.com/MaickellVilela/Customized-Bootstrap.v4-sass-environment.git
```
2. Then instal node modules
<br><sup>Então instale os módulos do node</sup>
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
<br><sup>É isso aí!</sup>

---

### Usage <sub>uso</sub>

#### File structure <sub>estrutura de arquivos</sub>
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
  <br><sup>para compilar os arquivos .scss para a pasta "css" com os prefixos dos navegadores</sup>
  ```sh
  $ npm run build:css
  ```

  Run build after every scss file change in scss folder
  <br><sup>O seguinte comando compila o css sempre que houver uma mudança na pasta "scss"</sup>
  ```sh
  $ npm run watch:css
  ```

### Todo:

We will keep it _simple_ for now, but we have a lot to do in other repos.
<br><sup>Vamos manter as coisas de modo simples por enquanto, mas temos muito a fazer em outros repositórios</sup>
:white_check_mark: Custom bootstrap file structure
:white_check_mark: Compile SASS
:white_check_mark: Watch file changes and compile
:white_check_mark: Vendor prefixes
- [ ] bootstrap 4 customization tutorial
- [ ] Interface test with [**BackstopJS**](https://garris.github.io/BackstopJS/)
- [ ] Performance improvements like mify
- [ ] Automate tasks

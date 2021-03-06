[Read in English](https://github.com/williamcanin/gosync-pug/blob/master/README_en.md)

# Go!Sync Pug

[![NodeJS with Gulp](https://github.com/williamcanin/gosync-pug/actions/workflows/npm-gulp.yml/badge.svg)](https://github.com/williamcanin/gosync-pug/actions/workflows/npm-gulp.yml)

Simples boilerplate usando [Pug](http://pugjs.org), [Gulp](http://gulpjs.com/), [Twitter Bootstrap](http://getbootstrap.com), e [Browser Sync](https://www.browsersync.io).

### Introdução

"Go!Sync Pug" facilita o desenvolver de projetos HTML's de uma forma em que o monitoramento de todas as alterações ocorridas em Pug, Folhas de estilos e Javascripts são feitas automaticamente através de tarefas do [Gulp](http://gulpjs.com/), [plugins](https://github.com/williamcanin/gosync-pug/blob/master/package.json), e [Browser Sync](https://www.browsersync.io). Uma facilidade pra esquecer o F5 do navegador ;)


### *Como é o funcionamento do **Go!Sync Pug**?*

* Toda estrutura de arquivos .pug são minificadas para html.

* Você cria as folhas de estilos com SASS que serão compiladas para CSS e minificadas automaticamente* a cada alteração.

* Os JavaScripts são concatenados e minificados automaticamente a cada alteração também.

* As imagens também são minificadas, porém, somente na inicialização do  Browser Sync ou na execução de compilação com a tarefa `$ gulp build` ou da própria tarefa de minificação da imagem ` gulp imagemin` .

* O projeto será armazenado na pasta `public`.


### Requerimentos

| Requerido       | Versão | Como verificar      | Como instalar  |
| --------------- | -------| ------------------- | -------------- |
| Git             | indiferente | `git --version`     | [Git](http://git-scm.com/) |
| Node            | >= 12.0 | `node -v`          | [Nodejs](http://nodejs.org/) |
| Python          | >=3.5    | `python --version`  | [Python](https://www.python.org/) |
| Npm             | indiferente | `npm --version`     | **Nodejs** contains **Npm** |
| Gulp            | >=4.0.0  | `gulp -v`           | [Gulp](http://gulpjs.com/) |

> Veja a documentação de cada requerimento para a instalação.

### Instalando

Após instalar todos requerimentos acima, faça os comando abaixo:

1 - Faz o clone do **Go!Sync Pug** e acesse a pasta:

~~~
$ git clone https://github.com/williamcanin/gosync-pug.git "mysite"; cd mysite
~~~

* 2 - Instalando as dependências do **Go!Sync Pug**:

~~~
$ npm install
~~~

### Compilando

* Use o comando abaixo para compilar seu projeto:

~~~
$ gulp build
~~~

ou

~~~
$ $(npm bin)/gulp build
~~~

Nota: Seu site irá ser compilado na pasta `public`.

### Iniciando servidor local

* O comando abaixo você inicia um servidor local com o [Browser Sync](https://www.browsersync.io) (para desenvolvimento):

~~~
$ gulp serve
~~~

ou

~~~
$ $(npm bin)/gulp serve
~~~

> Nota 1: Para obter mais tarefas do gulp, use `gulp --tasks`.
> Nota 2: Não há necessidade de compilar e, em seguida, iniciar o servidor.

### Desenvolvimento

* 1 - Você deve criar toda estrutura de layout e includes do seu projeto no diretório `src/templates` utilizando [Pug](http://pugjs.org).

* 2 - A pasta `src/views` é onde você deve criar suas páginas, que terá includes, extends e blocks
através das pastas `src/templates/includes` and `src/templates/layouts`.

* 3 - Antes de hospedar seu projeto no servidor, altere no arquivo `config.json` o valor de `url`, colocando a url do seu site. Após isso, você pode executar o comando `gulp build` e hospedar em um servidor na web.

### Doação

Se você gostou do meu trabalho, me compre um café <3

[![paypal](https://www.paypalobjects.com/pt_BR/BR/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=C4EEL62SFHZS4&source=url)

### Licença

[MIT License](https://opensource.org/licenses/MIT) © William Canin
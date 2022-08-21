# Projeto e-commerce gerado com [Angular CLI](https://github.com/angular/angular-cli) versão 14.1.2.

## Deploy - GitHub Pages [(Link do projeto)](https://sdeoliveira-r.github.io/e-commerce)

### Desenvolvimento

- 1> $ ng new e-commerce
- 2> $ cd e-commerce
- 3> $ npm start
  - Obs.: Abra outro terminal para criar o component header dentro do module app, e também para, posteriormente criar novos components, modules, etc. 
- 4> $ ng g c header --module app
* 5> Utilizando a biblioteca para ícones [Font Awesome](https://fontawesome.com/)
     - Etapas: cadastro + email + senha + acessar meus kit's + copiar o script Kit Code + colar o script Kit Code no index.html dentro da tag head
- 6> $ ng g component footer --module app
- 7> $ ng g module app-routing --flat --module app.module
- 8> $ ng g module produtos --route produtos --module app.module
- 9> $ ng g component nao-encontrada
- 10> $ ng g component produtos/detalhes-produto --module produtos.module
- 11> $ ng g service produtos
* 12> Utilizando a biblioteca [Angular Material](https://material.angular.io/guide/getting-started) 
  - Exemplo: Utilizando a Components - [Snackbar](https://material.angular.io/components/snack-bar/overview)
  - Instalar: $ ng add @angular/material
  - Stop server: Ctrl+c - Start server: $ ng serve --open
  - Importe dentro de app.module: import { MatSnackBarModule } from "@angular/material/snack-bar" e, aplicar em imports: MatSnackBarModule
- 13> $ ng g service notificacao
- 14> $ ng generate service carrinho
- 15> $ ng g module carrinho --route carrinho --module app.module
- 16> $ ng g module contato --route contato --module app.module
* 17> Utilizando a biblioteca [npmjs](https://www.npmjs.com/)
  - Exemplo: Utilizando o package [ngx-mask](https://www.npmjs.com/package/ngx-mask) 
  - Instalar: $ npm install --save ngx-mask
  - Importe dentro de app.module: import { NgxMaskModule, IConfig } from 'ngx-mask' e, aplicar em imports: NgxMaskModule.forRoot()
  - Aplicar a máscara em contato.component.html: mask="(00) 0 0000-0000"
- 18> $ ng g component barra-pesquisa
* 19> Building do projeto
  - Para gerar os arquivos de build acesse a src do projeto, entre no arquivo {} angular.json e adicione em outputPath a pasta docs: "outputPath": "docs" (ou utilize a flag --output-path docs no final do comando a seguir).
  - 20> $ ng build --base-href="https://sdeoliveira-r.github.io/e-commerce/"
  - 21> Instalar o Git, fazer as configurações iniciais do Git e fazer o deploy com GitHub Pages.

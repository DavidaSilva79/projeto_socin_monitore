
<p align="center"> 
      <img src="https://avatars.githubusercontent.com/u/48964967?v=4 width="350px" height="400px"/>
      <img src="https://static.wixstatic.com/media/b62a2d_c2df19675c714549aaa69b335bf37e13~mv2.png/v1/fill/w_188,h_188,al_c,q_85,usm_0.66_1.00_0.01/monitec_2.webp" alt="monitec_2.png" style="width: 94px; height: 94px; object-fit: cover; object-position: 50% 50%;">  
     
                                                                                                                                                 
<p align="center"> 

## 💻 Monitec
                 
O monitec é uma plataforma de monitoramento de funções e equipamentos de tecnologia que busca ampliar a visão de gestores de TI sobre o sistema e suas funcionalidades, oferecendo métricas para a tomada de decisão.
                 
Com um design baseado nas melhores práticas de UX fornece dados em tempo real para a análise da performance, ações preventivas, conexões e comunicações, entre outros. O monitec pode monitorar os seguintes itens.
                 
                 
<strong>Carga:</strong> Acompanhamento de fluxo de carga do PDV.

<strong>Hardware:</strong>  Gerenciamento funcional de Hardware.

<strong>Integrações:</strong> Controle e acompanhamento das integrações. 

<strong>Movimento:</strong> Follow Up e Gerenciamento de vendas.

<strong>NFCE:</strong> Controle e monitoramento de cupons fiscais.
                 
<strong>SAT:</strong> Controle e monitoramento de de cupons fiscais.
                 
<strong>Serviços:</strong> Gestão de dados online. 
                 
<strong>Versões:</strong> Releases, concentrador, matriz, pdvs  módulos. 
                 

## Tópicos

- [Tecnologias](#-Tecnologias)
- [Como executar o monitec](#-Como-executar-o-monitec)
- [Features](#-Features)
- [Contribuidores](#-Contribuidores)
- [Autor](#-Autor)
- [Licença](#-Licença)

## 🛠 Tecnologias

As seguintes ferramentas foram usadas na construção do projeto:
                 


<ul> 
  <li><a href="https://www.typescriptlang.org/">
    <img src="https://img.shields.io/badge/TypeScript_3.5.3-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="typescript">
  </a></li>
  <li><a href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript">
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="javascript">
  </a> </li>
  <li><a href="https://spring.io/projects/spring-boot">
    <img src="https://img.shields.io/badge/HTML5-E34F26?&style=for-the-badge&logo=html5&logoColor=white" alt="spring-boot">
  </a></li>
  <li><a href="https://sass-lang.com/">
    <img src="https://img.shields.io/badge/Sass-CC6699?&style=for-the-badge&logo=sass&logoColor=white" alt="sass">
  </a></li>                                                                                                                      
  <li><a href="https://angular.io/">
    <img src="https://img.shields.io/badge/AngularJS_8.2.13-E23237?&style=for-the-badge&logo=angular&logoColor=white" alt="angular">
  </a></li> 
  <li><a href="https://nodejs.org/en/">
    <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="node">
  </a></li> 
  <li><a href="https://www.npmjs.com/">
    <img src="https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white" alt="npm">
  </a></li>                                                                                                                          
 </ul>                                                                                                                                           


## 🚀 Como executar o monitec.
                                                                                                             
### Pré-requisitos

Antes de começar, você vai precisar ter instalado em sua máquina o e-conect o que inclui(Java JDK 1.8, MySQL 5.7, FTP e SSH, Mavem), além disto é bom ter um editor para trabalhar com o código como Eclipse e VScode ou Sublime.


### 🎲 Executando o monitec

                                                                                                                 
1. Instale o Node.js
Node.js é um ambiente de servidor de código aberto que usa JavaScript no servidor.
 
  ```curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -```
                                                                                                                 
  ```sudo apt-get install -y nodejs```   
                                                                                                              
2. Atualizar NPM
Normalmente, o NPM será instalado com o próprio Node.js. No entanto, podemos atualizá-lo para a versão mais recente usando o comando abaixo.

```sudo npm install npm@latest -g```                                                      
                                                                                                                 
3. Instale o Angular CLI    
                                                                                                                 
```sudo npm install -g @angular/cli```
                                                                                                             
4. Subindo o serviço web manager

No endereço `https://github.com/socin-econect/monitec/releases/` escolher uma versão do arquivo monitec_versao_.zip baixar e descompactar o mesmo ,abrir o arquivo `conf/SQLAPIDataSource.properties` configurar a conexão com sua base de dados. Em seguida executar o arquivo web-manager.jar no terminal com comando o `java -jar web-manager.jar`.
                                                                                                             
5. Development server
                                                                                                             
Dentro da raiz do projeto monitec no terminal rode o comando `ng serve` para subir o servidor de desenvolvimento. Navegue ate o endereço `http://localhost:4200/`.Caso algum arquivo do condigo fonte for alterado a aplicação ira recarregar automaticamente.

Caso na hora de subir no terminal der algumas exceptions executar os comandos `npm install --save-dev @angular-devkit/build-angular`
`npm install`
`ng serve -o`
                                                                                                             
Na tela de acesso do monitec ir ate a engrenagem de configuração no canto superior direito e trocar a url para `http://localhost:9999/`.

### 🎁 Geração de artefatos do monitec                                                                                                            

6. Build

Para rodar a build e gerar os artefatos do projeto no terminal use o comando `ng build`. Os artefatos gerados são encontrados no diretório `dist/` do projeto monitec. Para uma build de produção use a flag `--prod`em seguida do comando `ng build`.

Os artefatos gerados devem ser copiados para o diretório webapp do projeto do serviço baixado na sessão 4 deste tutorial.
                                                                                                            
<h3>Testes unitários</h3>

No terminal execute o comando `ng test` para executar testes unitários via [Karma](https://karma-runner.github.io).

<h3>Testes end-to-end</h3>
                                                                                                             
No terminal execute o comando `ng e2e` para executar testes end-to-end via [Protractor](http://www.protractortest.org/).
                                                                                                             
<h3>Code scaffolding</h3>
                                                                                                             
Execute no terminal o comando `ng generate component component-name` para gerar um novo componente. Você também pode usar o comando `ng generate directive|pipe|service|class|guard|interface|enum|module`.                                                                                                             
<h3>Para mais ajuda</h3>
                                                                                                             
Para obter mais ajuda sobre o uso do Angular CLI no terminal digite `ng help` ou acesse [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).                                                                                                            

## 💫 Features

O conteúdo referente as features do monitec se encontra no local  do link abaixo.

https://socincompany.atlassian.net/wiki/spaces/E

## 😃 Autor

<p align="center"> 
   <a href="https://www.socin.com.br/">
      <img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/48964967?v=4" width="100px;" alt="socin"/>
   </a>
</p>
<p align="center"> 
      <sub><b>Socin Sistemas</b></sub></a> <a href="https://www.socin.com.br/" title="Socin">🚀</a>
<p align="center"> 
 Feito com ❤️  pela equipe de desenvolvimento Socin Sistemas!
</p>
<p align="center"> 
 <a href="https://www.facebook.com/socinsistemas"><img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook"></a>
<a href="https://www.linkedin.com/company/socinsistemas/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="Linkedin"></a>
<a href="https://www.instagram.com/socinsistemas/?hl=pt-br"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram"></a> 
</p>

## 📝 Licença

🚧 Em construção... 🚧


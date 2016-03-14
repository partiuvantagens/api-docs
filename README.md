# Partiu API! Docs

[![Build Status](https://travis-ci.org/partiuvantagens/api-docs.svg?branch=master)](https://travis-ci.org/partiuvantagens/api-docs)
[![NPM version](https://badge.fury.io/js/swagger-ui.png)](http://badge.fury.io/js/swagger-ui)

[![Dependency Status](https://david-dm.org/partiuvantagens/api-docs/status.svg)](https://david-dm.org/partiuvantagens/api-docs)
[![devDependency Status](https://david-dm.org/partiuvantagens/api-docs/dev-status.svg)](https://david-dm.org/partiuvantagens/api-docs#info=devDependencies)


Este repositório é usado para gerar e publicar a interface web da Partiu API.

URL pública temporária: [https://partiuvantagens.github.io/api-docs/dist](https://partiuvantagens.github.io/api-docs/dist/)

## Vagrant

Inicie a máquina virtual:

```
vagrant up
```

Efetue o acesso via SSH:

```
vagrant ssh
```

Dentro da márquina virtual, o diretório `/vagrant` contém os dados do projeto api-docs:

```
cd /vagrant
```

Para desligar a máquina virtual, utilize o comando abaixo:

```
vagrant halt
```

## Desenvolvimento
Todas as alterações devem ser realizadas no diretório `src` e compiladas com o comando `build`:

```
npm run-script build
```
As páginas e assets serão gerados no diretório `dist` do projeto e deverão ser enviadas ao controle de versão.

Você poderá editar os arquivos do projeto em sua própria máquina (host), porém o comando `build` deverá ser executado dentro da máquina virtual.

## Deploy
Estratégia para deploy de um subdiretório no GitHub Pages (ver [http://yeoman.io/learning/deployment.html](http://yeoman.io/learning/deployment.html))

```
git subtree push --prefix dist origin gh-pages
git push
```

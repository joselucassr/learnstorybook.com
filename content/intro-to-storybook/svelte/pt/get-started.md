---
title: 'Tutorial de Storybook para Svelte'
tocTitle: 'Começado'
description: 'Configure o Storybook em seu ambiente de desenvolvimento'
---

Storybook é executado junto a sua aplicação em modo de desenvolvimento. Ele ajuda a construir componentes de interface de usuário isolados da lógica e contexto de sua aplicação. Esta edição de tutorial da Introdução ao Storybook é para Svelte; outras edições existem para [Vue](/intro-to-storybook/vue/pt/get-started), [Angular](/intro-to-storybook/angular/pt/get-started), [React](/intro-to-storybook/react/pt/get-started), [React Native (EN-US)](/intro-to-storybook/react-native/en/get-started) e [Ember (EN-US)](/intro-to-storybook/ember/en/get-started).

![Storybook and your app](/intro-to-storybook/storybook-relationship.jpg)

## Configurando Storybook com Svelte

Precisaremos seguir alguns passos para ter o processo de build configurado em nosso ambiente. Para começar, usaremos [degit](https://github.com/Rich-Harris/degit) para configurar nosso sistema de build. Usando este pacote, você pode baixar "templates" (aplicações parcialmente construídas com algumas configurações padrão) para te ajudar a acelerar seu processo de desenvolvimento.

Rodaremos os seguintes comandos:

```bash
# Criar nossa aplicação:
npx degit chromaui/intro-storybook-svelte-template taskbox

cd taskbox

# Instalar dependências
yarn
```

<div class="aside">
💡 Este template contem os estilos e arquivos adicionais necessários, além das configurações mais fundamentais para esta versão do tutorial. 
</div>

Agora podemos checar rapidamente que os vários ambientes de nossa aplicação estão funcionando corretamente:

```bash
# Roda os testes (Jest) em um terminal:
yarn test

# Roda o explorador de componentes na porta 6006:
yarn storybook

# Roda o aplicativo frontend:
yarn dev
```

Nossas três modalidades de aplicativo frontend: testes automatizados (Jest), desenvolvimento de componentes (Storybook), e o próprio aplicativo.

![3 modalities](/intro-to-storybook/app-three-modalities-svelte.png)

Dependendo de qual parte do aplicativo você estiver trabalhando, você pode querer rodar um ou mais desses comandos simultaneamente. Como nosso foco atual é criar um único componente de interface de usuário, rodaremos somente o Storybook por enquanto.

## Efetuando commit nas mudanças

Agora é seguro adicionar nossos arquivos a um repositório local. Rode os seguintes comandos para inicializar um repositório local, adicionar e efetuar commit nas mudanças que realizamos até o momento.

```shell
$ git init
```

Seguido de:

```shell
$ git add .
```

Depois:

```shell
$ git commit -m "first commit"
```

E por fim:

```shell
$ git branch -M main
```

Vamos começar a construir nosso primeiro componente!

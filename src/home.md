---
cover: .gitbook/assets/cdd2be42-4bfb-40ea-aa19-b046eff15378.jpeg
coverY: -4.149292149292149
---

# Boas-vindas!

### aoi.js

**Boas-vindas a documentação do Aoi.js**

### Introdução

![](https://aoi.js.org/assets/images/aoijs-new.png)

[![Servidor no Discord](https://img.shields.io/discord/773352845738115102?color=5865F2\&logo=discord\&logoColor=white)](https://aoi.js.org/invite) [![Versão NPM](https://img.shields.io/npm/v/aoi.js.svg?maxAge=3600)](https://www.npmjs.com/package/aoi.js) [![NPM Downloads](https://img.shields.io/npm/dt/aoi.js.svg?maxAge=3600)](https://www.npmjs.com/package/aoi.js)

#### Sobre nós

_**Aoi.JS é um pacote com funções simplificadas e prontas para uso para que os desenvolvedores do Discord desenvolvam seus próprios Bots.**_

_**Visando um aprendizado rápido e fácil**._ _**É rapido e flexível usando funções.**_

_**É um pacote open-source para a comunidade ♥️**_

### Instalação

**É necessário o Node.JS 16.6.0 ou mais recente.**

```sh-session
npm install aoi.js
```

### Configurando

```javascript
const aoijs = require("aoi.js")

const bot = new aoijs.Bot({
token: "TOKEN DO BOT",
prefix: "PREFIXO DO BOT",
intents: ["GUILDS", "GUILD_MESSAGES"]
})

//Eventos
bot.onMessage()

//Exemplo de Comando (ping)
bot.command({
name: "ping",
code: `Pong! $pingms`
})

//Evento Ready
bot.readyCommand({
    channel: "",
    code: `$log[Ready on $userTag[$clientID]]`
})
```

### Links úteis

* [Website](https://aoi.js.org)
* [NPM](https://www.npmjs.com/package/aoi.js)
* [Github](https://github.com/AkaruiDevelopment/aoi.js)
* [Discord Server](https://discord.gg/HMUfMXDQsV)
* [Documentação](https://akarui.leref.ga/v/aoi.js/)

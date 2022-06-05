# Raph Cosmo
## A custom theme for [discord-easy-dashboard](https://github.com/SimonLeclere/discord-easy-dashboard)

### Installing

```js
npm i discord-easy-dashboard raphcosmo
```

### Usage

To get started using the [discord-easy-dashboard](https://github.com/SimonLeclere/discord-easy-dashboard) package read the docs by clicking [here](https://github.com/SimonLeclere/discord-easy-dashboard/blob/master/docs/gettingStarted.md)

To get started using my custom theme into this package use the following code or learn more at the [theming guide](https://github.com/SimonLeclere/discord-easy-dashboard/blob/master/docs/THEMING.md) on the discord-easy-dashboard docs.

```js
const { Client, Intents } = require('discord.js');
const Dashboard = require('discord-easy-dashboard');
const RaphCosmoTheme = require('raphcosmo')

const client = new Client({ intents: [Intents.FLAGS.GUILDS, Intents.FLAGS.GUILD_MESSAGES] });

client.dashboard = new Dashboard(client, {
    name: 'RaphXSimon',
    description: 'A cool bot with a custom dashboard',
    baseUrl: 'http://localhost',
    port: 80,
    noPortIncallbackUrl: false,
    secret: '12345-SECRET-12345',
    theme: RaphCosmoTheme
});

client.login('12345-TOKEN-12345')
```

## Credits

Simon - Creator of [discord-easy-dashboard](https://github.com/SimonLeclere/discord-easy-dashboard) - View his github [here](https://github.com/SimonLeclere)

Raphael - Creator of [Raph Cosmo](https://npmjs.com/package/raphcosmo) - View his github [here](https://github.com/raph-exe)

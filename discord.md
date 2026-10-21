# Documentació del Bot de Discord

![Logotip de Discord](https://brandlogos.net/wp-content/uploads/2018/10/discord_icon_2015-2021-logo_brandlogos.net_buedx.png)

Pots registrar la teva aplicació al [Portal de Desenvolupadors de Discord](https://discord.com/developers/applications).

Per fer que el bot respongui, escoltem l'esdeveniment `messageCreate` i utilitzem el mètode `message.reply()`

```javascript
client.on('messageCreate', message => {
   if (message.content === 'ping') {
        message.reply('pong!');
    }
});
```
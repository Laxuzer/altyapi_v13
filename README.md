# DJS v13 Altyapı

- **Soru/İstek/Şikayet** ve __daha fazlası__ için [Discord Sunucum](https://discord.gg/VUNbq4SwxY) `Laxuzer#5643`

- Slash uyumlu olmayan v13 altyapı.

- Botu çalıştırmadan önce [`config.json`](src/config.json)'u doldurmalısınız.

# Ctx Info
Tek bir parametre ile `herşeye` erişim sağlayabilirsiniz.
- Ctx
    - [Client](src/base/Client.js#L3) ([Discord.Client](https://discord.js.org/#/docs/main/stable/class/Client))
        - [CommandHandler](src/base/CommandHandler.js#L4)
        - [ErrorHandler](src/base/ErrorHandler.js#L3)
        - [logger](src/base/Logger.js#L22)
        - [Emoji](src/base/Emoji.js#L3)
        - db `(LowDB)`
        - [config](src/config.json)
    - [Message](src/base/Ctx.js#L52) ([Discord.Message](https://discord.js.org/#/docs/main/stable/class/Message))
    - [Channel](src/base/Ctx.js#L57) ([Discord.Channel](https://discord.js.org/#/docs/main/stable/class/Channel))
    - [Guild](src/base/Ctx.js#L62) ([Discord.Guild](https://discord.js.org/#/docs/main/stable/class/Guild))
    - [Me](src/base/Ctx.js#L67) (Client [Discord.GuildMember](https://discord.js.org/#/docs/main/stable/class/GuildMember))
    - [Author](src/base/Ctx.js#L77) ([Discord.User](https://discord.js.org/#/docs/main/stable/class/User))
    - [Member](src/base/Ctx.js#L82) ([Discord.GuildMember](https://discord.js.org/#/docs/main/stable/class/GuildMember))
    - [Input](src/base/Ctx.js#L4)
        - Prefix
        - Flags `(-- ile başlayanlar --full gibi)`
        - Args `(Temiz Argümanlar)`
        - fullArgs `(Bütün Argümanlar)`
        - Content
        - cleanContent

# Client Info
- [`Client.js`](src/base/Client.js) dosyasında class adını **botunuzun adıyla** değiştirebilirsiniz.
- Client özel olduğu için kod yazarken size rahatlık sağlayacaktır.

# Command Info
- `src/commands/kategori/komutadı.js` gibi koymanız gerekmektedir. 
- Komutlar [`class`](https://www.w3schools.com/js/js_classes.asp) dır. 
- Örnek komut olarak [`eval`](src/commands/dev/eval.js) komutu koydum inceleyebilirsiniz. 
- Ayrıca [`Command.js`](src/base/Command.js) dosyasına giderek oradan detaylı inceleyebilirsiniz.

# Event Info
- Eventler [`class`](https://www.w3schools.com/js/js_classes.asp) dır. 
- [`ready.js`](src/events/ready.js) ve [`message.js`](src/events/message.js) yi örnek olarak koydum inceleyebilirsiniz.

# Function Handler
- `src/handlers/manual/functionHandler.js` dosyasında hazır functionlar bulunmaktadır.
- Functionlara dilerseniz `ekleme` yapabilir veya `çıkarabilirsiniz`.

-- [Laxuzer#0480](https://discord.com/users/576749207084466197)

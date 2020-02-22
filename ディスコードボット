import discord

client = discord.Client()

@client.event
async def on_ready():
    print('Logged in as')
    print('client.user.name')
    print('client.user.id')
    print('------')

@client.event
async def on_message(message):
    #「おはよう」に答える
    if message.content.startswith("おはよう"):
        #送り主がBotだった場合反応したくないので
        if client.user != message.author:
            #メッセージを書きます
            m = "おはようございます。" + message.author.name + "さん！\n 今日も一日がんばりましょう！"
            #メッセージが送られてきたチャンエルへメッセージを送ります
            await message.channel.send(m)

    #「おやすみ」に答える
    if message.content.startswith("おやすみ"):
        #送り主がBotだった場合反応したくないので
        if client.user != message.author:
            #メッセージを書きます
            m = "おやすみなさい" + message.author.name + "さん。\nいい夢見てね。"
            #メッセージが送られてきたチャンエルへメッセージを送ります
            await message.channel.send(m)



client.run("NjgwNzYzNzgwNDE3ODQ3Mzc2.XlEo1g.vYrNBidKNeHJHDxitfW3l5i4rJw")

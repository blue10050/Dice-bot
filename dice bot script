import discord
import random

client = discord.Client()


@client.event
async def on_ready():
    print("봇이 성공적으로 실행되었습니다")
    game = discord.Game('name')
    await client.change_presence(status=discord.Status.online, activity=game)


@client.event
async def on_message(message):
    if message.content.startswith('!주사위'):
        randomNum = random.randrange(1, 7)
        if randomNum == 1:
            await message.channel.send(embed=discord.Embed(description=':one:', color=0x7C40E5))
        if randomNum == 2:
            await message.channel.send(embed=discord.Embed(description=':two:', color=0x7C40E5))
        if randomNum == 3:
            await message.channel.send(embed=discord.Embed(description=':three:', color=0x7C40E5))
        if randomNum == 4:
            await message.channel.send(embed=discord.Embed(description=':four:', color=0x7C40E5))
        if randomNum == 5:
            await message.channel.send(embed=discord.Embed(description=':five:', color=0x7C40E5))
        if randomNum == 6:
            await message.channel.send(embed=discord.Embed(description=':six: ', color=0x7C40E5))
        
client.run('your bot token')

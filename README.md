import discord
from discord.ext import commands
intents = discord.Intents.default()
intents.message_content = True
bot = commands.Bot(command_prefix='$', intents=intents)

@bot.command()
async def yardım (ctx):
    await ctx.send(f'eğerÇevreye önem veren ve çevre dostu uygulamalar ve atıkları azaltmanın yolları hakkında daha fazla bilgi edinmek isteyen kişilerden misin !O zaman $bilgi yaz!')

@bot.command()
async def bilgi(ctx):
    await ctx.send(f'şimdi iki seçenek var $1 yazarsan buradan bilgi veririm $2 yazarsan seni web sitesine atarım(uras dan ilham aldım)')

@bot.command()
async def bir (ctx):
    await ctx.send(f'vay kral beni seçti!neyse konumuza geri dönelim.bunun için birinci yöntem kodland dan phyton pro kursunu alıp discorttan benim gibi bilgi alıp verebilirsin.ikinci ise geri dönüşüm kutuları kullanabilirsin ')

@bot.command()
async def iki (ctx):
    await ctx.send(f'https://www.akdenizkoruma.org.tr/tr/calismalarimiz/iklim-krizi/b/sulak-alanlar?gad_source=1&gclid=CjwKCAjwkJm0BhBxEiwAwT1AXO9r0sK9lb6VCkLlXiSumPb7PEy5Wi3SWgw7LdHp8F-8ooCzBuTOnRoCtVgQAvD_BwE')

bot.run("")

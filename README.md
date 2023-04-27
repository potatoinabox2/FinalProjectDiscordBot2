# a Discord bot with the capabilities to pull up the current standard legal set for the Pokémon Trading Card Game

import discord
from discord.ext import commands

intents = discord.Intents().all()
bot = commands.Bot(command_prefix="!", intents=intents, case_insensitive=True)
bot.remove_command('help')

@bot.command()
async def SVI(ctx):
  embed = discord.Embed(title="Scarlet & Violet Base Set", description="SVI: [Click here to redirect](https://pkmncards.com/set/scarlet-violet/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def SVP(ctx):
  embed = discord.Embed(title="Scarlet & Violet Promos", description="SVP: [Click here to redirect](https://pkmncards.com/set/scarlet-violet-promos/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def BST(ctx):
  embed = discord.Embed(title="Sword & Shield: Batlle Styles", description="BST: [Click here to redirect](https://pkmncards.com/set/battle-styles/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def CRE(ctx):
  embed = discord.Embed(title="Sword & Shield: Chilling Reign", description="CRE: [Click here to redirect](https://pkmncards.com/set/chilling-reign/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def EVS(ctx):
  embed = discord.Embed(title="Sword & Shield: Evolving Skies", description="EVS: [Click here to redirect](https://pkmncards.com/set/evolving-skies/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def CEL(ctx):
  embed = discord.Embed(title="Celebrations", description="CEL: [Click here to redirect](https://pkmncards.com/set/celebrations/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def FST(ctx):
  embed = discord.Embed(title="Sword & Shield: Fusion Strike", description="FST: [Click here to redirect](https://pkmncards.com/set/fusion-strike/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def BRS(ctx):
  embed = discord.Embed(title="Sword & Shield: Brilliant Stars", description="BRS: [Click here to redirect](https://pkmncards.com/set/brilliant-stars/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def ASR(ctx):
  embed = discord.Embed(title="Sword & Shield: Astral Radiance", description="ASR: [Click here to redirect](https://pkmncards.com/set/astral-radiance/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def PGO(ctx):
  embed = discord.Embed(title="Pokemon Go", description="PGO: [Click here to redirect](https://pkmncards.com/set/pokemon-go/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def LOR(ctx):
  embed = discord.Embed(title="Sword & Shield: Lost Origin", description="LOR: [Click here to redirect](https://pkmncards.com/set/lost-origin/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def SIT(ctx):
  embed = discord.Embed(title="Sword & Shield: Silver Tempest", description="SIT: [Click here to redirect](https://pkmncards.com/set/silver-tempest/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def CRZ(ctx):
  embed = discord.Embed(title="Sword & Shield: Crown Zenith", description="CRZ: [Click here to redirect](https://pkmncards.com/set/crown-zenith/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)

@bot.command()
async def SWSHP(ctx):
  embed = discord.Embed(title="Sword & Shield Promos", description="SWSHP: [Click here to redirect](https://pkmncards.com/set/sword-shield-promos/)", color=discord.Color.blue())
  await ctx.channel.send(embed=embed)


bot.run("TOKEN")

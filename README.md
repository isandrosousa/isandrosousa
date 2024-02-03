token = 'SEU_TOKEN'
prefixo = '!'

# Criação do bot
bot = commands.Bot(command_prefix=prefixo)

# Comando simples
@bot.command(name='oi', help='Cumprimenta o usuário')
async def oi(ctx):
    await ctx.send(f'Oi, {ctx.author.mention}!')

# Evento de inicialização
@bot.event
async def on_ready():
    print(f'Bot conectado como {lisboa rp}')

# Execução do bot
bot.run(token)

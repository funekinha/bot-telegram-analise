# README - Deploy Bot Telegram de Análise

## 1. Criar conta no GitHub e subir o repositório

- Crie uma conta grátis em https://github.com
- Crie um novo repositório público (ex: bot-telegram-analise)
- Faça upload dos arquivos: bot.py, requirements.txt, Dockerfile, README.txt
- Faça commit e confirme que os arquivos estão no repositório

## 2. Criar conta no Koyeb e configurar deploy

- Acesse https://app.koyeb.com e crie uma conta grátis
- Clique em Create Service
- Escolha GitHub e conecte sua conta GitHub ao Koyeb
- Selecione o repositório que você criou no GitHub (bot-telegram-analise)
- Configure para construir via Dockerfile
- Configure a porta do serviço para 8080
- Adicione uma variável de ambiente:
  - Nome: TELEGRAM_TOKEN
  - Valor: seu token do BotFather do Telegram (exemplo: 123456789:ABCDefGhIjkLMNopQRstUVwxyZ)
- Clique em Deploy

## 3. Manter o bot ativo (UptimeRobot)

- Acesse https://uptimerobot.com e crie uma conta grátis
- Crie um novo monitor HTTP, apontando para o endereço do seu serviço no Koyeb (exemplo: https://seuservico.koyeb.app/)
- Configure para verificar a cada 5 minutos
- Isso mantém o bot online e evita que ele entre em modo suspenso

## 4. Usar o bot

- No Telegram, abra uma conversa com seu bot (busque pelo username que você configurou)
- Primeiro envie o timeframe: 1m, 5m ou 15m
- Depois envie a foto do gráfico (print da IQ Option)
- Aguarde a resposta com a análise da direção do mercado e tempo estimado


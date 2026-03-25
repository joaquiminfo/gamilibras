# 🤟 LIBRAS Quest

Jogo de gamificação para aprender **Língua Brasileira de Sinais (LIBRAS)** com sistema de XP, níveis, badges e muito mais!

## ✨ Funcionalidades

- 🎯 **8 categorias**: Alfabeto, Números, Cumprimentos, Família, Cores, Animais, Comida, Emoções
- ⚡ **Sistema de XP** com 7 níveis (Aprendiz → Mestre)
- ❤️ **Sistema de vidas** (5 corações por sessão)
- 🔥 **Combo multiplier** — acerte em sequência para ganhar bônus
- 🏆 **10 badges** desbloqueáveis
- 📊 **Streak diário** para manter o hábito
- 💾 **Progresso salvo** no navegador (localStorage)
- 🎊 **Confetti e animações** nas conquistas

## 🚀 Deploy na Vercel

### Opção 1 — Interface Web (mais fácil)

1. Crie uma conta em [vercel.com](https://vercel.com)
2. Faça upload da pasta do projeto ou conecte ao GitHub
3. Vercel detecta automaticamente Vite → clique **Deploy**
4. Pronto! Link público gerado em segundos ✅

### Opção 2 — CLI

```bash
npm install -g vercel
cd libras-game
npm install
vercel
```

### Opção 3 — GitHub + Vercel (CI/CD automático)

```bash
git init
git add .
git commit -m "feat: LIBRAS Quest inicial"
git remote add origin https://github.com/SEU_USER/libras-game.git
git push -u origin main
```
Depois conecte o repositório na dashboard da Vercel.

## 💻 Rodar Localmente

```bash
npm install
npm run dev
```

## 🏗️ Build de Produção

```bash
npm run build    # gera a pasta /dist
npm run preview  # visualiza o build localmente
```

## 📁 Estrutura

```
libras-game/
├── src/
│   ├── components/
│   │   ├── Home.jsx        # Tela principal / dashboard
│   │   ├── Quiz.jsx        # Tela de jogo / questões
│   │   ├── Profile.jsx     # Perfil, badges, níveis
│   │   ├── XPBar.jsx       # Barra de experiência
│   │   ├── Hearts.jsx      # Corações / vidas
│   │   ├── BadgeToast.jsx  # Notificação de badge
│   │   └── Confetti.jsx    # Efeito de confete
│   ├── data.js             # Sinais, categorias, badges
│   ├── useGameState.js     # Lógica de estado do jogo
│   ├── App.jsx             # Roteamento principal
│   ├── main.jsx            # Entry point
│   └── index.css           # Estilos globais + animações
├── index.html
├── vite.config.js
├── vercel.json
└── package.json
```

## 🎨 Tecnologias

- **React 18** + **Vite** (sem TypeScript, pronto para Vercel)
- CSS puro com variáveis CSS
- LocalStorage para persistência
- Zero dependências externas de UI

## 📝 Próximas melhorias sugeridas

- [ ] Adicionar GIFs/vídeos reais dos sinais em LIBRAS
- [ ] Modo de revisão de erros
- [ ] Ranking / leaderboard online
- [ ] Sons e áudio
- [ ] Modo dark/light toggle
- [ ] PWA (instalável no celular)

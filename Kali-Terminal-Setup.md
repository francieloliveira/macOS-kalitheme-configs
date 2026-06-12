# Como deixar o Terminal do Mac com a cara do Kali Linux (Passo a Passo Completo)

Se você é pentester, dev ou simplesmente gosta de um terminal bonito e produtivo, este guia é pra você.

## Pré-requisitos
- macOS com zsh
- Conexão com a internet

## Passo 1: Instalar o Oh My Zsh
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Passo 2: Instalar o Tema Kali-Like
```bash
wget -O ~/.oh-my-zsh/themes/kali-like.zsh-theme \
https://raw.githubusercontent.com/clamy54/kali-like-zsh-theme/master/kali-like.zsh-theme
```

## Passo 3: Instalar os Plugins Essenciais
```bash
# Plugin de Autosugestões
git clone https://github.com/zsh-users/zsh-autosuggestions \
${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

# Plugin de Syntax Highlighting
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git \
${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

## Passo 4: Configurar o ~/.zshrc
```bash
nano ~/.zshrc
```

**Substitua ou altere:**
```bash
ZSH_THEME="kali-like"
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
```

Salve com `Ctrl + O` → `Enter` → `Ctrl + X`

## Passo 5: Aplicar as Mudanças
```bash
source ~/.zshrc
```

## Passo 6: Instalar Fonte Nerd Font
Baixe em: [Nerd Fonts](https://www.nerdfonts.com/font-downloads)

Recomendo **MesloLGS NF** ou **FiraCode NF**.

Configure no Terminal → Settings → Text.

## Passo 7: (Opcional) Melhoria de Cores
```bash
# Adicione no final do ~/.zshrc
ZSH_AUTOSUGGEST_HIGHLIGHT_STYLE='fg=green'
```

```bash
source ~/.zshrc
```

**Pronto!** Seu terminal agora tem cara de Kali Linux no Mac. 🔥

#OhMyZsh #KaliLinux #macOS #Terminal #CyberSecurity #Productivity
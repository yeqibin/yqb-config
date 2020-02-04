# yqb-config
Configures for iterm2, Emacs etc.

## Mac下终端设置

### 安装iTerm2

1. iTerm2 -> Make iTerm2 Default Term

2. preference -> Keys -> **Hotkey** Show/hide iTerms2 with a system-wide hotkey

3. 配色选择Solarized-Dark

4. 安装powerline字体

5. 把iTerm2字体设置为Meslo LG M DZ

   ### 安装oh-my-zsh

1. github：https://github.com/robbyrussell/oh-my-zsh

2. vim修改.zshrc文件

   ```
   ZSH_THEME="ys"
   plugins=(git zsh-autosuggestions)
   export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.tuna.tsinghua.edu.cn/homebrew-bottles
   export PATH="/Applications/Julia-1.3.app/Contents/Resources/julia/bin:$PATH"
   ```

3. 安装插件

   ```
   git clone git://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
   vim ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions 
   ```

   增加字体亮度，修改ZSH_AUTOSUGGEST_HIGHLIGHT_STYLE='fg=10' 

4. 语法亮度

   ```
   brew install zsh-syntax-highlighting
   ```

   在.zshrc插入

   ```
   source /usr/local/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
   ```

5. 让更改生效

   ```
   source ~/.zshrc
   ```

   
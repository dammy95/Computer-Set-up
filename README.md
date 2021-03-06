# Computer-Set-up
Set up for new computers to improve efficiency

## iTerm2
Download iTerm2 and set as default terminal

### Colour settings

Foreground: `e78238`

Background: `002833`

Cursor Text: `003541`

## Vim8

### Upgrade to Vim8
`brew install vim --override-system-vim`

### Change .vimrc file
`vim ~/.vimrc`

Paste vimrc.txt contents in .vimrc file

## Power Line

### Install power-line
`sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

### Install power-line fonts
```
    # clone
    git clone https://github.com/powerline/fonts.git --depth=1
    # install
    cd fonts
    ./install.sh
    # clean-up a bit
    cd ..
    rm -rf fonts 
 ```

### Use iTerm2 powerline font in settings
Also remember to change both the default and the non-ASCII font

Font Type: `11pt Meslo LG L Regular for Powerline`

### To remove user@hostname info
`vim ~/.oh-my-zsh/themes/agnoster.zsh-theme`

Uncomment the `prompt context` line in the `build_prompt()` (should be line 220) function and set `PROMPT='$(build_prompt) '`

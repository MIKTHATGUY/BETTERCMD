
# Better CMD

an easy guide to install some plugins to make your cmd look better on windows


# Tools setup

## Scoop Installation
scoop is a tool we will need for the installation of all the other packages if you already have it you can skip this part and go to the 
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

## Git Installation
after installing scoop you probably will have to download Git
```bat
scoop install git
```

# CMD enhancements

## Clink
Clink combines the native Windows shell cmd.exe with the powerful command line editing features of the GNU Readline library, which provides rich completion, history, and line-editing capabilities. Readline is best known for its use in the Unix shell Bash, the standard shell for Mac OS X and many Linux distributions.
### installation
```powershell
scoop install clink
```


## Starship
The minimal, blazing-fast, and infinitely customizable prompt for any shell!
### installation
install a nerdfont from: https://www.nerdfonts.com
```powershell
scoop install starship
echo load(io.popen('starship init cmd'):read("*a"))() >> %LocalAppData%\clink\starship.lua
```


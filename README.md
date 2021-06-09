# neovim-config

#install 
_____________________________-

arch : 
pacman -S neovim


ubuntu :
sudo apt install neovim
_________________________________
#install npm
arch :

sudo pacman -S nodejs npm


ubuntu :
sudo apt install nodejs npm

_______________________________
#config

git clone https://github.com/ms-m-py/neovim-config.git

cd neovim-config

mkdir -p ~/.config/nvim/autoload


curl -fLo ~/.config/nvim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim


pip3 install pynvim flake8 pylint isort jedi pynvim


cp init.vim ~/.config/nvim

nvim +PlugInstall


__________________________________________

#install coc-pyright and ...

run in neovim :

:CocInstall coc-tsserver

:CocInstall coc-json

:CocInstall coc-html

:CocInstall coc-pyright

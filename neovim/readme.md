# NeoVim Installation and Configuration Details
<br/>

- Taken from [Installing Neovim For Ubuntu](https://github.com/neovim/neovim/wiki/Installing-Neovim#ubuntu), open the ubunetu terminal with **CTRL+ALT+t** and run the following command:
```console
foo@bar_your_terimal_screen:~$ sudo apt install neovim
```
<br/>

- If not already present in your system, create the following directory path (recursively) or as needed in your system. Basically, the **nvim** directory is the place where all the configuration files will be placed. Use this command in the Home Directory
```console
foo@bar_your_terimal_screen:~$ mkdir -v -p ./.config/nvim
```
<br/>

- Create a file name **init.vim**. This will have all the basic configurations that will be needed for using neovim. I got this configurataion details from sources like [COC VIM Github Repository](https://github.com/neoclide/coc.nvim), [How to Configure Vim like VSCode](https://www.youtube.com/watch?v=gnupOrSEikQ), [Awesome Neovim Setup From Scratch - Full Guide](https://www.youtube.com/watch?v=JWReY93Vl6g). Copy the contents of the [Vim Init File](https://github.com/sricharankrishnan/config-files/blob/master/neovim/init.vim) of this repository into your local system.

- Save your **init.vim** file with the ```:w``` command. Then open the file again, run ```:PlugInstall``` command. On your screen, you will be able to see the list of plugins that would get installed into your system. Then run the command ```CocConfig```, this will help create a file named **coc-settings.json** file. Copy the contents of [this repo](https://github.com/sricharankrishnan/config-files/blob/master/neovim/coc-settings.json) file into your local system.

- Now you should be ready to use neovim in your system. Please note that neovim will auto format on save. For example, you can run a command like this to work on a typescript file:
```console
foo@bar_your_terimal_screen:~$ nvim functionality.ts
```

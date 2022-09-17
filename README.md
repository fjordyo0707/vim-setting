# vim-setting
My Unix setting

## Command Line Tool
* `Ctrl + u`: clear current line
* `Meta-b / Meta-f` to move backward/forward by a word respectively. 
    * In OSX, Meta translates as ESC, which sucks. But alternatively, you can open terminal preferences -> settings -> profile -> keyboard and check "use option as meta key"
* `Ctrl + a`: move to the front
* `Ctrl + e`: move to the end
* `Ctrl + w`: delete the word

## Vim

#### Comment
1. Go to the first line you want to comment, press **Ctrl+V**. This will put the editor in the **VISUAL BLOCK** mode.
2. Use the arrow key and select until the last line
3. **Shift+I**, which will put the editor in **INSERT mode**
4. Press **//**. This will add a hash to the first line.
5. Press **Esc** (give it a second), and it will insert a **//**  character on all other selected lines.

#### Uncomment
1. Put your cursor on the first **//** character
2. Press **Ctrl+V** (or CtrlQ for gVim), and go down until the last commented 
3. Press **x**, that will delete all the # characters vertically.

#### Search & replace
* **:%s/search_from/replace_to/g**
> 以上 vi 的語法會將檔案內，所有 “search_from” 的字串替換成 “replace_to”。
* **:%s/search_from/replace_to/gc**
> 將上面指令最後加上一個 “c” 字元，可以在取代前，向使用者確認： 
* **:%s/search_from/replace_to/gi**
> 除了可以替換輸入的字串，更可以設定搜尋時，略過英文大小寫的差異，以下對 “search_from” 及 “SEARCH_FROM” 同樣匹配：

#### Copy Paste on WSL
* [vim copy in wsl](https://superuser.com/questions/1291425/windows-subsystem-linux-make-vim-use-the-clipboard)

#### Nerdtree
* ### Usage
```
nmap <F9> :NERDTreeFind<CR><CR>
let NERDTreeWinPos=1
```
1. nmap : 將F9設為開啟nerdtree的快捷鍵
2. NERDTreeWinPos : 將nerdtree區塊放在右邊

* ### Switch to explorer
    * ctrl+shift+e

## Tmux

### TPM
[TPM](https://github.com/tmux-plugins/tpm)

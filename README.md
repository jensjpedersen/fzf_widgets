
# fzf_widgets
A collection of zsh widgets that makes you fly in the terminal. 
These widgets are used for moving to files/directories effectively.   
FZF is used for fuzzy searching.  



## Usage

Copy the `fzf_widgets.zsh` file to your local machine. 

Put the following command in your `.zshrc`: 
```bash
source /PATH-TO-SCRIPT/fzf_widgets.zsh
```


## Keybindings
### Fuzzy search files 
Press `^P` to fuzzy search all files from the current directory (ignoring .git files.)

Press `<Enter>` to select the file. If you command line buffer was empty when
`^P` was pressed. Then, pressing `<Enter>` will open the file specified by the
EDITOR variable (default: nvim) as defined in the Script.

If your command line buffer was not empty when `^P` was pressed. Then pressing
`<Enter>` will paste the file path to your buffer. Quotes will be added to
paths contains space.   

![file](https://user-images.githubusercontent.com/62065926/209685874-cfe52525-c83d-4981-b786-0c8f3acd58b4.gif)

### Fuzzy search directories 
* `^O` - Fuzzy search all directories from current path.  

Pressing `<Enter>` will `cd` into the selected directory only if your command line
buffer initially was empty. If your command line buffer is not empty then
pressing `<Enter>` will paste the directory to the buffer. 

![cd](https://user-images.githubusercontent.com/62065926/209685913-756fd505-4f03-42a4-9157-aad9bf1f0c7e.gif)

### Fuzzy search file content
* `^J` - Fuzzy search content in all files from current directory.  

### Navigation
| Keybinding   | Functionality                      |
|--------------|------------------------------------|
| `^N` or `^J` | Move cursor down                   |
| `^P` or `^K` | Move cursor up                     |
| `^<Space>`   | Toggle preview pane                |
| `^D`         | Move one page down in preview pane |
| `^U`         | Move one page up in preview pane   |



## Requirements
* zsh shell
* fzf, rg, fd, exa, bat



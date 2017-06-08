ColorConsole
============

Colorful console for Mac OS X

## Installation
- You need ```ls``` from the GNU coreutils package (You can install it using ```brew```)
- Copy the ```colors``` file to your home directory
- Rename it to ```colors```
- Edit your ```.profile``` or ```.bash_profile``` file and add the folowing lines

```bash
# Tells bash to use GNU ls instead of BSD ls and enables color usage 
# If you don't have `gls` program on your computer, you should write: alias ls='ls -G'
alias ls='gls --color=always'
# Writes the content from the colors file into the LS_COLORS variable
LS_COLORS=$(cat ~/.colors)
# Makes the variable an environment variable
export LS_COLORS

```

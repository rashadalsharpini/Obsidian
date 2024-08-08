#Linux-Command 

to search for a file you can just write 
`fzf`
if you want to search and preview the file 
```shell
fzf --preview='cat {}'
```
if you want to search and open with nvim
```shell
nvim $(fzf --preview='cat {}')
```

>[!note]
>it eats the processing power while it's running
> Special at the root directory

```shell
alias vf='nvim $(fzf --preview="cat {}")'
```
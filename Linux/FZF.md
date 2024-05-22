#Linux-Command 

to search for a file you can just write 
`fzf`
if you want to search and preview the file 
`fzf --preview='cat {}'`
if you want to search and open with nvim
`nvim $(fzf --preview='cat {}')`

>[!note]
>it eats the process while it's running
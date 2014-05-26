#Code_Complete

This repository is forked from [mbbill/code_complete](https://github.com/mbbill/code_complete)

I have changed something so that it is able to co-exist with YouCompleteMe and
Ultisnips plugins.

Removed all template related code from the original plugin due to we have
ultisnips plugin.

And now, we have `<tab>` to:

1. select what we want from the popup menu
2. trigger code snippets via Ultisnips
3. jump among Ultisnips' blocks
4. function parameters' completion
5. switch among function parameters

###script type
utility

###description
Demo :http://files.myopera.com/mbbill/files/code_complete.gif   

It shows what this script can do.   
In insert mode, when you type `<tab>`(default value of g:completekey) after
function name with a "(" , function parameters will be append behind, use
`<tab>` key again to switch between parameters.

This key is also used to complete code snippets.

###Example:
press `<tab>` after function name and (   
  foo ( `<tab>`   
becomes:   
  foo ( `<first param>`,`<second param>` )   

press `<tab>` after code template   
  if `<tab>`   
becomes:   
  if( `<...>` )   
  {   
      `<...>`   
  }

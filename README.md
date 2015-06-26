nim-mode
===========

An emacs major mode for the Nim programming language.

* [Install Nim](http://nim-lang.org/download.html)
* Install `nim-mode.el` via elpa.

If you want to use `company-mode` for completion, you can setup `nimsuggest` integration. Install `nimsuggest` with `nimble install nimsuggest`. 

Configure integration using the following code:
```el
(require 'company-nim)
(add-to-list 'company-backends 'company-nim)
(add-hook 'nim-mode-hook 'company-mode)

(setq nim-nimsuggest-path "~/.nimble/bin/nimsuggest")
```

If you use `auto-indent-mode` you need to add nim-mode to the list of `auto-indent-multiple-indent-modes`:
```el
(add-to-list 'auto-indent-multiple-indent-modes 'nim-mode)
```

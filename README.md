# nws-query
query [Nachtragswörterbuch des Sanskrit (NWS)](https://nws.uzi.uni-halle.de/) with Emacs and keep a slim backlog of your queries on your local machine.

## Dependencies
- w3m
- [emacs-w3m](https://melpa.org/#/w3m) (available on MELPA)

## Installation
1. Add `nws-query.el` to a directory included in the list `load-path` or modify this list to include the directory with
   `(add-to-list 'load-path "/PATH/TO/nws-query/")` in your init file,
2. add `(require 'nws-search)` to your init-file,
3. (optional) if you wish to keep a local backlog of your queries, set the variable `nws-local` to the directory you wish to keep your backlog in, e.g. `(setq nws-search "~/dictionaries/nws")`.

## Usage
1. Evaluate the main provided function with `M-x nws-search`, browse the opening dictionary frame with w3m-keybindings, close by pressing `q`,
2. if the online service is not accessible you can search your past queries with `M-x nws-search-local`, provided you have set the variable `nws-local` before,
3. (optional) if you are frequently using this function, consider [creating a keybinding](https://www.gnu.org/software/emacs/manual/html_node/elisp/Key-Binding-Commands.html).
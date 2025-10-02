# Emacs Init steps for typescript treesitter support

Adds TS/TSX recipie
``` shell
(progn
  (require 'treesit)
  (setq treesit-language-source-alist
        (append
         '((typescript "https://github.com/tree-sitter/tree-sitter-typescript" "v0.23.2" "typescript/src")
           (tsx        "https://github.com/tree-sitter/tree-sitter-typescript" "v0.23.2" "tsx/src")
           (javascript "https://github.com/tree-sitter/tree-sitter-javascript" "v0.21.2" "src"))
         (or treesit-language-source-alist '())))
  (message "Added TypeScript/TSX/JS recipes to treesit-language-source-alist"))

```

Code formatting for web
``npm install -g prettier``

selection.el
============

Emacs lisp script that allows to interact with clipboard whether its via a terminal or a graphical session of Emacs.

``selection.el`` is compatible with x11 (GNU/Linux, OpenBSD, FreeBSD, etc.) and Mac OS X on both terminal and graphical
environments, and with Windows within a graphical session of Emacs.

requirements
=============

Only under the X Window System as a graphical environment, the ``xclip`` tool is required.

installation and usage
======================
```
$ git clone git@github.com:mota/selection.el ~/.emacs.d/selection
$ cat << EOF >> ~/.emacs
(add-to-list 'load-path "~/emacs.d/selection")
(require 'selection)
(global-set-key (kbd "C-c c") 'copy-to-clipboard)
(global-set-key (kbd "C-c v") 'paste-from-clipboard)
EOF
```

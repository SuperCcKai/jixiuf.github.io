# -*- coding:utf-8 -*-
EMACS?=emacs
recent:
	$(EMACS) -nw  -q -l org-publish.el --eval "(publish-my-note-recent 5)" --eval '(with-current-buffer "*Messages*"(shell-command-on-region (point-min)(point-max) "cat >/tmp/emacs-org-page.log"))' --eval "(kill-emacs)"
	@-cat /tmp/emacs-org-page.log
all:
	$(EMACS) -nw  -q -l org-publish.el --eval "(publish-my-note-all)" --eval '(with-current-buffer "*Messages*"(shell-command-on-region (point-min)(point-max) "cat >/tmp/emacs-org-page.log"))' --eval   "(kill-emacs)"
	@-cat /tmp/emacs-org-page.log

preview:
	$(EMACS) -nw  -q -l org-publish.el --eval "(publish-my-note-local-preview)"
run-emacs:
	$(EMACS) -nw  -q -l org-publish.el

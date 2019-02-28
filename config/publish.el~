;; This buffer is for text that is not saved, and for Lisp evaluation.
;; To create a file, visit it with C-x C-f and enter text in its buffer.

(require 'org-publish)
(setq org-publish-project-alist
      '(

	;; ... add all the components here (see below)...
	("org-notes"
	 :base-directory "~/pavanmishra.github.io/org/"
	 :base-extension "org"
	 :publishing-directory "~/pavanmishra.github.io/"
	 :recursive t
	 :publishing-function org-html-publish-to-html
	 :headline-levels 4             ; Just the default for this project.
	 :auto-preamble t
	 )

	("org-static"
	 :base-directory "~/pavanmishra.github.io/org/"
	 :base-extension "css\\|js\\|png\\|jpg\\|gif\\|pdf\\|mp3\\|ogg\\|swf"
	 :publishing-directory "~/pavanmishra.github.io/"
	 :recursive t
	 :publishing-function org-publish-attachment
	 )

	("org" :components ("org-notes" "org-static"))

	))

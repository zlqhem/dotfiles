# Makefile for vim stuffs
# Author: Jaeho Shin <netj@sparcs.org>
# Created: 2010-08-07

VIMBALL := vim +"source %" +q


.PHONY: all
all: $(shell sed <Makefile -n '/:.*\#\#$$/ s/:.*$$//p')


xmledit: xmledit.vba ##
	$(VIMBALL) $<
xmledit.vba:
	wget -nv -NO $@ \
	    http://www.vim.org/scripts/download_script.php?src_id=13387


mkd: syntax/mkd.vim ##
syntax/mkd.vim:
	mkdir -p $(@D)
	wget -nv -NO $@ --no-check-certificate \
	    https://github.com/plasticboy/vim-markdown/raw/master/mkd.vim

json: syntax/json.vim ##
syntax/json.vim:
	mkdir -p $(@D)
	wget -nv -NO $@ \
	    http://www.vim.org/scripts/download_script.php?src_id=10853

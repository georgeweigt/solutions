.PHONY: default clean

# $* The stem with which an implicit rule matches

# https://www.gnu.org/software/make/manual/html_node/Automatic-Variables.html

%.pdf: %.tex
	pdflatex $*
	rm $*.aux $*.log

default:
	for file in $$(ls *.tex | sed "s/\.tex/\.pdf/") ; do make $$file ; done

# remove TeXShop files

clean:
	rm -f *.aux *.log *.synctex.gz

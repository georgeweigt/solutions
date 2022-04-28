.PHONY: default clean

%.pdf: %.tex
	pdflatex $<

default:
	for file in $$(ls *.tex | sed "s/\.tex/\.pdf/") ; do make $$file ; done
	rm -f *.aux *.log

clean:
	rm -f *.aux *.log *.out *.pdf *.synctex.gz *.toc

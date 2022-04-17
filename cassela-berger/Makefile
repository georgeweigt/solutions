.PHONY: default clean

%.pdf: %.tex
	pdflatex $<

default:
	for file in $$(ls *.tex | sed "s/\.tex/\.pdf/") ; do make $$file ; done
	make clean

clean:
	rm -f *.aux *.log *.out *.synctex.gz *.toc

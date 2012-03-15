
default: main.pdf clean

main.pdf: main.tex bibliografia
	pdflatex main
	pdflatex main

bibliografia: main.bib
	pdflatex main
	bibtex main

clean:
	$(RM) *.aux *.bbl *.blg *.dvi *.log *.toc *.nav *.snm *.out *.vrb


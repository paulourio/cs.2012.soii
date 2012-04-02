MAIN=exercicios
BIB=../referencias.bib

default: bib pdf
	@echo "\033[32;1mOK\033[0m"

pdf: $(MAIN) clean

$(MAIN):
	pdflatex $(MAIN)
	pdflatex $(MAIN)

$(BIB):
	@echo "\033[31;1mArquivo $(BIB) não encontrado\033[0m"
	@false

bib: $(BIB)
	pdflatex $(MAIN)
	bibtex $(MAIN)

distclean: clean
	$(RM) *.pdf

clean:
	$(RM) *.aux
	$(RM) *.bbl
	$(RM) *.blg
	$(RM) *.dat
	$(RM) *.dvi
	$(RM) *.gnuplot
	$(RM) *.log
	$(RM) *.nav
	$(RM) *.out
	$(RM) *.snm
	$(RM) *.toc
	$(RM) *.vrb


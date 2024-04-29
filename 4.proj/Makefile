# K souboru: proj4.tex
# Datum:    16.4.2024
# Autor:    Michael Babušík (xbabus01@stud.fit.vutbr.cz)
# Projekt:  ITY projekt 4
PROJ=proj4
PACK=xbabus01-fit

.PHONY: clean pack bibtex pdflatex

$(PROJ).pdf: $(PROJ).tex $(PROJ).bib
	pdflatex $(PROJ).tex
	bibtex $(PROJ)
	pdflatex $(PROJ).tex
	pdflatex $(PROJ).tex

pack: $(PACK).tar.gz

$(PACK).tar.gz: $(PROJ).tex $(PROJ).bib czechiso.bst
	tar -czf $@ $^ Makefile

clean:
	rm -f $(PROJ).aux $(PROJ).dvi $(PROJ).log $(PROJ).ps $(PROJ).synctex.gz $(PROJ).fls $(PROJ).fdb_latexmk $(PROJ).bbl $(PROJ).blg proj4.out $(PROJ).pdf
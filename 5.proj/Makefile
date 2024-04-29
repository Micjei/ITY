# K souboru: proj5.tex
# Datum:    24.4.2024
# Autor:    Michael Babušík (xbabus01@stud.fit.vutbr.cz)
# Projekt:  ITY projekt 5
PROJ=proj5
PACK=xbabus01-fit

.PHONY: clean pack pdflatex

$(PROJ).pdf: $(PROJ).tex
	pdflatex $(PROJ).tex
	pdflatex $(PROJ).tex

pack: $(PACK).tar.gz

$(PACK).tar.gz: $(PROJ).tex czechiso.bst
	tar -czf $@ $^

clean:
	rm -f $(PROJ).aux $(PROJ).dvi $(PROJ).log $(PROJ).ps $(PROJ).synctex.gz $(PROJ).fls $(PROJ).fdb_latexmk $(PROJ).bbl $(PROJ).blg proj5.out $(PROJ).pdf

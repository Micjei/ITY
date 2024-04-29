# K souboru: proj3.tex
# Datum:    2.4.2024
# Autor:    Michael Babušík (xbabus01@stud.fit.vutbr.cz)
# Projekt:  ITY projekt 3

PROJ=proj3
TEXFILES=$(PROJ).tex
STYFILES=algorithm2e.sty

$(PROJ).pdf: $(TEXFILES) $(STYFILES) ./img
	latex $(PROJ).tex
	latex $(PROJ).tex
	dvips -t a4 $(PROJ).dvi
	ps2pdf -sPAPERSIZE=a4 $(PROJ).ps

clean:
	rm -f $(PROJ).aux $(PROJ).dvi $(PROJ).log $(PROJ).ps $(PROJ).out 

clean-all: clean
	rm -f $(PROJ).pdf

.PHONY: clean-all clean

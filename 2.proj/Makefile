# K suboru: proj2.tex
# Datum:    11.3.2024
# Autor:    Michael Babušík (xbabus01@stud.fit.vutbr.cz)
# Projekt:  ITY projekt 2

PROJ=proj2

$(PROJ).pdf: $(PROJ).tex
	latex $(PROJ).tex
	latex $(PROJ).tex
	dvips -t a4 $(PROJ).dvi
	ps2pdf $(PROJ).ps

clean:
	rm -f $(PROJ).aux $(PROJ).dvi $(PROJ).log $(PROJ).ps $(PROJ).out

clean-all: clean
	rm -f $(PROJ).pdf

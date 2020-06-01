PAPER = CV
TEX = $(wildcard *.tex)
PICS = $(wildcard pictures/*.pdf pictures/*.png pictures/*.jpg)

.PHONY: all clean

$(PAPER).pdf: $(TEX) $(FIGS)
	echo $(FIGS)
	xelatex $(PAPER)
	xelatex $(PAPER)
	xelatex $(PAPER)
	rm -f *.aux *.bbl *.blg *.log *.out 

clean:
	rm -f *.aux *.bbl *.blg *.log *.out $(PAPER).pdf

open:
	open $(PAPER).pdf

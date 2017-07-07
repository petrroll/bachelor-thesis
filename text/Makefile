export TEXINPUTS=../macros//:

all: thesis.pdf

# LaTeX must be run multiple times to get references right
# -shell-excape is required for the syntax highlighter `minted` package
thesis.pdf: thesis.tex $(wildcard *.tex) bibliography.bib thesis.xmpdata
	pdflatex -shell-escape $<
	bibtex thesis
	pdflatex $<
	pdflatex $<

clean:
	rm -f *.log *.dvi *.aux *.toc *.lof *.lot *.out *.bbl *.blg *.xmpi
	rm -f thesis.pdf

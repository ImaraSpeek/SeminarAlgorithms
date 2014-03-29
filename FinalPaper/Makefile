
main: paper.pdf

paper.pdf: paper.tex
	pdflatex $<
	bibtex paper
	pdflatex $<

clean:
	rm *.pdf *.log *.aux


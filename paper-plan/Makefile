
main: paper-plan.pdf

paper-plan.pdf: paper-plan.tex
	bibtex paper-plan
	pdflatex $<

clean:
	rm *.pdf *.log *.aux


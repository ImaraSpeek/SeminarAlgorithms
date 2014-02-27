
main: Plan_presentation_monday.pdf Summary_presentation_plan.pdf

Plan_presentation_monday.pdf: Plan_presentation_monday.tex
	bibtex Plan_presentation_monday
	pdflatex $<

Summary_presentation_plan.pdf: Summary_presentation_plan.tex
	pdflatex $<

clean:
	rm *.pdf *.log *.aux


# basic makefile

nonlin_model: nonlin_model.pdf

nonlin_model.pdf: nonlin_model.tex crisdefs.tex figures/*.pdf Makefile
	pdflatex nonlin_model.tex -interaction nonstopmode && \
	pdflatex nonlin_model.tex -interaction nonstopmode && \
	pdflatex nonlin_model.tex -interaction nonstopmode || \
	rm nonlin_model.pdf 2> /dev/null || true

show: nonlin_model.pdf
#	evince nonlin_model.pdf
	acroread nonlin_model.pdf

clean:
	rm *.log *.aux *.toc *.vrb *.bbl \
	*.blg *.snm *.nav *.out 2> /dev/null || true


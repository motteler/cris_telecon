#
# makefile for ccast validation report
#

ccast_valid: ccast_valid.pdf

ccast_valid.pdf: ccast_valid.tex crisdefs.tex Makefile
	pdflatex ccast_valid.tex -interaction nonstopmode || \
	rm ccast_valid.pdf 2> /dev/null || true

show: ccast_valid.pdf
	evince ccast_valid.pdf > /dev/null 2>&1 &

clean:
	rm *.aux *.log *.nav *.out *.snm *.toc *.vrb 2> /dev/null || true


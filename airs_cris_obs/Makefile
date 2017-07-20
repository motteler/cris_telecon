#
# basic makefile
#

airs_cris: airs_cris.pdf

airs_cris.pdf: airs_cris.tex crisdefs.tex figures/*.png Makefile
	pdflatex airs_cris.tex -interaction nonstopmode || \
	rm airs_cris.pdf 2> /dev/null || true

show: airs_cris.pdf
	evince airs_cris.pdf 2> /dev/null &

clean:
	rm airs_cris.log airs_cris.aux airs_cris.toc airs_cris.vrb \
	airs_cris.bbl airs_cris.blg airs_cris.snm airs_cris.nav \
	airs_cris.out 2> /dev/null || true


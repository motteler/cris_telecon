# basic makefile

a2adjust: a2adjust.pdf

a2adjust.pdf: a2adjust.tex crisdefs.tex figures/*.pdf Makefile
	pdflatex a2adjust.tex -interaction nonstopmode || rm a2adjust.pdf

show: a2adjust.pdf
#	acroread /a "zoom=200" a2adjust.pdf 2> /dev/null
	evince a2adjust.pdf 2> /dev/null

clean:
	rm a2adjust.log a2adjust.aux a2adjust.toc a2adjust.vrb \
	a2adjust.snm a2adjust.nav a2adjust.out 2> /dev/null || true


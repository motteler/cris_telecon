# basic makefile

psinc: psinc.pdf

psinc.pdf: psinc.tex crisdefs.tex figures/*.pdf
	pdflatex psinc.tex -interaction nonstopmode || rm psinc.pdf

show: psinc.pdf
	acroread psinc.pdf

clean:
	rm psinc.log psinc.aux psinc.toc \
		psinc.snm psinc.nav psinc.out 2> /dev/null || true


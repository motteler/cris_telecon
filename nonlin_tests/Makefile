# basic makefile

nonlin: nonlin.pdf

nonlin.pdf: nonlin.tex crisdefs.tex umbc*.pdf idps*.pdf FIR*.pdf
	pdflatex nonlin.tex -interaction nonstopmode || rm nonlin.pdf

show: nonlin.pdf
	acroread /a "zoom=200" nonlin.pdf

clean:
	rm nonlin.log nonlin.aux nonlin.toc \
		nonlin.snm nonlin.nav nonlin.out 2> /dev/null || true



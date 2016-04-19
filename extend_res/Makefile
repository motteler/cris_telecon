# basic makefile

extend_res: extend_res.pdf

extend_res.pdf: extend_res.tex crisdefs.tex figures/*.pdf Makefile
	pdflatex extend_res.tex -interaction nonstopmode || rm extend_res.pdf

show: extend_res.pdf
	acroread /a "zoom=200" extend_res.pdf 2> /dev/null

clean:
	rm extend_res.log extend_res.aux extend_res.toc extend_res.vrb \
	extend_res.snm extend_res.nav extend_res.out 2> /dev/null || true


# basic makefile

report: report.pdf

report.pdf: report.tex crisdefs.tex figures/*.pdf Makefile
	pdflatex report.tex -interaction nonstopmode || rm report.pdf

show: report.pdf
	acroread report.pdf

slides: slides.pdf
	acroread /a "zoom=200" slides.pdf

slides.pdf: slides.tex crisdefs.tex figures/*.pdf Makefile
	pdflatex slides.tex -interaction nonstopmode || rm slides.pdf

clean:
	rm report.log report.aux report.toc report.vrb \
	  report.snm report.nav report.out 2> /dev/null || true
	rm slides.log slides.aux slides.toc slides.vrb \
	  slides.snm slides.nav slides.out 2> /dev/null || true


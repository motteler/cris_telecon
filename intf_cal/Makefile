# basic makefile

intf_cal: intf_cal.pdf

intf_cal.pdf: intf_cal.tex crisdefs.tex Makefile
	pdflatex intf_cal.tex -interaction nonstopmode && \
	pdflatex intf_cal.tex -interaction nonstopmode || \
	rm intf_cal.pdf 2> /dev/null || true

show: intf_cal.pdf
	evince intf_cal.pdf

clean:
	rm intf_cal.log intf_cal.aux intf_cal.toc intf_cal.vrb intf_cal.bbl \
	intf_cal.blg intf_cal.snm intf_cal.nav intf_cal.out 2> /dev/null || true


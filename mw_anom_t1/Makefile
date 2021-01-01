#
# makefile for decon paper
#

mw_anom_t1: mw_anom_t1.pdf

mw_anom_t1.pdf: mw_anom_t1.tex crisdefs.tex figures/*.pdf Makefile
	pdflatex mw_anom_t1.tex -interaction nonstopmode || \
	rm mw_anom_t1.pdf 2> /dev/null || true


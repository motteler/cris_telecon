#
# makefile for NPP MW fail tests
#

mw_anom_t2: mw_anom_t2.pdf

mw_anom_t2.pdf: mw_anom_t2.tex crisdefs.tex figures/*.pdf Makefile
	pdflatex mw_anom_t2.tex -interaction nonstopmode || \
	rm mw_anom_t2.pdf 2> /dev/null || true


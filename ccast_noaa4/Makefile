#
# makefile for ccast vs noaa comparisons
#

ccast_noaa4: ccast_noaa4.pdf

ccast_noaa4.pdf: ccast_noaa4.tex crisdefs.tex figures/*.pdf Makefile
	pdflatex ccast_noaa4.tex -interaction nonstopmode || rm ccast_noaa4.pdf

show: ccast_noaa4.pdf
	evince ccast_noaa4.pdf

clean:
	rm *.aux *.log *.nav *.out *.snm *.toc 2> /dev/null || true


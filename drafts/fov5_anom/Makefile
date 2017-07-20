#
# makefile for ccast vs noaa comparisons
#

fov5_anom: fov5_anom.pdf

fov5_anom.pdf: fov5_anom.tex crisdefs.tex figures/*.pdf Makefile
	pdflatex fov5_anom.tex -interaction nonstopmode || \
	rm fov5_anom.pdf2 > /dev/null || true

show: fov5_anom.pdf
#	evince fov5_anom.pdf
	acroread fov5_anom.pdf

clean:
	rm *.aux *.log *.nav *.out *.snm *.toc 2> /dev/null || true


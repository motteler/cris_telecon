# basic makefile

ccast_noaa: ccast_noaa.pdf

ccast_noaa.pdf: ccast_noaa.tex crisdefs.tex support.tex figures/*.pdf Makefile
	pdflatex ccast_noaa.tex -interaction nonstopmode || rm ccast_noaa.pdf

show: ccast_noaa.pdf
	acroread /a "zoom=200" ccast_noaa.pdf

clean:
	rm ccast_noaa.log ccast_noaa.aux ccast_noaa.toc ccast_noaa.vrb \
	ccast_noaa.snm ccast_noaa.nav ccast_noaa.out 2> /dev/null || true


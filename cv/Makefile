all: cv.pdf cv.pdf.asc

PDFTEXFLAGS = "--shell-escape"

cv.pdf: cv.tex
	pdflatex $(PDFTEXFLAGS) cv.tex
	pdflatex $(PDFTEXFLAGS) cv.tex
	pdflatex $(PDFTEXFLAGS) cv.tex

cv.pdf.asc: cv.pdf
	gpg --detach-sig -a cv.pdf

clean:
	rm -f *.log *.aux cv.pdf cv.pdf.asc

verify: cv.pdf cv.pdf.asc
	gpg --verify cv.pdf.asc cv.pdf

all: cv.pdf 

PDFTEXFLAGS = "--shell-escape"

cv.pdf: cv.tex
	pdflatex $(PDFTEXFLAGS) cv.tex
	pdflatex $(PDFTEXFLAGS) cv.tex
	pdflatex $(PDFTEXFLAGS) cv.tex

clean:
	rm -f *.log *.aux cv.pdf

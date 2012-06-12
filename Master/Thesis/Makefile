TITLE	= thesis

compilePDFLatex:
	pdflatex ${TITLE}.tex
	bibtex ${TITLE}
	pdflatex ${TITLE}.tex
	pdflatex ${TITLE}.tex
	
compileLatex:
	latex ${TITLE}
	bibtex ${TITLE}
	latex ${TITLE}
	latex ${TITLE}
	dvips -P pdf ${TITLE}.dvi
	ps2pdf ${TITLE}.ps

clean:
	${RM} *.blg *.out *.aux *.bbl *.log *.toc *.dvi *.ps *.lof *.lot

pdflatex: compilePDFLatex clean

latex: compileLatex clean

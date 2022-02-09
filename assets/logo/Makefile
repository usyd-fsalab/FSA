TARGET=logo
TEX=pdflatex
SVG=pdf2svg

all: ${TARGET}.svg

clean: 
	ls | grep logo | grep -v -F ".tex" | xargs rm         rm texput.log

${TARGET}.pdf: ${TARGET}.tex
	${TEX} $^


${TARGET}.svg : ${TARGET}.pdf
	${SVG} $^ $@

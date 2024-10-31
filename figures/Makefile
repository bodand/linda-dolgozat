PICS := lb-conf.pikchr scatter-gather.pikchr linda-rd.pikchr linda-in.pikchr query.pikchr
SVGS := linda-eval.svg linda-arch.svg
PDFS := $(PICS:.pikchr=.pdf) $(SVGS:.svg=.pdf)

INKSCAPE := "C:\Program Files\Inkscape\bin\inkscape.exe" 
PIKCHR   := pikchr

.SUFFIXES:
.SUFFIXES: .pikchr .svg .pdf

all: $(PDFS)

.pikchr.svg: 
	$(PIKCHR) --svg-only $< > $@

.svg.pdf:
	$(INKSCAPE) -D $< -o $@


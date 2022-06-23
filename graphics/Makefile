include $(MAKEFILE_TEMPLATES)/fig2pdf_rule/Makefile
include $(MAKEFILE_TEMPLATES)/pdf2svg_rule/Makefile
include $(MAKEFILE_TEMPLATES)/tex2pdf_rule/Makefile

# Original files
FIGs := $(wildcard *.fig)
TEXs := $(wildcard *.tex)

# Target files
PDFs += $(FIGs:%.fig=%.pdf)
TMPs += $(PDFs)
SVGs += $(FIGs:%.fig=%.svg)
TMPs += $(SVGs)

PDFs += $(TEXs:%.tex=%.pdf)
TMPs += $(PDFs)
SVGs += $(TEXs:%.tex=%.svg)
TMPs += $(SVGs)

default:	$(TMPs)

info:
	@echo $(TMPs)

clean:
	rm -f $(TMPs)

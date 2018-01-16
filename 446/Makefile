TARGET = ta_notes1
pdf:
	xelatex $(TARGET) && bibtex $(TARGET) && xelatex $(TARGET) && \
	xelatex $(TARGET)

quick:
	xelatex $(TARGET)

clean:
	rm -f *.aux *.log *.blg *.bbl *~ *.dvi *.out *.nav *.snm *.toc $(TARGETS)

final:
	ps2pdf13 -dPDFSETTINGS=/prepress -dEmbedAllFonts=true -dUseFlateCompression=true -dCompatibilityLevel=1.4 $(TARGET).pdf $(TARGET)_final.pdf

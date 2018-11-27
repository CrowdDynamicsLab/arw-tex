OUTPUT_DIR=/Users/harshay/code/github_research/ngm/attributed_graph_models/CIKM/tex/out

all: run

run:
	latexmk -outdir=$(OUTPUT_DIR) -cd -e -f -pdf -interaction=nonstopmode -synctex=1 "draft.tex"

open_pdf: run
	cd $(OUTPUT_DIR); open "draft.pdf"

clean:
	cd $(OUTPUT_DIR); \
	$(RM)  *.fls *.fdb_latexmk *.log *.aux \
	*.cfg *.glo *.idx *.toc \
	*.ilg *.ind *.out *.lof \
	*.lot *.bbl *.blg *.gls *.cut *.hd \
	*.dvi *.ps *.thm *.tgz *.zip *.rpi

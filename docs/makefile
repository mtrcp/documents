LANG=en_US.UTF-8
LC_ALL=en_US.UTF-8
TEMPLATE_DIR=../templates
OUTPUT_DIR=../output
HTMLBASE=../

MD = $(wildcard *.md)

.PHONY: all clean deploy

all: $(MD:.md=.pdf) $(MD:.md=.html)

deploy:
	cp -va *.pdf $(OUTPUT_DIR)
#add back in @.html after .pdf

%.pdf: %.html
	weasyprint --base-url $(HTMLBASE) $< $@

#%.html: %.md
#	../utils/kram.rb -t $(TEMPLATE_DIR)/main -o $@ $^

clean:
	rm -f *.html *.pdf

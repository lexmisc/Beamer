# 该 Makefile 用于编译一个 Beamer 制作的幻灯片
# 运行环境：Linux、texlive2010(XeTeX)、evince 阅读器

Compiler = xelatex
Reader = okular

Target = beamer_body.pdf
Source = beamer_body.tex
TmpFile = *.out *.log *.aux *.nav *.snm *.toc *.vrb

$(Target): $(Source)
	$(Compiler) $(Source)
	$(Compiler) $(Source)

all: $(Target) clean read 

read:
	$(Reader) $(Target)

clean:
	-rm -rf $(TmpFile)

cleanall:
	-rm -rf $(TmpFile) $(Target)

.PHONY: all read clean cleanall

# pandoc-test

Just a repo for testing out [Pandoc][1], using the Pandoc manual as sample content (used under GPLv2).

First install MacTeX and Pandoc (using Homebrew, MacOS):

    brew cask install mactex
    brew install pandoc

To build the doc:

    pandoc input.md --pdf-engine=xelatex -o output.pdf

Or, styled:

    pandoc -N --template=mytemplate.tex --variable mainfont="Palatino" --variable sansfont="Helvetica" --variable monofont="Menlo" --variable fontsize=12pt --variable version=2.0 input.md --pdf-engine=xelatex --toc -o output.pdf

[1]: https://pandoc.org


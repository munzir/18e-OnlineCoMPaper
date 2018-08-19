# 18e: Online CoM Paper
A repo that contains the files for the Online Center of Mass Estimation Paper

## Dependencies

- A LaTeX distribution (such as [TeX Live](www.tug.org/texlive/))

## Build and Run

1: Enter the project directory

2: Compile the project according to IEEE Standard

    latex onlinecom
    bibtex onlinecom
    latex onlinecom
    latex onlinecom
    dvips -Ppdf -G0 -tletter sample
    ps2pdf -dCompatibilityLevel=1.4 -dMAxSubsetPct=100 -dSubsetFonts=true -dEmbedAllFonts=true -sPAPERSIZE=letter onlinecom.ps onlinecom.pdf

Note: Make sure to compile with `latex` once, `bibtex` once, and then `latex` twice before compiling into a postscript file and then pdf file.

3: View the compiled pdf (`onlinecom.pdf`) file using your favorite pdf viewer

## IEEE PDF Compliance

- [IEEE LaTeX Support Page](http://ras.papercept.net/conferences/support/tex.php)
- [PDF Test](http://ras.papercept.net/conferences/scripts/pdftest.pl)

## Paper Prep
This folder contains small TeX files serving as drafts.

### Build and Run
Since these files will not be submitted to IEEE, there is no need to perform the
complex build procedure mentioned above. You can just:

    pdflatex {TeX filename}

to produce an output pdf file.

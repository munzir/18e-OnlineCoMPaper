# 18e: Online CoM Paper
A repo that contains the files for IEEE Humanoids Submission

## Dependencies

- A LaTeX distribution (such as [TeX Live](www.tug.org/texlive/))

## Build and Run

1: Enter the project directory

2: Compile the project according to IEEE Standard

    latex onlinecom
    dvips -Ppdf -G0 -tletter sample
    ps2pdf -dCompatibilityLevel=1.4 -dMAxSubsetPct=100 -dSubsetFonts=true -dEmbedAllFonts=true -sPAPERSIZE=letter onlinecom.ps onlinecom.pdf

3: View the compiled pdf (`onlinecom.pdf`) file using your favorite pdf viewer

To test IEEE pdf compliance
- [IEEE LaTeX Support Page](http://ras.papercept.net/conferences/support/tex.php)
- [PDF Test](http://ras.papercept.net/conferences/scripts/pdftest.pl)

# LaTeX Installation on Ubuntu
Ubuntu repository consist of 5 packages from which each targets different type of a LaTeX user. You can choice common installation packages for LaTeX and their approximate capacity disk requirements based on your installation selected goal:
#### texlive-base - 136 MB
#### texlive-latex-recommended - 177 MB
#### texlive - 240 MB
#### texlive-latex-extra - 404 MB
#### texlive-full - 4714 MB

texlive-base: will install just the basics to get you started with LaTeX. 
texlive or texlive-latex-extra: is most likely the best way to get started for most users.
texlive-full package: Vietnamese language pack.

$sudo apt-get install texlive-full
$sudo apt install texstudio

# Note for Compile LaTeX
\bibliography{ICT2019_Paper20.bib}
\bibliographystyle{ieeetr}

## Need to remove file name: .bbl before compile LaTEX if not it will be uncessfull.

### Struct bbl file like this, (it is generated automatically - don't write anything in this
###### \begin{thebibliography}{1}

###### \bibitem{ER2008}
E.~R. Mardis, ``Next-generation dna sequencing methods,'' {\em Annual Review of
  Genomics and Human Genetics}, vol.~9, no.~1, pp.~387--402, 2008.
\newblock PMID: 18576944.

\bibitem{Ginther2015}
J.~L. Ginther, M.~Mayo, S.~D. Warrington, M.~Kaestli, T.~Mullins, D.~M. Wagner,
  B.~J. Currie, A.~Tuanyok, and P.~Keim, ``{Identification of Burkholderia
  pseudomallei near-neighbor species in the Northern Territory of Australia},''
  {\em PLoS Neglected Tropical Diseases}, vol.~9, no.~6, pp.~1--13, 2015.

\bibitem{Li2013}
H.~Li, ``{Aligning sequence reads, clone sequences and assembly contigs with
  BWA-MEM},'' vol.~00, no.~00, pp.~1--3, 2013.

\bibitem{Li2010}
H.~Li and R.~Durbin, ``{Fast and accurate long-read alignment with
  Burrows-Wheeler transform},'' {\em Bioinformatics}, vol.~26, no.~5,
  pp.~589--595, 2010.

\bibitem{Li2009}
H.~Li and R.~Durbin, ``{Making the Leap: Maq to BWA},'' {\em Mass Genomics},
  vol.~25, no.~14, pp.~1754--1760, 2009.

\bibitem{Li2009a}
H.~Li, B.~Handsaker, A.~Wysoker, T.~Fennell, J.~Ruan, N.~Homer, G.~Marth,
  G.~Abecasis, and R.~Durbin, ``{The Sequence Alignment/Map format and
  SAMtools},'' {\em Bioinformatics}, vol.~25, no.~16, pp.~2078--2079, 2009.

\bibitem{Quinlan2010}
A.~R. Quinlan and I.~M. Hall, ``{BEDTools: A flexible suite of utilities for
  comparing genomic features},'' {\em Bioinformatics}, vol.~26, no.~6,
  pp.~841--842, 2010.

\end{thebibliography}


#Gõ Tiếng việt có dấu trong Latex in Ubuntu
Download:
http://vntex.sourceforge.net/download/vntex/vntex-3.1.9.zip
Unzip file:
unzip vntex-3.1.9.zip
==> result: tex folder
copy all folders in after unzip folder to Textlive

Find path for language package
find . -name "*.sty"

$sudo cp -r ~/Downloads/tex/latex/vntex/ /usr/share/texmf/tex/latex

# SUCCESS



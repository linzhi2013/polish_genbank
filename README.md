# polish_genbank

## 1 Introduction

see `https://github.com/linzhi2013/polish_genbank`.

This package is to check for the internal stop codon in Genbank or FASTA file (CDS), then
 substitute the internal stop codon with NNN. 

## 2 Installation

    pip3 install polish_genbank

There will be a command `polish_genbank` created under the same directory as your `pip3` command.

## 3 Usage
run `polish_genbank`


    usage: polish_genbank.py [-h] --in <file> [--format {gb,fa}] [--table <int>]
                             [--ntNs <str>] [--aaNs <str>] --out <file>

    Check for the internal stop codon, then substitute the internal stop codon
    with NNN. By mengguanliang [] genomics.cn, where [] == @. See
    https://github.com/linzhi2013/polish_genbank

    optional arguments:
      -h, --help        show this help message and exit
      --in <file>       input genbank file or CDS file (fasta format)
      --format {gb,fa}  the input file format. For fasta file, all sequences are
                        assumed to be forward strand, coding from +1 position [gb]
      --table <int>     The genetic code table used for translation, for fasta
                        input only [2]
      --ntNs <str>      the chars used for substituting an internal stop codon in
                        CDS sequence. [NNN]
      --aaNs <str>      the chars used for substituting an internal stop codon in
                        protein sequence. [X]
      --out <file>      output filename



## 5 Citation
Currently I have no plan to publish `polish_genbank`.

However, since `msa_cigars` makes use of `Biopython`, you should also cite it if you use `breakSeqInNs_then_translate` in your work:

    Peter J. A. Cock, Tiago Antao, Jeffrey T. Chang, Brad A. Chapman, Cymon J. Cox, Andrew Dalke, Iddo Friedberg, Thomas Hamelryck, Frank Kauff, Bartek Wilczynski, Michiel J. L. de Hoon: “Biopython: freely available Python tools for computational molecular biology and bioinformatics”. Bioinformatics 25 (11), 1422–1423 (2009). https://doi.org/10.1093/bioinformatics/btp163

Please go to `http://www.biopython.org/` for more details.







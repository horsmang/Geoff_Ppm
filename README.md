Ppm Analysis Project - started May 8, 2020

Using protocol established by Monica Papinski (see github.com/papi0310/ppm-pntC-clustering/wiki)

Started by updating file of Ppm protein sequences (Ppm_update2020.txt). Deleted Photorhabdus sequence (not sure why it was there) and added Olsenella uli Ppm Oul_594 (Dacheng and Maddison observed activity).

Installed HMMER 3.3

Downloaded Pfam-A.hmm database from ftp://ftp.ebi.ac.uk/pub/databases/Pfam/releases), latest was 33.1 (Pfam-A.hmm.gz) and installed in /bioinf/ directory.

First have to run hmmpress on hmmdb prior to running hmmscan:

from bioinf/Geoff_Ppm/

$hmmpress ../Pfam-A.hmm

Then run hmmscan

$hmmscan --domtblout ppm_scan --cut_ga ../Pfam-A.hmm Ppm_update2020.txt

Clearly only PF13714.7 returns for Ppm.


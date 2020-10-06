# PfamAnnotation
Performing gene annotation based on Pfam annotations on Linux operating systems.

version 1.0

Copyright (C) Runmao Lin

Contact (E-mail): linrunmao@caas.cn

This pipeline is provided under the terms of a personal license to the recipient and may only be used for the recipient's own research at an academic insititution.

For using this pipeline in a company or for commercial purposes, a commercial license is required.

The pipeline includes other five programs of ObtainPfamAStat, CheckPfamStatRepeat, FilterPfamStatEvalue, DomainListForGene, PfamFamilyStat

# Requirement
1. Download the Pfam hmm file (such as the 'Pfam-A.hmm' from Pfam v32.0, i.e., 'ftp://ftp.ebi.ac.uk/pub/databases/Pfam/releases/Pfam32.0/Pfam-A.hmm.gz'). Then uncompress the gz file by running the command:

gzip -d Pfam-A.hmm.gz

2. Install the HMMER software (http://hmmer.org/download.html).

# Installation
Go to the src direction, and type:

sh install.sh

# Example
PfamAnnotation  -hmmfile  /database/Pfam-A.hmm  -hmmsearch  /bin/hmmsearch  -proteins  Brassica_rapa.v1.5.pep -outprefix  Brapa

'/database/Pfam-A.hmm' is the hmm file download from Pfam database.

'/bin/hmmsearch' is the installed program of 'hmmsearch' from HMMER.

'Brassica_rapa.v1.5.pep' is the gene sequence file (amino acids).

# Citation
1. The citation of PfamAnnotation:

https://github.com/linrm2010/PfamAnnotation

2. The citation of Pfam database:

El-Gebali S, Mistry J, Bateman A, Eddy SR, Luciani A, Potter SC, Qureshi M, Richardson LJ, Salazar GA, Smart A, Sonnhammer ELL, Hirsh L, Paladin L, Piovesan D, Tosatto SCE, Finn RD. The Pfam protein families database in 2019. Nucleic Acids Res. 2019,47(D1):D427-D432.

3. The citation of HMMER:

http://hmmer.org/

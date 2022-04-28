This files clean and extract information from three databases:

1. [SKEMPI v2](https://life.bsc.es/pid/skempi2)
2. [PDBbind-CN](http://www.pdbbind.org.cn/index.php)
3. bending  affinition benchmark v2 - from bending affinition benchmark v2 (cannot find website) , thus extract from literatures :
   1. K.  Yugandhar, M. Michael Gromiha, Protein–protein binding affinity prediction  from amino acid sequence, Bioinformatics, Volume 30, Issue 24, 15  December 2014, Pages  3583–3589, https://doi.org/10.1093/bioinformatics/btu580      
   2. Kastritis, P.L., Moal, I.H., Hwang, H., Weng, Z., Bates, P.A., Bonvin,  A.M.J.J. and Janin, J. (2011), A structure-based benchmark for  protein–protein binding affinity. Protein Science, 20: 482-491.  https://doi.org/10.1002/pro.580

The **sequencing data** of each proteins were extracted in `.seq.txt`, **binding affinity** of protein complex were extracted in `.dg.txt`. All the results are stored in `result` folder.

### Overall 

| database          | number                              | note                                                  | files                                                        |
| ----------------- | ----------------------------------- | ----------------------------------------------------- | ------------------------------------------------------------ |
| Affinity bench v2 | 94                                  |                                                       | `./affinitybench/affinitybench.seq.txt`<br />`./affinitybench/affinitybench.dg.txt` |
| PDBbind-CN        | 635 (from pdb) +1557 (from uniprot) | could be overlap using two methods                    | from **pdb** <br />`/pdbbind/pdbbind.seq.txt` <br />`./pdbbind/pdbbind.dg.txt` <br />from **uniprot** <br />`./pdbbind/pdbbind_uniprot.seq.txt` <br />`./pdbbind/pdbbind_uniprot.dg.txt` |
| SKEMPI v2         | 225 wildtype + 4165 mutated type    | 1KBH sequencing data are lost, part of 4PCA  are lost | **wild-type** <br />`./skempi/wild.dg.txt`<br /> `./skempi/wild2.seq.txt`<br /> **mutated type**<br /> `./skempi/mut.seq.txt`  <br />`./skempi/mut.dg.txt` |


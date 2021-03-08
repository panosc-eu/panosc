Use Case 10 – Linking raw data to the Protein Data Bank in Europe (PDBe) (ESRF)
=========================================================
The protein data bank ([PDBe in Europe](https://www.ebi.ac.uk/pdbe/)) is the reference repository for protein structures. All protein structures determined by different techniques are stored in the PDB. Since 2019 it is possible to link the protein structure entry to the raw data (images) often taken at the photon sources. As described in [this article](https://www.ebi.ac.uk/pdbe/about/news/links-added-raw-experimental-data-pdbe), “the model file in the PDB is the culmination of much hard work and interpretation of raw experimental data. The OneDep deposition system enables depositors to provide the location of raw datasets as a ‘digital object identifier’ (doi), within their mmCIF file in the PDB archive and this DOI is now directly linked from an entry page at PDBe”.

This use case is to link raw data in the ESRF data repository to the PDBe entries as shown in the [example here](https://www.ebi.ac.uk/pdbe/entry/pdb/6gv0).

Description of needs
------
Modify PaNOSC data repositories to add support for linking PDBe entries to raw data.

Use case action flow
------
*ESRF data repository – add javascript adapter for PDBe
*PDBe repository – test adapter
*Scientists – add DOI to raw data to PDBe entry

Impacts from the implementation
------
Make Protein Data Bank entries FAIR by providing access to raw data. This will enable results to be verified and structures to be refined with new software. This ICUR CommDat committee has been a strong advocate of making raw data accessible for crystallography [1]

[1] https://doi.org/10.1107/S2052252519005918

Generalisation of the use case
------
All PaNOSC and ExPaNDS partners could add the adapter for linking PDB entries to raw data. Thereby making PDB entries FAIRer.

Resources
------
ESRF data repository + PDBe adapter
[pDB 6gv0 structure summary](https://www.ebi.ac.uk/pdbe/entry/pdb/6gv0)

PaNOSC related work packages:
------
[WP3 – Data Catalogue Services](https://www.panosc.eu/work-packages/work-package-3-data-catalog-services/)

Contact person
------
[Andy Götz](mailto:andy.gotz@esrf.fr) (ESRF)

Link to website:
------
https://www.panosc.eu/use-cases/panosc-use-case-10-linking-raw-data-to-the-protein-data-bank-in-europe-pdbe/

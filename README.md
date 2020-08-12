# Supplementary Material for **Exploring the M-dwarf Luminosity - Temperature - Radius Relationships using Gaia DR2**

Sam Morrell and Tim Naylor (2019) - Accepted for publication in MNRAS 03 August 2019.

**Paper**: https://academic.oup.com/mnras/article/489/2/2615/5549528

**ArXiv**: https://arxiv.org/abs/1908.03025

**ADS**: https://ui.adsabs.harvard.edu/abs/2019MNRAS.489.2615M/abstract

----
**Last Updated: 11th August 2020**

This repository contains the supplementary material for Morrell and Naylor (2019). Incuded are:

- **mdwarf-properties.*** - The main catalogue of the publication that contains the input data and fitted properties for stars in our sample.
- **table3-tsed-r-relation.*** - A tabulated form of our T_SED - R relation for M-dwarf stars. A sample of this appears in the publication as Table 3. 
- **table4-lsed-r-relation.*** - A tabulated form of our L_SED - R relation for M-dwarf stars. A sample of this appears in the publication as Table 4.
- **table5-tabulated-flsed.*** - An electronic version of Table 3, which contains the tabulated values of $F(L_{\rm SED})$ in equation 16. 

All of these files are provided in FITS, ASCII and CDS format for convenience. We also provide the raw provide the raw input catalogue used in the fitting as **input-catalogue.fits**. 

We also include the polynomial coefficients used for the $T_{\rm SED} - R$ relation and $L_{\rm SED} - R$ correction in **tsed-r-coeffs.json** and **dotter08-lsed-r-coeffs.json** respectively. Each JSON file contains the relation / correction in the **med** property of the root object, with the coefficients for the upper and lower bounds being given in the **lbound** and **ubound** properties. These are lists of coefficients that can be directly read into *numpy.poly1d*.  

We also provide **mn19.py** which includes a Python 3 module for easily working with the provided coefficients.

## Version History

[**2019.8**](https://github.com/sammorrell/mn19-supplementary-material/releases/tag/2019.8) - The original version of the catalogue. 

[**2020.3**](https://github.com/sammorrell/mn19-supplementary-material/releases/tag/2020.3) - A revised version of the catalogue, including a corrected Gaia zero point and re-normalisation of input stellar atmospheres. Details of the changes are included in the erratum paper. 

[**2020.8**](https://github.com/sammorrell/mn19-supplementary-material/releases/tag/2020.8) - A further revision of the catalogue which includes improved uncertainties. This is the version accompanying the erratum.  

---

For your convenience, these catalogues are also available on:

**CDS**: https://cdsarc.unistra.fr/viz-bin/cat/VI/156

**Open Research Exeter Repository**: https://ore.exeter.ac.uk/repository/handle/10871/38279


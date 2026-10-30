---
layout: page
title: REE cross-plot (MREE/MREE* vs HREE/LREE)
subtitle: Interactive tool for rare earth element patterns in marine geochemistry
---

This tool places your rare earth element (REE) data on the MREE/MREE\* vs HREE/LREE cross-plot, together with the marine authigenic array, the detrital array and density fields of published foraminifera, pore water and seawater data (including the GEOTRACES IDP2025). The diagram was introduced by Martin et al. (2010); Du et al. (2016) added the authigenic and detrital arrays, and Blaser et al. (2020, Fig. 3) the reference fields.

**How to use it.** Tick *Use example data* or upload your own file with one row per sample and one column per element (`La`, `Ce`, ..., `Lu`; names such as `La_ppm` or `La [mg/kg]` work). CSV and TSV files work, and so do `.tab` files downloaded from [PANGAEA](https://www.pangaea.de): their metadata header is skipped, the dataset citation is shown and carried into the results, and mass or molar units are recognised from the column names. Choose the shale or chondrite normalisation and, optionally, a group column, screening limits and how anthropogenic Gd is handled.

The *Spectra* tab shows the normalised REE patterns, *Data quality* compares the roughness of your patterns with the reference data to flag noisy or interference-affected analyses, and *Computed values* lists all results with the settings used. The buttons below each plot download the figures and the data. Your data are processed in your browser and are not uploaded to any server.

The first load takes a little while, because the R environment (WebAssembly) is downloaded. For a larger view, [open the tool in its own window](https://patrick-blaser.github.io/ree-crossplot/){:target="_blank"}.

<iframe
  src="https://patrick-blaser.github.io/ree-crossplot/"
  title="REE cross-plot: MREE/MREE* vs HREE/LREE"
  style="width:100%; height:1150px; border:1px solid #ccc; border-radius:6px;"
  loading="lazy"
  allow="clipboard-write"></iframe>

**Source code, R functions and documentation:** [github.com/patrick-blaser/ree-crossplot](https://github.com/patrick-blaser/ree-crossplot). The repository also provides the calculations as stand-alone R functions (`functions/REE_functions.R`) for scripted work, giving the same results as the tool. The methods, options and all references are in the *About & references* tab of the tool.

**Please cite** Blaser et al. (2020) when using the tool or its figures. Citing Martin et al. (2010) and Du et al. (2016) as well is optional but appreciated, and data from PANGAEA or the GEOTRACES IDP2025 should be cited as their licences require.

- Blaser, P., Gutjahr, M., Pöppelmeier, F., Frank, M., Kaboth-Bahr, S., Lippold, J., 2020. Labrador Sea bottom water provenance and REE exchange during the past 35,000 years. Earth Planet. Sci. Lett. 542, 116299. [https://doi.org/10.1016/j.epsl.2020.116299](https://doi.org/10.1016/j.epsl.2020.116299)
- Du, J., Haley, B.A., Mix, A.C., 2016. Neodymium isotopes in authigenic phases, bottom waters and detrital sediments in the Gulf of Alaska and their implications for paleo-circulation reconstruction. Geochim. Cosmochim. Acta 193, 14–35. [https://doi.org/10.1016/j.gca.2016.08.005](https://doi.org/10.1016/j.gca.2016.08.005)
- Martin, E.E., Blair, S.W., Kamenov, G.D., Scher, H.D., Bourbon, E., Basak, C., Newkirk, D.N., 2010. Extraction of Nd isotopes from bulk deep sea sediments for paleoceanographic studies on Cenozoic time scales. Chem. Geol. 269, 414–431. [https://doi.org/10.1016/j.chemgeo.2009.10.016](https://doi.org/10.1016/j.chemgeo.2009.10.016)

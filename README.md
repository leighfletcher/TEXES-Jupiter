# TEXES-Jupiter

Global maps of Jupiter’s atmospheric temperatures, gaseous composition, and aerosol opacity can be derived from a programme of 5–20 μm mid-infrared spectroscopic observations using the Texas Echelon Cross Echelle Spectrograph (TEXES, [Lacy et al., 2002](https://iopscience.iop.org/article/10.1086/338730)) on NASA’s Infrared Telescope Facility (IRTF).

For more than a decade, TEXES low-to-medium-resolution observations have been used to monitor the thermal structure of Jupiter, using 8-10 narrow wavenumber settings sensitive to different spectral features.  By simultaneously inverting these spectra, we can provide a 3D view of Jupiter's atmosphere from the upper troposphere (~0.6 bars) to the mid-stratosphere (~1 mbar).  Full details of the inversion approach are provided by [Fletcher et al. (2016)](http://dx.doi.org/10.1016/j.icarus.2016.06.008), which used data from December 2014.  

Two scans across Jupiter at each wavelength setting were performed in succession, requiring about 1.25 hours to cycle through all the wavelengths. This progression is then repeated for around 5 hours per night on two consecutive nights to capture global maps of Jupiter at all the targeted wavelengths.

This website serves as a repository for TEXES products from each observing run, but it is my no means complete - we will endeavour to add quick-looks and retrievals from all datasets in the years to come.  Within each subdirectory, you will find:
* `DATE_WAVENUMBER_rawspec.png` - Summed spectrum for each TEXES scan (black) compared to the telluric transmission (red).  Blue dashed lines show the usual limits considered for spectral inversion, and the file number is given in the top right.
* `DATE_WAVENUMBER_scalezonal.png` - Central-meridian scan for each individual cube (i.e., the different longitudes registered in the key) compared to zonal-mean brightness (averaged over the TEXES passband) from Cassini/CIRS medium-resolution data (black dashed) and high-resolution data (red dashed) from 2000.  The different longitude scans are forced to have the same brightness at low latitudes to prevent steps in the maps, and radiometric calibration offsets are approximately corrected.
* `DATE_WAVENUMBER_fullmap.png` - The final combined map for the setting, with crude corrections for limb darkening/brightening.
* `DATE_WAVENUMBER_allmaps.png` - One example of a single map, used for checking data quality.
* `DATE_WAVENUMBER_zonalmean.png` - Spectral radiance as a function of wavenumber and y-axis, producing the spectral inputs for inversion.
* `DATE_WAVENUMBER_skytrans.png` - Terrestrial transmission deduced from the sky frames, which is used to scale the uncertainty on the spectral data (i.e., forcing NEMESIS to ignore regions of low transmission.


## Key References using Low-Med Spectroscopy
* L.N. Fletcher, G.S. Orton, T.K. Greathouse, J.H. Rogers, Z. Zhang, F.A. Oyafuso, G. Eichstadt, H. Melin, C. Li, S.M. Levin, S. Bolton, M. Janssen, H-J. Mettig, D. Grassi, A. Mura, A. Adriani (2020), Jupiter's Equatorial Plumes and Hot Spots: Spectral Mapping from Gemini/TEXES and Juno/MWR, Journal of Geophysical Research: Planets, 125, e2020JE006399 (https://arxiv.org/abs/2004.00072) (http://dx.doi.org/10.1029/2020JE006399).

* Doriann Blain, Thierry Fouchet, Thomas Greathouse, Thérèse Encrenaz, Benjamin Charnay, Bruno Bézard, Cheng Li, Emmanuel Lellouch, Glenn Orton, Leigh N. Fletcher, Pierre Drossart (2018), Mapping of Jupiter’s tropospheric NH3 abundance using ground-based IRTF/TEXES observations at 5 µm, Icarus 314, p106-120 (https://doi.org/10.1016/j.icarus.2018.06.002) (https://arxiv.org/abs/1802.09379)

* Henrik Melin, L.N. Fletcher, P.T. Donnelly, T. Greathouse, J. Lacy, G.S. Orton, R. Giles, J. Sinclair, P.G.J. Irwin (2018), Assessing the long-term variability of acetylene and ethane in the stratosphere of Jupiter, Icarus 305, p301-313 (https://doi.org/10.1016/j.icarus.2017.12.041) (https://arxiv.org/abs/1801.00652)

* L.N. Fletcher, G.S. Orton, J.A. Sinclair, P. Donnelly, H. Melin, J.H. Rogers, T.K. Greathouse, Y. Kasaba, T. Fujiyoshi, T.M. Sato, J. Fernandes, P.G.J. Irwin, R.S. Giles, A.A Simon, M.H. Wong, M. Vedovato (2017), Jupiter’s North Equatorial Belt expansion and thermal wave activity ahead of Juno’s arrival, Geophys. Res. Lett., 44, 7140-7148 (http://dx.doi.org/10.1002/2017GL073383) (https://arxiv.org/abs/1708.05179)

* L.N. Fletcher, T.K. Greathouse, G.S. Orton, J.A. Sinclair, R.S. Giles, P.G.J. Irwin, T. Encrenaz (2016), Mid-Infrared Mapping of Jupiter's Temperatures, Aerosol Opacity and Chemical Distributions from IRTF/TEXES, Icarus 278, p128-161 (http://arxiv.org/abs/1606.05498) (http://dx.doi.org/10.1016/j.icarus.2016.06.008)

* Leigh N. Fletcher, T.K. Greathouse, G.S. Orton, P.G.J. Irwin, O. Mousis, J.A. Sinclair, R.S. Giles, The Origin of Giant Planet Nitrogen from the 15N/14N Ratio, Icarus 238, p170–190 (http://dx.doi.org/10.1016/j.icarus.2014.05.007) (http://arxiv.org/abs/1405.3800)

## Spectral Settings

The following table contains a list of spectral settings regularly used by the medium-res spectral programme:

| Wavenumber    | Key Species | Resolving Power |
| -------- | ------- | -------|
| 539 cm-1  | Hydrogen-helium continuum    | 7,907 |
| 587 cm-1 | H2-He continuum and H2 S(1) quadrupole     | 5,836 |
| 744 cm-1    | Acetylene    | 10,292 |
| 762 cm-1    | Acetylene & H2 continuum    |  - |
| 819 cm-1    | Ethane    | 7,724 |
| 900 cm-1    | Phosphine & ammonia    | 2,896 |
| 960 cm-1    | Ammonia    | 2,664 |
| 1165 cm-1    | Phosphine and clouds    | 2,157 |
| 1247 cm-1    | Stratospheric Methane    | 12,358 |
| 1935 cm-1    | Tropospheric Clouds & Ammonia    |- |
| 2125 cm-1    | Tropospheric Clouds    |- |
| 2140 cm-1    | Tropospheric Clouds & Arsine    | 12,366 |

## Data Record

*NB:  This table is continually being updated*

| Dates | Directory | Comments | Publication | 
| -------- | ------- | -------|-------|
|2012-JAN-11-19 |  | Poor weather | Unpublished |
|2012-SEP-28/OCT-05 | |   | Melin et al., 2019 |
|2013-FEB-04-12 | | | Fletcher et al., 2014; Melin et al., 2019 |
|2014-FEB-15-25 | |  Poor weather | Melin et al., 2019 |
|2014-DEC-06-09 | | Excellent coverage | Fletcher et al., 2016; Melin et al., 2019 | 
|2015-MAR-24/APR-06 | | | Melin et al., 2019 |
|2015-NOV-16-18 | | | Melin et al., 2019 |
|2016-JAN-13-20 | |  | Fletcher et al., 2017; Blain et al., 2018 |
|2016-MAY-02-03 | | | Fletcher et al., 2017; Melin et al., 2019 |
|2016-DEC-15-23 | | | Melin et al., 2019 |
|2017-JAN-15-16 | | | Melin et al., 2019 |
|2017-MAR-12-14 | | Gemini-North | Fletcher et al., 2020; between Juno PJ4 and PJ5 |
|2017-MAY-27-31 | | | Unpublished |
|2017-JUL-09-15 | | | Unpublished |
|2018-FEB-07-11 | | | Unpublished |
|2018-JUL-05-16 | | | Unpublished |
|2018-SEP-15-30 | | | Unpublished |
|2019-FEB-09-18 | | | Unpublished |
|2019-APR-13-24 | | | Unpublished |
|2019-AUG-13-17 | | | Unpublished |
|2019-SEP-13-20 | | Gemini-North | Unpublished |
|2021-JUN-26-27 | | First post-COVID observations | Unpublished |
|2021-OCT-02-04 | | | Unpublished |
|2021-NOV-10-11 | | | Unpublished |
|2022-JUN-27-30 | `2022jun` | Between PJ42-43; good conditions | Unpublished |
|2022-SEP-15-16 | `2022sep` | Between Juno PJ44-45; excellent conditions.  | Unpublished |
|2023-JUL-15-25 | `2023jul` | Between PJ52 and PJ53. | Unpublished |
|2023-OCT-01-08 | `2023oct` | Between PJ54-55; humidity and cirrus; best data 07/08. | Unpublished |
|2023-DEC-07-12 | `2023dec` | Between PJ56-57; excellent quality except for 2023-12-09. | Unpublished |
|2024-FEB-23-25 | `2024feb` | Between PJ58-59; mediocre conditions (clouds) over 3 nights (PI: Harkett) | Unpublished. |
|2024-JUL-29-30 | `2024jul` | 14d after PJ63; some cirrus on night 1; 75% of night 2 excellent (PI: Harkett) | Unpublished. |

Raw and pipeline-reduced data have been recently delivered and archived at the NASA/IPAC Infrared Science Archive within the IRTF archive hosted here: https://irsa.ipac.caltech.edu/frontpage/

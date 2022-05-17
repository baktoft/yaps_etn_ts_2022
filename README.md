YAPS - Yet Another Positioning Solver  
ETN Training Session 2022, České Budějovice, Czechia

================

[![](rmds/yaps_logo_hex_100px.png)](https://github.com/baktoft/yaps)

------------------------------------------------------------------------

Code and examples are tested using R4.1.3 and R4.2.0 running on Windows
10.

Please make sure that these packages are installed.

``` r
install.packages(c('data.table',
                  'caTools',
                  'dplyr',
                  'sp',
                  'knitr',
                  'leaflet',
                  'lubridate',
                  'ggplot2',
                  'remotes',
                  'rgdal',
                  'viridis'))
```

Install newest dev version of yaps from github, load it and check it is
working. When installing YAPS from github, a compiler is needed. If you
don’t already have one installed, download and install Rtools from
<https://cran.r-project.org/bin/windows/Rtools/>. Choose correct version
for your version of R. Restart of R (and perhaps your pc) might be
needed.

``` r
remotes::install_github('baktoft/yaps', ref='v.1.2.5.9000')
remotes::install_github('baktoft/yapsdata')
library(yaps)
testYaps()

# # # It might throw a message about version inconsistency for TMB and Matrix. If so, try to fix it by running
# install.packages("TMB", type = "source")
```

If the last line returned a plot of a simple track with overlapping
black and red lines, everything should be working.

------------------------------------------------------------------------

The code for this part of the workshop is available in two formats - the
code should be identical. All relevant files are found in the `rmds`
folder.

-   R-script
    -   `rmds/part1_setupAndTest.R`
    -   `rmds/part2_crayfish.R`
    -   `rmds/part3_hald.R`
-   R-notebooks
    -   `rmds/part1_setupAndTest.nb.html`
    -   `rmds/part2_crayfish.nb.html`
    -   `rmds/part3_hald.nb.html`

------------------------------------------------------------------------

You are encouraged to take a look at the yaps readme:
<https://github.com/baktoft/yaps>

If you can’t get enough of YAPS have a look at the original paper:  
[Positioning of aquatic animals based on time-of-arrival and random walk
models using YAPS (Yet Another Positioning
Solver)](https://www.nature.com/articles/s41598-017-14278-z.pdf)

And the pre-print including a step-by-step guide: [Opening the black box
of fish tracking using acoustic
telemetry](https://www.biorxiv.org/content/10.1101/2019.12.16.877688v1)

To keep updated, follow YAPS on
[github](https://github.com/baktoft/yaps) and
[researchgate](https://www.researchgate.net/project/YAPS-open-source-high-resolution-fish-tracking)

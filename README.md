# BISe Online

A dependency-free, browser-based teaching adaptation of the **Basic Irrigation Scheduling (BISe)** Excel workbook. It allows agricultural irrigation students to create a daily soil-water budget and an irrigation-event schedule from:

* monthly mean daily ETo, precipitation, and rainy days;
* BISe crop coefficients and crop-stage timing;
* root depth, available water capacity, allowable depletion, and wetted soil volume; and
* irrigation-system DU, precipitation rate, and estimated runoff.

No installation or build step is required. Open `dist/index.html` locally to use the program offline.

## Educational calculation model

* `ETc = ETo × Kc`
* `PAW = root depth × available water capacity`
* `allowable depletion = PAW × MAD × wetted fraction`
* `gross depth = low-quarter net depth ÷ DU ÷ (1 − runoff fraction)`
* `runtime = gross depth ÷ precipitation rate`

Monthly mean ETo values are linearly interpolated between monthly midpoints. Monthly precipitation is distributed across evenly spaced planning days. Effective rainfall is limited to the amount needed to refill current root-zone depletion.

## Important limitations

This is an instructional and preliminary-planning tool. The automatically generated schedule does not replace field measurements, soil-moisture monitoring, current weather observations, regulatory requirements, or professional judgment. Crop coefficients and root-zone assumptions must be checked for local conditions.

## Attribution

Adapted from the BISe spreadsheet and manual by R. L. Snyder, M. Orang, K. Bali, S. Eching, and later contributors. Original BISe copyright © 2000 Regents of the University of California. The original source materials should be retained with the course materials and consulted for methodology and limitations.


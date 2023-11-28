Oct 5 2022 R.Kessler

For compatibility with public SALT3-Frag release, replace CSP-B/u
with CSP-B/M (checked the /M was not already used). David Jones
made this update to avoid conflict with SDSS-u.

Oct 15 2022 R.K
For MAGSHIFT CSP-u, multuply by x4 to implment sigma(CSP-u) = 0.005 -> 0.02.
Note that sigma(CSP-BVri) ~ 0.01 from SuperCal, and sigma(CFA3) = 0.02 ...
thus the increase is sigma(CSP-u) makes it consistent with other UV band
uncertainties.

Apr 26 2023 GT
+ Added extra survey-filter combinations according to the Fragilistic training sample SN that are observed in multiple bands
Namely - CFA3 Bessell; CFA3 CSP; LOWZ Bessell; LOWZ CSP; LOWZ CFA3K; SDSS CSP; SDSS CFA3K
+ Changed CFA1 and CALAN_TOLOLO waveshifts from 0 to random (independent) shifts.
The SALT3 filters don't understand the "overlapping surveys" the way that SALT2 does

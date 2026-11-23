# ASCEND OVR

A companion to ASCEND for recording five weekly attribute scores and tracking weekly performance, cumulative OVR, radar ratings, monthly averages and trends.

## Install
Upload all files in this folder to the root of a GitHub repository, enable GitHub Pages from `main` and `/(root)`, then open the Pages URL in Chrome and choose Install app / Add to Home screen.

## Scoring model
- Weekly performance = average of the five scores entered for that week.
- The first logged week establishes the starting OVR and the five starting attribute ratings.
- From the second week onward, each rating increases by `(100 - current rating) × (that week's score / 100) × 0.04`.
- Therefore, a lower-but-positive week still adds progress; weekly performance can fall while cumulative OVR and attribute ratings keep increasing.
- This makes cumulative ratings non-decreasing for valid scores from 0 to 100, while weekly performance can rise or fall.
- Monthly averages are averages of the weekly performance scores logged in that calendar month.

This is a motivational progress system, not a medical, psychological or objective ability assessment. Entries are stored in local browser storage on the device. Export backups regularly; there is no cloud sync.

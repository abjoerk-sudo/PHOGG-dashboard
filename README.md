# PHOGG-dashboard

GREENLAND GLACIER RETREAT & ICE-MARGIN DASHBOARD

FILES
  index.html   Complete dashboard with all glacier rates and historical ice-margin line data embedded.

HOW TO USE
  - Open index.html in a current desktop browser while connected to the internet.
  - The background map comes from NunaGIS, and JavaScript maps are loaded from ArcGIS online.
  - If publishing with GitHub Pages, replace the existing index.html in the website repository with this version.

CONTROLS
  - Choose 4 glacier-rate layers, 1930s-2020s, and glacier type.
  - Turn glacier point markers and historical margin lines on/off independently.
  - Click any point for the decade series and any margin line for the observation date/source.

COLOR SCALES
  - Glacier points: red = negative/retreat; green = positive/advance.
    Fixed absolute-value class breaks (m/yr): 25, 50, 100, 250, 500, 1000, 2500, 5303.
    The same 8 classes apply to all decades and rate layers.
  - Margin lines: a single continuous cool-to-warm chronological scale for all glaciers,
    from the earliest date in 1931 to the latest date in 2025.

DATA INPUTS
  phogg_decadal_retreat_rates.gpkg (346 point features and 4 rate layers)
  MarginsCombined_MLD_Nov2026_with_Hexagon.gpkg (3337 margin lines across 306 layers)
  Margin features were transformed from EPSG:3413 to EPSG:32624 for NunaGIS map alignment.

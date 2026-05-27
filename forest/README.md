Forest Area Extraction & Change Detection
Dense vegetation was identified using NDVI > 0.6, representing healthy forest cover.
The NDVI raster was reclassified into a thematic raster:
✧ NDVI > 0.6 → forest
✧ NDVI ≤ 0.6 → ignored
A binary raster was generated in Raster Calculator:
✧ 1 = forest
✧ 0 = non-forest
The raster was polygonized, keeping only forest polygons.
Polygons smaller than 0.25 ha were removed to reduce noise.
Forest area was calculated in hectares from polygon geometry.
Results were visually validated using satellite imagery/topographic data.
Forest Change Analysis (ArcMap)
Intersect identified preserved forest areas.
Erase detected forest loss and gain.
Layers were merged and symbolized by change type:
✧ loss
✧ gain
✧ stable forest
Raster difference analysis produced:
✧ -1 → forest loss
✧ 0 → no change
✧ 1 → forest expansion
Pixel counts were converted to area values (m² and ha) using image resolution.
Final statistics were exported to Excel for analysis and visualization.

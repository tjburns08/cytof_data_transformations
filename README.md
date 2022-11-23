## CyTOF data transformations

This project explores the question of what data transformations are best for CyTOF data. In particular, the standard in the field at the time of writing is the inverse hyperbolic sine (asinh) with a scale argument of 5, written as asinh(x/5) where x is a data point (feature vector) in a CyTOF dataset. 

The single-cell sequencing community, in particular the users of Seurat, use the log1p transform, which is the log(x + 1) where x is a data point. 

Does the log1p transform work for CyTOF data? Where are there differences? Does the scale argument matter? See the visualizations in rmd/ for insights. 
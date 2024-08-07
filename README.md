
This is the repository that contains the code, a trained Random Forests and two Sentinel-2 (S-2) geotiff files for the region Bibibino and Yakusk, both located in Eastern Siberia. 
The geotiff images are there as an example of the data format needed to apply the trained RF to. We used a 11-band geotiff file.

The trained RFs are for the early summer season (ES), the peak summer season (PS) and the late summer season (LS). The average precision we achieved with these trained RFs on the separate SiDroTest set was 63%, 89% and 99% respectively. When all three seasons are combined the average accuracy was 82%. These are the exoected results when used on new data. The late summer is the best season to use, also when predicting on S-2 data from other seasons. 

The repository alos contains a trained RF for the LS season with an extra class for the non forested classes masked out. That class is class 9 and contains the value -999. 

There is a jupyter notebook that shows how to load and use the RFs to predict on an S-2 image. For questions please contact: femke.van.geffen@gmail.com

This repository is supplement to:
Random Forest Classification Using Late Summer Sentinel-2 Data in Eastern Siberia's Summergreen-Evergreen Forest Transition Zone by: 
F. van Geffen, R. Hänsch , S. Kruse, U. Herzschuh and B. Heim (2024)


Abstract
Circumboreal forests, covering about 30% of global forested areas, are undergoing significant climate-induced changes. In Eastern Siberia, global warming may shift the boreal forest transition zone, replacing summergreen larch with evergreen needleleaf species. To monitor these changes, we trained a Random Forest classifier to map summergreen and evergreen forests using the SiDroForest Sentinel-2 dataset. This dataset, informed by expert field knowledge, includes nearly two million pixels across early, peak, and late summer phenophases.
Feature importance analysis highlighted the Sentinel-2 long shortwave infrared band (B12) as crucial for distinguishing forest types in all seasons, likely due to moisture content differences. Additional key features include the normalized difference vegetation index (NDVI) and red band (B4) in early summer, shortwave bands and the blue band in peak summer, and B12, the near-infrared band (B8), and NDVI in late summer.
Validation with the SiDroTest dataset, linked to in-situ forest plots, showed accuracies of 63% for early summer, 89% for peak summer, and 99% for late summer, with an average accuracy of 82% across all seasons. The classifier performed best in late summer, leveraging distinct spectral differences between evergreen forests' greenness and the seasonal coloring of summergreen larch forests. This method provides a precise tool for mapping boreal forest types in the Siberian transition zone, particularly effective in late summer when these differences are most evident.


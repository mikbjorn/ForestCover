# Analysis of Cartographic Features and Forest Cover Type
Authur: Mikkel Bjornson

# Background
The analysis focused on Dominant tree cover in the Covertype dataset (Bache and Lichman 2013). Knowledge of dominant tree species typically requires boots on the ground, a difficult task in remote areas. Cartographic features can easily be extract from a GIS. This study explores associations between cartographic features and cover type with the goal of predicting dominant tree species. 
# Goals
-	Explore the association between topographic features and presence of spruce/fir trees.
-	Predict dominant tree cover based on topographic features. 
# Analysis and Findings
## Inferential Study
All cartographic features were found to have a strong association with the cover type. Increases in elevation and hill shade at 9am and 3pm result in increased odds of Spruce/fir trees. Slope, distance to water, and hill shade at noon resulted in decreased odds. 
## Predictive Study
Fitting a Random Forest model resulted in overall an overall accuracy of 96.5%. The model performed best on the predictions of Lodgepole pine (97.7% accurate), Ponderosa Pine (97.0% accurate), Krummholz (96.0% accurate), and spruce/fir (96.0% accurate). The worst prediction rates were for Aspen (84.7% accurate) and Cottonwood/willow (87.4% accurate).   
# Recommendations 
The predictive power of the cartographic features is likely strong enough to provide the necessary accuracy without the need for direct observation. The predictive power of this model can likely be increased even further with the inclusion of additional cartographic features and interactions between features. Additionally, more advanced models such as boosted models or neural networks may provide even stronger predictive powers. These techniques should be explored. 
# Benefits
Using the predictive model, it is possible to estimate the cover type with 96.5% accuracy. At this accuracy level, the need for direct observation is greatly reduced. With increased model training, it may be possible to surpass the accuracy of direct observations. 
# Citation 
Bache, K. & Lichman, M. (2013). UCI Machine Learning Repository https://archive.ics.uci.edu/ml/datasets/covertype. Irvine, CA: University of California, School of Information and Computer Science

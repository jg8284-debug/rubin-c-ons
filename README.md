[README.txt](https://github.com/user-attachments/files/29383071/README.txt)
#### README FOR TEAM 0029 ####
For this project we initially considered a few different methods, such as XGBoost with Causal Forest and a Neural Network. However, we still found that classic BART performed best. That said, we did find that doing the basics of tuning the model with increasing it to 10000 iterations with keeping every 10 helped improve the quality of the model.
From there, we were inspired by Vincent Dorie et al. to add the estimated propensity score back into the model as a covariate ("Automated versus Do-It-Yourself Methods for Causal Inference" (2019)) which slightly lowered the RMSE. From there, we finally just increased the tree count to 500 and k to 3 as final tweaks.
In regards to AI usage, we used it for assistance in troubleshooting errors and doublechecking for any unnecessary redundancies in the code.
The first submitted dataset (included here as well) is the exact same, but without the final tree count and k changes.

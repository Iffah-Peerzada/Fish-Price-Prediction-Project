# Fish-Price-Prediction-Project
This Repository contains datasets and final codes of my Final Year Project as a Bachelor of Engineering in Computer Science, executed by a team of four.
It contains:
1) The raw Dataset and after it was ready to feed to model
2) The Data Preparation codes for above
3) Hybrid model code

The Hybrid models used were, LSTM and XGBOost. The hyperparameters of the model were calculated before running the model live using IBES (Improved Bald Eagle Search) Algorithm.
This Project is based on the future scope of the Shanghai Ocean University paper, "An Aquatic Product Price Forecast Model Using VMD-IBES-LSTM Hybrid Approach" (2022). The paper suggested using optimization algorithms to further enhance the results, so we utilized SSA (SIngular Spectrum Analysis) to decompose data.

The front-end codes are not present here. I was in charge of mainly Data Preprocesiing, this includes Data Cleaning, Data Transformation anf Feature Engineering. I converted a 5 feature dataset into a 15+ feature dataset that now has rolling totals, tempurature and humidity (using a wheather API), time related features such as day_of_week, day_of_year, etc, all to assist the final models in learning the patterns of the data enough to predict the price of a certain fish when user provides fish species and date. I performed decomposition and reconstruction of the price feature using SSA as well.

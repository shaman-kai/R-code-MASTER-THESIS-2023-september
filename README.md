# R-code-MASTER-THESIS

This R code performs statistical data analysis for my master's thesis "Linguistic Relativity in Categorical Colour Perception: Evidence from a Biologically Constrained Network Model".
The study used computational modelling to investigate linguistic relativity effects.
An artificial neural network representing language, sensory and motor areas of the human left brain hemisphere was trained to learn patterns representing 4 colours (dark blue, light blue, dark green, light green) and either 2 or 3 colour terms (2 patterns represented 2 colour terms -- "green" and "blue" -- in English, and 3 colour terms represented 1 word for green and 2 different words for light and dark blue that exist in some languages, such as Greek or Russian).
The data ("data_1Stage.csv", "data_EN.csv", "data_GR.csv") represent neuronal assemblies that emerged in the network models as a result of that learning. "data_1Stage.csv" contains neuronal assemblies that emerged when colour patterns were learned separately from words, "data_EN.csv" contains neuronal assemblies that emerged in response to colour patterns after those patterns were associated with 2 word patterns (i.e. "green" and "blue" in English). "data_RU.csv" contains neuronal assemblies that emerged in response to colour patterns after those patterns were associated with 3 word patterns (like 3 different colour terms for green, dark blue and light blue in Greek or Russian).
The code in "MT_1_RSA.Rmd" performs representational similarity analysis on those neuronal assemblies.
The code in "MT_2_RSA_ANOVA.Rmd" compares the dissimilarity matrices created by "MT_1_RSA.Rmd" to see whether the differences are significant (using ANOVA).
The code in "MT_3_Barplots.Rmd" and "MT_4_Barplots_Difference.Rmd" plots the number of neurons unique for each cell assembly vs. neurons shared between two cell assemblies representing two shades of the same colour (i.e. dark and light blue, dark and light green).
The code in "MT_5_ANOVA.Rmd" performs ANOVA on the number of unique vs. shared neurons between language (Pre-Language, English, and Greek) and colour conditions.
The scripts have to be run in the same order as they are mentioned above.
The rest of the code is pretty self-explanatory.

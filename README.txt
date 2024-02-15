Python code for chemical profiling of polymer data measured with LA-ICP-MS.

Background
This work is accompanying a manuscript on 'Evaluating the strength of evidence of elemental profiling of polymers with LA-ICP-MS.'

Summary
In the analysis elemental LA-ICP-MS data was assessed. The aim was to compare several data pre-processing and statistical methods to improve classification and comparison of polymer evidence materials of forensic relevance. 
Four datasets of tapes, electrical wires, tubing, and Jerry cans with 220 forensically relevant polymer objects originating from 175 sources in total (n=8) were analyzed by LA-ICP-MS. 
The responses of 18 elements (23Na, 25Mg, 27Al, 29Si, 39K, 44Ca, 47Ti, 55Mn, 57Fe, 60Ni, 63Cu, 75As, 88Sr, 93Nb, 118Sn, 121Sb, 138Ba, 208Pb). ) was measured. 
Various normalization and quantification methods were applied, including the use of a novel matrix-matched polymer reference standard for quantification.

Data
Six csv files are provided:
* "Data_Polymer_Standard" contains the analysis of the performance of the polymer standards
* "Data_Polymers" contains the processed datafile with the uncorrected signals of 18 elements for the datasets of tapes, electrical wires, tubing, and Jerry cans
* "Data_Polymers_C" contains the processed datafile with the signals normalized by the carbon signal of 18 elements for the datasets of tapes, electrical wires, tubing, and Jerry cans
* "Data_Polymers_glass" contains the processed datafile with the signals semi-quantified with the NIST SRM 612 glass standard, of 18 elements for the datasets of tapes, electrical wires, tubing, and Jerry cans
* "Data_Polymers_PVC" contains the processed datafile with the signals (in mg/kg) quantified with the PVC standard, of 18 elements for the datasets of tapes, electrical wires, tubing, and Jerry cans
* "Data_Polymers_PVC_C" contains the processed datafile with the signals (in mg/kg) normalized by carbon and semi-quantified with the PVC standard, of 18 elements for the datasets of tapes, electrical wires, tubing, and Jerry cans

Notebooks
Four notebooks are provided:
* "Polymer_Profiling_1" contains the script for processing the raw data to the processed data.
* "Polymer_Profiling_2" evaluates the performance of the standards using the csv file "Data_Polymer_Standard".
* "Polymer_Profiling_3" applies various comparison models (4sigma, t-test, feature-based MVK LR model, and score-based SVM LR model) using the other 5 csv files.
* "Polymer_Profiling_4" classifies the various forensic objects (with e.g. PCA and LDA) using the other 5 csv files.

Contributing
The data analysis was performed by Mirjam de Bruin-Hoegee and Gerrit-Jan de Bruin.

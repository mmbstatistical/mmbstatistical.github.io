---
title: MINITAB Macros
nav_exclude: true
---



This page provides links to text files containing MINITAB macros. Open the files in NotePad or NotePad++ to see the code,
a description of the macro, and an example calling statement.  
  
The macros are of both LOCAL (.mac) and EXEC (.mtb) types. Copy them to the MINITAB macros folder on your hard drive.
If you don't already have a macros folder, I recommend that you create a folder like *C:/Documents/MINITAB/Macros/Macros V2/*
so that 1) your macros get backed up when you back up the rest of your data and 2) so that you can update your macros for different versions of MINITAB.  
  
Run EXEC macros from the **File> Run an EXEC** menu or from the command prompt.  
  
Run LOCAL macros from the command prompt. Make sure that MINITAB is looking for macros in the correct folder as specified
in **Tools> Options> General> Macro Location**. All macros should run on MINITAB V18 unless specified otherwise. E-mail me 
if you find something that doesn't run.  
  
Some of these macros are redundant to built-in commands in MINITAB; however, many of those were written before they were
supported by the program and have features that are different or code that might be of interest for other purposes.  
  
**These macros have been validated but they may give incorrect results for some input conditions. MM&B Inc. accepts no
responsibility for their results. Use these macros at your own risk.  
  
**MINITAB also maintains an extensive macro library *[here](https://support.minitab.com/en-us/minitab/macro-library/)*.  
<br/> <br/>

**Data and Worksheet Operations**
* [RepeatRows.mac](/assets/MINITAB/Macros/RepeatRows.mac) - Duplicates each row of the specified columns the specified number of times. Overwrites the original columns.
* [SetAColumn.mac](/assets/MINITAB/Macros/SetAColumn.mac) - Duplicates each row of a column the specified number of times and the whole sequence a specific number of times. Reproduces the functionality of the **Calc> Make Patterned Data> Arbitrary Set of Numbers** or **set** command for a column.
* [ColumnsOperation.mac](/assets/MINITAB/Macros/ColumnsOperation.mac) - Applies a simple math operation to all of the specified columns.   
* [FindUnique.mac](/assets/MINITAB/Macros/FindUnique.mac) - Removes rows with consecutive duplicate values in a specified column. Overwrites the original columns.
* [IsOneOf.mac](/assets/MINITAB/Macros/IsOneOf.mac) - Checks every observation in a column to see if it matches a value in another column.
* [RowOf.mac](/assets/MINITAB/Macros/RowOf.mac) - Finds the row containing the minimum and maximum value in the column.
* [SortIntoBins.mac](/assets/MINITAB/Macros/SortIntoBins.mac) - Identifies bins for observations based on bin class marks.
* [SplitText.mac](/assets/MINITAB/Macros/SplitText.mac) - Like the VB function **split()** - splits a text column by a character delimiter and writes the results to output columns.
* [ChangeCase.mac](/assets/MINITAB/Macros/ChangeCase.mac) - Changes entries in text columns from lower to upper case. MINITAB's **upper** function does this but only on one column at a time. The **ToLower** subcommand changes text from upper to lower case.
* [StackColsByRows.mac](/assets/MINITAB/Macros/StackColsByRows.mac) - Stacks the data in two or more columns by rows into a single column  
    

  
**Statistical Analysis**
* [MeansAndResiduals.mac](/assets/MINITAB/Macros/MeansAndResiduals.mac) - Extracts the subgroup means and the fits and residuals for a one-way classification.
* [HalfNorm.mac](/assets/MINITAB/Macros/HalfNorm.mac) - Creates a probability plot for half-normal, aka folded-normal data.
* [CircNorm.mac](/assets/MINITAB/Macros/CircNorm.mac) - Create a probability plot for circular-normal data.
* [UniformDistribution.mac](/Macros/UniformDistribution.mac) - Create a probability plot for uniformly distributed data.   
* [DefectivesOC.mac](/assets/MINITAB/Macros/DefectivesOC.mac) - Creates an operating characteristic curve for the single sampling plan for attributes using the specified sample size and acceptance number. The function of this macro is now supported in **Stat> Quality Tools> Acceptance Sampling by Attributes> Compare User Defined Sampling Plans** but the code may still be of interest.
* [OrthogonalRegression.mac](/assets/MINITAB/Macros/OrthogonalRegression.mac) - Performs orthogonal regression assuming var(x) = var(y). Duplicates the MINITAB method but allows regression through the origin.
* [NTIOneSided.mac](/assets/MINITAB/Macros/NTIOneSided.mac) - Calculates the one-sided normal tolerance interval factor k1 for either 1) one treatment group or 2) for one treatment group among several using the pooled standard deviation.
* [NTITwoSided.mac](/assets/MINITAB/Macros/NTITwoSided.mac) - Calculates the two-sided normal tolerance interval factor k2 for either 1) one treatment group or 2) for one treatment group among several using the pooled standard deviation.
* [ROC.mac](/assets/MINITAB/Macros/ROC.mac) - Creates the receiver operating characteristic curve (ROC) curve with AUC value for a binary diagnostic test. Use the **Stat> Regression> Binary Logistic Regression** method instead.  
    

  

**Design of Experiments**
* [FitFinder.mac](/assets/MINITAB/Macros/FitFinder.mac) - Creates a 6x6 matrix of scatterplots using common mathematical transformations applied to the x and y axes. The transformations used are: untransformed, square root, square, log, power, and reciprocal. Used to find transforms to x and/or y that linearize a nonlinear scatterplot when the first principles model is unknown.
* [MakeCRD.mac](/assets/MINITAB/Macros/MakeCRD.mac) - Creates the worksheet for a completely randomized design with the specified number of factor levels and replicates. Runs one-way ANOVA on the random order to confirm if the randomization was effective.
* [MakeRBD.mac](/assets/MINITAB/Macros/MakeRBD.mac) - Creates the worksheet for a randomized block design with the specified number of levels of the study variable and blocks.   
* [Correlate.mac](/assets/MINITAB/Macros/Correlate.mac) - Creates the correlation matrix of all of the specified columns, their two-factor interactions, and quadratic terms for up to 12 variables. Used to validate an experiment design/run matrix or to determine the consequences when a design is compromised because of missing runs, extra runs, or just bad design.
* [TwoSampleTestCorrelations.mac](/assets/MINITAB/Macros/TwoSampleTestCorrelations.mac) - Performs the two-correlations hypothesis test of H0: ρρ1 = ρ2 versus HA: ρ1 <> ρ2
* [Fold.mac](/assets/MINITAB/Macros/Fold.mac) - Folds a two-level experiment design on all columns. Consider using **Stat> DOE> Modify Design** instead.
* [RandomizeWithinBlocks.mac](/assets/MINITAB/Macros/RandomizeWithinBlocks.mac) - Creates a column for the random run order for runs within blocks.  
    

  
**Sample Size and Power Calculations**
* [Power.mac](/assets/MINITAB/Macros/Power.mac) - Calculates the power for the balanced fixed-effects full factorial design with optional graphs. This macro's capabilities are duplicated in **Stat> Power and Sample Size> General Full Factorial Design**; however, the macro is more flexible in its use.
* [OneSidedUpperCIforProportionSampleSize.mac](/assets/MINITAB/Macros/OneSidedUpperCIforProportionSampleSize.mac) - Calculates the sample size required to demonstrate that a proportion is less than a specified upper limit with specified confidence level.
* Power for Fisher's Exact Test:  
    * [FishersPower.mac](/assets/MINITAB/Macros/FishersPower.mac) - Calculates the power for Fisher's Exact Test using the one-sided test method.
    * [FishersPowerSlow.mac](/assets/MINITAB/Macros/FishersPowerSlow.mac) - Calculates the power for Fisher's Exact Test using the one-sided test method. Uses two different methods to complete the calculations - one fast but complicated and the other VERY slow but easier to understand. Study this macro to understand the calculations. Use FishersPower.mac to get the job done.
    * [FishersConditionalPower.mac](/assets/MINITAB/Macros/FishersConditionalPower.mac) - Calculates the power for Fisher's Exact Test (one-sided) and the conditional power given interim results.
* [TwoSamplePoissonPower.mac](/assets/MINITAB/Macros/TwoSamplePoissonPower.mac) - Calculates the power for the two-sample Poisson count problem. Consider using or checking this macro's result with (V17) **Stat> Power and Sample Size> 2-Sample Poisson Rate**.

  
  
**Simulations**
* [GRRSim.mac](/assets/MINITAB/Macros/GRRSim.mac) - Creates simulated data for a gage error study using the common operator by part crossed design. The operator controls how many operators, parts, and trials are used and EV, AV, and PV values can be set with subcommands.
* [PChartSim.mac](/assets/MINITAB/Macros/PChartSim.mac) - Creates simulated data for a P chart.
* [UChartSim.mac](/assets/MINITAB/Macros/UChartSim.mac) - Creates simulated data for a U chart.   
* [XbarChartSim.mac](/assets/MINITAB/Macros/XbarChartSim.mac) - Creates simulated data for an Xbar and R chart or process capability analysis using the one-way random effects model.
* [ProcessCapabilitySim.mtb](/assets/MINITAB/Macros/ProcessCapabilitySim.mtb) - Creates simulated data for a process capability analysis and runs the analyses. Could create similar data with the XbarChartSim.mac macro.
* [Sim3.mtb](/assets/MINITAB/Macros/Sim3.mtb) - Creates simulated response data for a three variable experiment design, e.g. two-level factorial with or without centers and response surface designs.
* [Sim5.mtb](/assets/MINITAB/Macros/Sim5.mtb) - Creates simulated response data for a five variable experiment design.
* [RunRuleExercise.mac](/assets/MINITAB/Macros/RunRuleExercise.mac) - This macro creates a series of control charts with one point added to each chart. Minimize the Session window, maximize the last graph created, and then delete each graph while watching for the process to go out of control.

  
[Return to MM&B Inc. Home Page]({% link index.md %})
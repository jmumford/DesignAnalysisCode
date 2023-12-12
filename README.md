# DesignAnalysisCode
Python notebooks that accompany the Poldrack Lab D&amp;A series.  Others are welcome to have a look!  The topics sort of meander, but the overall goal is to cover some basics about fMRI study design and model analysis.  Along the way other topics are likely to pop up, driven by interest in the lab.

If you find an error, please let me know! 

Order presented
* (Oct 4, 2023) one_and_tow_sample_t_tests.ipynb
      * An overview of 1- and 2-sample t-tests.
* (Oct 11, 2023) linear_regression_orthogonalization.ipynb
  * Believe it or not, this covers linear regression and orthogonalization.  The focus is on parameter interpretation in simple linear regression, regression with a categorical and a continuous covariate and 2 continuous covariates.  What does mean centering really do??  Is orthogonalization the answer to all of our collinearity problems? (Spoiler, the answer is NO)
* (Oct 18, 2023, time permitting) Suppression and colliders
      * This covers suppression, with a cool table I found (originally made by Cohen) that breaks down the settings that lead to all of the different types of suppression.  I also dig into colliders.  They're a little scary and are why we see headlines like, "Multiple studies find obsesity has a protective effect against mortality in patients with cardiovascular disease".  Really?!?  Many Covid study headlines were likely also driven by colliders (smoking has a protective effect?!?!).
* (Oct 24, 2023) fmri_regressors.ipynb
    * This covers convolution, parametric modulation, modeling RT overview and using VIF to assess collinearity of your regressors and contrasts.
  
* (Dec 12, 2023) efficiency_stop_signal.ipynb/utils.py This is a soup to nuts overview of efficiency.  It is a full efficiency analysis that I ran for a stop signal task.  The notebook runs through some different task design settings and shows how I chose the design I wanted to focus on for the main efficiency analysis (that code is not run in the notebook, but on a cluster see efficiency_stop_signal.py/run_eff_stop_signal.batch for those details).  The end of the notebook then digests the output from the analyses that ran for a while on the cluster that generated 100,000 random designs to choose from.  I step through how I evaluated the designs based on efficiency, VIF and the different psychological measures that were discussed earlier (only in google slides and not in code previously.)